# Comparing `tmp/ProjZ.py-2.4.4.tar.gz` & `tmp/ProjZ.py-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-2.4.4.tar", last modified: Sun Apr 30 22:26:00 2023, max compression
+gzip compressed data, was "ProjZ.py-2.4.5.tar", last modified: Mon May  8 17:31:13 2023, max compression
```

## Comparing `ProjZ.py-2.4.4.tar` & `ProjZ.py-2.4.5.tar`

### file list

```diff
@@ -1,100 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.690834 ProjZ.py-2.4.4/
--rw-rw-rw-   0        0        0     4076 2023-04-30 22:26:00.690834 ProjZ.py-2.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.061927 ProjZ.py-2.4.4/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2325 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3640 2023-04-29 17:20:16.000000 ProjZ.py-2.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.110101 ProjZ.py-2.4.4/projz/
--rw-rw-rw-   0        0        0      112 2023-04-30 20:29:06.000000 ProjZ.py-2.4.4/projz/__init__.py
--rw-rw-rw-   0        0        0     7271 2023-04-30 10:53:19.000000 ProjZ.py-2.4.4/projz/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.120485 ProjZ.py-2.4.4/projz/api/
--rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.136525 ProjZ.py-2.4.4/projz/api/control/
--rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/control/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/control/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.154662 ProjZ.py-2.4.4/projz/api/headers/
--rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/headers/__init__.py
--rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.4.4/projz/api/headers/abc_headers_provider.py
--rw-rw-rw-   0        0        0     2334 2023-04-29 15:38:12.000000 ProjZ.py-2.4.4/projz/api/headers/headers_provider.py
--rw-rw-rw-   0        0        0     4789 2023-04-30 22:24:02.000000 ProjZ.py-2.4.4/projz/api/request_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.160173 ProjZ.py-2.4.4/projz/api/secret/
--rw-rw-rw-   0        0        0      661 2023-04-30 20:41:57.000000 ProjZ.py-2.4.4/projz/api/secret/__init__.py
--rw-rw-rw-   0        0        0    11964 2023-04-29 15:20:01.000000 ProjZ.py-2.4.4/projz/api/secret/data.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.168846 ProjZ.py-2.4.4/projz/api/util/
--rw-rw-rw-   0        0        0       55 2023-04-30 20:41:25.000000 ProjZ.py-2.4.4/projz/api/util/__init__.py
--rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/util/copy_to_buffer_writer.py
--rw-rw-rw-   0        0        0    58016 2023-04-29 22:00:27.000000 ProjZ.py-2.4.4/projz/client.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.279593 ProjZ.py-2.4.4/projz/enum/
--rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/__init__.py
--rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/auth_purpose.py
--rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/auth_type.py
--rw-rw-rw-   0        0        0      165 2023-04-29 20:27:50.000000 ProjZ.py-2.4.4/projz/enum/chat_message_type.py
--rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/chat_query_type.py
--rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/chat_thread_type.py
--rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/circle_filter_type.py
--rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/circle_members_query_type.py
--rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/comment_type.py
--rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/content_region.py
--rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/currency_type.py
--rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/gender.py
--rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/object_type.py
--rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/party_query_type.py
--rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/upload_target.py
--rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/user_task_type.py
--rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/ws_event_type.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.290914 ProjZ.py-2.4.4/projz/error/
--rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/error/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/error/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.501891 ProjZ.py-2.4.4/projz/model/
--rw-rw-rw-   0        0        0     1140 2023-04-29 21:59:15.000000 ProjZ.py-2.4.4/projz/model/__init__.py
--rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/account.py
--rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/blocked_item_wrapper.py
--rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/blog.py
--rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/category.py
--rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/chat.py
--rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/chat_message.py
--rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/circle.py
--rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/comment.py
--rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/currency.py
--rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/default_background_media.py
--rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/dice.py
--rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/gift_box.py
--rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/link_info.py
--rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/media.py
--rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/member_title.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.593876 ProjZ.py-2.4.4/projz/model/parse/
--rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/parse/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/parse/parseutils.py
--rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/party.py
--rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/poll.py
--rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/qi_vote_full_info.py
--rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/qi_vote_info.py
--rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.636795 ProjZ.py-2.4.4/projz/model/response/
--rw-rw-rw-   0        0        0      198 2023-04-29 21:59:15.000000 ProjZ.py-2.4.4/projz/model/response/__init__.py
--rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/response/auth_result.py
--rw-rw-rw-   0        0        0      363 2023-04-29 21:58:26.000000 ProjZ.py-2.4.4/projz/model/response/block_users_info.py
--rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/response/member_titles_info.py
--rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/response/multi_invitation_code_info.py
--rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/rich_format.py
--rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/sticker.py
--rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/transfer_order.py
--rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/user.py
--rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/user_task.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.666953 ProjZ.py-2.4.4/projz/model/util/
--rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/util/__init__.py
--rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/util/paginated_list.py
--rw-rw-rw-   0        0        0     4388 2023-04-29 17:46:35.000000 ProjZ.py-2.4.4/projz/model/util/rich_format_builder.py
--rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/util/rich_format_text_builder.py
--rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/wallet.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.677834 ProjZ.py-2.4.4/projz/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/util/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/util/subscription_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.687782 ProjZ.py-2.4.4/projz/websocket/
--rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/websocket/__init__.py
--rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/websocket/websocket_listener.py
--rw-rw-rw-   0        0        0       42 2023-04-30 22:26:00.695823 ProjZ.py-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1980 2023-04-30 20:29:06.000000 ProjZ.py-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.301866 ProjZ.py-2.4.5/
+-rw-rw-rw-   0        0        0     3983 2023-05-08 17:31:13.302855 ProjZ.py-2.4.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.177152 ProjZ.py-2.4.5/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     3983 2023-05-08 17:31:13.000000 ProjZ.py-2.4.5/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2229 2023-05-08 17:31:13.000000 ProjZ.py-2.4.5/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:31:13.000000 ProjZ.py-2.4.5/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-05-08 17:31:13.000000 ProjZ.py-2.4.5/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-08 17:31:13.000000 ProjZ.py-2.4.5/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.182323 ProjZ.py-2.4.5/projz/
+-rw-rw-rw-   0        0        0      112 2023-05-08 17:31:10.000000 ProjZ.py-2.4.5/projz/__init__.py
+-rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.185339 ProjZ.py-2.4.5/projz/api/
+-rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.188293 ProjZ.py-2.4.5/projz/api/control/
+-rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/api/control/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/api/control/rpc.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.193313 ProjZ.py-2.4.5/projz/api/headers/
+-rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/api/headers/__init__.py
+-rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.4.5/projz/api/headers/abc_headers_provider.py
+-rw-rw-rw-   0        0        0     2773 2023-05-08 17:26:11.000000 ProjZ.py-2.4.5/projz/api/headers/headers_provider.py
+-rw-rw-rw-   0        0        0     4789 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/api/request_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.196269 ProjZ.py-2.4.5/projz/api/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/api/util/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/api/util/copy_to_buffer_writer.py
+-rw-rw-rw-   0        0        0    57414 2023-05-08 17:28:51.000000 ProjZ.py-2.4.5/projz/client.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.223574 ProjZ.py-2.4.5/projz/enum/
+-rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/auth_purpose.py
+-rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/auth_type.py
+-rw-rw-rw-   0        0        0      148 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/chat_message_type.py
+-rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/chat_query_type.py
+-rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/chat_thread_type.py
+-rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/circle_filter_type.py
+-rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/circle_members_query_type.py
+-rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/comment_type.py
+-rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/content_region.py
+-rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/currency_type.py
+-rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/gender.py
+-rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/object_type.py
+-rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/party_query_type.py
+-rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/upload_target.py
+-rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/user_task_type.py
+-rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/enum/ws_event_type.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.226561 ProjZ.py-2.4.5/projz/error/
+-rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/error/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/error/classes.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.271732 ProjZ.py-2.4.5/projz/model/
+-rw-rw-rw-   0        0        0     1102 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/account.py
+-rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/blocked_item_wrapper.py
+-rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/blog.py
+-rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/category.py
+-rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/chat.py
+-rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/chat_message.py
+-rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/circle.py
+-rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/comment.py
+-rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/currency.py
+-rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/default_background_media.py
+-rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/dice.py
+-rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/gift_box.py
+-rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/link_info.py
+-rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/media.py
+-rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/member_title.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.275717 ProjZ.py-2.4.5/projz/model/parse/
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/parse/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/parse/parseutils.py
+-rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/party.py
+-rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/poll.py
+-rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/qi_vote_full_info.py
+-rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/qi_vote_info.py
+-rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/reaction.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.287689 ProjZ.py-2.4.5/projz/model/response/
+-rw-rw-rw-   0        0        0      152 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/response/__init__.py
+-rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/response/auth_result.py
+-rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/response/member_titles_info.py
+-rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/response/multi_invitation_code_info.py
+-rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/rich_format.py
+-rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/sticker.py
+-rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/transfer_order.py
+-rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/user.py
+-rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/user_task.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.294669 ProjZ.py-2.4.5/projz/model/util/
+-rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/util/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/util/paginated_list.py
+-rw-rw-rw-   0        0        0     4330 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/util/rich_format_builder.py
+-rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/util/rich_format_text_builder.py
+-rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/model/wallet.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.297661 ProjZ.py-2.4.5/projz/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/util/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/util/subscription_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:13.300652 ProjZ.py-2.4.5/projz/websocket/
+-rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/websocket/__init__.py
+-rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.4.5/projz/websocket/websocket_listener.py
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:31:13.304856 ProjZ.py-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2023-05-08 17:31:10.000000 ProjZ.py-2.4.5/setup.py
```

### Comparing `ProjZ.py-2.4.4/PKG-INFO` & `ProjZ.py-2.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.4.4
+Version: 2.4.5
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
-Home-page: https://github.com/D4rkwat3r/ProjZ
-Author: D4rkwat3r
+Home-page: UNKNOWN
+Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ProjZ
 A simple asynchronous library for interaction with Project Z
 
