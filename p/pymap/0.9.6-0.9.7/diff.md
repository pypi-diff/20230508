# Comparing `tmp/pymap-0.9.6.tar.gz` & `tmp/pymap-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymap-0.9.6.tar", last modified: Tue Feb 12 00:51:54 2019, max compression
+gzip compressed data, was "dist/pymap-0.9.7.tar", last modified: Tue Feb 12 02:25:58 2019, max compression
```

## Comparing `pymap-0.9.6.tar` & `pymap-0.9.7.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/
--rw-r--r--   0 ian       (1100) ian       (1100)    13406 2019-02-12 00:51:54.000000 pymap-0.9.6/PKG-INFO
--rw-r--r--   0 ian       (1100) ian       (1100)     8937 2019-02-09 02:22:20.000000 pymap-0.9.6/README.md
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/
--rw-r--r--   0 ian       (1100) ian       (1100)      261 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/__init__.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/admin/
--rw-r--r--   0 ian       (1100) ian       (1100)     2873 2019-02-12 00:51:16.000000 pymap-0.9.6/pymap/admin/__init__.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/admin/client/
--rw-r--r--   0 ian       (1100) ian       (1100)     1649 2019-02-12 00:51:16.000000 pymap-0.9.6/pymap/admin/client/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     4171 2019-02-12 00:51:16.000000 pymap-0.9.6/pymap/admin/client/append.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1299 2019-02-12 00:51:16.000000 pymap-0.9.6/pymap/admin/client/command.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/admin/grpc/
--rw-r--r--   0 ian       (1100) ian       (1100)        0 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/admin/grpc/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)      964 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/admin/grpc/admin_grpc.py
--rw-r--r--   0 ian       (1100) ian       (1100)     9155 2019-01-27 22:34:37.000000 pymap-0.9.6/pymap/admin/grpc/admin_pb2.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3642 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/admin/handlers.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/backend/
--rw-r--r--   0 ian       (1100) ian       (1100)        8 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/backend/__init__.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/backend/dict/
--rw-r--r--   0 ian       (1100) ian       (1100)     7232 2019-02-09 02:22:20.000000 pymap-0.9.6/pymap/backend/dict/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1673 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/backend/dict/filter.py
--rw-r--r--   0 ian       (1100) ian       (1100)    10697 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/backend/dict/mailbox.py
--rw-r--r--   0 ian       (1100) ian       (1100)     9605 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/backend/mailbox.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/backend/maildir/
--rw-r--r--   0 ian       (1100) ian       (1100)     7936 2019-02-09 02:22:20.000000 pymap-0.9.6/pymap/backend/maildir/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     4091 2019-01-27 22:30:18.000000 pymap-0.9.6/pymap/backend/maildir/flags.py
--rw-r--r--   0 ian       (1100) ian       (1100)     5849 2019-01-27 22:30:18.000000 pymap-0.9.6/pymap/backend/maildir/io.py
--rw-r--r--   0 ian       (1100) ian       (1100)    10675 2019-01-27 22:30:18.000000 pymap-0.9.6/pymap/backend/maildir/layout.py
--rw-r--r--   0 ian       (1100) ian       (1100)    16239 2019-01-27 22:33:50.000000 pymap-0.9.6/pymap/backend/maildir/mailbox.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1897 2019-01-27 22:30:18.000000 pymap-0.9.6/pymap/backend/maildir/subscriptions.py
--rw-r--r--   0 ian       (1100) ian       (1100)     5815 2019-01-27 22:30:18.000000 pymap-0.9.6/pymap/backend/maildir/uidlist.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/backend/redis/
--rw-r--r--   0 ian       (1100) ian       (1100)     8991 2019-02-09 02:22:20.000000 pymap-0.9.6/pymap/backend/redis/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     5478 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/backend/redis/filter.py
--rw-r--r--   0 ian       (1100) ian       (1100)    19452 2019-02-12 00:51:16.000000 pymap-0.9.6/pymap/backend/redis/mailbox.py
--rw-r--r--   0 ian       (1100) ian       (1100)    11442 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/backend/session.py
--rw-r--r--   0 ian       (1100) ian       (1100)     6950 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/bytes.py
--rw-r--r--   0 ian       (1100) ian       (1100)    13451 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/concurrent.py
--rw-r--r--   0 ian       (1100) ian       (1100)     7146 2019-02-10 20:45:34.000000 pymap-0.9.6/pymap/config.py
--rw-r--r--   0 ian       (1100) ian       (1100)      951 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/context.py
--rw-r--r--   0 ian       (1100) ian       (1100)     4713 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/exceptions.py
--rw-r--r--   0 ian       (1100) ian       (1100)     6227 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/fetch.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3895 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/filter.py
--rw-r--r--   0 ian       (1100) ian       (1100)     6129 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/flags.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/imap/
--rw-r--r--   0 ian       (1100) ian       (1100)    15769 2019-02-10 16:17:02.000000 pymap-0.9.6/pymap/imap/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)    16159 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/imap/state.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/interfaces/
--rw-r--r--   0 ian       (1100) ian       (1100)       71 2018-10-25 20:40:15.000000 pymap-0.9.6/pymap/interfaces/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2801 2019-02-10 16:17:02.000000 pymap-0.9.6/pymap/interfaces/backend.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3836 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/interfaces/filter.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1856 2018-12-16 17:21:25.000000 pymap-0.9.6/pymap/interfaces/mailbox.py
--rw-r--r--   0 ian       (1100) ian       (1100)     7432 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/interfaces/message.py
--rw-r--r--   0 ian       (1100) ian       (1100)    12827 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/interfaces/session.py
--rw-r--r--   0 ian       (1100) ian       (1100)     5280 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/listtree.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2656 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/mailbox.py
--rw-r--r--   0 ian       (1100) ian       (1100)     4215 2019-02-12 00:51:16.000000 pymap-0.9.6/pymap/main.py
--rw-r--r--   0 ian       (1100) ian       (1100)    10648 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/message.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/mime/
--rw-r--r--   0 ian       (1100) ian       (1100)    14501 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/mime/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)      944 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/mime/_util.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2661 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/mime/cte.py
--rw-r--r--   0 ian       (1100) ian       (1100)     6492 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/mime/parsed.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/parsing/
--rw-r--r--   0 ian       (1100) ian       (1100)     8247 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/parsing/__init__.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/parsing/command/
--rw-r--r--   0 ian       (1100) ian       (1100)     2834 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/command/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)      584 2019-01-27 22:30:18.000000 pymap-0.9.6/pymap/parsing/command/any.py
--rw-r--r--   0 ian       (1100) ian       (1100)    10575 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/parsing/command/auth.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2199 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/command/nonauth.py
--rw-r--r--   0 ian       (1100) ian       (1100)    16439 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/command/select.py
--rw-r--r--   0 ian       (1100) ian       (1100)     5434 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/parsing/commands.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2017 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/exceptions.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2866 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/parsing/modutf7.py
--rw-r--r--   0 ian       (1100) ian       (1100)    14676 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/parsing/primitives.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/parsing/response/
--rw-r--r--   0 ian       (1100) ian       (1100)     9210 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/parsing/response/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     4070 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/parsing/response/code.py
--rw-r--r--   0 ian       (1100) ian       (1100)    18966 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/parsing/response/fetch.py
--rw-r--r--   0 ian       (1100) ian       (1100)     7096 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/parsing/response/specials.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/parsing/specials/
--rw-r--r--   0 ian       (1100) ian       (1100)      648 2019-01-27 22:30:19.000000 pymap-0.9.6/pymap/parsing/specials/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1755 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/astring.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1650 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/datetime_.py
--rw-r--r--   0 ian       (1100) ian       (1100)     9234 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/parsing/specials/fetchattr.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3310 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/flag.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1258 2019-01-27 22:32:58.000000 pymap-0.9.6/pymap/parsing/specials/mailbox.py
--rw-r--r--   0 ian       (1100) ian       (1100)     5381 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/options.py
--rw-r--r--   0 ian       (1100) ian       (1100)     7966 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/searchkey.py
--rw-r--r--   0 ian       (1100) ian       (1100)     7288 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/sequenceset.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1520 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/statusattr.py
--rw-r--r--   0 ian       (1100) ian       (1100)      988 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/parsing/specials/tag.py
--rw-r--r--   0 ian       (1100) ian       (1100)    13946 2019-01-27 22:31:26.000000 pymap-0.9.6/pymap/search.py
--rw-r--r--   0 ian       (1100) ian       (1100)    16497 2019-02-06 15:00:29.000000 pymap-0.9.6/pymap/selected.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/sieve/
--rw-r--r--   0 ian       (1100) ian       (1100)     2467 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/sieve/__init__.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap/sieve/manage/
--rw-r--r--   0 ian       (1100) ian       (1100)    12339 2019-02-12 00:51:16.000000 pymap-0.9.6/pymap/sieve/manage/__init__.py
--rw-r--r--   0 ian       (1100) ian       (1100)     9166 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/sieve/manage/command.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3861 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/sieve/manage/response.py
--rw-r--r--   0 ian       (1100) ian       (1100)     4556 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/sieve/manage/state.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2370 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/sieve/runner.py
--rw-r--r--   0 ian       (1100) ian       (1100)    10028 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/sieve/tests.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1721 2019-02-01 03:49:10.000000 pymap-0.9.6/pymap/sieve/util.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2587 2019-02-10 16:17:02.000000 pymap-0.9.6/pymap/sockets.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2440 2019-02-10 16:17:02.000000 pymap-0.9.6/pymap/sockinfo.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap.egg-info/
--rw-r--r--   0 ian       (1100) ian       (1100)    13406 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1100) ian       (1100)     2945 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1100) ian       (1100)        1 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1100) ian       (1100)      444 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1100) ian       (1100)       86 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap.egg-info/requires.txt
--rw-r--r--   0 ian       (1100) ian       (1100)        6 2019-02-12 00:51:54.000000 pymap-0.9.6/pymap.egg-info/top_level.txt
--rw-r--r--   0 ian       (1100) ian       (1100)     1487 2019-02-12 00:51:54.000000 pymap-0.9.6/setup.cfg
--rw-r--r--   0 ian       (1100) ian       (1100)     1303 2019-02-08 03:35:10.000000 pymap-0.9.6/setup.py
-drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 00:51:54.000000 pymap-0.9.6/test/
--rw-r--r--   0 ian       (1100) ian       (1100)     2172 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_listtree.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3582 2019-01-27 22:32:58.000000 pymap-0.9.6/test/test_mime.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1423 2019-02-06 15:00:29.000000 pymap-0.9.6/test/test_mime_cte.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2723 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_parsing.py
--rw-r--r--   0 ian       (1100) ian       (1100)      882 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_parsing_command.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3813 2018-10-22 13:47:50.000000 pymap-0.9.6/test/test_parsing_command_auth.py
--rw-r--r--   0 ian       (1100) ian       (1100)      629 2018-10-17 12:27:15.000000 pymap-0.9.6/test/test_parsing_command_nonauth.py
--rw-r--r--   0 ian       (1100) ian       (1100)     6960 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_parsing_command_select.py
--rw-r--r--   0 ian       (1100) ian       (1100)     7189 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_parsing_primitives.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2175 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_parsing_response.py
--rw-r--r--   0 ian       (1100) ian       (1100)     1584 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_parsing_response_code.py
--rw-r--r--   0 ian       (1100) ian       (1100)     2474 2019-02-06 15:00:29.000000 pymap-0.9.6/test/test_parsing_response_specials.py
--rw-r--r--   0 ian       (1100) ian       (1100)    15096 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_parsing_specials.py
--rw-r--r--   0 ian       (1100) ian       (1100)    10533 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_selected.py
--rw-r--r--   0 ian       (1100) ian       (1100)     3388 2019-01-27 22:31:26.000000 pymap-0.9.6/test/test_sequenceset.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/
+-rw-r--r--   0 ian       (1100) ian       (1100)    13406 2019-02-12 02:25:58.000000 pymap-0.9.7/PKG-INFO
+-rw-r--r--   0 ian       (1100) ian       (1100)     8937 2019-02-09 02:22:20.000000 pymap-0.9.7/README.md
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/
+-rw-r--r--   0 ian       (1100) ian       (1100)      261 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/__init__.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/admin/
+-rw-r--r--   0 ian       (1100) ian       (1100)     2873 2019-02-12 00:51:16.000000 pymap-0.9.7/pymap/admin/__init__.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/admin/client/
+-rw-r--r--   0 ian       (1100) ian       (1100)     1649 2019-02-12 00:51:16.000000 pymap-0.9.7/pymap/admin/client/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     4171 2019-02-12 00:51:16.000000 pymap-0.9.7/pymap/admin/client/append.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1299 2019-02-12 00:51:16.000000 pymap-0.9.7/pymap/admin/client/command.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/admin/grpc/
+-rw-r--r--   0 ian       (1100) ian       (1100)        0 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/admin/grpc/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)      964 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/admin/grpc/admin_grpc.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     9155 2019-01-27 22:34:37.000000 pymap-0.9.7/pymap/admin/grpc/admin_pb2.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3642 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/admin/handlers.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/backend/
+-rw-r--r--   0 ian       (1100) ian       (1100)        8 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/backend/__init__.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/backend/dict/
+-rw-r--r--   0 ian       (1100) ian       (1100)     7232 2019-02-09 02:22:20.000000 pymap-0.9.7/pymap/backend/dict/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1673 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/backend/dict/filter.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    10697 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/backend/dict/mailbox.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     9605 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/backend/mailbox.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/backend/maildir/
+-rw-r--r--   0 ian       (1100) ian       (1100)     7936 2019-02-09 02:22:20.000000 pymap-0.9.7/pymap/backend/maildir/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     4091 2019-01-27 22:30:18.000000 pymap-0.9.7/pymap/backend/maildir/flags.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     5849 2019-01-27 22:30:18.000000 pymap-0.9.7/pymap/backend/maildir/io.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    10675 2019-01-27 22:30:18.000000 pymap-0.9.7/pymap/backend/maildir/layout.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    16239 2019-01-27 22:33:50.000000 pymap-0.9.7/pymap/backend/maildir/mailbox.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1897 2019-01-27 22:30:18.000000 pymap-0.9.7/pymap/backend/maildir/subscriptions.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     5815 2019-01-27 22:30:18.000000 pymap-0.9.7/pymap/backend/maildir/uidlist.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/backend/redis/
+-rw-r--r--   0 ian       (1100) ian       (1100)     8991 2019-02-09 02:22:20.000000 pymap-0.9.7/pymap/backend/redis/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     5478 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/backend/redis/filter.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    19452 2019-02-12 00:51:16.000000 pymap-0.9.7/pymap/backend/redis/mailbox.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    11442 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/backend/session.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     6950 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/bytes.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    13451 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/concurrent.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     7146 2019-02-10 20:45:34.000000 pymap-0.9.7/pymap/config.py
+-rw-r--r--   0 ian       (1100) ian       (1100)      951 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/context.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     4713 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/exceptions.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     6227 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/fetch.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3895 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/filter.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     6129 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/flags.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/imap/
+-rw-r--r--   0 ian       (1100) ian       (1100)    15769 2019-02-10 16:17:02.000000 pymap-0.9.7/pymap/imap/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    16159 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/imap/state.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/interfaces/
+-rw-r--r--   0 ian       (1100) ian       (1100)       71 2018-10-25 20:40:15.000000 pymap-0.9.7/pymap/interfaces/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2801 2019-02-10 16:17:02.000000 pymap-0.9.7/pymap/interfaces/backend.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3836 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/interfaces/filter.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1856 2018-12-16 17:21:25.000000 pymap-0.9.7/pymap/interfaces/mailbox.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     7432 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/interfaces/message.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    12827 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/interfaces/session.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     5280 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/listtree.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2656 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/mailbox.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     4426 2019-02-12 02:25:48.000000 pymap-0.9.7/pymap/main.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    10648 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/message.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/mime/
+-rw-r--r--   0 ian       (1100) ian       (1100)    14501 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/mime/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)      944 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/mime/_util.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2661 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/mime/cte.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     6492 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/mime/parsed.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/parsing/
+-rw-r--r--   0 ian       (1100) ian       (1100)     8247 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/parsing/__init__.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/parsing/command/
+-rw-r--r--   0 ian       (1100) ian       (1100)     2834 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/command/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)      584 2019-01-27 22:30:18.000000 pymap-0.9.7/pymap/parsing/command/any.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    10575 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/parsing/command/auth.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2199 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/command/nonauth.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    16439 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/command/select.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     5434 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/parsing/commands.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2017 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/exceptions.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2866 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/parsing/modutf7.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    14676 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/parsing/primitives.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/parsing/response/
+-rw-r--r--   0 ian       (1100) ian       (1100)     9210 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/parsing/response/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     4070 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/parsing/response/code.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    18966 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/parsing/response/fetch.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     7096 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/parsing/response/specials.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/parsing/specials/
+-rw-r--r--   0 ian       (1100) ian       (1100)      648 2019-01-27 22:30:19.000000 pymap-0.9.7/pymap/parsing/specials/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1755 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/astring.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1650 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/datetime_.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     9234 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/parsing/specials/fetchattr.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3310 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/flag.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1258 2019-01-27 22:32:58.000000 pymap-0.9.7/pymap/parsing/specials/mailbox.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     5381 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/options.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     7966 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/searchkey.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     7288 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/sequenceset.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1520 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/statusattr.py
+-rw-r--r--   0 ian       (1100) ian       (1100)      988 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/parsing/specials/tag.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    13946 2019-01-27 22:31:26.000000 pymap-0.9.7/pymap/search.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    16497 2019-02-06 15:00:29.000000 pymap-0.9.7/pymap/selected.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/sieve/
+-rw-r--r--   0 ian       (1100) ian       (1100)     2467 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/sieve/__init__.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap/sieve/manage/
+-rw-r--r--   0 ian       (1100) ian       (1100)    12339 2019-02-12 00:51:16.000000 pymap-0.9.7/pymap/sieve/manage/__init__.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     9166 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/sieve/manage/command.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3861 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/sieve/manage/response.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     4556 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/sieve/manage/state.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2370 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/sieve/runner.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    10028 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/sieve/tests.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1721 2019-02-01 03:49:10.000000 pymap-0.9.7/pymap/sieve/util.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2587 2019-02-10 16:17:02.000000 pymap-0.9.7/pymap/sockets.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2440 2019-02-10 16:17:02.000000 pymap-0.9.7/pymap/sockinfo.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap.egg-info/
+-rw-r--r--   0 ian       (1100) ian       (1100)    13406 2019-02-12 02:25:57.000000 pymap-0.9.7/pymap.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1100) ian       (1100)     2945 2019-02-12 02:25:58.000000 pymap-0.9.7/pymap.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1100) ian       (1100)        1 2019-02-12 02:25:57.000000 pymap-0.9.7/pymap.egg-info/dependency_links.txt
+-rw-r--r--   0 ian       (1100) ian       (1100)      444 2019-02-12 02:25:57.000000 pymap-0.9.7/pymap.egg-info/entry_points.txt
+-rw-r--r--   0 ian       (1100) ian       (1100)       86 2019-02-12 02:25:57.000000 pymap-0.9.7/pymap.egg-info/requires.txt
+-rw-r--r--   0 ian       (1100) ian       (1100)        6 2019-02-12 02:25:57.000000 pymap-0.9.7/pymap.egg-info/top_level.txt
+-rw-r--r--   0 ian       (1100) ian       (1100)     1487 2019-02-12 02:25:58.000000 pymap-0.9.7/setup.cfg
+-rw-r--r--   0 ian       (1100) ian       (1100)     1303 2019-02-08 03:35:10.000000 pymap-0.9.7/setup.py
+drwxr-xr-x   0 ian       (1100) ian       (1100)        0 2019-02-12 02:25:58.000000 pymap-0.9.7/test/
+-rw-r--r--   0 ian       (1100) ian       (1100)     2172 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_listtree.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3582 2019-01-27 22:32:58.000000 pymap-0.9.7/test/test_mime.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1423 2019-02-06 15:00:29.000000 pymap-0.9.7/test/test_mime_cte.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2723 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_parsing.py
+-rw-r--r--   0 ian       (1100) ian       (1100)      882 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_parsing_command.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3813 2018-10-22 13:47:50.000000 pymap-0.9.7/test/test_parsing_command_auth.py
+-rw-r--r--   0 ian       (1100) ian       (1100)      629 2018-10-17 12:27:15.000000 pymap-0.9.7/test/test_parsing_command_nonauth.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     6960 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_parsing_command_select.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     7189 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_parsing_primitives.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2175 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_parsing_response.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     1584 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_parsing_response_code.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     2474 2019-02-06 15:00:29.000000 pymap-0.9.7/test/test_parsing_response_specials.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    15096 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_parsing_specials.py
+-rw-r--r--   0 ian       (1100) ian       (1100)    10533 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_selected.py
+-rw-r--r--   0 ian       (1100) ian       (1100)     3388 2019-01-27 22:31:26.000000 pymap-0.9.7/test/test_sequenceset.py
```

### Comparing `pymap-0.9.6/PKG-INFO` & `pymap-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymap
-Version: 0.9.6
+Version: 0.9.7
 Summary: Lightweight, asynchronous IMAP serving in Python.
 Home-page: https://github.com/icgood/pymap/
 Author: Ian Good
 Author-email: icgood@gmail.com
 License: MIT
 Description: pymap
         =====
