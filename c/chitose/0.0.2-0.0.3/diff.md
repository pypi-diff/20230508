# Comparing `tmp/chitose-0.0.2.tar.gz` & `tmp/chitose-0.0.3.tar.gz`

## Comparing `chitose-0.0.2.tar` & `chitose-0.0.3.tar`

### file list

```diff
@@ -1,148 +1,154 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 chitose-0.0.2/.gitmodules
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 chitose-0.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/agent.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/object.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/record.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/xrpc.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/record.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/defs.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/post.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/repost.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/block.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/__init__.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/defs.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/defs.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/make.bat
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.actor.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.embed.rst
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.feed.rst
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.graph.rst
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.notification.rst
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.richtext.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.unspecced.rst
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.rst
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.admin.rst
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.identity.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.label.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.moderation.rst
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.repo.rst
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.rst
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.server.rst
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.sync.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.rst
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/conf.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/index.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/modules.rst
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chitose-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chitose-0.0.2/LICENSE
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 chitose-0.0.2/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 chitose-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 chitose-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 chitose-0.0.3/.gitmodules
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 chitose-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/agent.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/blob.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/link.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/object.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/record.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/xrpc.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/__init__.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/block.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/__init__.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/label/defs.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 chitose-0.0.3/chitose/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.actor.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.embed.rst
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.feed.rst
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.graph.rst
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.notification.rst
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.richtext.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.bsky.unspecced.rst
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.app.rst
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.admin.rst
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.identity.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.label.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.moderation.rst
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.repo.rst
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.rst
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.server.rst
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.atproto.sync.rst
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.com.rst
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/chitose.rst
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/conf.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/index.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chitose-0.0.3/docs/source/modules.rst
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 chitose-0.0.3/examples/get_profiles.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 chitose-0.0.3/examples/get_timeline.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 chitose-0.0.3/examples/post.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 chitose-0.0.3/examples/post_with_image.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chitose-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chitose-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 chitose-0.0.3/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 chitose-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 chitose-0.0.3/PKG-INFO
```

### Comparing `chitose-0.0.2/chitose/agent.py` & `chitose-0.0.3/chitose/agent.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/chitose/xrpc.py` & `chitose-0.0.3/chitose/xrpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import urllib.parse
 import urllib.request
 
 
 def call(method: str,
          params: list[tuple[str, Union[str, Optional[str],
                                        Optional[int], list[str]]]],
-         d: Optional[dict], service: str, headers: dict[str, str]) -> bytes:
+         d: Union[bytes, Optional[dict]], service: str, headers: dict[str, str]) -> bytes:
     url = f'{service}/xrpc/{method}'
 
     query: list[tuple[str, Union[str, int]]] = []
     for key, val in params:
         if val is None:
             continue
 
@@ -26,20 +26,24 @@
         url = f'{url}?{urllib.parse.urlencode(query)}'
 
     req = urllib.request.Request(url)
     for key, val in headers.items():
         req.add_header(key, val)
 
     if d:
-        d = {
-            key: val for key, val in d.items()
-            if val is not None
-        }
-        data = json.dumps(d, default=lambda obj: {
-                          key: val for key, val in obj.to_dict().items()
-                          if val is not None
-                          }).encode()
+        # for com.atproto.repo.uploadBlob
+        if isinstance(d, bytes):
+            data = d
+        else:
+            d = {
+                key: val for key, val in d.items()
+                if val is not None
+            }
+            data = json.dumps(d, default=lambda obj: {
+                              key: val for key, val in obj.to_dict().items()
+                              if val is not None
+                              }).encode()
     else:
         data = None
 
     r = urllib.request.urlopen(req, data)
     return r.read()
```

### Comparing `chitose-0.0.2/chitose/app/bsky/__init__.py` & `chitose-0.0.3/chitose/app/bsky/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from .feed import Feed_
 from .graph import Graph_
 from .notification import Notification_
 from .richtext import Richtext_
 from .unspecced import Unspecced_
 
 class Bsky_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
     @property
     def actor(self):
         return Actor_(self.service, self.headers)
```

### Comparing `chitose-0.0.2/chitose/app/bsky/actor/defs.py` & `chitose-0.0.3/chitose/app/bsky/actor/defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 # GENERATED CODE - DO NOT MODIFY
+"""A reference to an actor in the network."""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.com.atproto.label.defs
 import typing
 
 class ProfileViewBasic(chitose.Object):
+    """"""
 
     def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, avatar: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
         self.handle = handle
         self.display_name = display_name
         self.avatar = avatar
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self):
-        return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'avatar': self.avatar, 'viewer': self.viewer, 'labels': self.labels}
+    def to_dict(self) -> dict:
+        return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'avatar': self.avatar, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileViewBasic'}
 
 class ProfileView(chitose.Object):
+    """"""
 
     def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
         self.handle = handle
         self.display_name = display_name
         self.description = description
         self.avatar = avatar
         self.indexed_at = indexed_at
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self):
-        return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels}
+    def to_dict(self) -> dict:
+        return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileView'}
 
 class ProfileViewDetailed(chitose.Object):
+    """"""
 
     def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, banner: typing.Optional[str]=None, followers_count: typing.Optional[int]=None, follows_count: typing.Optional[int]=None, posts_count: typing.Optional[int]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
         self.handle = handle
         self.display_name = display_name
         self.description = description
         self.avatar = avatar
@@ -45,21 +49,22 @@
         self.followers_count = followers_count
         self.follows_count = follows_count
         self.posts_count = posts_count
         self.indexed_at = indexed_at
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self):
-        return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner, 'followersCount': self.followers_count, 'followsCount': self.follows_count, 'postsCount': self.posts_count, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels}
+    def to_dict(self) -> dict:
+        return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner, 'followersCount': self.followers_count, 'followsCount': self.follows_count, 'postsCount': self.posts_count, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileViewDetailed'}
 
 class ViewerState(chitose.Object):
+    """"""
 
     def __init__(self, muted: typing.Optional[str]=None, blocked_by: typing.Optional[str]=None, blocking: typing.Optional[str]=None, following: typing.Optional[str]=None, followed_by: typing.Optional[str]=None) -> None:
         self.muted = muted
         self.blocked_by = blocked_by
         self.blocking = blocking
         self.following = following
         self.followed_by = followed_by
 
