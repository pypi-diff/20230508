# Comparing `tmp/atproto-0.0.2.tar.gz` & `tmp/atproto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.2.tar", max compression
+gzip compressed data, was "atproto-0.0.3.tar", max compression
```

## Comparing `atproto-0.0.2.tar` & `atproto-0.0.3.tar`

### file list

```diff
@@ -1,151 +1,152 @@
--rw-r--r--   0        0        0     1061 2023-05-06 18:19:17.839834 atproto-0.0.2/LICENSE
--rw-r--r--   0        0        0     9736 2023-05-06 18:19:17.839834 atproto-0.0.2/README.md
--rw-r--r--   0        0        0      300 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/__init__.py
--rw-r--r--   0        0        0      619 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/cid/__init__.py
--rw-r--r--   0        0        0       23 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/cli/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-06 18:19:17.839834 atproto-0.0.2/atproto/codegen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/clients/__init__.py
--rw-r--r--   0        0        0     1156 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/clients/generate_async_client.py
--rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/models/__init__.py
--rw-r--r--   0        0        0     2317 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/models/builder.py
--rw-r--r--   0        0        0    17423 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/models/generator.py
--rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/namespaces/__init__.py
--rw-r--r--   0        0        0     2562 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/namespaces/builder.py
--rw-r--r--   0        0        0    11855 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/codegen/namespaces/generator.py
--rw-r--r--   0        0        0      891 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/lexicon/__init__.py
--rw-r--r--   0        0        0     4658 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/lexicon/models.py
--rw-r--r--   0        0        0     3871 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/lexicon/parser.py
--rw-r--r--   0        0        0     5298 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/nsid/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/uri/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/__init__.py
--rw-r--r--   0        0        0     5994 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/async_client.py
--rw-r--r--   0        0        0      489 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/async_raw.py
--rw-r--r--   0        0        0     3719 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/base.py
--rw-r--r--   0        0        0     5555 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/client.py
--rw-r--r--   0        0        0      469 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/client/raw.py
--rw-r--r--   0        0        0    10098 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/__init__.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/__init__.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/__init__.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     3057 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      836 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      890 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0     1014 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      927 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/profile.py
--rw-r--r--   0        0        0     1061 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      970 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1417 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2163 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1145 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     3776 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1041 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0     1449 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0     1039 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      855 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0     1181 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0     1066 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      734 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2257 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/post.py
--rw-r--r--   0        0        0      738 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/repost.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      665 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/block.py
--rw-r--r--   0        0        0      667 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/follow.py
--rw-r--r--   0        0        0     1004 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0     1133 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0     1123 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      999 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      574 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      576 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      830 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1845 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      586 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1551 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      297 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/base.py
--rw-r--r--   0        0        0      713 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/blob_ref.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/__init__.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/__init__.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0     8856 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      712 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0     1071 2023-05-06 18:19:17.843834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      839 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0     1097 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      839 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1161 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      890 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      824 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      953 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      911 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0     1129 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1341 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      651 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      621 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      887 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      586 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1191 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      957 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0     1452 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      825 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1898 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0     1222 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      969 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0     1024 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1157 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1747 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1305 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      644 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      742 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      983 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      880 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0     1282 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0     1117 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1183 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/defs.py
--rw-r--r--   0        0        0      659 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0     1211 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0     1028 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      704 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      956 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      729 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      589 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      628 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      583 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0      323 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      752 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      744 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      822 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      986 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      764 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      872 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      916 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      969 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0     1201 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      637 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      640 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2426 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0     2810 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/models/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/__init__.py
--rw-r--r--   0        0        0    65433 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/async_ns.py
--rw-r--r--   0        0        0      361 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/base.py
--rw-r--r--   0        0        0    64495 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/namespaces/sync_ns.py
--rw-r--r--   0        0        0     4353 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_client/request.py
--rw-r--r--   0        0        0       43 2023-05-06 18:19:17.847834 atproto-0.0.2/atproto/xrpc_server/__init__.py
--rw-r--r--   0        0        0     2083 2023-05-06 18:19:17.859834 atproto-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    11556 1970-01-01 00:00:00.000000 atproto-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-08 19:05:45.792914 atproto-0.0.3/LICENSE
+-rw-r--r--   0        0        0     9776 2023-05-08 19:05:45.792914 atproto-0.0.3/README.md
+-rw-r--r--   0        0        0      300 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/__init__.py
+-rw-r--r--   0        0        0      619 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/cid/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/cli/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0     1156 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0     2317 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    18794 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0     2562 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11855 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0      944 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0     4658 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3871 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5298 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/uri/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0     5994 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0     3719 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     5555 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0      469 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    10098 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     3057 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      836 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      890 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0     1014 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      927 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0     1061 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      970 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1417 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2248 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1192 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     3913 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1041 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1449 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0     1076 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      855 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1181 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0     1066 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      734 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2298 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      738 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0      667 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0     1004 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1133 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1123 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      999 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      574 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      576 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      830 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1859 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      586 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1580 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      553 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0     9028 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      712 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0     1071 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      839 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0     1097 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      839 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1161 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      890 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      824 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      953 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      911 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1129 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1370 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      651 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      621 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      586 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1191 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0      957 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0     1499 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      825 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1972 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1236 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      969 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1038 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1171 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1761 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1319 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      644 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      742 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      983 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      880 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1282 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0     1117 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1183 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      659 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1211 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0     1028 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      704 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      956 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      729 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      589 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      628 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      583 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      744 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      822 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      986 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      764 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      872 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      916 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      969 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1201 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      637 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      640 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2426 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      425 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/models/type_conversion.py
+-rw-r--r--   0        0        0     3175 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0    65433 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      361 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    64495 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4353 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0     2083 2023-05-08 19:05:45.808914 atproto-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11596 1970-01-01 00:00:00.000000 atproto-0.0.3/PKG-INFO
```

### Comparing `atproto-0.0.2/LICENSE` & `atproto-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/README.md` & `atproto-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     <a href="https://discord.gg/PCyVJXU9jN">
         Discord Bluesky API
     </a>
 </p>
 
 ## The AT Protocol SDK
 