```

### Comparing `pymap-0.9.6/README.md` & `pymap-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/admin/__init__.py` & `pymap-0.9.7/pymap/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/admin/client/__init__.py` & `pymap-0.9.7/pymap/admin/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/admin/client/append.py` & `pymap-0.9.7/pymap/admin/client/append.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/admin/client/command.py` & `pymap-0.9.7/pymap/admin/client/command.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/admin/grpc/admin_grpc.py` & `pymap-0.9.7/pymap/admin/grpc/admin_grpc.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/admin/grpc/admin_pb2.py` & `pymap-0.9.7/pymap/admin/grpc/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/admin/handlers.py` & `pymap-0.9.7/pymap/admin/handlers.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/dict/__init__.py` & `pymap-0.9.7/pymap/backend/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/dict/filter.py` & `pymap-0.9.7/pymap/backend/dict/filter.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/dict/mailbox.py` & `pymap-0.9.7/pymap/backend/dict/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/mailbox.py` & `pymap-0.9.7/pymap/backend/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/maildir/__init__.py` & `pymap-0.9.7/pymap/backend/maildir/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/maildir/flags.py` & `pymap-0.9.7/pymap/backend/maildir/flags.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/maildir/io.py` & `pymap-0.9.7/pymap/backend/maildir/io.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/maildir/layout.py` & `pymap-0.9.7/pymap/backend/maildir/layout.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/maildir/mailbox.py` & `pymap-0.9.7/pymap/backend/maildir/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/maildir/subscriptions.py` & `pymap-0.9.7/pymap/backend/maildir/subscriptions.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/maildir/uidlist.py` & `pymap-0.9.7/pymap/backend/maildir/uidlist.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/redis/__init__.py` & `pymap-0.9.7/pymap/backend/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/redis/filter.py` & `pymap-0.9.7/pymap/backend/redis/filter.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/redis/mailbox.py` & `pymap-0.9.7/pymap/backend/redis/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/backend/session.py` & `pymap-0.9.7/pymap/backend/session.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/bytes.py` & `pymap-0.9.7/pymap/bytes.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/concurrent.py` & `pymap-0.9.7/pymap/concurrent.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/config.py` & `pymap-0.9.7/pymap/config.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/context.py` & `pymap-0.9.7/pymap/context.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/exceptions.py` & `pymap-0.9.7/pymap/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/fetch.py` & `pymap-0.9.7/pymap/fetch.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/filter.py` & `pymap-0.9.7/pymap/filter.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/flags.py` & `pymap-0.9.7/pymap/flags.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/imap/__init__.py` & `pymap-0.9.7/pymap/imap/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/imap/state.py` & `pymap-0.9.7/pymap/imap/state.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/interfaces/backend.py` & `pymap-0.9.7/pymap/interfaces/backend.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/interfaces/filter.py` & `pymap-0.9.7/pymap/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/interfaces/mailbox.py` & `pymap-0.9.7/pymap/interfaces/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/interfaces/message.py` & `pymap-0.9.7/pymap/interfaces/message.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/interfaces/session.py` & `pymap-0.9.7/pymap/interfaces/session.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/listtree.py` & `pymap-0.9.7/pymap/listtree.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/mailbox.py` & `pymap-0.9.7/pymap/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/main.py` & `pymap-0.9.7/pymap/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 from typing import Any, Type, Sequence, Mapping
 
 from pkg_resources import iter_entry_points, DistributionNotFound
 
 from . import __version__
 from .interfaces.backend import BackendInterface, ServiceInterface
 