-    def to_dict(self):
-        return {'muted': self.muted, 'blockedBy': self.blocked_by, 'blocking': self.blocking, 'following': self.following, 'followedBy': self.followed_by}
+    def to_dict(self) -> dict:
+        return {'muted': self.muted, 'blockedBy': self.blocked_by, 'blocking': self.blocking, 'following': self.following, 'followedBy': self.followed_by, '$type': 'app.bsky.actor.defs#viewerState'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/actor/profile.py` & `chitose-0.0.3/chitose/app/bsky/actor/profile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
 class Profile(chitose.Record):
+    """"""
 
-    def __init__(self, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[typing.Any]=None, banner: typing.Optional[typing.Any]=None) -> None:
+    def __init__(self, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[chitose.Blob]=None, banner: typing.Optional[chitose.Blob]=None) -> None:
         self.display_name = display_name
         self.description = description
         self.avatar = avatar
         self.banner = banner
 
-    def to_dict(self):
-        return {'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner}
+    def to_dict(self) -> dict:
+        return {'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner, '$type': 'app.bsky.actor.profile'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/embed/external.py` & `chitose-0.0.3/chitose/app/bsky/embed/external.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 # GENERATED CODE - DO NOT MODIFY
+"""A representation of some externally linked content, embedded in another form of content"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.embed.external
 import typing
 
 class External(chitose.Object):
+    """"""
 
     def __init__(self, external: chitose.app.bsky.embed.external.ExternalExternal) -> None:
         self.external = external
 
-    def to_dict(self):
-        return {'external': self.external}
+    def to_dict(self) -> dict:
+        return {'external': self.external, '$type': 'app.bsky.embed.external'}
 
 class ExternalExternal(chitose.Object):
+    """"""
 
-    def __init__(self, uri: str, title: str, description: str, thumb: typing.Optional[typing.Any]=None) -> None:
+    def __init__(self, uri: str, title: str, description: str, thumb: typing.Optional[chitose.Blob]=None) -> None:
         self.uri = uri
         self.title = title
         self.description = description
         self.thumb = thumb
 
-    def to_dict(self):
-        return {'uri': self.uri, 'title': self.title, 'description': self.description, 'thumb': self.thumb}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'title': self.title, 'description': self.description, 'thumb': self.thumb, '$type': 'app.bsky.embed.external#external'}
 
 class View(chitose.Object):
+    """"""
 
     def __init__(self, external: chitose.app.bsky.embed.external.ViewExternal) -> None:
         self.external = external
 
-    def to_dict(self):
-        return {'external': self.external}
+    def to_dict(self) -> dict:
+        return {'external': self.external, '$type': 'app.bsky.embed.external#view'}
 
 class ViewExternal(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, title: str, description: str, thumb: typing.Optional[str]=None) -> None:
         self.uri = uri
         self.title = title
         self.description = description
         self.thumb = thumb
 
-    def to_dict(self):
-        return {'uri': self.uri, 'title': self.title, 'description': self.description, 'thumb': self.thumb}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'title': self.title, 'description': self.description, 'thumb': self.thumb, '$type': 'app.bsky.embed.external#viewExternal'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/embed/images.py` & `chitose-0.0.3/chitose/app/bsky/embed/images.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # GENERATED CODE - DO NOT MODIFY
+"""A set of images embedded in some other form of content"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.embed.images
-import typing
 
 class Images(chitose.Object):
+    """"""
 
     def __init__(self, images: list[chitose.app.bsky.embed.images.Image]) -> None:
         self.images = images
 
-    def to_dict(self):
-        return {'images': self.images}
+    def to_dict(self) -> dict:
+        return {'images': self.images, '$type': 'app.bsky.embed.images'}
 
 class Image(chitose.Object):
+    """"""
 
-    def __init__(self, image: typing.Any, alt: str) -> None:
+    def __init__(self, image: chitose.Blob, alt: str) -> None:
         self.image = image
         self.alt = alt
 
-    def to_dict(self):
-        return {'image': self.image, 'alt': self.alt}
+    def to_dict(self) -> dict:
+        return {'image': self.image, 'alt': self.alt, '$type': 'app.bsky.embed.images#image'}
 
 class View(chitose.Object):
+    """"""
 
     def __init__(self, images: list[chitose.app.bsky.embed.images.ViewImage]) -> None:
         self.images = images
 
-    def to_dict(self):
-        return {'images': self.images}
+    def to_dict(self) -> dict:
+        return {'images': self.images, '$type': 'app.bsky.embed.images#view'}
 
 class ViewImage(chitose.Object):
+    """"""
 
     def __init__(self, thumb: str, fullsize: str, alt: str) -> None:
         self.thumb = thumb
         self.fullsize = fullsize
         self.alt = alt
 
-    def to_dict(self):
-        return {'thumb': self.thumb, 'fullsize': self.fullsize, 'alt': self.alt}
+    def to_dict(self) -> dict:
+        return {'thumb': self.thumb, 'fullsize': self.fullsize, 'alt': self.alt, '$type': 'app.bsky.embed.images#viewImage'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/embed/record.py` & `chitose-0.0.3/chitose/app/bsky/embed/record.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 # GENERATED CODE - DO NOT MODIFY
+"""A representation of a record embedded in another form of content"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import chitose.app.bsky.embed.record_with_media
 import chitose.com.atproto.label.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
 class Record(chitose.Object):
+    """"""
 
     def __init__(self, record: chitose.com.atproto.repo.strong_ref.StrongRef) -> None:
         self.record = record
 
-    def to_dict(self):
-        return {'record': self.record}
+    def to_dict(self) -> dict:
+        return {'record': self.record, '$type': 'app.bsky.embed.record'}
 
 class View(chitose.Object):
+    """"""
 
     def __init__(self, record: typing.Union[chitose.app.bsky.embed.record.ViewRecord, chitose.app.bsky.embed.record.ViewNotFound, chitose.app.bsky.embed.record.ViewBlocked]) -> None:
         self.record = record
 
-    def to_dict(self):
-        return {'record': self.record}
+    def to_dict(self) -> dict:
+        return {'record': self.record, '$type': 'app.bsky.embed.record#view'}
 
 class ViewRecord(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileViewBasic, value: typing.Any, indexed_at: str, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, embeds: typing.Optional[list[typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View, chitose.app.bsky.embed.record.View, chitose.app.bsky.embed.record_with_media.View]]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.author = author
         self.value = value
         self.indexed_at = indexed_at
         self.labels = labels
         self.embeds = embeds
 
-    def to_dict(self):
-        return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'value': self.value, 'indexedAt': self.indexed_at, 'labels': self.labels, 'embeds': self.embeds}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'value': self.value, 'indexedAt': self.indexed_at, 'labels': self.labels, 'embeds': self.embeds, '$type': 'app.bsky.embed.record#viewRecord'}
 
 class ViewNotFound(chitose.Object):
+    """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
 
-    def to_dict(self):
-        return {'uri': self.uri}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, '$type': 'app.bsky.embed.record#viewNotFound'}
 
 class ViewBlocked(chitose.Object):
+    """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
 
-    def to_dict(self):
-        return {'uri': self.uri}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, '$type': 'app.bsky.embed.record#viewBlocked'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/embed/record_with_media.py` & `chitose-0.0.3/chitose/app/bsky/embed/record_with_media.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # GENERATED CODE - DO NOT MODIFY
+"""A representation of a record embedded in another form of content, alongside other compatible embeds"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import typing
 
 class RecordWithMedia(chitose.Object):
+    """"""
 
     def __init__(self, record: chitose.app.bsky.embed.record.Record, media: typing.Union[chitose.app.bsky.embed.images.Images, chitose.app.bsky.embed.external.External]) -> None:
         self.record = record
         self.media = media
 
-    def to_dict(self):
-        return {'record': self.record, 'media': self.media}
+    def to_dict(self) -> dict:
+        return {'record': self.record, 'media': self.media, '$type': 'app.bsky.embed.recordWithMedia'}
 
 class View(chitose.Object):
+    """"""
 
     def __init__(self, record: chitose.app.bsky.embed.record.View, media: typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View]) -> None:
         self.record = record
         self.media = media
 
-    def to_dict(self):
-        return {'record': self.record, 'media': self.media}
+    def to_dict(self) -> dict:
+        return {'record': self.record, 'media': self.media, '$type': 'app.bsky.embed.recordWithMedia#view'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/feed/__init__.py` & `chitose-0.0.3/chitose/app/bsky/feed/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,35 +6,36 @@
 from .get_posts import _get_posts
 from .get_reposted_by import _get_reposted_by
 from .get_timeline import _get_timeline
 import chitose
 import typing
 
 class Feed_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_timeline(self, algorithm: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_timeline(self, algorithm: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A view of the user's home timeline."""
         return _get_timeline(self.service, self.headers, algorithm, limit, cursor)
 
-    def get_author_feed(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_author_feed(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """A view of an actor's feed."""
         return _get_author_feed(self.service, self.headers, actor, limit, cursor)
 
-    def get_likes(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_likes(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """"""
         return _get_likes(self.service, self.headers, uri, cid, limit, cursor)
 
-    def get_post_thread(self, uri: str, depth: typing.Optional[int]=None):
+    def get_post_thread(self, uri: str, depth: typing.Optional[int]=None) -> bytes:
         """"""
         return _get_post_thread(self.service, self.headers, uri, depth)
 
-    def get_reposted_by(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_reposted_by(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """"""
         return _get_reposted_by(self.service, self.headers, uri, cid, limit, cursor)
 
-    def get_posts(self, uris: list[str]):
+    def get_posts(self, uris: list[str]) -> bytes:
         """A view of an actor's feed."""
         return _get_posts(self.service, self.headers, uris)
```

### Comparing `chitose-0.0.2/chitose/app/bsky/feed/defs.py` & `chitose-0.0.3/chitose/app/bsky/feed/defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,103 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import chitose.app.bsky.embed.record_with_media
 import chitose.app.bsky.feed.defs
 import chitose.com.atproto.label.defs
 import typing
 
 class PostView(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileViewBasic, record: typing.Any, indexed_at: str, embed: typing.Optional[typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View, chitose.app.bsky.embed.record.View, chitose.app.bsky.embed.record_with_media.View]]=None, reply_count: typing.Optional[int]=None, repost_count: typing.Optional[int]=None, like_count: typing.Optional[int]=None, viewer: typing.Optional[chitose.app.bsky.feed.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.author = author
         self.record = record
         self.indexed_at = indexed_at
         self.embed = embed
         self.reply_count = reply_count
         self.repost_count = repost_count
         self.like_count = like_count
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self):
-        return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'record': self.record, 'indexedAt': self.indexed_at, 'embed': self.embed, 'replyCount': self.reply_count, 'repostCount': self.repost_count, 'likeCount': self.like_count, 'viewer': self.viewer, 'labels': self.labels}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'record': self.record, 'indexedAt': self.indexed_at, 'embed': self.embed, 'replyCount': self.reply_count, 'repostCount': self.repost_count, 'likeCount': self.like_count, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.feed.defs#postView'}
 
 class ViewerState(chitose.Object):
+    """"""
 
     def __init__(self, repost: typing.Optional[str]=None, like: typing.Optional[str]=None) -> None:
         self.repost = repost
         self.like = like
 
-    def to_dict(self):
-        return {'repost': self.repost, 'like': self.like}
+    def to_dict(self) -> dict:
+        return {'repost': self.repost, 'like': self.like, '$type': 'app.bsky.feed.defs#viewerState'}
 
 class FeedViewPost(chitose.Object):
+    """"""
 
     def __init__(self, post: chitose.app.bsky.feed.defs.PostView, reply: typing.Optional[chitose.app.bsky.feed.defs.ReplyRef]=None, reason: typing.Optional[chitose.app.bsky.feed.defs.ReasonRepost]=None) -> None:
         self.post = post
         self.reply = reply
         self.reason = reason
 
-    def to_dict(self):
-        return {'post': self.post, 'reply': self.reply, 'reason': self.reason}
+    def to_dict(self) -> dict:
+        return {'post': self.post, 'reply': self.reply, 'reason': self.reason, '$type': 'app.bsky.feed.defs#feedViewPost'}
 
 class ReplyRef(chitose.Object):
+    """"""
 
     def __init__(self, root: chitose.app.bsky.feed.defs.PostView, parent: chitose.app.bsky.feed.defs.PostView) -> None:
         self.root = root
         self.parent = parent
 
-    def to_dict(self):
-        return {'root': self.root, 'parent': self.parent}
+    def to_dict(self) -> dict:
+        return {'root': self.root, 'parent': self.parent, '$type': 'app.bsky.feed.defs#replyRef'}
 
 class ReasonRepost(chitose.Object):
+    """"""
 
     def __init__(self, by: chitose.app.bsky.actor.defs.ProfileViewBasic, indexed_at: str) -> None:
         self.by = by
         self.indexed_at = indexed_at
 
-    def to_dict(self):
-        return {'by': self.by, 'indexedAt': self.indexed_at}
+    def to_dict(self) -> dict:
+        return {'by': self.by, 'indexedAt': self.indexed_at, '$type': 'app.bsky.feed.defs#reasonRepost'}
 
 class ThreadViewPost(chitose.Object):
+    """"""
 
     def __init__(self, post: chitose.app.bsky.feed.defs.PostView, parent: typing.Optional[typing.Union[chitose.app.bsky.feed.defs.ThreadViewPost, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost]]=None, replies: typing.Optional[list[typing.Union[chitose.app.bsky.feed.defs.ThreadViewPost, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost]]]=None) -> None:
         self.post = post
         self.parent = parent
         self.replies = replies
 
-    def to_dict(self):
-        return {'post': self.post, 'parent': self.parent, 'replies': self.replies}
+    def to_dict(self) -> dict:
+        return {'post': self.post, 'parent': self.parent, 'replies': self.replies, '$type': 'app.bsky.feed.defs#threadViewPost'}
 
 class NotFoundPost(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, not_found: str) -> None:
         self.uri = uri
         self.not_found = not_found
 
-    def to_dict(self):
-        return {'uri': self.uri, 'notFound': self.not_found}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'notFound': self.not_found, '$type': 'app.bsky.feed.defs#notFoundPost'}
 
 class BlockedPost(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, blocked: str) -> None:
         self.uri = uri
         self.blocked = blocked
 
-    def to_dict(self):
-        return {'uri': self.uri, 'blocked': self.blocked}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'blocked': self.blocked, '$type': 'app.bsky.feed.defs#blockedPost'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/feed/get_likes.py` & `chitose-0.0.3/chitose/app/bsky/feed/get_likes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import typing
 
-def _get_likes(service: str, headers: dict[str, str], uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _get_likes(service: str, headers: dict[str, str], uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """"""
     return chitose.xrpc.call('app.bsky.feed.getLikes', [('uri', uri), ('cid', cid), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
 
 class Like(chitose.Object):
+    """"""
 
     def __init__(self, indexed_at: str, created_at: str, actor: chitose.app.bsky.actor.defs.ProfileView) -> None:
         self.indexed_at = indexed_at
         self.created_at = created_at
         self.actor = actor
 
-    def to_dict(self):
-        return {'indexedAt': self.indexed_at, 'createdAt': self.created_at, 'actor': self.actor}
+    def to_dict(self) -> dict:
+        return {'indexedAt': self.indexed_at, 'createdAt': self.created_at, 'actor': self.actor, '$type': 'app.bsky.feed.getLikes#like'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/feed/post.py` & `chitose-0.0.3/chitose/app/bsky/feed/post.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import chitose.app.bsky.embed.record_with_media
 import chitose.app.bsky.feed.post
 import chitose.app.bsky.richtext.facet
 import chitose.com.atproto.repo.strong_ref
 import typing
 
 class Post(chitose.Record):
+    """
+
+
+    :param entities: Deprecated: replaced by app.bsky.richtext.facet.
+    """
 
     def __init__(self, text: str, created_at: str, entities: typing.Optional[list[chitose.app.bsky.feed.post.Entity]]=None, facets: typing.Optional[list[chitose.app.bsky.richtext.facet.Facet]]=None, reply: typing.Optional[chitose.app.bsky.feed.post.ReplyRef]=None, embed: typing.Optional[typing.Union[chitose.app.bsky.embed.images.Images, chitose.app.bsky.embed.external.External, chitose.app.bsky.embed.record.Record, chitose.app.bsky.embed.record_with_media.RecordWithMedia]]=None) -> None:
         self.text = text
         self.created_at = created_at
         self.entities = entities
         self.facets = facets
         self.reply = reply
         self.embed = embed
 
-    def to_dict(self):
-        return {'text': self.text, 'createdAt': self.created_at, 'entities': self.entities, 'facets': self.facets, 'reply': self.reply, 'embed': self.embed}
+    def to_dict(self) -> dict:
+        return {'text': self.text, 'createdAt': self.created_at, 'entities': self.entities, 'facets': self.facets, 'reply': self.reply, 'embed': self.embed, '$type': 'app.bsky.feed.post'}
 
 class ReplyRef(chitose.Object):
+    """"""
 
     def __init__(self, root: chitose.com.atproto.repo.strong_ref.StrongRef, parent: chitose.com.atproto.repo.strong_ref.StrongRef) -> None:
         self.root = root
         self.parent = parent
 
-    def to_dict(self):
-        return {'root': self.root, 'parent': self.parent}
+    def to_dict(self) -> dict:
+        return {'root': self.root, 'parent': self.parent, '$type': 'app.bsky.feed.post#replyRef'}
 
 class Entity(chitose.Object):
+    """
+
+
+    :param type: Expected values are 'mention' and 'link'.
+    """
 
     def __init__(self, index: chitose.app.bsky.feed.post.TextSlice, type: str, value: str) -> None:
         self.index = index
         self.type = type
         self.value = value
 
-    def to_dict(self):
-        return {'index': self.index, 'type': self.type, 'value': self.value}
+    def to_dict(self) -> dict:
+        return {'index': self.index, 'type': self.type, 'value': self.value, '$type': 'app.bsky.feed.post#entity'}
 
 class TextSlice(chitose.Object):
+    """"""
 
     def __init__(self, start: int, end: int) -> None:
         self.start = start
         self.end = end
 
-    def to_dict(self):
-        return {'start': self.start, 'end': self.end}
+    def to_dict(self) -> dict:
+        return {'start': self.start, 'end': self.end, '$type': 'app.bsky.feed.post#textSlice'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/graph/__init__.py` & `chitose-0.0.3/chitose/app/bsky/graph/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,35 +5,36 @@
 from .get_follows import _get_follows
 from .get_mutes import _get_mutes
 from .mute_actor import _mute_actor
 from .unmute_actor import _unmute_actor
 import typing
 
 class Graph_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_followers(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_followers(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is following an actor?"""
         return _get_followers(self.service, self.headers, actor, limit, cursor)
 
-    def mute_actor(self, actor: str):
+    def mute_actor(self, actor: str) -> bytes:
         """Mute an actor by did or handle."""
         return _mute_actor(self.service, self.headers, actor)
 
-    def get_mutes(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_mutes(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who does the viewer mute?"""
         return _get_mutes(self.service, self.headers, limit, cursor)
 
-    def get_follows(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_follows(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is an actor following?"""
         return _get_follows(self.service, self.headers, actor, limit, cursor)
 
-    def get_blocks(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_blocks(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Who is the requester's account blocking?"""
         return _get_blocks(self.service, self.headers, limit, cursor)
 
-    def unmute_actor(self, actor: str):
+    def unmute_actor(self, actor: str) -> bytes:
         """Unmute an actor by did or handle."""
         return _unmute_actor(self.service, self.headers, actor)
```

### Comparing `chitose-0.0.2/chitose/app/bsky/notification/__init__.py` & `chitose-0.0.3/chitose/app/bsky/unspecced/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .get_unread_count import _get_unread_count
-from .list_notifications import _list_notifications
-from .update_seen import _update_seen
-import chitose
+from .get_popular import _get_popular
 import typing
 
-class Notification_:
+class Unspecced_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def update_seen(self, seen_at: str):
-        """Notify server that the user has seen notifications."""
-        return _update_seen(self.service, self.headers, seen_at)
-
-    def list_notifications(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None):
-        """"""
-        return _list_notifications(self.service, self.headers, limit, cursor, seen_at)
-
-    def get_unread_count(self, seen_at: typing.Optional[str]=None):
-        """"""
-        return _get_unread_count(self.service, self.headers, seen_at)
+    def get_popular(self, include_nsfw: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
+        """An unspecced view of globally popular items"""
+        return _get_popular(self.service, self.headers, include_nsfw, limit, cursor)
```

### Comparing `chitose-0.0.2/chitose/app/bsky/notification/list_notifications.py` & `chitose-0.0.3/chitose/app/bsky/notification/list_notifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.com.atproto.label.defs
 import typing
 
-def _list_notifications(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None):
+def _list_notifications(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None) -> bytes:
     """"""
     return chitose.xrpc.call('app.bsky.notification.listNotifications', [('limit', limit), ('cursor', cursor), ('seenAt', seen_at)], None, service, {} | headers)
 
 class Notification(chitose.Object):
+    """
+
+
+    :param reason: Expected values are 'like', 'repost', 'follow', 'mention', 'reply', and 'quote'.
+    """
 
     def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileView, reason: str, record: typing.Any, is_read: str, indexed_at: str, reason_subject: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.author = author
         self.reason = reason
         self.record = record
         self.is_read = is_read
         self.indexed_at = indexed_at
         self.reason_subject = reason_subject
         self.labels = labels
 
-    def to_dict(self):
-        return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'reason': self.reason, 'record': self.record, 'isRead': self.is_read, 'indexedAt': self.indexed_at, 'reasonSubject': self.reason_subject, 'labels': self.labels}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'reason': self.reason, 'record': self.record, 'isRead': self.is_read, 'indexedAt': self.indexed_at, 'reasonSubject': self.reason_subject, 'labels': self.labels, '$type': 'app.bsky.notification.listNotifications#notification'}
```

### Comparing `chitose-0.0.2/chitose/app/bsky/richtext/facet.py` & `chitose-0.0.3/chitose/app/bsky/richtext/facet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.richtext.facet
 import typing
 
 class Facet(chitose.Object):
+    """"""
 
     def __init__(self, index: chitose.app.bsky.richtext.facet.ByteSlice, features: list[typing.Union[chitose.app.bsky.richtext.facet.Mention, chitose.app.bsky.richtext.facet.Link]]) -> None:
         self.index = index
         self.features = features
 
-    def to_dict(self):
-        return {'index': self.index, 'features': self.features}
+    def to_dict(self) -> dict:
+        return {'index': self.index, 'features': self.features, '$type': 'app.bsky.richtext.facet'}
 
 class Mention(chitose.Object):
+    """"""
 
     def __init__(self, did: str) -> None:
         self.did = did
 
-    def to_dict(self):
-        return {'did': self.did}
+    def to_dict(self) -> dict:
+        return {'did': self.did, '$type': 'app.bsky.richtext.facet#mention'}
 
 class Link(chitose.Object):
+    """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
 
-    def to_dict(self):
-        return {'uri': self.uri}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, '$type': 'app.bsky.richtext.facet#link'}
 
 class ByteSlice(chitose.Object):
+    """"""
 
     def __init__(self, byte_start: int, byte_end: int) -> None:
         self.byte_start = byte_start
         self.byte_end = byte_end
 
-    def to_dict(self):
-        return {'byteStart': self.byte_start, 'byteEnd': self.byte_end}
+    def to_dict(self) -> dict:
+        return {'byteStart': self.byte_start, 'byteEnd': self.byte_end, '$type': 'app.bsky.richtext.facet#byteSlice'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/admin/__init__.py` & `chitose-0.0.3/chitose/com/atproto/admin/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,71 +14,72 @@
 from .take_moderation_action import _take_moderation_action
 from .update_account_email import _update_account_email
 from .update_account_handle import _update_account_handle
 import chitose
 import typing
 
 class Admin_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_repo(self, did: str):
+    def get_repo(self, did: str) -> bytes:
         """View details about a repository."""
         return _get_repo(self.service, self.headers, did)
 
-    def get_moderation_reports(self, subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_moderation_reports(self, subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """List moderation reports related to a subject."""
         return _get_moderation_reports(self.service, self.headers, subject, resolved, limit, cursor)
 
-    def take_moderation_action(self, action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None):
+    def take_moderation_action(self, action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
         """Take a moderation action on a repo."""
         return _take_moderation_action(self.service, self.headers, action, subject, reason, created_by, subject_blob_cids, create_label_vals, negate_label_vals)
 
-    def update_account_email(self, account: str, email: str):
+    def update_account_email(self, account: str, email: str) -> bytes:
         """Administrative action to update an account's email
 
 
         :param account: The handle or DID of the repo.
         """
         return _update_account_email(self.service, self.headers, account, email)
 
-    def get_moderation_action(self, id: int):
+    def get_moderation_action(self, id: int) -> bytes:
         """View details about a moderation action."""
         return _get_moderation_action(self.service, self.headers, id)
 
-    def update_account_handle(self, did: str, handle: str):
+    def update_account_handle(self, did: str, handle: str) -> bytes:
         """Administrative action to update an account's handle"""
         return _update_account_handle(self.service, self.headers, did, handle)
 
-    def get_invite_codes(self, sort: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_invite_codes(self, sort: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Admin view of invite codes"""
         return _get_invite_codes(self.service, self.headers, sort, limit, cursor)
 
-    def get_moderation_report(self, id: int):
+    def get_moderation_report(self, id: int) -> bytes:
         """View details about a moderation report."""
         return _get_moderation_report(self.service, self.headers, id)
 
-    def disable_invite_codes(self, codes: typing.Optional[list[str]]=None, accounts: typing.Optional[list[str]]=None):
+    def disable_invite_codes(self, codes: typing.Optional[list[str]]=None, accounts: typing.Optional[list[str]]=None) -> bytes:
         """Disable some set of codes and/or all codes associated with a set of users"""
         return _disable_invite_codes(self.service, self.headers, codes, accounts)
 
-    def reverse_moderation_action(self, id: int, reason: str, created_by: str):
+    def reverse_moderation_action(self, id: int, reason: str, created_by: str) -> bytes:
         """Reverse a moderation action."""
         return _reverse_moderation_action(self.service, self.headers, id, reason, created_by)
 
-    def get_record(self, uri: str, cid: typing.Optional[str]=None):
+    def get_record(self, uri: str, cid: typing.Optional[str]=None) -> bytes:
         """View details about a record."""
         return _get_record(self.service, self.headers, uri, cid)
 
-    def resolve_moderation_reports(self, action_id: int, report_ids: list[int], created_by: str):
+    def resolve_moderation_reports(self, action_id: int, report_ids: list[int], created_by: str) -> bytes:
         """Resolve moderation reports by an action."""
         return _resolve_moderation_reports(self.service, self.headers, action_id, report_ids, created_by)
 
-    def search_repos(self, term: typing.Optional[str]=None, invited_by: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def search_repos(self, term: typing.Optional[str]=None, invited_by: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Find repositories based on a search term."""
         return _search_repos(self.service, self.headers, term, invited_by, limit, cursor)
 
-    def get_moderation_actions(self, subject: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def get_moderation_actions(self, subject: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """List moderation actions related to a subject."""
         return _get_moderation_actions(self.service, self.headers, subject, limit, cursor)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/admin/defs.py` & `chitose-0.0.3/chitose/com/atproto/admin/defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,220 +1,237 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.label.defs
 import chitose.com.atproto.moderation.defs
 import chitose.com.atproto.repo.strong_ref
 import chitose.com.atproto.server.defs
 import enum
 import typing
 
 class ActionView(chitose.Object):
+    """"""
 
     def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], subject_blob_cids: list[str], reason: str, created_by: str, created_at: str, resolved_report_ids: list[int], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
         self.id = id
         self.action = action
         self.subject = subject
         self.subject_blob_cids = subject_blob_cids
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
         self.resolved_report_ids = resolved_report_ids
         self.create_label_vals = create_label_vals
         self.negate_label_vals = negate_label_vals
         self.reversal = reversal
 
-    def to_dict(self):
-        return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobCids': self.subject_blob_cids, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReportIds': self.resolved_report_ids, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal}
+    def to_dict(self) -> dict:
+        return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobCids': self.subject_blob_cids, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReportIds': self.resolved_report_ids, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal, '$type': 'com.atproto.admin.defs#actionView'}
 
 class ActionViewDetail(chitose.Object):
+    """"""
 
     def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RecordView], subject_blobs: list[chitose.com.atproto.admin.defs.BlobView], reason: str, created_by: str, created_at: str, resolved_reports: list[chitose.com.atproto.admin.defs.ReportView], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
         self.id = id
         self.action = action
         self.subject = subject
         self.subject_blobs = subject_blobs
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
         self.resolved_reports = resolved_reports
         self.create_label_vals = create_label_vals
         self.negate_label_vals = negate_label_vals
         self.reversal = reversal
 
-    def to_dict(self):
-        return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobs': self.subject_blobs, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReports': self.resolved_reports, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal}
+    def to_dict(self) -> dict:
+        return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobs': self.subject_blobs, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReports': self.resolved_reports, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal, '$type': 'com.atproto.admin.defs#actionViewDetail'}
 
 class ActionViewCurrent(chitose.Object):
+    """"""
 
     def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType) -> None:
         self.id = id
         self.action = action
 
-    def to_dict(self):
-        return {'id': self.id, 'action': self.action}
+    def to_dict(self) -> dict:
+        return {'id': self.id, 'action': self.action, '$type': 'com.atproto.admin.defs#actionViewCurrent'}
 
 class ActionReversal(chitose.Object):
+    """"""
 
     def __init__(self, reason: str, created_by: str, created_at: str) -> None:
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
 
-    def to_dict(self):
-        return {'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at}
+    def to_dict(self) -> dict:
+        return {'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, '$type': 'com.atproto.admin.defs#actionReversal'}
 
 class ActionType(enum.Enum):
     TAKEDOWN = '#takedown'
     FLAG = '#flag'
     ACKNOWLEDGE = '#acknowledge'
     ESCALATE = '#escalate'
 TAKEDOWN = 'com.atproto.admin.defs#takedown'
 FLAG = 'com.atproto.admin.defs#flag'
 ACKNOWLEDGE = 'com.atproto.admin.defs#acknowledge'
 ESCALATE = 'com.atproto.admin.defs#escalate'
 
 class ReportView(chitose.Object):
+    """"""
 
     def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reported_by: str, created_at: str, resolved_by_action_ids: list[int], reason: typing.Optional[str]=None) -> None:
         self.id = id
         self.reason_type = reason_type
         self.subject = subject
         self.reported_by = reported_by
         self.created_at = created_at
         self.resolved_by_action_ids = resolved_by_action_ids
         self.reason = reason
 
-    def to_dict(self):
-        return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActionIds': self.resolved_by_action_ids, 'reason': self.reason}
+    def to_dict(self) -> dict:
+        return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActionIds': self.resolved_by_action_ids, 'reason': self.reason, '$type': 'com.atproto.admin.defs#reportView'}
 
 class ReportViewDetail(chitose.Object):
+    """"""
 
     def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RecordView], reported_by: str, created_at: str, resolved_by_actions: list[chitose.com.atproto.admin.defs.ActionView], reason: typing.Optional[str]=None) -> None:
         self.id = id
         self.reason_type = reason_type
         self.subject = subject
         self.reported_by = reported_by
         self.created_at = created_at
         self.resolved_by_actions = resolved_by_actions
         self.reason = reason
 
-    def to_dict(self):
-        return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActions': self.resolved_by_actions, 'reason': self.reason}
+    def to_dict(self) -> dict:
+        return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActions': self.resolved_by_actions, 'reason': self.reason, '$type': 'com.atproto.admin.defs#reportViewDetail'}
 
 class RepoView(chitose.Object):
+    """"""
 
     def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.invited_by = invited_by
 
-    def to_dict(self):
-        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'invitedBy': self.invited_by}
+    def to_dict(self) -> dict:
+        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'invitedBy': self.invited_by, '$type': 'com.atproto.admin.defs#repoView'}
 
 class RepoViewDetail(chitose.Object):
+    """"""
 
     def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.labels = labels
         self.invited_by = invited_by
         self.invites = invites
 
-    def to_dict(self):
-        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'labels': self.labels, 'invitedBy': self.invited_by, 'invites': self.invites}
+    def to_dict(self) -> dict:
+        return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'labels': self.labels, 'invitedBy': self.invited_by, 'invites': self.invites, '$type': 'com.atproto.admin.defs#repoViewDetail'}
 
 class RepoRef(chitose.Object):
+    """"""
 
     def __init__(self, did: str) -> None:
         self.did = did
 
-    def to_dict(self):
-        return {'did': self.did}
+    def to_dict(self) -> dict:
+        return {'did': self.did, '$type': 'com.atproto.admin.defs#repoRef'}
 
 class RecordView(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, cid: str, value: typing.Any, blob_cids: list[str], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, repo: chitose.com.atproto.admin.defs.RepoView) -> None:
         self.uri = uri
         self.cid = cid
         self.value = value
         self.blob_cids = blob_cids
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.repo = repo
 
-    def to_dict(self):
-        return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobCids': self.blob_cids, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobCids': self.blob_cids, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo, '$type': 'com.atproto.admin.defs#recordView'}
 
 class RecordViewDetail(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, cid: str, value: typing.Any, blobs: list[chitose.com.atproto.admin.defs.BlobView], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, repo: chitose.com.atproto.admin.defs.RepoView, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.value = value
         self.blobs = blobs
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.repo = repo
         self.labels = labels
 
-    def to_dict(self):
-        return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobs': self.blobs, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo, 'labels': self.labels}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobs': self.blobs, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo, 'labels': self.labels, '$type': 'com.atproto.admin.defs#recordViewDetail'}
 
 class Moderation(chitose.Object):
+    """"""
 
     def __init__(self, current_action: typing.Optional[chitose.com.atproto.admin.defs.ActionViewCurrent]=None) -> None:
         self.current_action = current_action
 
-    def to_dict(self):
-        return {'currentAction': self.current_action}
+    def to_dict(self) -> dict:
+        return {'currentAction': self.current_action, '$type': 'com.atproto.admin.defs#moderation'}
 
 class ModerationDetail(chitose.Object):
+    """"""
 
     def __init__(self, actions: list[chitose.com.atproto.admin.defs.ActionView], reports: list[chitose.com.atproto.admin.defs.ReportView], current_action: typing.Optional[chitose.com.atproto.admin.defs.ActionViewCurrent]=None) -> None:
         self.actions = actions
         self.reports = reports
         self.current_action = current_action
 
-    def to_dict(self):
-        return {'actions': self.actions, 'reports': self.reports, 'currentAction': self.current_action}
+    def to_dict(self) -> dict:
+        return {'actions': self.actions, 'reports': self.reports, 'currentAction': self.current_action, '$type': 'com.atproto.admin.defs#moderationDetail'}
 
 class BlobView(chitose.Object):
+    """"""
 
     def __init__(self, cid: str, mime_type: str, size: int, created_at: str, details: typing.Optional[typing.Union[chitose.com.atproto.admin.defs.ImageDetails, chitose.com.atproto.admin.defs.VideoDetails]]=None, moderation: typing.Optional[chitose.com.atproto.admin.defs.Moderation]=None) -> None:
         self.cid = cid
         self.mime_type = mime_type
         self.size = size
         self.created_at = created_at
         self.details = details
         self.moderation = moderation
 
-    def to_dict(self):
-        return {'cid': self.cid, 'mimeType': self.mime_type, 'size': self.size, 'createdAt': self.created_at, 'details': self.details, 'moderation': self.moderation}
+    def to_dict(self) -> dict:
+        return {'cid': self.cid, 'mimeType': self.mime_type, 'size': self.size, 'createdAt': self.created_at, 'details': self.details, 'moderation': self.moderation, '$type': 'com.atproto.admin.defs#blobView'}
 
 class ImageDetails(chitose.Object):
+    """"""
 
     def __init__(self, width: int, height: int) -> None:
         self.width = width
         self.height = height
 
-    def to_dict(self):
-        return {'width': self.width, 'height': self.height}
+    def to_dict(self) -> dict:
+        return {'width': self.width, 'height': self.height, '$type': 'com.atproto.admin.defs#imageDetails'}
 
 class VideoDetails(chitose.Object):
+    """"""
 
     def __init__(self, width: int, height: int, length: int) -> None:
         self.width = width
         self.height = height
         self.length = length
 
-    def to_dict(self):
-        return {'width': self.width, 'height': self.height, 'length': self.length}
+    def to_dict(self) -> dict:
+        return {'width': self.width, 'height': self.height, 'length': self.length, '$type': 'com.atproto.admin.defs#videoDetails'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/admin/get_moderation_reports.py` & `chitose-0.0.3/chitose/com/atproto/admin/get_moderation_reports.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """List moderation reports related to a subject."""
     return chitose.xrpc.call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/admin/search_repos.py` & `chitose-0.0.3/chitose/com/atproto/admin/search_repos.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _search_repos(service: str, headers: dict[str, str], term: typing.Optional[str]=None, invited_by: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _search_repos(service: str, headers: dict[str, str], term: typing.Optional[str]=None, invited_by: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """Find repositories based on a search term."""
     return chitose.xrpc.call('com.atproto.admin.searchRepos', [('term', term), ('invitedBy', invited_by), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/admin/take_moderation_action.py` & `chitose-0.0.3/chitose/com/atproto/admin/take_moderation_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
-def _take_moderation_action(service: str, headers: dict[str, str], action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None):
+def _take_moderation_action(service: str, headers: dict[str, str], action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
     """Take a moderation action on a repo."""
     return chitose.xrpc.call('com.atproto.admin.takeModerationAction', [], {'action': action, 'subject': subject, 'subjectBlobCids': subject_blob_cids, 'createLabelVals': create_label_vals, 'negateLabelVals': negate_label_vals, 'reason': reason, 'createdBy': created_by}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/label/__init__.py` & `chitose-0.0.3/chitose/com/atproto/label/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 from .query_labels import _query_labels
 import typing
 
 class Label_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def query_labels(self, uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def query_labels(self, uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """Find labels relevant to the provided URI patterns.
 
 
         :param uri_patterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI
 
         :param sources: Optional list of label sources (DIDs) to filter on
         """
```

### Comparing `chitose-0.0.2/chitose/com/atproto/label/query_labels.py` & `chitose-0.0.3/chitose/com/atproto/label/query_labels.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _query_labels(service: str, headers: dict[str, str], uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _query_labels(service: str, headers: dict[str, str], uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """Find labels relevant to the provided URI patterns.
 
 
     :param uri_patterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI
 
     :param sources: Optional list of label sources (DIDs) to filter on
     """
```

### Comparing `chitose-0.0.2/chitose/com/atproto/label/subscribe_labels.py` & `chitose-0.0.3/chitose/com/atproto/label/subscribe_labels.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.label.defs
 import typing
 
 class Labels(chitose.Object):
+    """"""
 
     def __init__(self, seq: int, labels: list[chitose.com.atproto.label.defs.Label]) -> None:
         self.seq = seq
         self.labels = labels
 
-    def to_dict(self):
-        return {'seq': self.seq, 'labels': self.labels}
+    def to_dict(self) -> dict:
+        return {'seq': self.seq, 'labels': self.labels, '$type': 'com.atproto.label.subscribeLabels#labels'}
 
 class Info(chitose.Object):
+    """"""
 
     def __init__(self, name: str, message: typing.Optional[str]=None) -> None:
         self.name = name
         self.message = message
 
-    def to_dict(self):
-        return {'name': self.name, 'message': self.message}
+    def to_dict(self) -> dict:
+        return {'name': self.name, 'message': self.message, '$type': 'com.atproto.label.subscribeLabels#info'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/moderation/__init__.py` & `chitose-0.0.3/chitose/com/atproto/moderation/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 from .create_report import _create_report
 import chitose
 import typing
 
 class Moderation_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def create_report(self, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None):
+    def create_report(self, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None) -> bytes:
         """Report a repo or a record."""
         return _create_report(self.service, self.headers, reason_type, subject, reason)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/moderation/create_report.py` & `chitose-0.0.3/chitose/com/atproto/moderation/create_report.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.moderation.defs
 import chitose.com.atproto.repo.strong_ref
 import typing
 
-def _create_report(service: str, headers: dict[str, str], reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None):
+def _create_report(service: str, headers: dict[str, str], reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None) -> bytes:
     """Report a repo or a record."""
     return chitose.xrpc.call('com.atproto.moderation.createReport', [], {'reasonType': reason_type, 'reason': reason, 'subject': subject}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/moderation/defs.py` & `chitose-0.0.3/chitose/com/atproto/moderation/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import enum
 
 class ReasonType(enum.Enum):
     REASON_SPAM = 'com.atproto.moderation.defs#reasonSpam'
     REASON_VIOLATION = 'com.atproto.moderation.defs#reasonViolation'
     REASON_MISLEADING = 'com.atproto.moderation.defs#reasonMisleading'
```

### Comparing `chitose-0.0.2/chitose/com/atproto/repo/__init__.py` & `chitose-0.0.3/chitose/com/atproto/repo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from .list_records import _list_records
 from .put_record import _put_record
 from .upload_blob import _upload_blob
 import chitose
 import typing
 
 class Repo_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def create_record(self, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+    def create_record(self, repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Create a new record.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record collection.
 
@@ -31,15 +32,15 @@
 
         :param validate: Validate the record?
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
         return _create_record(self.service, self.headers, repo, collection, record, rkey, validate, swap_commit)
 
-    def delete_record(self, repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+    def delete_record(self, repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Delete a record, or ensure it doesn't exist.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record collection.
 
@@ -47,15 +48,15 @@
 
         :param swap_record: Compare and swap with the previous record by cid.
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
         return _delete_record(self.service, self.headers, repo, collection, rkey, swap_record, swap_commit)
 
-    def put_record(self, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[str]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+    def put_record(self, repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[str]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Write a record, creating or updating it as needed.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record collection.
 
@@ -67,51 +68,51 @@
 
         :param swap_record: Compare and swap with the previous record by cid.
 
         :param swap_commit: Compare and swap with the previous commit by cid.
         """
         return _put_record(self.service, self.headers, repo, collection, rkey, record, validate, swap_record, swap_commit)
 
-    def upload_blob(self):
+    def upload_blob(self, input_: bytes) -> bytes:
         """Upload a new blob to be added to repo in a later request."""
-        return _upload_blob(self.service, self.headers)
+        return _upload_blob(self.service, self.headers, input_)
 
-    def describe_repo(self, repo: str):
+    def describe_repo(self, repo: str) -> bytes:
         """Get information about the repo, including the list of collections.
 
 
         :param repo: The handle or DID of the repo.
         """
         return _describe_repo(self.service, self.headers, repo)
 
-    def get_record(self, repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None):
+    def get_record(self, repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None) -> bytes:
         """Get a record.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record collection.
 
         :param rkey: The key of the record.
 
         :param cid: The CID of the version of the record. If not specified, then return the most recent version.
         """
         return _get_record(self.service, self.headers, repo, collection, rkey, cid)
 
-    def apply_writes(self, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+    def apply_writes(self, repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
         """Apply a batch transaction of creates, updates, and deletes.
 
 
         :param repo: The handle or DID of the repo.
 
         :param validate: Validate the records?
         """
         return _apply_writes(self.service, self.headers, repo, writes, validate, swap_commit)
 
-    def list_records(self, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None):
+    def list_records(self, repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None) -> bytes:
         """List a range of records in a collection.
 
 
         :param repo: The handle or DID of the repo.
 
         :param collection: The NSID of the record type.
```

### Comparing `chitose-0.0.2/chitose/com/atproto/repo/apply_writes.py` & `chitose-0.0.3/chitose/com/atproto/repo/apply_writes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.repo.apply_writes
 import typing
 
-def _apply_writes(service: str, headers: dict[str, str], repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+def _apply_writes(service: str, headers: dict[str, str], repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Apply a batch transaction of creates, updates, and deletes.
 
 
     :param repo: The handle or DID of the repo.
 
     :param validate: Validate the records?
     """
     return chitose.xrpc.call('com.atproto.repo.applyWrites', [], {'repo': repo, 'validate': validate, 'writes': writes, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
 
 class Create(chitose.Object):
+    """"""
 
     def __init__(self, collection: str, value: typing.Any, rkey: typing.Optional[str]) -> None:
         self.collection = collection
         self.value = value
         self.rkey = rkey
 
-    def to_dict(self):
-        return {'collection': self.collection, 'value': self.value, 'rkey': self.rkey}
+    def to_dict(self) -> dict:
+        return {'collection': self.collection, 'value': self.value, 'rkey': self.rkey, '$type': 'com.atproto.repo.applyWrites#create'}
 
 class Update(chitose.Object):
+    """"""
 
     def __init__(self, collection: str, rkey: str, value: typing.Any) -> None:
         self.collection = collection
         self.rkey = rkey
         self.value = value
 
-    def to_dict(self):
-        return {'collection': self.collection, 'rkey': self.rkey, 'value': self.value}
+    def to_dict(self) -> dict:
+        return {'collection': self.collection, 'rkey': self.rkey, 'value': self.value, '$type': 'com.atproto.repo.applyWrites#update'}
 
 class Delete(chitose.Object):
+    """"""
 
     def __init__(self, collection: str, rkey: str) -> None:
         self.collection = collection
         self.rkey = rkey
 
-    def to_dict(self):
-        return {'collection': self.collection, 'rkey': self.rkey}
+    def to_dict(self) -> dict:
+        return {'collection': self.collection, 'rkey': self.rkey, '$type': 'com.atproto.repo.applyWrites#delete'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/repo/create_record.py` & `chitose-0.0.3/chitose/com/atproto/repo/create_record.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_record(service: str, headers: dict[str, str], repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+def _create_record(service: str, headers: dict[str, str], repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Create a new record.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.2/chitose/com/atproto/repo/delete_record.py` & `chitose-0.0.3/chitose/com/atproto/repo/delete_record.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _delete_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+def _delete_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Delete a record, or ensure it doesn't exist.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.2/chitose/com/atproto/repo/get_record.py` & `chitose-0.0.3/chitose/com/atproto/repo/get_record.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None):
+def _get_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, cid: typing.Optional[str]=None) -> bytes:
     """Get a record.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.2/chitose/com/atproto/repo/list_records.py` & `chitose-0.0.3/chitose/com/atproto/repo/list_records.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_records(service: str, headers: dict[str, str], repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None):
+def _list_records(service: str, headers: dict[str, str], repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None) -> bytes:
     """List a range of records in a collection.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record type.
 
@@ -18,15 +19,16 @@
     :param rkey_end: DEPRECATED: The highest sort-ordered rkey to stop at (exclusive)
 
     :param reverse: Reverse the order of the returned records?
     """
     return chitose.xrpc.call('com.atproto.repo.listRecords', [('repo', repo), ('collection', collection), ('limit', limit), ('cursor', cursor), ('rkeyStart', rkey_start), ('rkeyEnd', rkey_end), ('reverse', reverse)], None, service, {} | headers)
 
 class Record(chitose.Object):
+    """"""
 
     def __init__(self, uri: str, cid: str, value: typing.Any) -> None:
         self.uri = uri
         self.cid = cid
         self.value = value
 
-    def to_dict(self):
-        return {'uri': self.uri, 'cid': self.cid, 'value': self.value}
+    def to_dict(self) -> dict:
+        return {'uri': self.uri, 'cid': self.cid, 'value': self.value, '$type': 'com.atproto.repo.listRecords#record'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/repo/put_record.py` & `chitose-0.0.3/chitose/com/atproto/repo/put_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _put_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[str]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+def _put_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[str]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None) -> bytes:
     """Write a record, creating or updating it as needed.
 
 
     :param repo: The handle or DID of the repo.
 
     :param collection: The NSID of the record collection.
```

### Comparing `chitose-0.0.2/chitose/com/atproto/server/__init__.py` & `chitose-0.0.3/chitose/com/atproto/server/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,79 +15,80 @@
 from .request_account_delete import _request_account_delete
 from .request_password_reset import _request_password_reset
 from .reset_password import _reset_password
 from .revoke_app_password import _revoke_app_password
 import typing
 
 class Server_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_account_invite_codes(self, include_used: typing.Optional[str]=None, create_available: typing.Optional[str]=None):
+    def get_account_invite_codes(self, include_used: typing.Optional[str]=None, create_available: typing.Optional[str]=None) -> bytes:
         """Get all invite codes for a given account"""
         return _get_account_invite_codes(self.service, self.headers, include_used, create_available)
 
-    def create_session(self, identifier: str, password: str):
+    def create_session(self, identifier: str, password: str) -> bytes:
         """Create an authentication session.
 
 
         :param identifier: Handle or other identifier supported by the server for the authenticating user.
         """
         return _create_session(self.service, self.headers, identifier, password)
 
-    def list_app_passwords(self):
+    def list_app_passwords(self) -> bytes:
         """List all app-specific passwords."""
         return _list_app_passwords(self.service, self.headers)
 
-    def create_invite_codes(self, code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None):
+    def create_invite_codes(self, code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
         """Create an invite code."""
         return _create_invite_codes(self.service, self.headers, code_count, use_count, for_accounts)
 
-    def delete_session(self):
+    def delete_session(self) -> bytes:
         """Delete the current session."""
         return _delete_session(self.service, self.headers)
 
-    def revoke_app_password(self, name: str):
+    def revoke_app_password(self, name: str) -> bytes:
         """Revoke an app-specific password by name."""
         return _revoke_app_password(self.service, self.headers, name)
 
-    def create_app_password(self, name: str):
+    def create_app_password(self, name: str) -> bytes:
         """Create an app-specific password."""
         return _create_app_password(self.service, self.headers, name)
 
-    def describe_server(self):
+    def describe_server(self) -> bytes:
         """Get a document describing the service's accounts configuration."""
         return _describe_server(self.service, self.headers)
 
-    def get_session(self):
+    def get_session(self) -> bytes:
         """Get information about the current session."""
         return _get_session(self.service, self.headers)
 
-    def refresh_session(self):
+    def refresh_session(self) -> bytes:
         """Refresh an authentication session."""
         return _refresh_session(self.service, self.headers)
 
-    def reset_password(self, token: str, password: str):
+    def reset_password(self, token: str, password: str) -> bytes:
         """Reset a user account password using a token."""
         return _reset_password(self.service, self.headers, token, password)
 
-    def request_password_reset(self, email: str):
+    def request_password_reset(self, email: str) -> bytes:
         """Initiate a user account password reset via email."""
         return _request_password_reset(self.service, self.headers, email)
 
-    def request_account_delete(self):
+    def request_account_delete(self) -> bytes:
         """Initiate a user account deletion via email."""
         return _request_account_delete(self.service, self.headers)
 
-    def create_account(self, email: str, handle: str, password: str, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None):
+    def create_account(self, email: str, handle: str, password: str, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
         """Create an account."""
         return _create_account(self.service, self.headers, email, handle, password, invite_code, recovery_key)
 
-    def delete_account(self, did: str, password: str, token: str):
+    def delete_account(self, did: str, password: str, token: str) -> bytes:
         """Delete a user account with a token and password."""
         return _delete_account(self.service, self.headers, did, password, token)
 
-    def create_invite_code(self, use_count: int, for_account: typing.Optional[str]=None):
+    def create_invite_code(self, use_count: int, for_account: typing.Optional[str]=None) -> bytes:
         """Create an invite code."""
         return _create_invite_code(self.service, self.headers, use_count, for_account)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/server/create_account.py` & `chitose-0.0.3/chitose/com/atproto/server/create_account.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_account(service: str, headers: dict[str, str], email: str, handle: str, password: str, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None):
+def _create_account(service: str, headers: dict[str, str], email: str, handle: str, password: str, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None) -> bytes:
     """Create an account."""
     return chitose.xrpc.call('com.atproto.server.createAccount', [], {'email': email, 'handle': handle, 'inviteCode': invite_code, 'password': password, 'recoveryKey': recovery_key}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/server/create_app_password.py` & `chitose-0.0.3/chitose/com/atproto/server/create_app_password.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 
-def _create_app_password(service: str, headers: dict[str, str], name: str):
+def _create_app_password(service: str, headers: dict[str, str], name: str) -> bytes:
     """Create an app-specific password."""
     return chitose.xrpc.call('com.atproto.server.createAppPassword', [], {'name': name}, service, {'Content-Type': 'application/json'} | headers)
 
 class AppPassword(chitose.Object):
+    """"""
 
     def __init__(self, name: str, password: str, created_at: str) -> None:
         self.name = name
         self.password = password
         self.created_at = created_at
 
-    def to_dict(self):
-        return {'name': self.name, 'password': self.password, 'createdAt': self.created_at}
+    def to_dict(self) -> dict:
+        return {'name': self.name, 'password': self.password, 'createdAt': self.created_at, '$type': 'com.atproto.server.createAppPassword#appPassword'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/server/create_invite_codes.py` & `chitose-0.0.3/chitose/com/atproto/server/create_invite_codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _create_invite_codes(service: str, headers: dict[str, str], code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None):
+def _create_invite_codes(service: str, headers: dict[str, str], code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None) -> bytes:
     """Create an invite code."""
     return chitose.xrpc.call('com.atproto.server.createInviteCodes', [], {'codeCount': code_count, 'useCount': use_count, 'forAccounts': for_accounts}, service, {'Content-Type': 'application/json'} | headers)
 
 class AccountCodes(chitose.Object):
+    """"""
 
     def __init__(self, account: str, codes: list[str]) -> None:
         self.account = account
         self.codes = codes
 
-    def to_dict(self):
-        return {'account': self.account, 'codes': self.codes}
+    def to_dict(self) -> dict:
+        return {'account': self.account, 'codes': self.codes, '$type': 'com.atproto.server.createInviteCodes#accountCodes'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/server/defs.py` & `chitose-0.0.3/chitose/com/atproto/server/defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.server.defs
 
 class InviteCode(chitose.Object):
+    """"""
 
     def __init__(self, code: str, available: int, disabled: str, for_account: str, created_by: str, created_at: str, uses: list[chitose.com.atproto.server.defs.InviteCodeUse]) -> None:
         self.code = code
         self.available = available
         self.disabled = disabled
         self.for_account = for_account
         self.created_by = created_by
         self.created_at = created_at
         self.uses = uses
 
-    def to_dict(self):
-        return {'code': self.code, 'available': self.available, 'disabled': self.disabled, 'forAccount': self.for_account, 'createdBy': self.created_by, 'createdAt': self.created_at, 'uses': self.uses}
+    def to_dict(self) -> dict:
+        return {'code': self.code, 'available': self.available, 'disabled': self.disabled, 'forAccount': self.for_account, 'createdBy': self.created_by, 'createdAt': self.created_at, 'uses': self.uses, '$type': 'com.atproto.server.defs#inviteCode'}
 
 class InviteCodeUse(chitose.Object):
+    """"""
 
     def __init__(self, used_by: str, used_at: str) -> None:
         self.used_by = used_by
         self.used_at = used_at
 
-    def to_dict(self):
-        return {'usedBy': self.used_by, 'usedAt': self.used_at}
+    def to_dict(self) -> dict:
+        return {'usedBy': self.used_by, 'usedAt': self.used_at, '$type': 'com.atproto.server.defs#inviteCodeUse'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/server/describe_server.py` & `chitose-0.0.3/chitose/com/atproto/server/describe_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _describe_server(service: str, headers: dict[str, str]):
+def _describe_server(service: str, headers: dict[str, str]) -> bytes:
     """Get a document describing the service's accounts configuration."""
     return chitose.xrpc.call('com.atproto.server.describeServer', [], None, service, {} | headers)
 
 class Links(chitose.Object):
+    """"""
 
     def __init__(self, privacy_policy: typing.Optional[str]=None, terms_of_service: typing.Optional[str]=None) -> None:
         self.privacy_policy = privacy_policy
         self.terms_of_service = terms_of_service
 
-    def to_dict(self):
-        return {'privacyPolicy': self.privacy_policy, 'termsOfService': self.terms_of_service}
+    def to_dict(self) -> dict:
+        return {'privacyPolicy': self.privacy_policy, 'termsOfService': self.terms_of_service, '$type': 'com.atproto.server.describeServer#links'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/__init__.py` & `chitose-0.0.3/chitose/com/atproto/sync/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,112 +10,113 @@
 from .list_blobs import _list_blobs
 from .list_repos import _list_repos
 from .notify_of_update import _notify_of_update
 from .request_crawl import _request_crawl
 import typing
 
 class Sync_:
+    """We recommend calling methods in this class via the `chitose.BskyAgent` class instead of creating instances of this class directly."""
 
-    def __init__(self, service: str, headers: dict[str, str]):
+    def __init__(self, service: str, headers: dict[str, str]) -> None:
         self.service = service
         self.headers = headers
 
-    def get_head(self, did: str):
+    def get_head(self, did: str) -> bytes:
         """Gets the current HEAD CID of a repo.
 
 
         :param did: The DID of the repo.
         """
         return _get_head(self.service, self.headers, did)
 
-    def get_blob(self, did: str, cid: str):
+    def get_blob(self, did: str, cid: str) -> bytes:
         """Get a blob associated with a given repo.
 
 
         :param did: The DID of the repo.
 
         :param cid: The CID of the blob to fetch
         """
         return _get_blob(self.service, self.headers, did, cid)
 
-    def get_repo(self, did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None):
+    def get_repo(self, did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None) -> bytes:
         """Gets the repo state.
 
 
         :param did: The DID of the repo.
 
         :param earliest: The earliest commit in the commit range (not inclusive)
 
         :param latest: The latest commit in the commit range (inclusive)
         """
         return _get_repo(self.service, self.headers, did, earliest, latest)
 
-    def notify_of_update(self, hostname: str):
+    def notify_of_update(self, hostname: str) -> bytes:
         """Notify a crawling service of a recent update. Often when a long break between updates causes the connection with the crawling service to break.
 
 
         :param hostname: Hostname of the service that is notifying of update.
         """
         return _notify_of_update(self.service, self.headers, hostname)
 
-    def request_crawl(self, hostname: str):
+    def request_crawl(self, hostname: str) -> bytes:
         """Request a service to persistently crawl hosted repos.
 
 
         :param hostname: Hostname of the service that is requesting to be crawled.
         """
         return _request_crawl(self.service, self.headers, hostname)
 
-    def list_blobs(self, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None):
+    def list_blobs(self, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
         """List blob cids for some range of commits
 
 
         :param did: The DID of the repo.
 
         :param latest: The most recent commit
 
         :param earliest: The earliest commit to start from
         """
         return _list_blobs(self.service, self.headers, did, latest, earliest)
 
-    def get_record(self, did: str, collection: str, rkey: str, commit: typing.Optional[str]=None):
+    def get_record(self, did: str, collection: str, rkey: str, commit: typing.Optional[str]=None) -> bytes:
         """Gets blocks needed for existence or non-existence of record.
 
 
         :param did: The DID of the repo.
 
         :param commit: An optional past commit CID.
         """
         return _get_record(self.service, self.headers, did, collection, rkey, commit)
 
-    def list_repos(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    def list_repos(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
         """List dids and root cids of hosted repos"""
         return _list_repos(self.service, self.headers, limit, cursor)
 
-    def get_commit_path(self, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None):
+    def get_commit_path(self, did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
         """Gets the path of repo commits
 
 
         :param did: The DID of the repo.
 
         :param latest: The most recent commit
 
         :param earliest: The earliest commit to start from
         """
         return _get_commit_path(self.service, self.headers, did, latest, earliest)
 
-    def get_blocks(self, did: str, cids: list[str]):
+    def get_blocks(self, did: str, cids: list[str]) -> bytes:
         """Gets blocks from a given repo.
 
 
         :param did: The DID of the repo.
         """
         return _get_blocks(self.service, self.headers, did, cids)
 
-    def get_checkout(self, did: str, commit: typing.Optional[str]=None):
+    def get_checkout(self, did: str, commit: typing.Optional[str]=None) -> bytes:
         """Gets the repo state.
 
 
         :param did: The DID of the repo.
 
         :param commit: The commit to get the checkout from. Defaults to current HEAD.
         """
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/get_commit_path.py` & `chitose-0.0.3/chitose/com/atproto/sync/get_commit_path.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_commit_path(service: str, headers: dict[str, str], did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None):
+def _get_commit_path(service: str, headers: dict[str, str], did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
     """Gets the path of repo commits
 
 
     :param did: The DID of the repo.
 
     :param latest: The most recent commit
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/get_record.py` & `chitose-0.0.3/chitose/com/atproto/sync/get_record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_record(service: str, headers: dict[str, str], did: str, collection: str, rkey: str, commit: typing.Optional[str]=None):
+def _get_record(service: str, headers: dict[str, str], did: str, collection: str, rkey: str, commit: typing.Optional[str]=None) -> bytes:
     """Gets blocks needed for existence or non-existence of record.
 
 
     :param did: The DID of the repo.
 
     :param commit: An optional past commit CID.
     """
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/get_repo.py` & `chitose-0.0.3/chitose/com/atproto/sync/get_repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_repo(service: str, headers: dict[str, str], did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None):
+def _get_repo(service: str, headers: dict[str, str], did: str, earliest: typing.Optional[str]=None, latest: typing.Optional[str]=None) -> bytes:
     """Gets the repo state.
 
 
     :param did: The DID of the repo.
 
     :param earliest: The earliest commit in the commit range (not inclusive)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/list_blobs.py` & `chitose-0.0.3/chitose/com/atproto/sync/list_blobs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_blobs(service: str, headers: dict[str, str], did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None):
+def _list_blobs(service: str, headers: dict[str, str], did: str, latest: typing.Optional[str]=None, earliest: typing.Optional[str]=None) -> bytes:
     """List blob cids for some range of commits
 
 
     :param did: The DID of the repo.
 
     :param latest: The most recent commit
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/list_repos.py` & `chitose-0.0.3/chitose/com/atproto/sync/list_repos.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import typing
 
-def _list_repos(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _list_repos(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None) -> bytes:
     """List dids and root cids of hosted repos"""
     return chitose.xrpc.call('com.atproto.sync.listRepos', [('limit', limit), ('cursor', cursor)], None, service, {} | headers)
 
 class Repo(chitose.Object):
+    """"""
 
     def __init__(self, did: str, head: str) -> None:
         self.did = did
         self.head = head
 
-    def to_dict(self):
-        return {'did': self.did, 'head': self.head}
+    def to_dict(self) -> dict:
+        return {'did': self.did, 'head': self.head, '$type': 'com.atproto.sync.listRepos#repo'}
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/notify_of_update.py` & `chitose-0.0.3/chitose/com/atproto/sync/notify_of_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 
-def _notify_of_update(service: str, headers: dict[str, str], hostname: str):
+def _notify_of_update(service: str, headers: dict[str, str], hostname: str) -> bytes:
     """Notify a crawling service of a recent update. Often when a long break between updates causes the connection with the crawling service to break.
 
 
     :param hostname: Hostname of the service that is notifying of update.
     """
     return chitose.xrpc.call('com.atproto.sync.notifyOfUpdate', [('hostname', hostname)], None, service, {} | headers)
```

### Comparing `chitose-0.0.2/chitose/com/atproto/sync/subscribe_repos.py` & `chitose-0.0.3/chitose/com/atproto/sync/subscribe_repos.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,84 @@
 # GENERATED CODE - DO NOT MODIFY
+""""""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.sync.subscribe_repos
 import typing
 
 class Commit(chitose.Object):
+    """
+
+
+    :param blocks: CAR file containing relevant blocks
+    """
 
     def __init__(self, seq: int, rebase: str, too_big: str, repo: str, commit: typing.Any, prev: typing.Any, blocks: typing.Any, ops: list[chitose.com.atproto.sync.subscribe_repos.RepoOp], blobs: list[typing.Any], time: str) -> None:
         self.seq = seq
         self.rebase = rebase
         self.too_big = too_big
         self.repo = repo
         self.commit = commit
         self.prev = prev
         self.blocks = blocks
         self.ops = ops
         self.blobs = blobs
         self.time = time
 
-    def to_dict(self):
-        return {'seq': self.seq, 'rebase': self.rebase, 'tooBig': self.too_big, 'repo': self.repo, 'commit': self.commit, 'prev': self.prev, 'blocks': self.blocks, 'ops': self.ops, 'blobs': self.blobs, 'time': self.time}
+    def to_dict(self) -> dict:
+        return {'seq': self.seq, 'rebase': self.rebase, 'tooBig': self.too_big, 'repo': self.repo, 'commit': self.commit, 'prev': self.prev, 'blocks': self.blocks, 'ops': self.ops, 'blobs': self.blobs, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#commit'}
 
 class Handle(chitose.Object):
+    """"""
 
     def __init__(self, seq: int, did: str, handle: str, time: str) -> None:
         self.seq = seq
         self.did = did
         self.handle = handle
         self.time = time
 
-    def to_dict(self):
-        return {'seq': self.seq, 'did': self.did, 'handle': self.handle, 'time': self.time}
+    def to_dict(self) -> dict:
+        return {'seq': self.seq, 'did': self.did, 'handle': self.handle, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#handle'}
 
 class Migrate(chitose.Object):
+    """"""
 
     def __init__(self, seq: int, did: str, migrate_to: str, time: str) -> None:
         self.seq = seq
         self.did = did
         self.migrate_to = migrate_to
         self.time = time
 
-    def to_dict(self):
-        return {'seq': self.seq, 'did': self.did, 'migrateTo': self.migrate_to, 'time': self.time}
+    def to_dict(self) -> dict:
+        return {'seq': self.seq, 'did': self.did, 'migrateTo': self.migrate_to, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#migrate'}
 
 class Tombstone(chitose.Object):
+    """"""
 
     def __init__(self, seq: int, did: str, time: str) -> None:
         self.seq = seq
         self.did = did
         self.time = time
 
-    def to_dict(self):
-        return {'seq': self.seq, 'did': self.did, 'time': self.time}
+    def to_dict(self) -> dict:
+        return {'seq': self.seq, 'did': self.did, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#tombstone'}
 
 class Info(chitose.Object):
+    """"""
 
     def __init__(self, name: str, message: typing.Optional[str]=None) -> None:
         self.name = name
         self.message = message
 
-    def to_dict(self):
-        return {'name': self.name, 'message': self.message}
+    def to_dict(self) -> dict:
+        return {'name': self.name, 'message': self.message, '$type': 'com.atproto.sync.subscribeRepos#info'}
 
 class RepoOp(chitose.Object):
+    """"""
 
     def __init__(self, action: str, path: str, cid: typing.Any) -> None:
         self.action = action
         self.path = path
         self.cid = cid
 
-    def to_dict(self):
-        return {'action': self.action, 'path': self.path, 'cid': self.cid}
+    def to_dict(self) -> dict:
+        return {'action': self.action, 'path': self.path, 'cid': self.cid, '$type': 'com.atproto.sync.subscribeRepos#repoOp'}
```

### Comparing `chitose-0.0.2/docs/Makefile` & `chitose-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/make.bat` & `chitose-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.app.bsky.actor.rst` & `chitose-0.0.3/docs/source/chitose.app.bsky.actor.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.app.bsky.embed.rst` & `chitose-0.0.3/docs/source/chitose.app.bsky.embed.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.app.bsky.feed.rst` & `chitose-0.0.3/docs/source/chitose.app.bsky.feed.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.app.bsky.graph.rst` & `chitose-0.0.3/docs/source/chitose.app.bsky.graph.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.app.bsky.notification.rst` & `chitose-0.0.3/docs/source/chitose.app.bsky.notification.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.com.atproto.admin.rst` & `chitose-0.0.3/docs/source/chitose.com.atproto.admin.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.com.atproto.identity.rst` & `chitose-0.0.3/docs/source/chitose.com.atproto.identity.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.com.atproto.label.rst` & `chitose-0.0.3/docs/source/chitose.com.atproto.label.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.com.atproto.moderation.rst` & `chitose-0.0.3/docs/source/chitose.com.atproto.moderation.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.com.atproto.repo.rst` & `chitose-0.0.3/docs/source/chitose.com.atproto.repo.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.com.atproto.server.rst` & `chitose-0.0.3/docs/source/chitose.com.atproto.server.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.com.atproto.sync.rst` & `chitose-0.0.3/docs/source/chitose.com.atproto.sync.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/chitose.rst` & `chitose-0.0.3/docs/source/chitose.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/docs/source/conf.py` & `chitose-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/.gitignore` & `chitose-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/LICENSE` & `chitose-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chitose-0.0.2/README.md` & `chitose-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # Chitose
 
-Chitose is a Python client library for the AT Protocol.
+Chitose is a Python client library for the AT Protocol (Bluesky).
 
 ## Usage
 
 The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/tree/main/packages/api#advanced-api-calls).
 
 For example, you can use `app.bsky.feed.get_timeline()` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
 $ python3
->>> from chitose.agent import BskyAgent
+>>> from chitose import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
 You can also post with `com.atproto.repo.create_record()`:
 ```python
 from datetime import datetime
-from chitose.agent import BskyAgent
+from chitose import BskyAgent
 from chitose.app.bsky.feed.post import Post
 
 agent = BskyAgent(service='https://example.com')
 agent.login(identifier='alice@mail.com', password='hunter2')
 
 record = Post(text='Hello, world!', created_at=datetime.now().isoformat())
 agent.com.atproto.repo.create_record(
     repo=alice.did, collection='app.bsky.feed.post', record=record)
 ```
 
+See also the [`examples`](https://github.com/mnogu/chitose/tree/main/examples) directory for sample code.
+
 ## Documentation
 
 For all the functions and classes available in Chitose, refer to [the Chitose’s documentation](https://chitose.readthedocs.io/en/latest/).
 
-## Installing
+## Install
 
 While you can use Chitose without installing its Python package, you can install [the package](https://pypi.org/project/chitose/):
 ```
 $ python3 -m pip install chitose
 ```
 
 Alternatively, you can build a Python package and install it:
```

### Comparing `chitose-0.0.2/pyproject.toml` & `chitose-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chitose"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Muneyuki Noguchi", email="nogu.dev@gmail.com" },
 ]
 description = "A client library for the AT Protocol (Bluesky) "
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -25,8 +25,9 @@
 
 [tool.hatch.build]
 exclude = [
     '/atproto',
     '/codegen',
     '/generate.py',
     '/test.py',
+    '/.github/'
 ]
```

### Comparing `chitose-0.0.2/PKG-INFO` & `chitose-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitose
-Version: 0.0.2
+Version: 0.0.3
 Summary: A client library for the AT Protocol (Bluesky) 
 Project-URL: Homepage, https://github.com/mnogu/chitose
 Project-URL: Bug Tracker, https://github.com/mnogu/chitose/issues
 Author-email: Muneyuki Noguchi <nogu.dev@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -12,50 +12,52 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Chitose
 
-Chitose is a Python client library for the AT Protocol.
+Chitose is a Python client library for the AT Protocol (Bluesky).
 
 ## Usage
 
 The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/tree/main/packages/api#advanced-api-calls).
 
 For example, you can use `app.bsky.feed.get_timeline()` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
 $ python3
->>> from chitose.agent import BskyAgent
+>>> from chitose import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
 You can also post with `com.atproto.repo.create_record()`:
 ```python
 from datetime import datetime
-from chitose.agent import BskyAgent
+from chitose import BskyAgent
 from chitose.app.bsky.feed.post import Post
 
 agent = BskyAgent(service='https://example.com')
 agent.login(identifier='alice@mail.com', password='hunter2')
 
 record = Post(text='Hello, world!', created_at=datetime.now().isoformat())
 agent.com.atproto.repo.create_record(
     repo=alice.did, collection='app.bsky.feed.post', record=record)
 ```
 
+See also the [`examples`](https://github.com/mnogu/chitose/tree/main/examples) directory for sample code.
+
 ## Documentation
 
 For all the functions and classes available in Chitose, refer to [the Chitose’s documentation](https://chitose.readthedocs.io/en/latest/).
 
-## Installing
+## Install
 
 While you can use Chitose without installing its Python package, you can install [the package](https://pypi.org/project/chitose/):
 ```
 $ python3 -m pip install chitose
 ```
 
 Alternatively, you can build a Python package and install it:
```

