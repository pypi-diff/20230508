# Comparing `tmp/discordia-0.1.tar.gz` & `tmp/discordia-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordia-0.1.tar", last modified: Mon May  8 05:15:50 2023, max compression
+gzip compressed data, was "discordia-0.2.tar", last modified: Mon May  8 05:32:58 2023, max compression
```

## Comparing `discordia-0.1.tar` & `discordia-0.2.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.566611 discordia-0.1/
--rw-rw-rw-   0        0        0     1149 2023-05-08 05:05:44.000000 discordia-0.1/LICENSE
--rw-rw-rw-   0        0        0      393 2023-05-08 04:30:04.000000 discordia-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1369 2023-05-08 05:15:50.565597 discordia-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-08 04:53:01.000000 discordia-0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.452609 discordia-0.1/discord/
--rw-rw-rw-   0        0        0     1834 2023-05-08 05:15:13.000000 discordia-0.1/discord/__init__.py
--rw-rw-rw-   0        0        0    11015 2023-05-08 05:15:13.000000 discordia-0.1/discord/__main__.py
--rw-rw-rw-   0        0        0     1543 2023-05-08 05:15:13.000000 discordia-0.1/discord/_typed_dict.py
--rw-rw-rw-   0        0        0     4919 2023-05-08 05:15:13.000000 discordia-0.1/discord/_version.py
--rw-rw-rw-   0        0        0    66773 2023-05-08 05:15:13.000000 discordia-0.1/discord/abc.py
--rw-rw-rw-   0        0        0    27700 2023-05-08 05:15:13.000000 discordia-0.1/discord/activity.py
--rw-rw-rw-   0        0        0     9036 2023-05-08 05:15:13.000000 discordia-0.1/discord/appinfo.py
--rw-rw-rw-   0        0        0     5019 2023-05-08 05:15:13.000000 discordia-0.1/discord/application_role_connection.py
--rw-rw-rw-   0        0        0    13739 2023-05-08 05:15:13.000000 discordia-0.1/discord/asset.py
--rw-rw-rw-   0        0        0    25318 2023-05-08 05:15:13.000000 discordia-0.1/discord/audit_logs.py
--rw-rw-rw-   0        0        0    19209 2023-05-08 05:15:13.000000 discordia-0.1/discord/automod.py
--rw-rw-rw-   0        0        0     3864 2023-05-08 05:15:13.000000 discordia-0.1/discord/backoff.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.455649 discordia-0.1/discord/bin/
--rw-rw-rw-   0        0        0   441856 2023-05-08 04:30:04.000000 discordia-0.1/discord/bin/libopus-0.x64.dll
--rw-rw-rw-   0        0        0   366080 2023-05-08 04:30:04.000000 discordia-0.1/discord/bin/libopus-0.x86.dll
--rw-rw-rw-   0        0        0    58446 2023-05-08 05:15:13.000000 discordia-0.1/discord/bot.py
--rw-rw-rw-   0        0        0   110451 2023-05-08 05:15:13.000000 discordia-0.1/discord/channel.py
--rw-rw-rw-   0        0        0    67232 2023-05-08 05:15:13.000000 discordia-0.1/discord/client.py
--rw-rw-rw-   0        0        0    42775 2023-05-08 05:15:13.000000 discordia-0.1/discord/cog.py
--rw-rw-rw-   0        0        0    11527 2023-05-08 05:15:13.000000 discordia-0.1/discord/colour.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.461222 discordia-0.1/discord/commands/
--rw-rw-rw-   0        0        0     1258 2023-05-08 05:15:13.000000 discordia-0.1/discord/commands/__init__.py
--rw-rw-rw-   0        0        0    13893 2023-05-08 05:15:14.000000 discordia-0.1/discord/commands/context.py
--rw-rw-rw-   0        0        0    71288 2023-05-08 05:15:14.000000 discordia-0.1/discord/commands/core.py
--rw-rw-rw-   0        0        0    17637 2023-05-08 05:15:14.000000 discordia-0.1/discord/commands/options.py
--rw-rw-rw-   0        0        0     4535 2023-05-08 05:15:14.000000 discordia-0.1/discord/commands/permissions.py
--rw-rw-rw-   0        0        0    16679 2023-05-08 05:15:13.000000 discordia-0.1/discord/components.py
--rw-rw-rw-   0        0        0     3032 2023-05-08 05:15:13.000000 discordia-0.1/discord/context_managers.py
--rw-rw-rw-   0        0        0    28599 2023-05-08 05:15:13.000000 discordia-0.1/discord/embeds.py
--rw-rw-rw-   0        0        0     8650 2023-05-08 05:15:13.000000 discordia-0.1/discord/emoji.py
--rw-rw-rw-   0        0        0    27172 2023-05-08 05:15:13.000000 discordia-0.1/discord/enums.py
--rw-rw-rw-   0        0        0    13276 2023-05-08 05:15:13.000000 discordia-0.1/discord/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.378627 discordia-0.1/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.464769 discordia-0.1/discord/ext/bridge/
--rw-rw-rw-   0        0        0     1226 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/bridge/__init__.py
--rw-rw-rw-   0        0        0     7569 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/bridge/bot.py
--rw-rw-rw-   0        0        0     8067 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/bridge/context.py
--rw-rw-rw-   0        0        0    20620 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/bridge/core.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.477941 discordia-0.1/discord/ext/commands/
--rw-rw-rw-   0        0        0      446 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     1860 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    16509 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/bot.py
--rw-rw-rw-   0        0        0     3152 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    14933 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/context.py
--rw-rw-rw-   0        0        0    41377 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/converter.py
--rw-rw-rw-   0        0        0    13214 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    84563 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/core.py
--rw-rw-rw-   0        0        0    30393 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    22632 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    50155 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/help.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.479967 discordia-0.1/discord/ext/pages/
--rw-rw-rw-   0        0        0      230 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/pages/__init__.py
--rw-rw-rw-   0        0        0    54303 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/pages/pagination.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.481487 discordia-0.1/discord/ext/tasks/
--rw-rw-rw-   0        0        0    27569 2023-05-08 05:15:14.000000 discordia-0.1/discord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     4966 2023-05-08 05:15:13.000000 discordia-0.1/discord/file.py
--rw-rw-rw-   0        0        0    48208 2023-05-08 05:15:13.000000 discordia-0.1/discord/flags.py
--rw-rw-rw-   0        0        0    33291 2023-05-08 05:15:13.000000 discordia-0.1/discord/gateway.py
--rw-rw-rw-   0        0        0   130772 2023-05-08 05:15:13.000000 discordia-0.1/discord/guild.py
--rw-rw-rw-   0        0        0    93139 2023-05-08 05:15:13.000000 discordia-0.1/discord/http.py
--rw-rw-rw-   0        0        0    12176 2023-05-08 05:15:13.000000 discordia-0.1/discord/integrations.py
--rw-rw-rw-   0        0        0    47880 2023-05-08 05:15:13.000000 discordia-0.1/discord/interactions.py
--rw-rw-rw-   0        0        0    19721 2023-05-08 05:15:13.000000 discordia-0.1/discord/invite.py
--rw-rw-rw-   0        0        0    31382 2023-05-08 05:15:13.000000 discordia-0.1/discord/iterators.py
--rw-rw-rw-   0        0        0    38209 2023-05-08 05:15:13.000000 discordia-0.1/discord/member.py
--rw-rw-rw-   0        0        0     5910 2023-05-08 05:15:13.000000 discordia-0.1/discord/mentions.py
--rw-rw-rw-   0        0        0    74888 2023-05-08 05:15:13.000000 discordia-0.1/discord/message.py
--rw-rw-rw-   0        0        0     1690 2023-05-08 05:15:13.000000 discordia-0.1/discord/mixins.py
--rw-rw-rw-   0        0        0     3499 2023-05-08 05:15:13.000000 discordia-0.1/discord/object.py
--rw-rw-rw-   0        0        0     3896 2023-05-08 05:15:13.000000 discordia-0.1/discord/oggparse.py
--rw-rw-rw-   0        0        0    17475 2023-05-08 05:15:13.000000 discordia-0.1/discord/opus.py
--rw-rw-rw-   0        0        0     7665 2023-05-08 05:15:13.000000 discordia-0.1/discord/partial_emoji.py
--rw-rw-rw-   0        0        0    28133 2023-05-08 05:15:13.000000 discordia-0.1/discord/permissions.py
--rw-rw-rw-   0        0        0    27841 2023-05-08 05:15:13.000000 discordia-0.1/discord/player.py
--rw-rw-rw-   0        0        0        0 2023-05-08 04:30:04.000000 discordia-0.1/discord/py.typed
--rw-rw-rw-   0        0        0    26449 2023-05-08 05:15:13.000000 discordia-0.1/discord/raw_models.py
--rw-rw-rw-   0        0        0     7289 2023-05-08 05:15:13.000000 discordia-0.1/discord/reaction.py
--rw-rw-rw-   0        0        0    16754 2023-05-08 05:15:13.000000 discordia-0.1/discord/role.py
--rw-rw-rw-   0        0        0    19155 2023-05-08 05:15:13.000000 discordia-0.1/discord/scheduled_events.py
--rw-rw-rw-   0        0        0    20309 2023-05-08 05:15:13.000000 discordia-0.1/discord/shard.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.492632 discordia-0.1/discord/sinks/
--rw-rw-rw-   0        0        0      395 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/__init__.py
--rw-rw-rw-   0        0        0     6484 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/core.py
--rw-rw-rw-   0        0        0     2542 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/errors.py
--rw-rw-rw-   0        0        0     3320 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/m4a.py
--rw-rw-rw-   0        0        0     3087 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/mka.py
--rw-rw-rw-   0        0        0     3055 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/mkv.py
--rw-rw-rw-   0        0        0     3082 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/mp3.py
--rw-rw-rw-   0        0        0     3319 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/mp4.py
--rw-rw-rw-   0        0        0     3082 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/ogg.py
--rw-rw-rw-   0        0        0     1613 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/pcm.py
--rw-rw-rw-   0        0        0     2388 2023-05-08 05:15:14.000000 discordia-0.1/discord/sinks/wave.py
--rw-rw-rw-   0        0        0     6526 2023-05-08 05:15:13.000000 discordia-0.1/discord/stage_instance.py
--rw-rw-rw-   0        0        0    75699 2023-05-08 05:15:13.000000 discordia-0.1/discord/state.py
--rw-rw-rw-   0        0        0    16777 2023-05-08 05:15:13.000000 discordia-0.1/discord/sticker.py
--rw-rw-rw-   0        0        0     4838 2023-05-08 05:15:13.000000 discordia-0.1/discord/team.py
--rw-rw-rw-   0        0        0     9593 2023-05-08 05:15:13.000000 discordia-0.1/discord/template.py
--rw-rw-rw-   0        0        0    31433 2023-05-08 05:15:13.000000 discordia-0.1/discord/threads.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.529620 discordia-0.1/discord/types/
--rw-rw-rw-   0        0        0      195 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/__init__.py
--rw-rw-rw-   0        0        0     2867 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/activity.py
--rw-rw-rw-   0        0        0     2056 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/appinfo.py
--rw-rw-rw-   0        0        0     1592 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/application_role_connection.py
--rw-rw-rw-   0        0        0     6995 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/audit_log.py
--rw-rw-rw-   0        0        0     2884 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/automod.py
--rw-rw-rw-   0        0        0     4838 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/channel.py
--rw-rw-rw-   0        0        0     2633 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/components.py
--rw-rw-rw-   0        0        0     2489 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/embed.py
--rw-rw-rw-   0        0        0     1640 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/emoji.py
--rw-rw-rw-   0        0        0     1454 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/gateway.py
--rw-rw-rw-   0        0        0     5558 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/guild.py
--rw-rw-rw-   0        0        0     2344 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/integration.py
--rw-rw-rw-   0        0        0     7124 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/interactions.py
--rw-rw-rw-   0        0        0     2856 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/invite.py
--rw-rw-rw-   0        0        0     1928 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/member.py
--rw-rw-rw-   0        0        0     4086 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/message.py
--rw-rw-rw-   0        0        0     4001 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/raw_models.py
--rw-rw-rw-   0        0        0     1623 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/role.py
--rw-rw-rw-   0        0        0     2144 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/scheduled_events.py
--rw-rw-rw-   0        0        0     1257 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/snowflake.py
--rw-rw-rw-   0        0        0     2452 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/sticker.py
--rw-rw-rw-   0        0        0     1572 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/team.py
--rw-rw-rw-   0        0        0     1688 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/template.py
--rw-rw-rw-   0        0        0     2390 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/threads.py
--rw-rw-rw-   0        0        0     1657 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/user.py
--rw-rw-rw-   0        0        0     2415 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/voice.py
--rw-rw-rw-   0        0        0     2049 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/webhook.py
--rw-rw-rw-   0        0        0     1527 2023-05-08 05:15:14.000000 discordia-0.1/discord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1950 2023-05-08 05:15:15.000000 discordia-0.1/discord/types/widget.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.540769 discordia-0.1/discord/ui/
--rw-rw-rw-   0        0        0      333 2023-05-08 05:15:15.000000 discordia-0.1/discord/ui/__init__.py
--rw-rw-rw-   0        0        0    11078 2023-05-08 05:15:15.000000 discordia-0.1/discord/ui/button.py
--rw-rw-rw-   0        0        0     8368 2023-05-08 04:30:04.000000 discordia-0.1/discord/ui/input_text.py
--rw-rw-rw-   0        0        0     4337 2023-05-08 05:15:15.000000 discordia-0.1/discord/ui/item.py
--rw-rw-rw-   0        0        0    11652 2023-05-08 04:30:04.000000 discordia-0.1/discord/ui/modal.py
--rw-rw-rw-   0        0        0    25517 2023-05-08 05:15:15.000000 discordia-0.1/discord/ui/select.py
--rw-rw-rw-   0        0        0    22218 2023-05-08 05:15:15.000000 discordia-0.1/discord/ui/view.py
--rw-rw-rw-   0        0        0    15819 2023-05-08 05:15:13.000000 discordia-0.1/discord/user.py
--rw-rw-rw-   0        0        0    43237 2023-05-08 05:15:13.000000 discordia-0.1/discord/utils.py
--rw-rw-rw-   0        0        0    33728 2023-05-08 05:15:13.000000 discordia-0.1/discord/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.545330 discordia-0.1/discord/webhook/
--rw-rw-rw-   0        0        0      252 2023-05-08 05:15:15.000000 discordia-0.1/discord/webhook/__init__.py
--rw-rw-rw-   0        0        0    66202 2023-05-08 05:15:15.000000 discordia-0.1/discord/webhook/async_.py
--rw-rw-rw-   0        0        0    42196 2023-05-08 05:15:15.000000 discordia-0.1/discord/webhook/sync.py
--rw-rw-rw-   0        0        0     8037 2023-05-08 05:15:13.000000 discordia-0.1/discord/welcome_screen.py
--rw-rw-rw-   0        0        0    10343 2023-05-08 05:15:13.000000 discordia-0.1/discord/widget.py
-drwxrwxrwx   0        0        0        0 2023-05-08 05:15:50.564584 discordia-0.1/discordia.egg-info/
--rw-rw-rw-   0        0        0     1369 2023-05-08 05:15:50.000000 discordia-0.1/discordia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3412 2023-05-08 05:15:50.000000 discordia-0.1/discordia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 05:15:50.000000 discordia-0.1/discordia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      379 2023-05-08 05:15:50.000000 discordia-0.1/discordia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 05:15:50.000000 discordia-0.1/discordia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2598 2023-05-08 05:15:13.000000 discordia-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 05:15:50.566611 discordia-0.1/setup.cfg
--rw-rw-rw-   0        0        0      214 2023-05-08 04:54:10.000000 discordia-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.362090 discordia-0.2/
+-rw-rw-rw-   0        0        0     1149 2023-05-08 05:05:44.000000 discordia-0.2/LICENSE
+-rw-rw-rw-   0        0        0      393 2023-05-08 04:30:04.000000 discordia-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1369 2023-05-08 05:32:58.361583 discordia-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-05-08 04:53:01.000000 discordia-0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.250607 discordia-0.2/discord/
+-rw-rw-rw-   0        0        0     1834 2023-05-08 05:15:13.000000 discordia-0.2/discord/__init__.py
+-rw-rw-rw-   0        0        0    11015 2023-05-08 05:15:13.000000 discordia-0.2/discord/__main__.py
+-rw-rw-rw-   0        0        0     1543 2023-05-08 05:15:13.000000 discordia-0.2/discord/_typed_dict.py
+-rw-rw-rw-   0        0        0     4919 2023-05-08 05:15:13.000000 discordia-0.2/discord/_version.py
+-rw-rw-rw-   0        0        0    66773 2023-05-08 05:15:13.000000 discordia-0.2/discord/abc.py
+-rw-rw-rw-   0        0        0    27700 2023-05-08 05:15:13.000000 discordia-0.2/discord/activity.py
+-rw-rw-rw-   0        0        0     9036 2023-05-08 05:15:13.000000 discordia-0.2/discord/appinfo.py
+-rw-rw-rw-   0        0        0     5019 2023-05-08 05:15:13.000000 discordia-0.2/discord/application_role_connection.py
+-rw-rw-rw-   0        0        0    13739 2023-05-08 05:15:13.000000 discordia-0.2/discord/asset.py
+-rw-rw-rw-   0        0        0    25318 2023-05-08 05:15:13.000000 discordia-0.2/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    19209 2023-05-08 05:15:13.000000 discordia-0.2/discord/automod.py
+-rw-rw-rw-   0        0        0     3864 2023-05-08 05:15:13.000000 discordia-0.2/discord/backoff.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.253141 discordia-0.2/discord/bin/
+-rw-rw-rw-   0        0        0   441856 2023-05-08 04:30:04.000000 discordia-0.2/discord/bin/libopus-0.x64.dll
+-rw-rw-rw-   0        0        0   366080 2023-05-08 04:30:04.000000 discordia-0.2/discord/bin/libopus-0.x86.dll
+-rw-rw-rw-   0        0        0    58446 2023-05-08 05:15:13.000000 discordia-0.2/discord/bot.py
+-rw-rw-rw-   0        0        0   110451 2023-05-08 05:15:13.000000 discordia-0.2/discord/channel.py
+-rw-rw-rw-   0        0        0    67232 2023-05-08 05:15:13.000000 discordia-0.2/discord/client.py
+-rw-rw-rw-   0        0        0    42775 2023-05-08 05:15:13.000000 discordia-0.2/discord/cog.py
+-rw-rw-rw-   0        0        0    11527 2023-05-08 05:15:13.000000 discordia-0.2/discord/colour.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.259727 discordia-0.2/discord/commands/
+-rw-rw-rw-   0        0        0     1258 2023-05-08 05:15:13.000000 discordia-0.2/discord/commands/__init__.py
+-rw-rw-rw-   0        0        0    13893 2023-05-08 05:15:14.000000 discordia-0.2/discord/commands/context.py
+-rw-rw-rw-   0        0        0    71288 2023-05-08 05:15:14.000000 discordia-0.2/discord/commands/core.py
+-rw-rw-rw-   0        0        0    17637 2023-05-08 05:15:14.000000 discordia-0.2/discord/commands/options.py
+-rw-rw-rw-   0        0        0     4535 2023-05-08 05:15:14.000000 discordia-0.2/discord/commands/permissions.py
+-rw-rw-rw-   0        0        0    16679 2023-05-08 05:15:13.000000 discordia-0.2/discord/components.py
+-rw-rw-rw-   0        0        0     3032 2023-05-08 05:15:13.000000 discordia-0.2/discord/context_managers.py
+-rw-rw-rw-   0        0        0    28599 2023-05-08 05:15:13.000000 discordia-0.2/discord/embeds.py
+-rw-rw-rw-   0        0        0     8650 2023-05-08 05:15:13.000000 discordia-0.2/discord/emoji.py
+-rw-rw-rw-   0        0        0    27172 2023-05-08 05:15:13.000000 discordia-0.2/discord/enums.py
+-rw-rw-rw-   0        0        0    13276 2023-05-08 05:15:13.000000 discordia-0.2/discord/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.176628 discordia-0.2/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.264796 discordia-0.2/discord/ext/bridge/
+-rw-rw-rw-   0        0        0     1226 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/bridge/__init__.py
+-rw-rw-rw-   0        0        0     7569 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/bridge/bot.py
+-rw-rw-rw-   0        0        0     8067 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/bridge/context.py
+-rw-rw-rw-   0        0        0    20620 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/bridge/core.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.278984 discordia-0.2/discord/ext/commands/
+-rw-rw-rw-   0        0        0      446 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     1860 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    16509 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0     3152 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    14933 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    41377 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0    13214 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    84563 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    30393 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22632 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    50155 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.281518 discordia-0.2/discord/ext/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/pages/__init__.py
+-rw-rw-rw-   0        0        0    54303 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/pages/pagination.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.282531 discordia-0.2/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    27569 2023-05-08 05:15:14.000000 discordia-0.2/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4966 2023-05-08 05:15:13.000000 discordia-0.2/discord/file.py
+-rw-rw-rw-   0        0        0    48208 2023-05-08 05:15:13.000000 discordia-0.2/discord/flags.py
+-rw-rw-rw-   0        0        0    33291 2023-05-08 05:15:13.000000 discordia-0.2/discord/gateway.py
+-rw-rw-rw-   0        0        0   130772 2023-05-08 05:15:13.000000 discordia-0.2/discord/guild.py
+-rw-rw-rw-   0        0        0    93139 2023-05-08 05:15:13.000000 discordia-0.2/discord/http.py
+-rw-rw-rw-   0        0        0    12176 2023-05-08 05:15:13.000000 discordia-0.2/discord/integrations.py
+-rw-rw-rw-   0        0        0    47880 2023-05-08 05:15:13.000000 discordia-0.2/discord/interactions.py
+-rw-rw-rw-   0        0        0    19721 2023-05-08 05:15:13.000000 discordia-0.2/discord/invite.py
+-rw-rw-rw-   0        0        0    31382 2023-05-08 05:15:13.000000 discordia-0.2/discord/iterators.py
+-rw-rw-rw-   0        0        0    38209 2023-05-08 05:15:13.000000 discordia-0.2/discord/member.py
+-rw-rw-rw-   0        0        0     5910 2023-05-08 05:15:13.000000 discordia-0.2/discord/mentions.py
+-rw-rw-rw-   0        0        0    74888 2023-05-08 05:15:13.000000 discordia-0.2/discord/message.py
+-rw-rw-rw-   0        0        0     1690 2023-05-08 05:15:13.000000 discordia-0.2/discord/mixins.py
+-rw-rw-rw-   0        0        0     3499 2023-05-08 05:15:13.000000 discordia-0.2/discord/object.py
+-rw-rw-rw-   0        0        0     3896 2023-05-08 05:15:13.000000 discordia-0.2/discord/oggparse.py
+-rw-rw-rw-   0        0        0    17475 2023-05-08 05:15:13.000000 discordia-0.2/discord/opus.py
+-rw-rw-rw-   0        0        0     7665 2023-05-08 05:15:13.000000 discordia-0.2/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    28133 2023-05-08 05:15:13.000000 discordia-0.2/discord/permissions.py
+-rw-rw-rw-   0        0        0    27841 2023-05-08 05:15:13.000000 discordia-0.2/discord/player.py
+-rw-rw-rw-   0        0        0        0 2023-05-08 04:30:04.000000 discordia-0.2/discord/py.typed
+-rw-rw-rw-   0        0        0    26449 2023-05-08 05:15:13.000000 discordia-0.2/discord/raw_models.py
+-rw-rw-rw-   0        0        0     7289 2023-05-08 05:15:13.000000 discordia-0.2/discord/reaction.py
+-rw-rw-rw-   0        0        0    16754 2023-05-08 05:15:13.000000 discordia-0.2/discord/role.py
+-rw-rw-rw-   0        0        0    19155 2023-05-08 05:15:13.000000 discordia-0.2/discord/scheduled_events.py
+-rw-rw-rw-   0        0        0    20309 2023-05-08 05:15:13.000000 discordia-0.2/discord/shard.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.294692 discordia-0.2/discord/sinks/
+-rw-rw-rw-   0        0        0      395 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/__init__.py
+-rw-rw-rw-   0        0        0     6484 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/core.py
+-rw-rw-rw-   0        0        0     2542 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/errors.py
+-rw-rw-rw-   0        0        0     3320 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/m4a.py
+-rw-rw-rw-   0        0        0     3087 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/mka.py
+-rw-rw-rw-   0        0        0     3055 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/mkv.py
+-rw-rw-rw-   0        0        0     3082 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/mp3.py
+-rw-rw-rw-   0        0        0     3319 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/mp4.py
+-rw-rw-rw-   0        0        0     3082 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/ogg.py
+-rw-rw-rw-   0        0        0     1613 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/pcm.py
+-rw-rw-rw-   0        0        0     2388 2023-05-08 05:15:14.000000 discordia-0.2/discord/sinks/wave.py
+-rw-rw-rw-   0        0        0     6526 2023-05-08 05:15:13.000000 discordia-0.2/discord/stage_instance.py
+-rw-rw-rw-   0        0        0    75699 2023-05-08 05:15:13.000000 discordia-0.2/discord/state.py
+-rw-rw-rw-   0        0        0    16777 2023-05-08 05:15:13.000000 discordia-0.2/discord/sticker.py
+-rw-rw-rw-   0        0        0     4838 2023-05-08 05:15:13.000000 discordia-0.2/discord/team.py
+-rw-rw-rw-   0        0        0     9593 2023-05-08 05:15:13.000000 discordia-0.2/discord/template.py
+-rw-rw-rw-   0        0        0    31433 2023-05-08 05:15:13.000000 discordia-0.2/discord/threads.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.329661 discordia-0.2/discord/types/
+-rw-rw-rw-   0        0        0      195 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2867 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/activity.py
+-rw-rw-rw-   0        0        0     2056 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/appinfo.py
+-rw-rw-rw-   0        0        0     1592 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/application_role_connection.py
+-rw-rw-rw-   0        0        0     6995 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     2884 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/automod.py
+-rw-rw-rw-   0        0        0     4838 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/channel.py
+-rw-rw-rw-   0        0        0     2633 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/components.py
+-rw-rw-rw-   0        0        0     2489 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1640 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     1454 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5558 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2344 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/integration.py
+-rw-rw-rw-   0        0        0     7124 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2856 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1928 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/member.py
+-rw-rw-rw-   0        0        0     4086 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/message.py
+-rw-rw-rw-   0        0        0     4001 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/raw_models.py
+-rw-rw-rw-   0        0        0     1623 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/role.py
+-rw-rw-rw-   0        0        0     2144 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/scheduled_events.py
+-rw-rw-rw-   0        0        0     1257 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2452 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     1572 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/team.py
+-rw-rw-rw-   0        0        0     1688 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/template.py
+-rw-rw-rw-   0        0        0     2390 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/threads.py
+-rw-rw-rw-   0        0        0     1657 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/user.py
+-rw-rw-rw-   0        0        0     2415 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/voice.py
+-rw-rw-rw-   0        0        0     2049 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1527 2023-05-08 05:15:14.000000 discordia-0.2/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1950 2023-05-08 05:15:15.000000 discordia-0.2/discord/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.337261 discordia-0.2/discord/ui/
+-rw-rw-rw-   0        0        0      333 2023-05-08 05:15:15.000000 discordia-0.2/discord/ui/__init__.py
+-rw-rw-rw-   0        0        0    11078 2023-05-08 05:15:15.000000 discordia-0.2/discord/ui/button.py
+-rw-rw-rw-   0        0        0     8368 2023-05-08 04:30:04.000000 discordia-0.2/discord/ui/input_text.py
+-rw-rw-rw-   0        0        0     4337 2023-05-08 05:15:15.000000 discordia-0.2/discord/ui/item.py
+-rw-rw-rw-   0        0        0    11652 2023-05-08 04:30:04.000000 discordia-0.2/discord/ui/modal.py
+-rw-rw-rw-   0        0        0    25517 2023-05-08 05:15:15.000000 discordia-0.2/discord/ui/select.py
+-rw-rw-rw-   0        0        0    22218 2023-05-08 05:31:45.000000 discordia-0.2/discord/ui/view.py
+-rw-rw-rw-   0        0        0    15819 2023-05-08 05:15:13.000000 discordia-0.2/discord/user.py
+-rw-rw-rw-   0        0        0    43237 2023-05-08 05:15:13.000000 discordia-0.2/discord/utils.py
+-rw-rw-rw-   0        0        0    33728 2023-05-08 05:15:13.000000 discordia-0.2/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.342329 discordia-0.2/discord/webhook/
+-rw-rw-rw-   0        0        0      252 2023-05-08 05:15:15.000000 discordia-0.2/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    66202 2023-05-08 05:15:15.000000 discordia-0.2/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    42196 2023-05-08 05:15:15.000000 discordia-0.2/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     8037 2023-05-08 05:15:13.000000 discordia-0.2/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10343 2023-05-08 05:15:13.000000 discordia-0.2/discord/widget.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:32:58.360569 discordia-0.2/discordia.egg-info/
+-rw-rw-rw-   0        0        0     1369 2023-05-08 05:32:58.000000 discordia-0.2/discordia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3412 2023-05-08 05:32:58.000000 discordia-0.2/discordia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 05:32:58.000000 discordia-0.2/discordia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      379 2023-05-08 05:32:58.000000 discordia-0.2/discordia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 05:32:58.000000 discordia-0.2/discordia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2598 2023-05-08 05:15:13.000000 discordia-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 05:32:58.362596 discordia-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      214 2023-05-08 05:31:58.000000 discordia-0.2/setup.py
```

### Comparing `discordia-0.1/LICENSE` & `discordia-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discordia-0.1/PKG-INFO` & `discordia-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordia
-Version: 0.1
+Version: 0.2
 Summary: A Python wrapper for the Discord API
 Author: discordia Development
 License: MIT
 Project-URL: Homepage, https://discordia.dev
 Project-URL: Changelog, https://docs.discordia.dev/en/master/changelog.html
 Project-URL: Source, https://github.com/discordia-Development/discordia
 Project-URL: Documentation, https://docs.discordia.dev