+try:
+    import systemd.daemon  # type: ignore
+except ImportError:
+    def notify_ready() -> None:
+        pass
+else:
+    def notify_ready() -> None:
+        systemd.daemon.notify('READY=1')
+
 _Backends = Mapping[str, Type[BackendInterface]]
 _Services = Mapping[str, Type[ServiceInterface]]
 
 
 def main() -> None:
     parser = ArgumentParser(
         description=__doc__,
@@ -70,14 +79,15 @@
               service_types: Sequence[Type[ServiceInterface]]) -> None:
     backend, config = await backend_type.init(args)
     config.apply_context()
     services = [await service.start(backend, config)
                 for service in service_types]
 
     _drop_privileges(args)
+    notify_ready()
     await asyncio.gather(*[service.task for service in services])
 
 
 def _load_entry_points(group: str) \
         -> Mapping[str, Type[Any]]:
     ret = {}
     for entry_point in iter_entry_points(group):
```

### Comparing `pymap-0.9.6/pymap/message.py` & `pymap-0.9.7/pymap/message.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/mime/__init__.py` & `pymap-0.9.7/pymap/mime/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/mime/_util.py` & `pymap-0.9.7/pymap/mime/_util.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/mime/cte.py` & `pymap-0.9.7/pymap/mime/cte.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/mime/parsed.py` & `pymap-0.9.7/pymap/mime/parsed.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/__init__.py` & `pymap-0.9.7/pymap/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/command/__init__.py` & `pymap-0.9.7/pymap/parsing/command/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/command/any.py` & `pymap-0.9.7/pymap/parsing/command/any.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/command/auth.py` & `pymap-0.9.7/pymap/parsing/command/auth.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/command/nonauth.py` & `pymap-0.9.7/pymap/parsing/command/nonauth.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/command/select.py` & `pymap-0.9.7/pymap/parsing/command/select.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/commands.py` & `pymap-0.9.7/pymap/parsing/commands.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/exceptions.py` & `pymap-0.9.7/pymap/parsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/modutf7.py` & `pymap-0.9.7/pymap/parsing/modutf7.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/primitives.py` & `pymap-0.9.7/pymap/parsing/primitives.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/response/__init__.py` & `pymap-0.9.7/pymap/parsing/response/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/response/code.py` & `pymap-0.9.7/pymap/parsing/response/code.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/response/fetch.py` & `pymap-0.9.7/pymap/parsing/response/fetch.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/response/specials.py` & `pymap-0.9.7/pymap/parsing/response/specials.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/__init__.py` & `pymap-0.9.7/pymap/parsing/specials/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/astring.py` & `pymap-0.9.7/pymap/parsing/specials/astring.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/datetime_.py` & `pymap-0.9.7/pymap/parsing/specials/datetime_.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/fetchattr.py` & `pymap-0.9.7/pymap/parsing/specials/fetchattr.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/flag.py` & `pymap-0.9.7/pymap/parsing/specials/flag.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/mailbox.py` & `pymap-0.9.7/pymap/parsing/specials/mailbox.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/options.py` & `pymap-0.9.7/pymap/parsing/specials/options.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/searchkey.py` & `pymap-0.9.7/pymap/parsing/specials/searchkey.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/sequenceset.py` & `pymap-0.9.7/pymap/parsing/specials/sequenceset.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/statusattr.py` & `pymap-0.9.7/pymap/parsing/specials/statusattr.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/parsing/specials/tag.py` & `pymap-0.9.7/pymap/parsing/specials/tag.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/search.py` & `pymap-0.9.7/pymap/search.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/selected.py` & `pymap-0.9.7/pymap/selected.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/__init__.py` & `pymap-0.9.7/pymap/sieve/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/manage/__init__.py` & `pymap-0.9.7/pymap/sieve/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/manage/command.py` & `pymap-0.9.7/pymap/sieve/manage/command.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/manage/response.py` & `pymap-0.9.7/pymap/sieve/manage/response.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/manage/state.py` & `pymap-0.9.7/pymap/sieve/manage/state.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/runner.py` & `pymap-0.9.7/pymap/sieve/runner.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/tests.py` & `pymap-0.9.7/pymap/sieve/tests.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sieve/util.py` & `pymap-0.9.7/pymap/sieve/util.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sockets.py` & `pymap-0.9.7/pymap/sockets.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap/sockinfo.py` & `pymap-0.9.7/pymap/sockinfo.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/pymap.egg-info/PKG-INFO` & `pymap-0.9.7/pymap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymap
-Version: 0.9.6
+Version: 0.9.7
 Summary: Lightweight, asynchronous IMAP serving in Python.
 Home-page: https://github.com/icgood/pymap/
 Author: Ian Good
 Author-email: icgood@gmail.com
 License: MIT
 Description: pymap
         =====