-## Installation
- ```commandline
- pip install projz.py
- ```
-
 ### Example - login and get object id from link
 ```python3
 import projz
 from asyncio import get_event_loop
 
 client = projz.Client()
 
@@ -94,15 +89,15 @@
 
 
 if __name__ == "__main__":
     loop = get_event_loop()
     loop.run_until_complete(main())
     loop.run_forever()
 ```
-## Addition: Using CLI functions
+## Addition: Using CLI functions,
 ### Print available functions
 ```commandline
 python -m projz list-actions
 ```
 ### Login to an account with email and print info about it
 ```commandline
 python -m projz login --auth email --login yourlogin --password yourpassword
@@ -128,8 +123,7 @@
 python -m projz leave-circle --auth email --login yourlogin --password yourpassword --circle circlelink
 ```
 ### Listen for the chat messages
 ```commandline
 python -m projz listen --auth email --login yourlogin --password yourpassword
 ```
 
-
```

### Comparing `ProjZ.py-2.4.4/ProjZ.py.egg-info/PKG-INFO` & `ProjZ.py-2.4.5/ProjZ.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.4.4
+Version: 2.4.5
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
-Home-page: https://github.com/D4rkwat3r/ProjZ
-Author: D4rkwat3r
+Home-page: UNKNOWN
+Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ProjZ
 A simple asynchronous library for interaction with Project Z
 