```

### Comparing `discordia-0.1/discord/__init__.py` & `discordia-0.2/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/__main__.py` & `discordia-0.2/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/_typed_dict.py` & `discordia-0.2/discord/_typed_dict.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/_version.py` & `discordia-0.2/discord/_version.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/abc.py` & `discordia-0.2/discord/abc.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/activity.py` & `discordia-0.2/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/appinfo.py` & `discordia-0.2/discord/appinfo.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/application_role_connection.py` & `discordia-0.2/discord/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/asset.py` & `discordia-0.2/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/audit_logs.py` & `discordia-0.2/discord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/automod.py` & `discordia-0.2/discord/automod.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/backoff.py` & `discordia-0.2/discord/backoff.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/bin/libopus-0.x64.dll` & `discordia-0.2/discord/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/bin/libopus-0.x86.dll` & `discordia-0.2/discord/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/bot.py` & `discordia-0.2/discord/bot.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/channel.py` & `discordia-0.2/discord/channel.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/client.py` & `discordia-0.2/discord/client.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/cog.py` & `discordia-0.2/discord/cog.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/colour.py` & `discordia-0.2/discord/colour.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/commands/__init__.py` & `discordia-0.2/discord/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/commands/context.py` & `discordia-0.2/discord/commands/context.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/commands/core.py` & `discordia-0.2/discord/commands/core.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/commands/options.py` & `discordia-0.2/discord/commands/options.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/commands/permissions.py` & `discordia-0.2/discord/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/components.py` & `discordia-0.2/discord/components.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/context_managers.py` & `discordia-0.2/discord/context_managers.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/embeds.py` & `discordia-0.2/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/emoji.py` & `discordia-0.2/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/enums.py` & `discordia-0.2/discord/enums.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/errors.py` & `discordia-0.2/discord/errors.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/bridge/__init__.py` & `discordia-0.2/discord/ext/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/bridge/bot.py` & `discordia-0.2/discord/ext/bridge/bot.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/bridge/context.py` & `discordia-0.2/discord/ext/bridge/context.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/bridge/core.py` & `discordia-0.2/discord/ext/bridge/core.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/_types.py` & `discordia-0.2/discord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/bot.py` & `discordia-0.2/discord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/cog.py` & `discordia-0.2/discord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/context.py` & `discordia-0.2/discord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/converter.py` & `discordia-0.2/discord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/cooldowns.py` & `discordia-0.2/discord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/core.py` & `discordia-0.2/discord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/errors.py` & `discordia-0.2/discord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/flags.py` & `discordia-0.2/discord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/help.py` & `discordia-0.2/discord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/commands/view.py` & `discordia-0.2/discord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/pages/pagination.py` & `discordia-0.2/discord/ext/pages/pagination.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ext/tasks/__init__.py` & `discordia-0.2/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/file.py` & `discordia-0.2/discord/file.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/flags.py` & `discordia-0.2/discord/flags.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/gateway.py` & `discordia-0.2/discord/gateway.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/guild.py` & `discordia-0.2/discord/guild.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/http.py` & `discordia-0.2/discord/http.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/integrations.py` & `discordia-0.2/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/interactions.py` & `discordia-0.2/discord/interactions.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/invite.py` & `discordia-0.2/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/iterators.py` & `discordia-0.2/discord/iterators.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/member.py` & `discordia-0.2/discord/member.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/mentions.py` & `discordia-0.2/discord/mentions.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/message.py` & `discordia-0.2/discord/message.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/mixins.py` & `discordia-0.2/discord/mixins.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/object.py` & `discordia-0.2/discord/object.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/oggparse.py` & `discordia-0.2/discord/oggparse.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/opus.py` & `discordia-0.2/discord/opus.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/partial_emoji.py` & `discordia-0.2/discord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/permissions.py` & `discordia-0.2/discord/permissions.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/player.py` & `discordia-0.2/discord/player.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/raw_models.py` & `discordia-0.2/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/reaction.py` & `discordia-0.2/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/role.py` & `discordia-0.2/discord/role.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/scheduled_events.py` & `discordia-0.2/discord/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/shard.py` & `discordia-0.2/discord/shard.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/core.py` & `discordia-0.2/discord/sinks/core.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/errors.py` & `discordia-0.2/discord/sinks/errors.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/m4a.py` & `discordia-0.2/discord/sinks/m4a.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/mka.py` & `discordia-0.2/discord/sinks/mka.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/mkv.py` & `discordia-0.2/discord/sinks/mkv.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/mp3.py` & `discordia-0.2/discord/sinks/mp3.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/mp4.py` & `discordia-0.2/discord/sinks/mp4.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/ogg.py` & `discordia-0.2/discord/sinks/ogg.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/pcm.py` & `discordia-0.2/discord/sinks/pcm.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sinks/wave.py` & `discordia-0.2/discord/sinks/wave.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/stage_instance.py` & `discordia-0.2/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/state.py` & `discordia-0.2/discord/state.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/sticker.py` & `discordia-0.2/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/team.py` & `discordia-0.2/discord/team.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/template.py` & `discordia-0.2/discord/template.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/threads.py` & `discordia-0.2/discord/threads.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/activity.py` & `discordia-0.2/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/appinfo.py` & `discordia-0.2/discord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/application_role_connection.py` & `discordia-0.2/discord/types/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/audit_log.py` & `discordia-0.2/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/automod.py` & `discordia-0.2/discord/types/automod.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/channel.py` & `discordia-0.2/discord/types/channel.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/components.py` & `discordia-0.2/discord/types/components.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/embed.py` & `discordia-0.2/discord/types/embed.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/emoji.py` & `discordia-0.2/discord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/gateway.py` & `discordia-0.2/discord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/guild.py` & `discordia-0.2/discord/types/guild.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/integration.py` & `discordia-0.2/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/interactions.py` & `discordia-0.2/discord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/invite.py` & `discordia-0.2/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/member.py` & `discordia-0.2/discord/types/member.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/message.py` & `discordia-0.2/discord/types/message.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/raw_models.py` & `discordia-0.2/discord/types/raw_models.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/role.py` & `discordia-0.2/discord/types/role.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/scheduled_events.py` & `discordia-0.2/discord/types/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/snowflake.py` & `discordia-0.2/discord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/sticker.py` & `discordia-0.2/discord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/team.py` & `discordia-0.2/discord/types/team.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/template.py` & `discordia-0.2/discord/types/template.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/threads.py` & `discordia-0.2/discord/types/threads.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/user.py` & `discordia-0.2/discord/types/user.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/voice.py` & `discordia-0.2/discord/types/voice.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/webhook.py` & `discordia-0.2/discord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/welcome_screen.py` & `discordia-0.2/discord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/types/widget.py` & `discordia-0.2/discord/types/widget.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ui/button.py` & `discordia-0.2/discord/ui/button.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ui/input_text.py` & `discordia-0.2/discord/ui/input_text.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ui/item.py` & `discordia-0.2/discord/ui/item.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ui/modal.py` & `discordia-0.2/discord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ui/select.py` & `discordia-0.2/discord/ui/select.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/ui/view.py` & `discordia-0.2/discord/ui/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,75 +111,75 @@
             item._rendered_row = None
 
     def clear(self) -> None:
         self.weights = [0, 0, 0, 0, 0]
 
 
 class View:
-    """Represents a UI view.
+    """Represents a UI View.
 
     This object must be inherited to create a UI within Discord.
 
     .. versionadded:: 2.0
 
     Parameters
     ----------
     *items: :class:`Item`
-        The initial items attached to this view.
+        The initial items attached to this View.
     timeout: Optional[:class:`float`]
         Timeout in seconds from last interaction with the UI before no longer accepting input.
         If ``None`` then there is no timeout.
 
     Attributes
     ----------
     timeout: Optional[:class:`float`]
         Timeout from last interaction with the UI before no longer accepting input.
         If ``None`` then there is no timeout.
     children: List[:class:`Item`]
-        The list of children attached to this view.
+        The list of children attached to this View.
     disable_on_timeout: :class:`bool`
-        Whether to disable the view when the timeout is reached. Defaults to ``False``.
+        Whether to disable the View when the timeout is reached. Defaults to ``False``.
     message: Optional[:class:`.Message`]
-        The message that this view is attached to.
-        If ``None`` then the view has not been sent with a message.
+        The message that this View is attached to.
+        If ``None`` then the View has not been sent with a message.
     parent: Optional[:class:`.Interaction`]
-        The parent interaction which this view was sent from.
-        If ``None`` then the view was not sent using :meth:`InteractionResponse.send_message`.
+        The parent interaction which this View was sent from.
+        If ``None`` then the View was not sent using :meth:`InteractionResponse.send_message`.
     """
 
-    __discord_ui_view__: ClassVar[bool] = True
-    __view_children_items__: ClassVar[list[ItemCallbackType]] = []
+    __discord_ui_View__: ClassVar[bool] = True
+    __View_children_items__: ClassVar[list[ItemCallbackType]] = []
 
     def __init_subclass__(cls) -> None:
         children: list[ItemCallbackType] = []
         for base in reversed(cls.__mro__):
             for member in base.__dict__.values():
                 if hasattr(member, "__discord_ui_model_type__"):
                     children.append(member)
 
         if len(children) > 25:
             raise TypeError("View cannot have more than 25 children")
 
-        cls.__view_children_items__ = children
+        cls.__View_children_items__ = children
 
     def __init__(
         self,
         *items: Item,
         timeout: float | None = 180.0,
         disable_on_timeout: bool = False,
     ):
         self.timeout = timeout
         self.disable_on_timeout = disable_on_timeout
         self.children: list[Item] = []
-        for func in self.__view_children_items__:
+        for func in self.__View_children_items__:
             item: Item = func.__discord_ui_model_type__(
                 **func.__discord_ui_model_kwargs__
             )
             item.callback = partial(func, self, item)
-            item._view = self
+            item._View = self
             setattr(self, func.__name__, item)
             self.children.append(item)
 
         self.__weights = _ViewWeights(self.children)
         for item in items:
             self.add_item(item)
 
@@ -242,42 +242,42 @@
         and separate types from those in the ``discord.ui`` namespace.
         In order to modify and edit message components they must be
         converted into a :class:`View` first.
 
         Parameters
         ----------
         message: :class:`.Message`
-            The message with components to convert into a view.
+            The message with components to convert into a View.
         timeout: Optional[:class:`float`]
-            The timeout of the converted view.
+            The timeout of the converted View.
 
         Returns
         -------
         :class:`View`
-            The converted view. This always returns a :class:`View` and not
+            The converted View. This always returns a :class:`View` and not
             one of its subclasses.
         """