-> ⚠️ Under construction. The SDK was built from scratch for 40 hours. Somewhere I speedran. I have a list of things that will break backward compatibility. Until the 1.0.0 release, I am not going to care about it. 
+> ⚠️ Under construction. The SDK was built from scratch in 40 hours. Somewhere I speedran. I have a list of things that will break backward compatibility. Until the 1.0.0 release, I am not going to care about it. 
 
 Code snippet:
 ```python
 from atproto import Client
 
 
 def main():
@@ -59,14 +59,15 @@
     print('Welcome,', profile.displayName)
     
     post_ref = await client.send_post(text='Hello World from Python!')
     await client.like(post_ref)
 
     
 if __name__ == '__main__':
+    # use run() for higher Python version
     asyncio.get_event_loop().run_until_complete(main())
 
 ```
 </details>
 
 ### Introduction
 
@@ -87,15 +88,15 @@
 #### From main branch of the repository
 ``` bash
 pip install -U git+https://github.com/MarshalX/atproto.git
 ```
 
 ### Quick start
 
-First of all, you need to create the instance of the XRPC Client. To do so you have 2 major options: asynchronous, and synchronous. The dereference only in import and how you call the methods. If you are not familiar with async use sync instead.
+First of all, you need to create the instance of the XRPC Client. To do so you have 2 major options: asynchronous, and synchronous. The difference only in import and how you call the methods. If you are not familiar with async use sync instead.
 
 For sync:
 ```python
 from atproto import Client
 
 client = Client()
 # by default, it uses the server of bsky.app. To change this behaviour pass the base api URL to constructor
```