```

### Comparing `pymap-0.9.6/pymap.egg-info/SOURCES.txt` & `pymap-0.9.7/pymap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/setup.cfg` & `pymap-0.9.7/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymap
-version = 0.9.6
+version = 0.9.7
 author = Ian Good
 author_email = icgood@gmail.com
 description = Lightweight, asynchronous IMAP serving in Python.
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/icgood/pymap/
```

### Comparing `pymap-0.9.6/setup.py` & `pymap-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_listtree.py` & `pymap-0.9.7/test/test_listtree.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_mime.py` & `pymap-0.9.7/test/test_mime.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_mime_cte.py` & `pymap-0.9.7/test/test_mime_cte.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing.py` & `pymap-0.9.7/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_command.py` & `pymap-0.9.7/test/test_parsing_command.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_command_auth.py` & `pymap-0.9.7/test/test_parsing_command_auth.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_command_nonauth.py` & `pymap-0.9.7/test/test_parsing_command_nonauth.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_command_select.py` & `pymap-0.9.7/test/test_parsing_command_select.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_primitives.py` & `pymap-0.9.7/test/test_parsing_primitives.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_response.py` & `pymap-0.9.7/test/test_parsing_response.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_response_code.py` & `pymap-0.9.7/test/test_parsing_response_code.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_response_specials.py` & `pymap-0.9.7/test/test_parsing_response_specials.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_parsing_specials.py` & `pymap-0.9.7/test/test_parsing_specials.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_selected.py` & `pymap-0.9.7/test/test_selected.py`

 * *Files identical despite different names*

### Comparing `pymap-0.9.6/test/test_sequenceset.py` & `pymap-0.9.7/test/test_sequenceset.py`

 * *Files identical despite different names*