-        view = View(timeout=timeout)
+        View = View(timeout=timeout)
         for component in _walk_all_components(message.components):
-            view.add_item(_component_to_item(component))
-        return view
+            View.add_item(_component_to_item(component))
+        return View
 
     @property
     def _expires_at(self) -> float | None:
         if self.timeout:
             return time.monotonic() + self.timeout
         return None
 
     def add_item(self, item: Item) -> None:
-        """Adds an item to the view.
+        """Adds an item to the View.
 
         Parameters
         ----------
         item: :class:`Item`
-            The item to add to the view.
+            The item to add to the View.
 
         Raises
         ------
         TypeError
             An :class:`Item` was not passed.
         ValueError
             Maximum number of children has been exceeded (25)
@@ -288,40 +288,40 @@
             raise ValueError("maximum number of children exceeded")
 
         if not isinstance(item, Item):
             raise TypeError(f"expected Item not {item.__class__!r}")
 
         self.__weights.add_item(item)
 
-        item._view = self
+        item._View = self
         self.children.append(item)
 
     def remove_item(self, item: Item) -> None:
-        """Removes an item from the view.
+        """Removes an item from the View.
 
         Parameters
         ----------
         item: :class:`Item`
-            The item to remove from the view.
+            The item to remove from the View.
         """
 
         try:
             self.children.remove(item)
         except ValueError:
             pass
         else:
             self.__weights.remove_item(item)
 
     def clear_items(self) -> None:
-        """Removes all items from the view."""
+        """Removes all items from the View."""
         self.children.clear()
         self.__weights.clear()
 
     def get_item(self, custom_id: str) -> Item | None:
-        """Get an item from the view with the given custom ID. Alias for `utils.get(view.children, custom_id=custom_id)`.
+        """Get an item from the View with the given custom ID. Alias for `utils.get(View.children, custom_id=custom_id)`.
 
         Parameters
         ----------
         custom_id: :class:`str`
             The custom_id of the item to get
 
         Returns
@@ -330,16 +330,16 @@
             The item with the matching ``custom_id`` if it exists.
         """
         return get(self.children, custom_id=custom_id)
 
     async def interaction_check(self, interaction: Interaction) -> bool:
         """|coro|
 
-        A callback that is called when an interaction happens within the view
-        that checks whether the view should process item callbacks for the interaction.
+        A callback that is called when an interaction happens within the View
+        that checks whether the View should process item callbacks for the interaction.
 
         This is useful to override if, for example, you want to ensure that the
         interaction author is a given user.
 
         The default implementation of this returns ``True``.
 
         If this returns ``False``, :meth:`on_check_failure` is called.
@@ -353,28 +353,28 @@
         ----------
         interaction: :class:`~discord.Interaction`
             The interaction that occurred.
 
         Returns
         -------
         :class:`bool`
-            Whether the view children's callbacks should be called.
+            Whether the View children's callbacks should be called.
         """
         return True
 
     async def on_timeout(self) -> None:
         """|coro|
 
-        A callback that is called when a view's timeout elapses without being explicitly stopped.
+        A callback that is called when a View's timeout elapses without being explicitly stopped.
         """
         if self.disable_on_timeout:
             self.disable_all_items()
             message = self._message or self.parent
             if message:
-                m = await message.edit(view=self)
+                m = await message.edit(View=self)
                 if m:
                     self._message = m
 
     async def on_check_failure(self, interaction: Interaction) -> None:
         """|coro|
         A callback that is called when a :meth:`View.interaction_check` returns ``False``.
         This can be used to send a response when a check failure occurs.
@@ -400,15 +400,15 @@
         error: :class:`Exception`
             The exception that was raised.
         item: :class:`Item`
             The item that failed the dispatch.
         interaction: :class:`~discord.Interaction`
             The interaction that led to the failure.
         """
-        print(f"Ignoring exception in view {self} for item {item}:", file=sys.stderr)
+        print(f"Ignoring exception in View {self} for item {item}:", file=sys.stderr)
         traceback.print_exception(
             error.__class__, error, error.__traceback__, file=sys.stderr
         )
 
     async def _scheduled_task(self, item: Item, interaction: Interaction):
         try:
             if self.timeout:
@@ -419,42 +419,42 @@
                 return await self.on_check_failure(interaction)
 
             await item.callback(interaction)
         except Exception as e:
             return await self.on_error(e, item, interaction)
 
     def _start_listening_from_store(self, store: ViewStore) -> None:
-        self.__cancel_callback = partial(store.remove_view)
+        self.__cancel_callback = partial(store.remove_View)
         if self.timeout:
             loop = asyncio.get_running_loop()
             if self.__timeout_task is not None:
                 self.__timeout_task.cancel()
 
             self.__timeout_expiry = time.monotonic() + self.timeout
             self.__timeout_task = loop.create_task(self.__timeout_task_impl())
 
     def _dispatch_timeout(self):
         if self.__stopped.done():
             return
 
         self.__stopped.set_result(True)
         asyncio.create_task(
-            self.on_timeout(), name=f"discord-ui-view-timeout-{self.id}"
+            self.on_timeout(), name=f"discord-ui-View-timeout-{self.id}"
         )
 
     def _dispatch_item(self, item: Item, interaction: Interaction):
         if self.__stopped.done():
             return
 
         if interaction.message:
             self.message = interaction.message
 
         asyncio.create_task(
             self._scheduled_task(item, interaction),
-            name=f"discord-ui-view-dispatch-{self.id}",
+            name=f"discord-ui-View-dispatch-{self.id}",
         )
 
     def refresh(self, components: list[Component]):
         # This is pretty hacky at the moment
         old_state: dict[tuple[int, str], Item] = {
             (item.type.value, item.custom_id): item for item in self.children if item.is_dispatchable()  # type: ignore
         }