-## Installation
- ```commandline
- pip install projz.py
- ```
-
 ### Example - login and get object id from link
 ```python3
 import projz
 from asyncio import get_event_loop
 
 client = projz.Client()
 
@@ -94,15 +89,15 @@
 
 
 if __name__ == "__main__":
     loop = get_event_loop()
     loop.run_until_complete(main())
     loop.run_forever()
 ```
-## Addition: Using CLI functions
+## Addition: Using CLI functions,
 ### Print available functions
 ```commandline
 python -m projz list-actions
 ```
 ### Login to an account with email and print info about it
 ```commandline
 python -m projz login --auth email --login yourlogin --password yourpassword
@@ -128,8 +123,7 @@
 python -m projz leave-circle --auth email --login yourlogin --password yourpassword --circle circlelink
 ```
 ### Listen for the chat messages
 ```commandline
 python -m projz listen --auth email --login yourlogin --password yourpassword
 ```
 
-
```

### Comparing `ProjZ.py-2.4.4/ProjZ.py.egg-info/SOURCES.txt` & `ProjZ.py-2.4.5/ProjZ.py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 projz/api/__init__.py
 projz/api/request_manager.py
 projz/api/control/__init__.py
 projz/api/control/rpc.py
 projz/api/headers/__init__.py
 projz/api/headers/abc_headers_provider.py
 projz/api/headers/headers_provider.py