### Comparing `atproto-0.0.2/atproto/cid/__init__.py` & `atproto-0.0.3/atproto/cid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/codegen/__init__.py` & `atproto-0.0.3/atproto/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/codegen/clients/generate_async_client.py` & `atproto-0.0.3/atproto/codegen/clients/generate_async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/codegen/models/builder.py` & `atproto-0.0.3/atproto/codegen/models/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/codegen/models/generator.py` & `atproto-0.0.3/atproto/codegen/models/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     append_code(_MODELS_OUTPUT_DIR.joinpath(path_to_file), code)
 
 
 def _get_model_imports() -> str:
     # TODO(MarshalX): isort can't delete unused imports. mb add ruff
     lines = [
         'from dataclasses import dataclass',
-        'from typing import TYPE_CHECKING, Any, List, Optional, Type, Union',
+        'from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union',
         '',
         'from typing_extensions import Literal',
         'from atproto.xrpc_client import models',
         'from atproto.xrpc_client.models import base',
         'from atproto.xrpc_client.models.blob_ref import BlobRef',
         '',
         'from atproto import CID',
@@ -142,24 +142,31 @@
 
 def _get_ref_union_typehint(nsid: NSID, field_type_def, *, optional: bool) -> str:
     def_names = []
     for ref in field_type_def.refs:
         import_path, _ = _resolve_nsid_ref(nsid, ref)
         def_names.append(import_path)
 
+    # unbelievable but it's true. If schema doesn't describe the right type in Union
+    # we should fall back to the plain data
+    # maybe it's for the records that have custom fields... idk
+    # ref: https://github.com/bluesky-social/atproto/blob/b01e47b61730d05a780f7a42667b91ccaa192e8e/packages/lex-cli/src/codegen/lex-gen.ts#L325
+    # grep by "{$type: string; [k: string]: unknown}" string
+    def_names.append('Dict[str, Any]')
+
     def_names = ', '.join([f"'{name}'" for name in def_names])
     return _get_optional_typehint(f"Union[{def_names}]", optional=optional)
 
 
 def _get_model_field_typehint(nsid: NSID, field_name: str, field_type_def, *, optional: bool) -> str:
     field_type = type(field_type_def)
 
     if field_type == models.LexUnknown:
-        # TODO(MarshalX): it's record. think about could we add useful typehint
-        return _get_optional_typehint('Any', optional=optional)
+        # TODO(MarshalX): some of "unknown" types are well known...
+        return _get_optional_typehint(f"'base.RecordModelBase'", optional=optional)
 
     type_hint = _LEXICON_TYPE_TO_PRIMITIVE_TYPEHINT.get(field_type)
     if type_hint:
         return _get_optional_typehint(type_hint, optional=optional)
 
     if field_type is models.LexArray:
         items_type_hint = _get_model_field_typehint(nsid, field_name, field_type_def.items, optional=False)
@@ -396,14 +403,36 @@
 
         for def_name, def_record in defs.items():
             if isinstance(def_record, models.LexRecord):
                 # TODO(MarshalX): Process somehow def_record.key?
                 save_code_part(nsid, _generate_def_model(nsid, def_name, def_record.record, ModelType.RECORD))
 
 
+def _generate_record_type_database(lex_db: builder.LexDB) -> None:
+    lines = ['from atproto.xrpc_client import models', 'RECORD_TYPE_TO_MODEL_CLASS = {']
+
+    for nsid, defs in lex_db.items():
+        _save_code_import_if_not_exist(nsid)
+
+        for def_name, def_record in defs.items():
+            # for now there are records only in under "main" definition name.
+            # need to rework a bit if this behaviour will be changed
+            if isinstance(def_record, models.LexRecord):
+                class_name = get_def_model_name(def_name)
+                record_type = str(nsid)
+
+                path_to_class = f'models.{get_import_path(nsid)}.{class_name}'
+
+                lines.append(f"'{record_type}': {path_to_class},")
+
+    lines.append('}')
+
+    write_code(_MODELS_OUTPUT_DIR.joinpath('type_conversion.py'), join_code(lines))
+
+
 def _generate_ref_models(lex_db: builder.LexDB) -> None:
     for nsid, defs in lex_db.items():
         definition = defs['main']
         if hasattr(definition, 'input') and definition.input and definition.input.schema:
             if isinstance(definition.input.schema, models.LexRef):
                 save_code_part(nsid, _get_model_ref(nsid, definition.input.schema))
 
@@ -501,15 +530,18 @@
 
 
 def generate_models():
     _generate_params_models(builder.build_params_models())
     _generate_data_models(builder.build_data_models())
     _generate_response_models(builder.build_response_models())
     _generate_def_models(builder.build_def_models())
+
     _generate_record_models(builder.build_record_models())
+    _generate_record_type_database(builder.build_record_models())
+
     # refs should be generated at the end!
     _generate_ref_models(builder.build_refs_models())
 
     _generate_empty_init_files(_MODELS_OUTPUT_DIR)
     _generate_import_aliases(_MODELS_OUTPUT_DIR)
 
     format_code(_MODELS_OUTPUT_DIR)
```

### Comparing `atproto-0.0.2/atproto/codegen/namespaces/builder.py` & `atproto-0.0.3/atproto/codegen/namespaces/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/codegen/namespaces/generator.py` & `atproto-0.0.3/atproto/codegen/namespaces/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/exceptions.py` & `atproto-0.0.3/atproto/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     ...
 
 
 class WrongTypeError(ModelFieldError):
     ...
 
 
+class ModelFieldNotFoundError(ModelError):
+    ...
+
+
 class NetworkError(AtProtocolError):
     ...
 
 
 class InvokeTimeoutError(NetworkError):
     ...
```

### Comparing `atproto-0.0.2/atproto/lexicon/models.py` & `atproto-0.0.3/atproto/lexicon/models.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/lexicon/parser.py` & `atproto-0.0.3/atproto/lexicon/parser.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/nsid/__init__.py` & `atproto-0.0.3/atproto/nsid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/uri/__init__.py` & `atproto-0.0.3/atproto/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/client/async_client.py` & `atproto-0.0.3/atproto/xrpc_client/client/async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/client/base.py` & `atproto-0.0.3/atproto/xrpc_client/client/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/client/client.py` & `atproto-0.0.3/atproto/xrpc_client/client/client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/__init__.py` & `atproto-0.0.3/atproto/xrpc_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/defs.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_profile.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/profile.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/search_actors.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/external.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/images.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/record.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
@@ -35,14 +35,15 @@
         record: Record.
     """
 
     record: Union[
         'models.AppBskyEmbedRecord.ViewRecord',
         'models.AppBskyEmbedRecord.ViewNotFound',
         'models.AppBskyEmbedRecord.ViewBlocked',
+        'Dict[str, Any]',
     ]
 
 
 @dataclass
 class ViewRecord(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.record`.
@@ -57,22 +58,23 @@
         indexedAt: Indexed at.
     """
 
     author: 'models.AppBskyActorDefs.ProfileViewBasic'
     cid: str
     indexedAt: str
     uri: str
-    value: Any
+    value: 'base.RecordModelBase'
     embeds: Optional[
         List[
             Union[
                 'models.AppBskyEmbedImages.View',
                 'models.AppBskyEmbedExternal.View',
                 'models.AppBskyEmbedRecord.View',
                 'models.AppBskyEmbedRecordWithMedia.View',
+                'Dict[str, Any]',
             ]
         ]
     ] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
 
 @dataclass
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Union
+from typing import Any, Dict, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
@@ -18,15 +18,15 @@
     """Definition model for :obj:`app.bsky.embed.recordWithMedia`.
 
     Attributes:
         record: Record.
         media: Media.
     """
 
-    media: Union['models.AppBskyEmbedImages.Main', 'models.AppBskyEmbedExternal.Main']
+    media: Union['models.AppBskyEmbedImages.Main', 'models.AppBskyEmbedExternal.Main', 'Dict[str, Any]']
     record: 'models.AppBskyEmbedRecord.Main'
 
     _type: str = 'app.bsky.embed.recordWithMedia'
 
 
 @dataclass
 class View(base.ModelBase):
@@ -34,9 +34,9 @@
     """Definition model for :obj:`app.bsky.embed.recordWithMedia`.
 
     Attributes:
         record: Record.
         media: Media.
     """
 
-    media: Union['models.AppBskyEmbedImages.View', 'models.AppBskyEmbedExternal.View']
+    media: Union['models.AppBskyEmbedImages.View', 'models.AppBskyEmbedExternal.View', 'Dict[str, Any]']
     record: 'models.AppBskyEmbedRecord.View'
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/defs.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class PostView(base.ModelBase):
@@ -30,22 +30,23 @@
         viewer: Viewer.
         labels: Labels.
     """
 
     author: 'models.AppBskyActorDefs.ProfileViewBasic'
     cid: str
     indexedAt: str
-    record: Any
+    record: 'base.RecordModelBase'
     uri: str
     embed: Optional[
         Union[
             'models.AppBskyEmbedImages.View',
             'models.AppBskyEmbedExternal.View',
             'models.AppBskyEmbedRecord.View',
             'models.AppBskyEmbedRecordWithMedia.View',
+            'Dict[str, Any]',
         ]
     ] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
     likeCount: Optional[int] = None
     replyCount: Optional[int] = None
     repostCount: Optional[int] = None
     viewer: Optional['models.AppBskyFeedDefs.ViewerState'] = None
@@ -73,15 +74,15 @@
     Attributes:
         post: Post.
         reply: Reply.
         reason: Reason.
     """
 
     post: 'models.AppBskyFeedDefs.PostView'
-    reason: Optional[Union['models.AppBskyFeedDefs.ReasonRepost']] = None
+    reason: Optional[Union['models.AppBskyFeedDefs.ReasonRepost', 'Dict[str, Any]']] = None
     reply: Optional['models.AppBskyFeedDefs.ReplyRef'] = None
 
 
 @dataclass
 class ReplyRef(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
@@ -122,22 +123,24 @@
 
     post: 'models.AppBskyFeedDefs.PostView'
     parent: Optional[
         Union[
             'models.AppBskyFeedDefs.ThreadViewPost',
             'models.AppBskyFeedDefs.NotFoundPost',
             'models.AppBskyFeedDefs.BlockedPost',
+            'Dict[str, Any]',
         ]
     ] = None
     replies: Optional[
         List[
             Union[
                 'models.AppBskyFeedDefs.ThreadViewPost',
                 'models.AppBskyFeedDefs.NotFoundPost',
                 'models.AppBskyFeedDefs.BlockedPost',
+                'Dict[str, Any]',
             ]
         ]
     ] = None
 
 
 @dataclass
 class NotFoundPost(base.ModelBase):
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_likes.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_likes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -35,8 +35,9 @@
         thread: Thread.
     """
 
     thread: Union[
         'models.AppBskyFeedDefs.ThreadViewPost',
         'models.AppBskyFeedDefs.NotFoundPost',
         'models.AppBskyFeedDefs.BlockedPost',
+        'Dict[str, Any]',
     ]
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_posts.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_posts.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/like.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/like.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/post.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ReplyRef(base.ModelBase):
@@ -74,14 +74,15 @@
     text: str
     embed: Optional[
         Union[
             'models.AppBskyEmbedImages.Main',
             'models.AppBskyEmbedExternal.Main',
             'models.AppBskyEmbedRecord.Main',
             'models.AppBskyEmbedRecordWithMedia.Main',
+            'Dict[str, Any]',
         ]
     ] = None
     entities: Optional[List['models.AppBskyFeedPost.Entity']] = None
     facets: Optional[List['models.AppBskyRichtextFacet.Main']] = None
     reply: Optional['models.AppBskyFeedPost.ReplyRef'] = None
 
     _type: str = 'app.bsky.feed.post'
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/feed/repost.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/repost.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/block.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/block.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/follow.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/follow.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_followers.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_followers.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_follows.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_follows.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, List, Optional
+from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -60,11 +60,11 @@
     """
 
     author: 'models.AppBskyActorDefs.ProfileView'
     cid: str
     indexedAt: str
     isRead: bool
     reason: str
-    record: Any
+    record: 'base.RecordModelBase'
     uri: str
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
     reasonSubject: Optional[str] = None
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/notification/update_seen.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/update_seen.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/richtext/facet.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/richtext/facet.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import List, Union
+from typing import Any, Dict, List, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
@@ -18,15 +18,15 @@
     """Definition model for :obj:`app.bsky.richtext.facet`.
 
     Attributes:
         index: Index.
         features: Features.
     """
 
-    features: List[Union['models.AppBskyRichtextFacet.Mention', 'models.AppBskyRichtextFacet.Link']]
+    features: List[Union['models.AppBskyRichtextFacet.Mention', 'models.AppBskyRichtextFacet.Link', 'Dict[str, Any]']]
     index: 'models.AppBskyRichtextFacet.ByteSlice'
 
     _type: str = 'app.bsky.richtext.facet'
 
 
 @dataclass
 class Mention(base.ModelBase):
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py` & `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/blob_ref.py` & `atproto-0.0.3/atproto/xrpc_client/models/blob_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/defs.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from typing_extensions import Literal
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
@@ -35,15 +35,15 @@
 
     action: 'models.ComAtprotoAdminDefs.ActionType'
     createdAt: str
     createdBy: str
     id: int
     reason: str
     resolvedReportIds: List[int]
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main']
+    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
     subjectBlobCids: List[str]
     createLabelVals: Optional[List[str]] = None
     negateLabelVals: Optional[List[str]] = None
     reversal: Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
 
 
 @dataclass
@@ -67,15 +67,15 @@
 
     action: 'models.ComAtprotoAdminDefs.ActionType'
     createdAt: str
     createdBy: str
     id: int
     reason: str
     resolvedReports: List['models.ComAtprotoAdminDefs.ReportView']
-    subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView']
+    subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView', 'Dict[str, Any]']
     subjectBlobs: List['models.ComAtprotoAdminDefs.BlobView']
     createLabelVals: Optional[List[str]] = None
     negateLabelVals: Optional[List[str]] = None
     reversal: Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
 
 
 @dataclass
@@ -135,15 +135,15 @@
     """
 
     createdAt: str
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
     resolvedByActionIds: List[int]
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main']
+    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
     reason: Optional[str] = None
 
 
 @dataclass
 class ReportViewDetail(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
@@ -159,15 +159,15 @@
     """
 
     createdAt: str
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
     resolvedByActions: List['models.ComAtprotoAdminDefs.ActionView']
-    subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView']
+    subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView', 'Dict[str, Any]']
     reason: Optional[str] = None
 
 
 @dataclass
 class RepoView(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
@@ -182,15 +182,15 @@
         invitedBy: Invited by.
     """
 
     did: str
     handle: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.Moderation'
-    relatedRecords: List[Any]
+    relatedRecords: List['base.RecordModelBase']
     email: Optional[str] = None
     invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
 
 
 @dataclass
 class RepoViewDetail(base.ModelBase):
 
@@ -208,15 +208,15 @@
         invites: Invites.
     """
 
     did: str
     handle: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.ModerationDetail'
-    relatedRecords: List[Any]
+    relatedRecords: List['base.RecordModelBase']
     email: Optional[str] = None
     invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
     invites: Optional[List['models.ComAtprotoServerDefs.InviteCode']] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
 
 @dataclass
@@ -248,15 +248,15 @@
 
     blobCids: List[str]
     cid: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.Moderation'
     repo: 'models.ComAtprotoAdminDefs.RepoView'
     uri: str
-    value: Any
+    value: 'base.RecordModelBase'
 
 
 @dataclass
 class RecordViewDetail(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
@@ -273,15 +273,15 @@
 
     blobs: List['models.ComAtprotoAdminDefs.BlobView']
     cid: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.ModerationDetail'
     repo: 'models.ComAtprotoAdminDefs.RepoView'
     uri: str
-    value: Any
+    value: 'base.RecordModelBase'
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
 
 @dataclass
 class Moderation(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
@@ -324,15 +324,15 @@
     """
 
     cid: str
     createdAt: str
     mimeType: str
     size: int
     details: Optional[
-        Union['models.ComAtprotoAdminDefs.ImageDetails', 'models.ComAtprotoAdminDefs.VideoDetails']
+        Union['models.ComAtprotoAdminDefs.ImageDetails', 'models.ComAtprotoAdminDefs.VideoDetails', 'Dict[str, Any]']
     ] = None
     moderation: Optional['models.ComAtprotoAdminDefs.Moderation'] = None
 
 
 @dataclass
 class ImageDetails(base.ModelBase):
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_record.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/get_repo.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/search_repos.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import List, Optional, Type, Union
+from typing import Any, Dict, List, Optional, Type, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -26,15 +26,15 @@
         reason: Reason.
         createdBy: Created by.
     """
 
     action: str
     createdBy: str
     reason: str
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main']
+    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
     createLabelVals: Optional[List[str]] = None
     negateLabelVals: Optional[List[str]] = None
     subjectBlobCids: Optional[List[str]] = None
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
 ResponseRef: Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/identity/update_handle.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/update_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/defs.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/query_labels.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/create_report.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/create_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -20,15 +20,15 @@
     Attributes:
         reasonType: Reason type.
         reason: Reason.
         subject: Subject.
     """
 
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main']
+    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
     reason: Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.moderation.createReport`.
@@ -42,9 +42,9 @@
         createdAt: Created at.
     """
 
     createdAt: str
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main']
+    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
     reason: Optional[str] = None
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/moderation/defs.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -26,14 +26,15 @@
 
     repo: str
     writes: List[
         Union[
             'models.ComAtprotoRepoApplyWrites.Create',
             'models.ComAtprotoRepoApplyWrites.Update',
             'models.ComAtprotoRepoApplyWrites.Delete',
+            'Dict[str, Any]',
         ]
     ]
     swapCommit: Optional[str] = None
     validate: Optional[bool] = None
 
 
 @dataclass
@@ -44,15 +45,15 @@
     Attributes:
         collection: Collection.
         rkey: Rkey.
         value: Value.
     """
 
     collection: str
-    value: Any
+    value: 'base.RecordModelBase'
     rkey: Optional[str] = None
 
 
 @dataclass
 class Update(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.repo.applyWrites`. Update an existing record.
@@ -61,15 +62,15 @@
         collection: Collection.
         rkey: Rkey.
         value: Value.
     """
 
     collection: str
     rkey: str
-    value: Any
+    value: 'base.RecordModelBase'
 
 
 @dataclass
 class Delete(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.repo.applyWrites`. Delete an existing record.
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/create_record.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/put_record.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,45 +2,47 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, Optional
+from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.createRecord`.
+    """Input data model for :obj:`com.atproto.repo.putRecord`.
 
     Attributes:
         repo: The handle or DID of the repo.
         collection: The NSID of the record collection.
         rkey: The key of the record.
         validate: Validate the record?
-        record: The record to create.
+        record: The record to write.
+        swapRecord: Compare and swap with the previous record by cid.
         swapCommit: Compare and swap with the previous commit by cid.
     """
 
     collection: str
-    record: Any
+    record: 'base.RecordModelBase'
     repo: str
-    rkey: Optional[str] = None
+    rkey: str
     swapCommit: Optional[str] = None
+    swapRecord: Optional[str] = None
     validate: Optional[bool] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.createRecord`.
+    """Output data model for :obj:`com.atproto.repo.putRecord`.
 
     Attributes:
         uri: Uri.
         cid: Cid.
     """
 
     cid: str
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/delete_record.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, List
+from typing import List
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
@@ -34,10 +34,10 @@
         didDoc: Did doc.
         collections: Collections.
         handleIsCorrect: Handle is correct.
     """
 
     collections: List[str]
     did: str
-    didDoc: Any
+    didDoc: 'base.RecordModelBase'
     handle: str
     handleIsCorrect: bool
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/get_record.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/get_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, Optional
+from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
@@ -37,9 +37,9 @@
     Attributes:
         uri: Uri.
         cid: Cid.
         value: Value.
     """
 
     uri: str
-    value: Any
+    value: 'base.RecordModelBase'
     cid: Optional[str] = None
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/list_records.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/list_records.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, List, Optional
+from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -59,8 +59,8 @@
         uri: Uri.
         cid: Cid.
         value: Value.
     """
 
     cid: str
     uri: str
-    value: Any
+    value: 'base.RecordModelBase'
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/put_record.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/create_record.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,47 +2,45 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Any, Optional
+from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.putRecord`.
+    """Input data model for :obj:`com.atproto.repo.createRecord`.
 
     Attributes:
         repo: The handle or DID of the repo.
         collection: The NSID of the record collection.
         rkey: The key of the record.
         validate: Validate the record?
-        record: The record to write.
-        swapRecord: Compare and swap with the previous record by cid.
+        record: The record to create.
         swapCommit: Compare and swap with the previous commit by cid.
     """
 
     collection: str
-    record: Any
+    record: 'base.RecordModelBase'
     repo: str
-    rkey: str
+    rkey: Optional[str] = None
     swapCommit: Optional[str] = None
-    swapRecord: Optional[str] = None
     validate: Optional[bool] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.putRecord`.
+    """Output data model for :obj:`com.atproto.repo.createRecord`.
 
     Attributes:
         uri: Uri.
         cid: Cid.
     """
 
     cid: str
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_account.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_app_password.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/create_session.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/defs.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/delete_account.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/delete_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/describe_server.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/describe_server.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/get_session.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/refresh_session.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/refresh_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/reset_password.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/reset_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_blob.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_head.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_head.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_record.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/get_repo.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/list_repos.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py` & `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/models/utils.py` & `atproto-0.0.3/atproto/xrpc_client/models/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,33 @@
 from atproto.exceptions import (
     MissingValueError,
     ModelError,
     ModelFieldError,
     UnexpectedFieldError,
     WrongTypeError,
 )
+from atproto.xrpc_client.models.base import RecordModelBase
 from atproto.xrpc_client.models.blob_ref import BlobRef
+from atproto.xrpc_client.models.type_conversion import RECORD_TYPE_TO_MODEL_CLASS
 
 if TYPE_CHECKING:
     from atproto.xrpc_client.request import Response
 
 M = TypeVar('M')
 
+
+def _record_model_type_hook(data: dict) -> RecordModelBase:
+    record_type = data.pop('$type')
+    return get_or_create_model(data, RECORD_TYPE_TO_MODEL_CLASS[record_type])
+
+
 _TYPE_HOOKS = {
     BlobRef: lambda ref: BlobRef.from_dict(ref),
     CID: lambda ref: CID.decode(ref),
+    RecordModelBase: _record_model_type_hook,
 }
 _DACITE_CONFIG = Config(type_hooks=_TYPE_HOOKS)
 
 
 def get_or_create_model(model_data: Union[dict], model: Type[M]) -> Optional[M]:
     if model_data is None:
         return None
```

### Comparing `atproto-0.0.2/atproto/xrpc_client/namespaces/async_ns.py` & `atproto-0.0.3/atproto/xrpc_client/namespaces/async_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/namespaces/sync_ns.py` & `atproto-0.0.3/atproto/xrpc_client/namespaces/sync_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/atproto/xrpc_client/request.py` & `atproto-0.0.3/atproto/xrpc_client/request.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.2/pyproject.toml` & `atproto-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atproto"
-version = "0.0.2"
+version = "0.0.3"
 description = "The AT Protocol SDK"
 authors = ["Ilya (Marshal) <ilya@marshal.dev>"]
 license = "MIT"
 repository = "https://github.com/MarshalX/atproto"
 readme = "README.md"
 keywords = ["library", "sdk", "codegen", "xrpc", "xrpc-client", "atprotocol", "atproto", "lexicon", "parser", "schema", "bluesky", "bluesky-api", "at", "uri", "atp", "nsid", "did", "cid"]
 classifiers = [
```

### Comparing `atproto-0.0.2/PKG-INFO` & `atproto-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atproto
-Version: 0.0.2
+Version: 0.0.3
 Summary: The AT Protocol SDK
 Home-page: https://github.com/MarshalX/atproto
 License: MIT
 Keywords: library,sdk,codegen,xrpc,xrpc-client,atprotocol,atproto,lexicon,parser,schema,bluesky,bluesky-api,at,uri,atp,nsid,did,cid
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 Requires-Python: >=3.7,<4.0
@@ -60,15 +60,15 @@
     <a href="https://discord.gg/PCyVJXU9jN">
         Discord Bluesky API
     </a>
 </p>
 
 ## The AT Protocol SDK
 
-> ⚠️ Under construction. The SDK was built from scratch for 40 hours. Somewhere I speedran. I have a list of things that will break backward compatibility. Until the 1.0.0 release, I am not going to care about it. 
+> ⚠️ Under construction. The SDK was built from scratch in 40 hours. Somewhere I speedran. I have a list of things that will break backward compatibility. Until the 1.0.0 release, I am not going to care about it. 
 
 Code snippet:
 ```python
 from atproto import Client
 
 
 def main():
@@ -100,14 +100,15 @@
     print('Welcome,', profile.displayName)
     
     post_ref = await client.send_post(text='Hello World from Python!')
     await client.like(post_ref)
 
     
 if __name__ == '__main__':
+    # use run() for higher Python version
     asyncio.get_event_loop().run_until_complete(main())
 
 ```
 </details>
 
 ### Introduction
 
@@ -128,15 +129,15 @@
 #### From main branch of the repository
 ``` bash
 pip install -U git+https://github.com/MarshalX/atproto.git
 ```
 
 ### Quick start
 
-First of all, you need to create the instance of the XRPC Client. To do so you have 2 major options: asynchronous, and synchronous. The dereference only in import and how you call the methods. If you are not familiar with async use sync instead.
+First of all, you need to create the instance of the XRPC Client. To do so you have 2 major options: asynchronous, and synchronous. The difference only in import and how you call the methods. If you are not familiar with async use sync instead.
 
 For sync:
 ```python
 from atproto import Client
 
 client = Client()
 # by default, it uses the server of bsky.app. To change this behaviour pass the base api URL to constructor
```