@@ -472,15 +472,15 @@
             else:
                 older.refresh_component(component)
                 children.append(older)
 
         self.children = children
 
     def stop(self) -> None:
-        """Stops listening to interaction events from this view.
+        """Stops listening to interaction events from this View.
 
         This operation cannot be undone.
         """
         if not self.__stopped.done():
             self.__stopped.set_result(False)
 
         self.__timeout_expiry = None
@@ -489,66 +489,66 @@
             self.__timeout_task = None
 
         if self.__cancel_callback:
             self.__cancel_callback(self)
             self.__cancel_callback = None
 
     def is_finished(self) -> bool:
-        """Whether the view has finished interacting."""
+        """Whether the View has finished interacting."""
         return self.__stopped.done()
 
     def is_dispatching(self) -> bool:
-        """Whether the view has been added for dispatching purposes."""
+        """Whether the View has been added for dispatching purposes."""
         return self.__cancel_callback is not None
 
     def is_persistent(self) -> bool:
-        """Whether the view is set up as persistent.
+        """Whether the View is set up as persistent.
 
-        A persistent view has all their components with a set ``custom_id`` and
+        A persistent View has all their components with a set ``custom_id`` and
         a :attr:`timeout` set to ``None``.
         """
         return self.timeout is None and all(
             item.is_persistent() for item in self.children
         )
 
     async def wait(self) -> bool:
-        """Waits until the view has finished interacting.
+        """Waits until the View has finished interacting.
 
-        A view is considered finished when :meth:`stop`
+        A View is considered finished when :meth:`stop`
         is called, or it times out.
 
         Returns
         -------
         :class:`bool`
-            If ``True``, then the view timed out. If ``False`` then
-            the view finished normally.
+            If ``True``, then the View timed out. If ``False`` then
+            the View finished normally.
         """
         return await self.__stopped
 
     def disable_all_items(self, *, exclusions: list[Item] | None = None) -> None:
         """
-        Disables all items in the view.
+        Disables all items in the View.
 
         Parameters
         ----------
         exclusions: Optional[List[:class:`Item`]]
-            A list of items in `self.children` to not disable from the view.
+            A list of items in `self.children` to not disable from the View.
         """
         for child in self.children:
             if exclusions is None or child not in exclusions:
                 child.disabled = True
 
     def enable_all_items(self, *, exclusions: list[Item] | None = None) -> None:
         """
-        Enables all items in the view.
+        Enables all items in the View.
 
         Parameters
         ----------
         exclusions: Optional[List[:class:`Item`]]
-            A list of items in `self.children` to not enable from the view.
+            A list of items in `self.children` to not enable from the View.
         """
         for child in self.children:
             if exclusions is None or child not in exclusions:
                 child.disabled = False
 
     @property
     def message(self):
@@ -558,77 +558,77 @@
     def message(self, value):
         self._message = value
 
 
 class ViewStore:
     def __init__(self, state: ConnectionState):
         # (component_type, message_id, custom_id): (View, Item)
-        self._views: dict[tuple[int, int | None, str], tuple[View, Item]] = {}
+        self._Views: dict[tuple[int, int | None, str], tuple[View, Item]] = {}
         # message_id: View
-        self._synced_message_views: dict[int, View] = {}
+        self._synced_message_Views: dict[int, View] = {}
         self._state: ConnectionState = state
 
     @property
-    def persistent_views(self) -> Sequence[View]:
-        views = {
-            view.id: view
-            for (_, (view, _)) in self._views.items()
-            if view.is_persistent()
+    def persistent_Views(self) -> Sequence[View]:
+        Views = {
+            View.id: View
+            for (_, (View, _)) in self._Views.items()
+            if View.is_persistent()
         }
-        return list(views.values())
+        return list(Views.values())
 
     def __verify_integrity(self):
         to_remove: list[tuple[int, int | None, str]] = []
-        for k, (view, _) in self._views.items():
-            if view.is_finished():
+        for k, (View, _) in self._Views.items():
+            if View.is_finished():
                 to_remove.append(k)
 
         for k in to_remove:
-            del self._views[k]
+            del self._Views[k]
 
-    def add_view(self, view: View, message_id: int | None = None):
+    def add_View(self, View: View, message_id: int | None = None):
         self.__verify_integrity()
 
-        view._start_listening_from_store(self)
-        for item in view.children:
+        View._start_listening_from_store(self)
+        for item in View.children:
             if item.is_dispatchable():
-                self._views[(item.type.value, message_id, item.custom_id)] = (view, item)  # type: ignore
+                self._Views[(item.type.value, message_id, item.custom_id)] = (View, item)  # type: ignore
 
         if message_id is not None:
-            self._synced_message_views[message_id] = view
+            self._synced_message_Views[message_id] = View
 
-    def remove_view(self, view: View):
-        for item in view.children:
+    def remove_View(self, View: View):
+        for item in View.children:
             if item.is_dispatchable():
-                self._views.pop((item.type.value, item.custom_id), None)  # type: ignore
+                self._Views.pop((item.type.value, item.custom_id), None)  # type: ignore
 
-        for key, value in self._synced_message_views.items():
-            if value.id == view.id:
-                del self._synced_message_views[key]
+        for key, value in self._synced_message_Views.items():
+            if value.id == View.id:
+                del self._synced_message_Views[key]
                 break
 
     def dispatch(self, component_type: int, custom_id: str, interaction: Interaction):
         self.__verify_integrity()
         message_id: int | None = interaction.message and interaction.message.id
         key = (component_type, message_id, custom_id)
-        # Fallback to None message_id searches in case a persistent view
+        # Fallback to None message_id searches in case a persistent View
         # was added without an associated message_id
-        value = self._views.get(key) or self._views.get(
+        value = self._Views.get(key) or self._Views.get(
             (component_type, None, custom_id)
         )
         if value is None:
             return
 
-        view, item = value
+        View, item = value
         item.refresh_state(interaction)
-        view._dispatch_item(item, interaction)
+        View._dispatch_item(item, interaction)
 
     def is_message_tracked(self, message_id: int):
-        return message_id in self._synced_message_views
+        return message_id in self._synced_message_Views
 
     def remove_message_tracking(self, message_id: int) -> View | None:
-        return self._synced_message_views.pop(message_id, None)
+        return self._synced_message_Views.pop(message_id, None)
 
     def update_from_message(self, message_id: int, components: list[ComponentPayload]):
         # pre-req: is_message_tracked == true
-        view = self._synced_message_views[message_id]
-        view.refresh([_component_factory(d) for d in components])
+        View = self._synced_message_Views[message_id]
+        View.refresh([_component_factory(d) for d in components])
```

### Comparing `discordia-0.1/discord/user.py` & `discordia-0.2/discord/user.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/utils.py` & `discordia-0.2/discord/utils.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/voice_client.py` & `discordia-0.2/discord/voice_client.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/webhook/async_.py` & `discordia-0.2/discord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/webhook/sync.py` & `discordia-0.2/discord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/welcome_screen.py` & `discordia-0.2/discord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discord/widget.py` & `discordia-0.2/discord/widget.py`

 * *Files identical despite different names*

### Comparing `discordia-0.1/discordia.egg-info/PKG-INFO` & `discordia-0.2/discordia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordia
-Version: 0.1
+Version: 0.2
 Summary: A Python wrapper for the Discord API
 Author: discordia Development
 License: MIT
 Project-URL: Homepage, https://discordia.dev
 Project-URL: Changelog, https://docs.discordia.dev/en/master/changelog.html
 Project-URL: Source, https://github.com/discordia-Development/discordia
 Project-URL: Documentation, https://docs.discordia.dev
```

### Comparing `discordia-0.1/discordia.egg-info/SOURCES.txt` & `discordia-0.2/discordia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discordia-0.1/pyproject.toml` & `discordia-0.2/pyproject.toml`

 * *Files identical despite different names*