-projz/api/secret/__init__.py
-projz/api/secret/data.txt
 projz/api/util/__init__.py
 projz/api/util/copy_to_buffer_writer.py
 projz/enum/__init__.py
 projz/enum/auth_purpose.py
 projz/enum/auth_type.py
 projz/enum/chat_message_type.py
 projz/enum/chat_query_type.py
@@ -66,15 +64,14 @@
 projz/model/user.py
 projz/model/user_task.py
 projz/model/wallet.py
 projz/model/parse/__init__.py
 projz/model/parse/parseutils.py
 projz/model/response/__init__.py
 projz/model/response/auth_result.py
-projz/model/response/block_users_info.py
 projz/model/response/member_titles_info.py
 projz/model/response/multi_invitation_code_info.py
 projz/model/util/__init__.py
 projz/model/util/paginated_list.py
 projz/model/util/rich_format_builder.py
 projz/model/util/rich_format_text_builder.py
 projz/util/__init__.py
```

### Comparing `ProjZ.py-2.4.4/README.md` & `ProjZ.py-2.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 # ProjZ
 A simple asynchronous library for interaction with Project Z
 
-## Installation
- ```commandline
- pip install projz.py
- ```
-
 ### Example - login and get object id from link
 ```python3
 import projz
 from asyncio import get_event_loop
 
 client = projz.Client()
 
@@ -81,15 +76,15 @@
 
 
 if __name__ == "__main__":
     loop = get_event_loop()
     loop.run_until_complete(main())
     loop.run_forever()
 ```
-## Addition: Using CLI functions
+## Addition: Using CLI functions,
 ### Print available functions
 ```commandline
 python -m projz list-actions
 ```
 ### Login to an account with email and print info about it
 ```commandline
 python -m projz login --auth email --login yourlogin --password yourpassword
@@ -113,8 +108,8 @@
 ### Leave from the circle
 ```commandline
 python -m projz leave-circle --auth email --login yourlogin --password yourpassword --circle circlelink
 ```
 ### Listen for the chat messages
 ```commandline
 python -m projz listen --auth email --login yourlogin --password yourpassword
-```
+```
```

### Comparing `ProjZ.py-2.4.4/projz/__main__.py` & `ProjZ.py-2.4.5/projz/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from argparse import ArgumentParser
 from asyncio import get_event_loop
 from asyncio import create_task
 from asyncio import gather
 from inspect import iscoroutinefunction
-from inspect import signature
 from sys import exit as sys_exit
 from . import *
 
 parser = ArgumentParser(description="ProjZ.py library command line interface")
 parser.add_argument("action", type=str, help="The action to be performed. "
                                              "You can view the list of possible actions by "
                                              "setting the value \"list-actions\"")
@@ -31,26 +30,21 @@
                 else func(*args, **kwargs)
         except Exception as e:
             print(f"Error: {e}")
 
     return wrapper
 
 
-def authenticated(func: Callable):
+def authenticated(func):
     def wrapper(*args, **kwargs):
         if cli_args.login is None or cli_args.password is None or cli_args.auth_type is None:
             print("Specify login, password and auth type.")
             return
-        loop = get_event_loop()
-        auth_result = loop.run_until_complete(login())
-        if len(signature(func).parameters) > 0:
-            args = (auth_result,) + args
-        return loop.run_until_complete(func(*args, **kwargs)) if iscoroutinefunction(func) \
+        return get_event_loop().run_until_complete(func(*args, **kwargs)) if iscoroutinefunction(func) \
             else func(*args, **kwargs)
-
     return wrapper
 
 
 async def login() -> AuthResult:
     return await (
         client.login_email if cli_args.auth_type == "email"
         else client.login_phone_number
@@ -68,15 +62,16 @@
 def action_list_actions():
     for i, key in enumerate(action_mapping, start=1):
         print(f"{i}. {key} - {action_mapping[key][1]}")
 
 
 @print_error
 @authenticated
-async def action_login(auth: AuthResult):
+async def action_login():
+    auth = await login()
     print(f"[+] Session ID: {auth.sid}")
     print(f"[+] Refresh token (secret): {auth.secret}")
     print("[+] Account:")
     print(f"    -- Email: {auth.account.email or '-'}")
     print(f"    -- Phone number: {auth.account.phone_number or '-'}")
     print(f"    -- Registration time: {auth.account.created_time or '-'}")
     print(f"    -- Registered IPv4: {auth.account.registered_ipv4 or '-'}")
@@ -98,14 +93,15 @@
 
 @print_error
 @authenticated
 async def action_link_info():
     if cli_args.info is None:
         print("Specify --info.")
         return
+    await login()
     info = await client.get_link_info(cli_args.info)
     print(f"[+] Path: {info.path or '-'}")
     print(f"[+] Object ID: {info.object_id or '-'}")
     print(f"[+] Object type: {info.object_type or '-'}")
     print(f"[+] Share link: {info.share_link or '-'}")
     print(f"[+] Parent type: {info.parent_type or '-'}")
 
@@ -115,47 +111,52 @@
 async def action_send_message():
     if cli_args.thread is None or cli_args.message is None or cli_args.repeat is None:
         print("Specify --thread, --message and --repeat.")
         return
     if cli_args.repeat == 0:
         print("Illegal argument (repeat=0).")
         return
+    await login()
 
     chat_id = (await client.get_link_info(cli_args.thread)).object_id
     results = await gather(*[create_task(safe_send_chat_message(chat_id)) for _ in range(cli_args.repeat)])
     sent = list(filter(lambda x: x, results))
 
     print(f"[{'+' if any(results) else '-'}] Sent: {len(sent)}/{len(results)}")
 
 
 @print_error
 @authenticated
 async def action_join_circle():
     if cli_args.circle is None:
         print("Specify --circle.")
         return
+    await login()
 
     await client.join_circle(cli_args.circle)
     print(f"[+] Joined successfully.")
 
 
 @print_error
 @authenticated
 async def action_leave_circle():
     if cli_args.circle is None:
         print("Specify --circle.")
         return
+    await login()
 
     await client.leave_circle(cli_args.circle)
     print(f"[+] Left successfully.")
 
 
 @print_error
 @authenticated
 async def action_listen():
+    await login()
+
     client.register_chat_message_handler(
         lambda x: print(f"{x.author.nickname}: {x.content}"),
         lambda x: x.content is not None and x.author is not None
     )
     print(f"[+] Waiting for the messages...")
 
 action_mapping = {
```

### Comparing `ProjZ.py-2.4.4/projz/api/control/rpc.py` & `ProjZ.py-2.4.5/projz/api/control/rpc.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/api/headers/abc_headers_provider.py` & `ProjZ.py-2.4.5/projz/api/headers/abc_headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/api/request_manager.py` & `ProjZ.py-2.4.5/projz/api/request_manager.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/client.py` & `ProjZ.py-2.4.5/projz/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,17 @@
         birthday: str,
         code: str,
         name_card_background: Optional[Media] = None,
         invitation_code: Optional[str] = None,
         *,
         update_auth_credentials: bool = True
     ) -> AuthResult:
+        print("ProjZ.py: "
+              "Using the registration function in a public library is not recommended. "
+              "RPC functions are used.")
         data = {
             "purpose": 1,
             "password": password,
             "securityCode": code,
             "invitationCode": invitation_code or "",
             "nickname": nickname,
             "tagLine": tag_line,
@@ -380,63 +383,47 @@
                            message_type: Union[ChatMessageType, int] = 1,
                            content: Optional[str] = None,
                            reply_to: Optional[int] = None,
                            message_rich_format: Optional[RichFormat] = None,
                            attached_media: Optional[Media] = None,
                            attached_audio: Optional[Media] = None,
                            poll_id: Optional[int] = None,
-                           dice_id: Optional[int] = None,
-                           *,
-                           get_sent_message: bool = True) -> Optional[ChatMessage]:
+                           dice_id: Optional[int] = None) -> ChatMessage:
         """
         Send message to the chat
         :param thread_id: id of the chat
         :param message_type: ChatMessageType enum field or int identifier
         :param content: text content of the message
         :param reply_to: reply message id
         :param message_rich_format: RichFormat object, can be created by RichFormatBuilder
         :param attached_media: attached to the message file model.Media object
         :param attached_audio: attached to the message audio model.Media object
         :param poll_id: attached to the message poll id
         :param dice_id: attached to the message dice id
-        :param get_sent_message: If set to False, the request for information about the
-        sent message will not be executed and the function will return None.
         :return:
         """
         if attached_media is not None and attached_audio is not None:
             raise ValueError("You can't send audio and media in one message")
         seq_id = randint(0, maxsize)
         data = {
             "type": message_type if isinstance(message_type, int) else message_type.value,
             "threadId": thread_id,
             "uid": self.user_profile.uid,
             "seqId": seq_id,
             "extensions": {}
         }
         if content is not None: data["content"] = content
-        if reply_to is not None: data["extensions"]["replyMessageId"] = reply_to
+        if reply_to is not None: data["extensions"]["replyMessage"] = reply_to
         if message_rich_format is not None: data["richFormat"] = message_rich_format.to_dict()
         if attached_media is not None: data["media"] = attached_media.to_dict()
         if attached_audio is not None: data["media"] = attached_audio.to_dict()
         if poll_id is not None: data["extensions"]["pollId"] = poll_id
         if dice_id is not None: data["extensions"]["diceId"] = dice_id
         resp = await self.websocket.send_request(1, True, seq_id, **dict(threadId=thread_id, msg=data))
-        if get_sent_message:
-            return await self.get_chat_message(resp["threadId"], resp["messageId"])
-
-    async def show_typing(self, thread_id: int) -> None:
-        """
-        Displays the text to the chat members that the account is "typing".
-        :param thread_id: id of the chat
-        :return:
-        """
-        await self.send_message(thread_id, ChatMessageType.TYPING, get_sent_message=False)
-
-    async def get_block_users_info(self) -> BlockUsersInfo:
-        return BlockUsersInfo.from_dict(await self.get("/v1/users/block-uids"))
+        return await self.get_chat_message(resp["threadId"], resp["messageId"])
 
     async def get_link_info(self, link: str) -> LinkInfo:
         """
         Get object info by link
         :param link: object link
         :return: model.LinkInfo
         """
```

### Comparing `ProjZ.py-2.4.4/projz/enum/__init__.py` & `ProjZ.py-2.4.5/projz/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/error/classes.py` & `ProjZ.py-2.4.5/projz/error/classes.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/__init__.py` & `ProjZ.py-2.4.5/projz/model/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from .response import AuthResult
-from .response import MemberTitlesInfo
 from .response import MultiInvitationCodeInfo
-from .response import BlockUsersInfo
 from .util import PaginatedList
 from .util import RichFormatBuilder
 from .util import RichFormatTextBuilder
 from .media import Media
 from .account import Account
 from .user import User
 from .link_info import LinkInfo
@@ -19,14 +17,15 @@
 from .chat_message import ChatMessage
 from .poll import Poll
 from .dice import Dice
 from .rich_format import RichFormat
 from .qi_vote_info import QiVoteInfo
 from .qi_vote_full_info import QiVoteFullInfo
 from .member_title import MemberTitle
+from .response import MemberTitlesInfo
 from .comment import Comment
 from .currency import Currency
 from .user_task import UserTask
 from .wallet import Wallet
 from .gift_box import GiftBox
 from .transfer_order import TransferOrder
 from .party import Party
```

### Comparing `ProjZ.py-2.4.4/projz/model/account.py` & `ProjZ.py-2.4.5/projz/model/account.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/blocked_item_wrapper.py` & `ProjZ.py-2.4.5/projz/model/blocked_item_wrapper.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/blog.py` & `ProjZ.py-2.4.5/projz/model/blog.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/category.py` & `ProjZ.py-2.4.5/projz/model/category.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/chat.py` & `ProjZ.py-2.4.5/projz/model/chat.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/chat_message.py` & `ProjZ.py-2.4.5/projz/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/circle.py` & `ProjZ.py-2.4.5/projz/model/circle.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/comment.py` & `ProjZ.py-2.4.5/projz/model/comment.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/currency.py` & `ProjZ.py-2.4.5/projz/model/currency.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/default_background_media.py` & `ProjZ.py-2.4.5/projz/model/default_background_media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/gift_box.py` & `ProjZ.py-2.4.5/projz/model/gift_box.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/media.py` & `ProjZ.py-2.4.5/projz/model/media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/member_title.py` & `ProjZ.py-2.4.5/projz/model/member_title.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/parse/parseutils.py` & `ProjZ.py-2.4.5/projz/model/parse/parseutils.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/poll.py` & `ProjZ.py-2.4.5/projz/model/poll.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/qi_vote_full_info.py` & `ProjZ.py-2.4.5/projz/model/qi_vote_full_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/qi_vote_info.py` & `ProjZ.py-2.4.5/projz/model/qi_vote_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/reaction.py` & `ProjZ.py-2.4.5/projz/model/reaction.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/response/member_titles_info.py` & `ProjZ.py-2.4.5/projz/model/response/member_titles_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/response/multi_invitation_code_info.py` & `ProjZ.py-2.4.5/projz/model/response/multi_invitation_code_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/rich_format.py` & `ProjZ.py-2.4.5/projz/model/rich_format.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/transfer_order.py` & `ProjZ.py-2.4.5/projz/model/transfer_order.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/user.py` & `ProjZ.py-2.4.5/projz/model/user.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/user_task.py` & `ProjZ.py-2.4.5/projz/model/user_task.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/util/rich_format_builder.py` & `ProjZ.py-2.4.5/projz/model/util/rich_format_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,15 @@
     ) -> "RichFormatBuilder":
         self._fmt.text_spans.append(RichFormat.TextSpan(start, end, RichFormat.TextSpan.Data(
             bold, italic, strikethrough, underline, foreground, background
         )))
         return self
 
     def paragraph_span(self, start: int, end: int, style: Optional[str] = None, alignment: Optional[str] = None) -> "RichFormatBuilder":
-        self._fmt.paragraph_spans.append(
-            RichFormat.ParagraphSpan(start, end, RichFormat.ParagraphSpan.Data(style, alignment))
-        )
-        return self
-
-    def attachment_span(self, start: int, end: int, data: RichFormat.AttachmentSpan.Data) -> "RichFormatBuilder":
-        self._fmt.attachment_spans.append(
-            RichFormat.AttachmentSpan(start, end, data)
-        )
+        self._fmt.paragraph_spans.append(RichFormat.ParagraphSpan(start, end, RichFormat.ParagraphSpan.Data(style, alignment)))
         return self
 
     def bold(self, start: int, end: int) -> "RichFormatBuilder": return self.text_span(start, end, bold=True)
 
     def italic(self, start: int, end: int) -> "RichFormatBuilder": return self.text_span(start, end, italic=True)
 
     def strikethrough(self, start: int, end: int) -> "RichFormatBuilder": return self.text_span(start, end,strikethrough=True)
@@ -65,34 +57,38 @@
         self,
         start: int,
         url: str,
         custom_title: str = "",
         title: str = "",
         media_id: int = 0
     ) -> "RichFormatBuilder":
-        return self.attachment_span(start, start + 1, RichFormat.AttachmentSpan.Data(
+        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, start + 1, RichFormat.AttachmentSpan.Data(
             type="link",
             link=RichFormat.AttachmentSpan.Data.Link(url, custom_title, title, media_id, str(uuid4()))
-        ))
+        )))
+        return self
 
     def mention(self, start: int, username: str, uid: int, role_id: int = 0,
                 role_name_length: int = 0) -> "RichFormatBuilder":
         end = len(f"@{username}" if not username.startswith("@") else username)
-        return self.attachment_span(start, end, RichFormat.AttachmentSpan.Data(
+        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, end, RichFormat.AttachmentSpan.Data(
             type="mention",
             mention=RichFormat.AttachmentSpan.Data.Mention(uid, role_id, role_name_length)
-        ))
+        )))
+        return self
 
     def poll(self, start: int, poll_id: int) -> "RichFormatBuilder":
-        return self.attachment_span(start, start + 1, RichFormat.AttachmentSpan.Data(
+        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, start + 1, RichFormat.AttachmentSpan.Data(
             type="poll",
             poll=RichFormat.AttachmentSpan.Data.Poll(poll_id)
-        ))
+        )))
+        return self
 
     def media(self, start: int, media_id: int) -> "RichFormatBuilder":
-        return self.attachment_span(start, start + 1, RichFormat.AttachmentSpan.Data(
+        self._fmt.attachment_spans.append(RichFormat.AttachmentSpan(start, start + 1, RichFormat.AttachmentSpan.Data(
             type="media",
             media=RichFormat.AttachmentSpan.Data.Media(media_id)
-        ))
+        )))
+        return self
 
     def build(self) -> RichFormat:
         return self._fmt
```

### Comparing `ProjZ.py-2.4.4/projz/model/util/rich_format_text_builder.py` & `ProjZ.py-2.4.5/projz/model/util/rich_format_text_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/model/wallet.py` & `ProjZ.py-2.4.5/projz/model/wallet.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/util/subscription_handler.py` & `ProjZ.py-2.4.5/projz/util/subscription_handler.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/projz/websocket/websocket_listener.py` & `ProjZ.py-2.4.5/projz/websocket/websocket_listener.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.4/setup.py` & `ProjZ.py-2.4.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     return [
         "aiohttp",
         "aiofiles",
         "ujson",
         "dataclasses",
         "dataclasses-json",
         "python-dateutil",
-        "dill",
         "python-magic-bin" if system().lower() == "windows" else "python-magic"
     ]
 
 
 def main():
     if "PREFIX" in environ and "/com.termux" in environ["PREFIX"]:
         print("Termux detected, checking Sox package...")
@@ -33,25 +32,23 @@
             else:
                 print("Failed to install Sox. The stability of the library is not guaranteed.")
         else:
             print("Sox found, no installation required.")
 
     setup(
         name="ProjZ.py",
-        version="2.4.4",
-        author="D4rkwat3r",
+        version="2.4.5",
+        author="D4krwat3r",
         description="An asynchronous library for creating scripts and chatbots in Project Z.",
-        url="https://github.com/D4rkwat3r/ProjZ",
         packages=find_packages(),
         author_email="ktoya170214@gmail.com",
         install_requires=get_requirements(),
         long_description=get_readme(),
         long_description_content_type="text/markdown",
         python_requires=">=3.7",
-        package_data={"projz": ["api/secret/data.txt"]},
         keywords=[
             "project-z", "projectz", "projz",
             "bots", "api", "supersymlab",
             "projz-bot", "projz-bots", "projz-api",
         ]
     )
```

