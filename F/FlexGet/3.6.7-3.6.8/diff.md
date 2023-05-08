# Comparing `tmp/FlexGet-3.6.7.tar.gz` & `tmp/FlexGet-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-pu2qd2mx/FlexGet-3.6.7.tar", last modified: Thu May  4 15:13:51 2023, max compression
+gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-r5m8npav/FlexGet-3.6.8.tar", last modified: Mon May  8 15:13:18 2023, max compression
```

## Comparing `FlexGet-3.6.7.tar` & `FlexGet-3.6.8.tar`

### file list

```diff
@@ -1,981 +1,982 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/FlexGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-04 15:13:50.000000 FlexGet-3.6.7/FlexGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-05-04 15:13:51.000000 FlexGet-3.6.7/FlexGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:13:50.000000 FlexGet-3.6.7/FlexGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 15:13:50.000000 FlexGet-3.6.7/FlexGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-04 15:13:50.000000 FlexGet-3.6.7/FlexGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 15:13:50.000000 FlexGet-3.6.7/FlexGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-04 15:13:18.000000 FlexGet-3.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 15:13:18.000000 FlexGet-3.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-04 15:13:51.000000 FlexGet-3.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-04 15:13:18.000000 FlexGet-3.6.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-04 15:13:18.000000 FlexGet-3.6.7/dev-requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-04 15:13:18.000000 FlexGet-3.6.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/templates/api_response.html
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/api/templates/swagger-ui.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archive/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/archives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archives/archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archives/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/backlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/backlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/backlog/backlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/backlog/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/backlog/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/bittorrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/convert_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/magnet_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/private_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/torrent_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/torrent_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/torrent_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/torrent_scrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/torrent_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/bittorrent/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/emby/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/emby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83287 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/emby/api_emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/emby/emby_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/emby/emby_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/emby/emby_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/emby/emby_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/emby/from_emby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/estimate_release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/estimate_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/estimate_release/estimate_release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/estimate_release/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/estimate_release/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/estimate_release/estimators/est_movies_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/estimate_release/estimators/est_released_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/estimate_release/estimators/est_series_tvmaze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/failed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/failed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/failed/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/failed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/failed/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/failed/retry_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/ftp/ftp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/ftp/ftp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/ftp/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/ftp/sftp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/history/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/history/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/history/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/history/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/imdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/from_imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/imdb_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/imdb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/imdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/irc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/irc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/irc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/irc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/irc/irc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/managed_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/list_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/list_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/list_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/list_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/couchpotato_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/entry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/imdb_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/movie_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/pending_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/plex_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/radarr_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/sonarr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/subtitle_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/thetvdb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/managed_lists/lists/yaml_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/notify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notification_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/cronitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/gotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/ifttt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/microsoftteams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/notifymyandroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/ntfysh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/prowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/pushalot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/pushover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/pushsafer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/rapidpush.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/sms_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/toast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notifiers/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/notify/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/parsing/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/parsing/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/parsing/parsers/parser_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/parsing/parsers/parser_guessit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/parsing/parsers/parser_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/parsing/plugin_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/pending_approval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/pending_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/pending_approval/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/pending_approval/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/pending_approval/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/pending_approval/pending_approval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/rejected/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/rejected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/rejected/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/rejected/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/rejected/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/rejected/remember_rejected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/scheduler/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/seen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/seen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/seen/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/seen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/seen/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/seen/seen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/seen/seen_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/seen/seen_movies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/all_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    47009 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/configure_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    56988 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/gen_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/internal_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/metainfo_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/next_series_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/next_series_seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)    53376 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/series_begin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/series_premiere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/series_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/series/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/sites/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/allyoulike.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/alpharatio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/animeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/anirena.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/archetorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/argenteam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/awesomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/bakabt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/btn.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/cinemageddon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/cpasbien.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/deadfrog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/descargas2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/ettv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/eztv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/filelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/filelist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/frenchtorrentdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/fuzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/google_cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/hebits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/hliang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/horriblesubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/koreus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/limetorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26049 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/lostfilm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/magnetdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/morethantv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/ncore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/newtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/newznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/nnmclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/passthepopcorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/ptn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/rarbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/rlsbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/rmz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/serienjunkies.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/shortened.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/site_1337x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/site_rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/solidtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/torrent_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/torrentday.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/torrentz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/wordpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/sites/yts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/urlrewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/urlrewrite_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/urlrewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/sites/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/status/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/status/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/status/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/status/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/thetvdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/thetvdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/thetvdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30407 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/thetvdb/api_tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/thetvdb/thetvdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/tmdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tmdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tmdb/api_tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tmdb/tmdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/api_trakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    42193 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/next_trakt_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/trakt_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/trakt_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/trakt/trakt_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/tvmaze/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tvmaze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tvmaze/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26621 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tvmaze/api_tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/tvmaze/tvmaze_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/components/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/variables/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/components/variables/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/db_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    42591 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/explain_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/inject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/perf_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/try_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/wiki_qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/cli/win32_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/pyload.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    40203 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/clients/transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/daemon/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/abort_if_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/accept_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/best_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/content_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/crossmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/exists_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/exists_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/if_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/limit_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/magnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/only_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/proper_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/require_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/thetvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/filter/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/generic/cron_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/generic/db_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/generic/db_vacuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/generic/log_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/generic/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/generic/welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/input/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/anidb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/apple_trailers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/betaseries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/filmweb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/from_piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/from_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/from_telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/input_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/kitsu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/letterboxd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/medusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/my_anime_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/myepisodes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/next_sonarr_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/npo_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/plex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/pogcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/regexp_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/rlslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/rottentomatoes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/sceper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/sickbeard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/torznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/input/twitterfeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/internal/api_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/internal/api_rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/internal/change_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/metainfo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/assume_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/bluray_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/media_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/metainfo_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/nfo_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/nzb_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/rottentomatoes_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/subtitles_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/metainfo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/modify/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/path_by_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/path_by_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/plugin_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/reorder_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/set_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/modify/sort_by_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/operate/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/abort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/cfscraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/debug_db_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/debug_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/disable_phases.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/domain_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/entry_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/formlogin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/free_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/max_reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/spy_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/verbose_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/verify_ssl_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/operate/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/output/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22419 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/download_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/dump_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/memusage.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/mock_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/rtorrent_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/subtitles_periscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/subtitles_subliminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/output/utorrent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/services/kodi_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/services/myepisodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/plugins/services/pogcal_acquired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/resources/flexget.png
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/templates/entry/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/templates/entry/default.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/templates/task/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/templates/task/default.template
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/templates/task/html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/templates/task/rss.template
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/tray_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/app.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/app/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/app/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/assets/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.eot
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/app/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-05-04 15:13:45.000000 FlexGet-3.6.7/flexget/ui/v1/app/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-04 15:13:45.000000 FlexGet-3.6.7/flexget/ui/v1/app/scripts/splash.js
--rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-05-04 15:13:45.000000 FlexGet-3.6.7/flexget/ui/v1/app/scripts/vendor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/app/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/styles/splash.css
--rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-05-04 15:13:44.000000 FlexGet-3.6.7/flexget/ui/v1/app/styles/vendor.css
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/build.js
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/inject.js
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/lint.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/scripts.js
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/server.js
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/styles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/test.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulp/watch.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/load.failure.html
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/specs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/app.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/app.loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/app.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/app.scss
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/app.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/assets/images/header.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/_error-dialog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/exception/exception.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/exception/exception.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/pagination.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/pagination.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/router/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/router/router-helper.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/router/router-helper.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/url-interceptor/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/404/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/_login.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.config.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/components.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/core/core.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/core/core.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/core/core.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/core/core.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/core/core.route.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/database/_database.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/home/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/_sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/user/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/components/user/user.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/construction.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/directives/directives.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/directives/palette-background/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/layout.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-input/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-stream/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-list/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/new-list/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.route.js
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.scss
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/plugins.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-entry/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-field/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-releases/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.service.js
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/server.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/server.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/server.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/scss/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/scss/_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/scss/_loading-bar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/scss/flexget.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/src/services/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/src/services/schema.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/execute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/history.js
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/movie_list.js
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/registerPlugin.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/schedules.js
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/seen.js
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/series.js
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/states.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
--rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
--rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
--rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
--rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
--rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
--rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
--rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
--rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
--rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
--rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
--rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
--rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
--rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-04 15:13:46.000000 FlexGet-3.6.7/flexget/ui/v2/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/ui/v2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/bittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/cached_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/lazy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:51.000000 FlexGet-3.6.7/flexget/utils/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/parsers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/parsers/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/parsers/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/simple_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/soup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16956 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-04 15:13:18.000000 FlexGet-3.6.7/flexget/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-04 15:13:18.000000 FlexGet-3.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-04 15:13:18.000000 FlexGet-3.6.7/requirements-docker.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-04 15:13:18.000000 FlexGet-3.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:13:51.000000 FlexGet-3.6.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/FlexGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-08 15:13:17.000000 FlexGet-3.6.8/FlexGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39131 2023-05-08 15:13:17.000000 FlexGet-3.6.8/FlexGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:13:17.000000 FlexGet-3.6.8/FlexGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 15:13:17.000000 FlexGet-3.6.8/FlexGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 15:13:17.000000 FlexGet-3.6.8/FlexGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 15:13:17.000000 FlexGet-3.6.8/FlexGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-08 15:12:54.000000 FlexGet-3.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 15:12:54.000000 FlexGet-3.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-08 15:13:18.000000 FlexGet-3.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-08 15:12:54.000000 FlexGet-3.6.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-08 15:12:54.000000 FlexGet-3.6.8/dev-requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-08 15:12:54.000000 FlexGet-3.6.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-08 15:13:07.000000 FlexGet-3.6.8/flexget/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/templates/api_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/api/templates/swagger-ui.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archive/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/archives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archives/archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archives/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/backlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/backlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/backlog/backlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/backlog/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/backlog/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/bittorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/convert_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/magnet_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/private_torrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/torrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/torrent_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/torrent_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/torrent_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/torrent_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/torrent_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/bittorrent/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/emby/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/emby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83287 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/emby/api_emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/emby/emby_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/emby/emby_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/emby/emby_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/emby/emby_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/emby/from_emby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/estimate_release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/estimate_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/estimate_release/estimate_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/estimate_release/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/estimate_release/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/estimate_release/estimators/est_movies_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/estimate_release/estimators/est_released_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/estimate_release/estimators/est_series_tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/failed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/failed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/failed/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/failed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/failed/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/failed/retry_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/ftp/ftp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/ftp/ftp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/ftp/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/ftp/sftp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/history/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/history/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/history/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/imdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/from_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/imdb_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/imdb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/imdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/irc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/irc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/irc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/irc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/irc/irc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/managed_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/list_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/list_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/list_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/list_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/couchpotato_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/entry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/imdb_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/movie_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/pending_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/plex_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/radarr_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/sonarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/subtitle_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/thetvdb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/managed_lists/lists/yaml_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notification_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/cronitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/ifttt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/microsoftteams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/notifymyandroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/ntfysh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/pushalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/pushsafer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/rapidpush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/sms_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/toast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notifiers/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/notify/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/parsing/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/parsing/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/parsing/parsers/parser_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/parsing/parsers/parser_guessit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/parsing/parsers/parser_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/parsing/plugin_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/pending_approval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/pending_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/pending_approval/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/pending_approval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/pending_approval/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/pending_approval/pending_approval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/rejected/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/rejected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/rejected/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/rejected/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/rejected/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/rejected/remember_rejected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/scheduler/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/seen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/seen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/seen/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/seen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/seen/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/seen/seen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/seen/seen_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/seen/seen_movies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/all_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47009 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/configure_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56988 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/gen_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/internal_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/metainfo_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/next_series_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/next_series_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53376 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/series_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/series_premiere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/series_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/series/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/sites/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/allyoulike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/alpharatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/animeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/anirena.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/archetorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/argenteam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/awesomehd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/bakabt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/btn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/cinemageddon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/cpasbien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/deadfrog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/descargas2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/ettv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/eztv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/filelist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/frenchtorrentdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/fuzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/google_cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/hebits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/hliang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/horriblesubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/koreus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/limetorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26049 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/lostfilm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/magnetdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/morethantv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/ncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/newtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/nnmclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/passthepopcorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/ptn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/rarbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/rlsbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/rmz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/serienjunkies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/shortened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/site_1337x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/site_rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/solidtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/torrent_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/torrentday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/torrentz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/wordpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/sites/yts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/urlrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/urlrewrite_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/urlrewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/sites/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/status/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/status/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/status/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/thetvdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/thetvdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/thetvdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30407 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/thetvdb/api_tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/thetvdb/thetvdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tmdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tmdb/api_tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tmdb/tmdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/api_trakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42193 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/next_trakt_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/trakt_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/trakt_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/trakt/trakt_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/tvmaze/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tvmaze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tvmaze/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26621 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tvmaze/api_tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/tvmaze/tvmaze_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/components/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/variables/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/components/variables/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/db_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42591 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/plugins/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/explain_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/perf_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/try_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/wiki_qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/cli/win32_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/plugins/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/pyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40203 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/clients/transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/plugins/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/daemon/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/abort_if_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/accept_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/best_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/content_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/crossmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/exists_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/exists_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/if_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/limit_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/magnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/only_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/proper_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/require_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/thetvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/filter/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/generic/cron_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/generic/db_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/generic/db_vacuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/generic/log_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/generic/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/generic/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/anidb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/apple_trailers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/betaseries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/filmweb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/from_piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/from_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/from_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/input_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/kitsu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/letterboxd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/medusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/my_anime_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/myepisodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/next_sonarr_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/npo_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/plex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/pogcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/regexp_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/rlslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/rottentomatoes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/sceper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/sickbeard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/torznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/input/twitterfeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/internal/api_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/internal/api_rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/internal/change_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/metainfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/assume_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/bluray_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/media_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/metainfo_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/nfo_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/nzb_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/rottentomatoes_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/subtitles_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/metainfo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/modify/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/path_by_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/path_by_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/plugin_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/reorder_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/set_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/modify/sort_by_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/abort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/cfscraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/debug_db_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/debug_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/disable_phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/domain_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/entry_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/formlogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/free_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/max_reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/spy_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/verbose_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/verify_ssl_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/operate/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22419 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/download_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/dump_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/mock_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/rtorrent_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/subtitles_periscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/subtitles_subliminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/output/utorrent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/services/kodi_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/services/myepisodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/plugins/services/pogcal_acquired.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/resources/flexget.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/templates/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/templates/entry/default.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/templates/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/templates/task/default.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/templates/task/html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/templates/task/rss.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/tray_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/app.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/ui/v1/app/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/app/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/assets/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/app/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/scripts/splash.js
+-rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/scripts/vendor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/styles/splash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-05-08 15:13:08.000000 FlexGet-3.6.8/flexget/ui/v1/app/styles/vendor.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/build.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/inject.js
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/lint.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/scripts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/styles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulp/watch.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/load.failure.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/specs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/app.loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/app.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/app.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/app.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/ui/v1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/assets/images/header.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/_error-dialog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/exception/exception.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/exception/exception.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/pagination.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/pagination.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/router/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/router/router-helper.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/router/router-helper.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/url-interceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/404/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/_login.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.config.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/components.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/core/core.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/core/core.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/core/core.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/core/core.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/core/core.route.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/database/_database.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/_sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/components/user/user.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/construction.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/directives/directives.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/directives/palette-background/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/layout.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/new-list/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/plugins.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-field/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:17.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/server.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/server.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/server.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/scss/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/scss/_loading-bar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/scss/flexget.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/src/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/src/services/schema.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/execute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/history.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/movie_list.js
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/registerPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/schedules.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/seen.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/series.js
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/states.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
+-rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
+-rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
+-rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-08 15:13:09.000000 FlexGet-3.6.8/flexget/ui/v2/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/ui/v2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/bittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/cached_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/lazy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:13:18.000000 FlexGet-3.6.8/flexget/utils/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/parsers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/parsers/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/parsers/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/simple_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/soup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16956 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-08 15:12:54.000000 FlexGet-3.6.8/flexget/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-08 15:12:54.000000 FlexGet-3.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-08 15:12:54.000000 FlexGet-3.6.8/requirements-docker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-08 15:12:54.000000 FlexGet-3.6.8/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-08 15:12:54.000000 FlexGet-3.6.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:13:18.000000 FlexGet-3.6.8/setup.cfg
```

### Comparing `FlexGet-3.6.7/FlexGet.egg-info/PKG-INFO` & `FlexGet-3.6.8/FlexGet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.6.7
+Version: 3.6.8
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.6.7/FlexGet.egg-info/SOURCES.txt` & `FlexGet-3.6.8/FlexGet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 dev-requirements-extras.txt
 dev-requirements.txt
 pyproject.toml
 requirements-docker.txt
+requirements-release.txt
 requirements.txt
 FlexGet.egg-info/PKG-INFO
 FlexGet.egg-info/SOURCES.txt
 FlexGet.egg-info/dependency_links.txt
 FlexGet.egg-info/entry_points.txt
 FlexGet.egg-info/requires.txt
 FlexGet.egg-info/top_level.txt
```

### Comparing `FlexGet-3.6.7/FlexGet.egg-info/requires.txt` & `FlexGet-3.6.8/FlexGet.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/LICENSE` & `FlexGet-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/PKG-INFO` & `FlexGet-3.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.6.7
+Version: 3.6.8
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.6.7/README.rst` & `FlexGet-3.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/dev-requirements-extras.txt` & `FlexGet-3.6.8/dev-requirements-extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 appdirs==1.4.4 ; python_version >= "3.7" and python_version < "4.0"
 babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
+bcrypt==4.0.1 ; python_version >= "3.7" and python_version < "4.0"
 beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
 boto3==1.26.27 ; python_version >= "3.7" and python_version < "4.0"
 botocore==1.29.27 ; python_version >= "3.7" and python_version < "4.0"
 certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
+cffi==1.15.1 ; python_version >= "3.7" and python_version < "4.0"
 chardet==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
+cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.7" and python_version < "4.0"
 dogpile-cache==1.1.8 ; python_version >= "3.7" and python_version < "4.0"
 enzyme==0.4.1 ; python_version >= "3.7" and python_version < "4.0"
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4"
 importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.8"
 importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 jmespath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
+paramiko==2.12.0 ; python_version >= "3.7" and python_version < "4.0"
 pbr==5.11.0 ; python_version >= "3.7" and python_version < "4.0"
 plexapi==4.13.1 ; python_version >= "3.7" and python_version < "4.0"
+pycparser==2.21 ; python_version >= "3.7" and python_version < "4.0"
+pynacl==1.5.0 ; python_version >= "3.7" and python_version < "4.0"
+pysftp==0.2.9 ; python_version >= "3.7" and python_version < "4.0"
 pysrt==1.1.2 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 rarfile==4.0 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
 s3transfer==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.6.7/dev-requirements.txt` & `FlexGet-3.6.8/requirements-docker.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,81 @@
-alabaster==0.7.12 ; python_version >= "3.7" and python_version < "4.0"
+aniso8601==9.0.1 ; python_version >= "3.7" and python_version < "4.0"
+apscheduler==3.9.1.post1 ; python_version >= "3.7" and python_version < "4"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
-babel==2.11.0 ; python_version >= "3.7" and python_version < "4.0"
-black==22.12.0 ; python_version >= "3.7" and python_version < "4.0"
-bleach==5.0.1 ; python_version >= "3.7" and python_version < "4.0"
-build==0.9.0 ; python_version >= "3.7" and python_version < "4.0"
+autocommand==2.2.2 ; python_version >= "3.7" and python_version < "4.0"
+babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
+backports-zoneinfo==0.2.1 ; python_version >= "3.7" and python_version < "3.9"
+beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
+brotli==1.0.9 ; python_version >= "3.7" and python_version < "4.0"
 certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
-cffi==1.15.1 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
-cfgv==3.3.1 ; python_version >= "3.7" and python_version < "4.0"
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
+cheroot==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
+cherrypy==18.8.0 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
-codacy-coverage==1.3.11 ; python_version >= "3.7" and python_version < "4.0"
-colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and os_name == "nt" or python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows" or python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
+cloudscraper==1.2.69 ; python_version >= "3.7" and python_version < "4.0"
+colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0"
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
-coverage==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
-coverage[toml]==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
-cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
-distlib==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
-docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
-exceptiongroup==1.0.4 ; python_version >= "3.7" and python_version < "3.11"
-execnet==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
-filelock==3.8.2 ; python_version >= "3.7" and python_version < "4.0"
-gitdb==4.0.10 ; python_version >= "3.7" and python_version < "4.0"
-gitpython==3.1.29 ; python_version >= "3.7" and python_version < "4.0"
-identify==2.5.9 ; python_version >= "3.7" and python_version < "4.0"
+deluge-client==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
+feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
+flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
+flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
+flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
+flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
+flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
+flask==2.2.5 ; python_version >= "3.7" and python_version < "4.0"
+greenlet==2.0.1 ; python_version >= "3.7" and platform_machine == "aarch64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "ppc64le" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "x86_64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "amd64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "AMD64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "win32" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "WIN32" and python_version < "4.0"
+guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
+html5lib==1.1 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4"
-imagesize==1.4.1 ; python_version >= "3.7" and python_version < "4.0"
-importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "4.0"
-iniconfig==1.1.1 ; python_version >= "3.7" and python_version < "4.0"
+importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
+importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
+inflect==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
+itsdangerous==2.1.2 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
-jeepney==0.8.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+jaraco-collections==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
+jaraco-context==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
+jaraco-functools==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
+jaraco-text==3.11.0 ; python_version >= "3.7" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.7" and python_version < "4.0"
-keyring==23.11.0 ; python_version >= "3.7" and python_version < "4.0"
+jsonschema==4.17.3 ; python_version >= "3.7" and python_version < "4.0"
+loguru==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 markupsafe==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 more-itertools==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
-multidict==6.0.3 ; python_version >= "3.7" and python_version < "4.0"
-mypy-extensions==0.4.3 ; python_version >= "3.7" and python_version < "4.0"
-mypy==0.991 ; python_version >= "3.7" and python_version < "4.0"
-nodeenv==1.7.0 ; python_version >= "3.7" and python_version < "4.0"
 packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
-pathspec==0.10.3 ; python_version >= "3.7" and python_version < "4.0"
-pep517==0.13.0 ; python_version >= "3.7" and python_version < "4.0"
-pkginfo==1.9.2 ; python_version >= "3.7" and python_version < "4.0"
-platformdirs==2.6.0 ; python_version >= "3.7" and python_version < "4.0"
-pluggy==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
-pre-commit==2.20.0 ; python_version >= "3.7" and python_version < "4.0"
-pycparser==2.21 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+pkgutil-resolve-name==1.3.10 ; python_version >= "3.7" and python_version < "3.9"
+plumbum==1.8.0 ; python_version >= "3.7" and python_version < "4.0"
+portend==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
+psutil==5.9.4 ; python_version >= "3.7" and python_version < "4.0"
+pydantic==1.10.2 ; python_version >= "3.7" and python_version < "4.0"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
-pytest-cov==4.0.0 ; python_version >= "3.7" and python_version < "4.0"
-pytest-runner==6.0.0 ; python_version >= "3.7" and python_version < "4.0"
-pytest-xdist==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
-pytest==7.2.0 ; python_version >= "3.7" and python_version < "4.0"
-pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
-pywin32-ctypes==0.2.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
+pynzb==0.1.0 ; python_version >= "3.7" and python_version < "4.0"
+pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "4.0"
+pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
+pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
+python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
+pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4"
+pytz==2022.6 ; python_version >= "3.7" and python_version < "4"
+pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
-readme-renderer==37.3 ; python_version >= "3.7" and python_version < "4.0"
+qbittorrent-api==2023.3.44 ; python_version >= "3.7" and python_version < "4.0"
+rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests-toolbelt==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
-rfc3986==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
-ruff==0.0.261 ; python_version >= "3.7" and python_version < "4.0"
-secretstorage==3.3.3 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
-setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
-six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
-smmap==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
-snowballstemmer==2.2.0 ; python_version >= "3.7" and python_version < "4.0"
-sphinx==5.3.0 ; python_version >= "3.7" and python_version < "4.0"
-sphinxcontrib-applehelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
-sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
-sphinxcontrib-htmlhelp==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
-sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
-sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
-sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.7" and python_version < "4.0"
-sqlalchemy-stubs==0.4 ; python_version >= "3.7" and python_version < "4.0"
-toml==0.10.2 ; python_version >= "3.7" and python_version < "4.0"
-tomli==2.0.1 ; python_version >= "3.7" and python_full_version < "3.11.0a7"
-twine==4.0.2 ; python_version >= "3.7" and python_version < "4.0"
-typed-ast==1.5.4 ; python_version < "3.8" and python_version >= "3.7"
+rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
+setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4"
+sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
+six==1.16.0 ; python_version >= "3.7" and python_version < "4"
+soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
+sqlalchemy==1.4.45 ; python_version >= "3.7" and python_version < "4.0"
+tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
+transmission-rpc==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
-urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
-vcrpy==4.2.1 ; python_version >= "3.7" and python_version < "4.0"
-virtualenv==20.17.1 ; python_version >= "3.7" and python_version < "4.0"
+tzdata==2022.7 ; python_version >= "3.7" and python_version < "4"
+tzlocal==4.2 ; python_version >= "3.7" and python_version < "4"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
-wrapt==1.14.1 ; python_version >= "3.7" and python_version < "4.0"
-yarl==1.8.2 ; python_version >= "3.7" and python_version < "4.0"
-zipp==3.11.0 ; python_version >= "3.7" and python_version < "4.0"
+werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
+win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
+zc-lockfile==2.0 ; python_version >= "3.7" and python_version < "4.0"
+zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.10"
+zxcvbn-python==4.4.24 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.6.7/flexget/__init__.py` & `FlexGet-3.6.8/flexget/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/app.py` & `FlexGet-3.6.8/flexget/api/app.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/authentication.py` & `FlexGet-3.6.8/flexget/api/core/authentication.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/cached.py` & `FlexGet-3.6.8/flexget/api/core/cached.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/database.py` & `FlexGet-3.6.8/flexget/api/core/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/format_checker.py` & `FlexGet-3.6.8/flexget/api/core/format_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/plugins.py` & `FlexGet-3.6.8/flexget/api/core/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/schema.py` & `FlexGet-3.6.8/flexget/api/core/schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/server.py` & `FlexGet-3.6.8/flexget/api/core/server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/tasks.py` & `FlexGet-3.6.8/flexget/api/core/tasks.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/core/user.py` & `FlexGet-3.6.8/flexget/api/core/user.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/templates/api_response.html` & `FlexGet-3.6.8/flexget/api/templates/api_response.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/api/templates/swagger-ui.html` & `FlexGet-3.6.8/flexget/api/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/archive/archive.py` & `FlexGet-3.6.8/flexget/components/archive/archive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/archive/cli.py` & `FlexGet-3.6.8/flexget/components/archive/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/archive/db.py` & `FlexGet-3.6.8/flexget/components/archive/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/archives/archives.py` & `FlexGet-3.6.8/flexget/components/archives/archives.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/archives/decompress.py` & `FlexGet-3.6.8/flexget/components/archives/decompress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/archives/utils.py` & `FlexGet-3.6.8/flexget/components/archives/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/backlog/backlog.py` & `FlexGet-3.6.8/flexget/components/backlog/backlog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/backlog/cli.py` & `FlexGet-3.6.8/flexget/components/backlog/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/backlog/db.py` & `FlexGet-3.6.8/flexget/components/backlog/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/convert_magnet.py` & `FlexGet-3.6.8/flexget/components/bittorrent/convert_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/magnet_info_hash.py` & `FlexGet-3.6.8/flexget/components/bittorrent/magnet_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/private_torrents.py` & `FlexGet-3.6.8/flexget/components/bittorrent/private_torrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/torrent.py` & `FlexGet-3.6.8/flexget/components/bittorrent/torrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/torrent_alive.py` & `FlexGet-3.6.8/flexget/components/bittorrent/torrent_alive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/torrent_files.py` & `FlexGet-3.6.8/flexget/components/bittorrent/torrent_files.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/torrent_match.py` & `FlexGet-3.6.8/flexget/components/bittorrent/torrent_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/torrent_scrub.py` & `FlexGet-3.6.8/flexget/components/bittorrent/torrent_scrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/torrent_size.py` & `FlexGet-3.6.8/flexget/components/bittorrent/torrent_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/bittorrent/trackers.py` & `FlexGet-3.6.8/flexget/components/bittorrent/trackers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/emby/api_emby.py` & `FlexGet-3.6.8/flexget/components/emby/api_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/emby/emby_list.py` & `FlexGet-3.6.8/flexget/components/emby/emby_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/emby/emby_lookup.py` & `FlexGet-3.6.8/flexget/components/emby/emby_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/emby/emby_refresh.py` & `FlexGet-3.6.8/flexget/components/emby/emby_refresh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/emby/emby_util.py` & `FlexGet-3.6.8/flexget/components/emby/emby_util.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/emby/from_emby.py` & `FlexGet-3.6.8/flexget/components/emby/from_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/estimate_release/estimate_release.py` & `FlexGet-3.6.8/flexget/components/estimate_release/estimate_release.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/estimate_release/estimators/est_movies_bluray.py` & `FlexGet-3.6.8/flexget/components/estimate_release/estimators/est_movies_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/estimate_release/estimators/est_released_movies.py` & `FlexGet-3.6.8/flexget/components/estimate_release/estimators/est_released_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/estimate_release/estimators/est_series_tvmaze.py` & `FlexGet-3.6.8/flexget/components/estimate_release/estimators/est_series_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/failed/api.py` & `FlexGet-3.6.8/flexget/components/failed/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/failed/cli.py` & `FlexGet-3.6.8/flexget/components/failed/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/failed/db.py` & `FlexGet-3.6.8/flexget/components/failed/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/failed/retry_failed.py` & `FlexGet-3.6.8/flexget/components/failed/retry_failed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/ftp/ftp_download.py` & `FlexGet-3.6.8/flexget/components/ftp/ftp_download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/ftp/ftp_list.py` & `FlexGet-3.6.8/flexget/components/ftp/ftp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/ftp/sftp.py` & `FlexGet-3.6.8/flexget/components/ftp/sftp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/ftp/sftp_client.py` & `FlexGet-3.6.8/flexget/components/ftp/sftp_client.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/history/api.py` & `FlexGet-3.6.8/flexget/components/history/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/history/cli.py` & `FlexGet-3.6.8/flexget/components/history/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/history/db.py` & `FlexGet-3.6.8/flexget/components/history/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/history/history.py` & `FlexGet-3.6.8/flexget/components/history/history.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/api.py` & `FlexGet-3.6.8/flexget/components/imdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/db.py` & `FlexGet-3.6.8/flexget/components/imdb/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/from_imdb.py` & `FlexGet-3.6.8/flexget/components/imdb/from_imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/imdb.py` & `FlexGet-3.6.8/flexget/components/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/imdb_lookup.py` & `FlexGet-3.6.8/flexget/components/imdb/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/imdb_url.py` & `FlexGet-3.6.8/flexget/components/imdb/imdb_url.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/imdb_watchlist.py` & `FlexGet-3.6.8/flexget/components/imdb/imdb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/imdb/utils.py` & `FlexGet-3.6.8/flexget/components/imdb/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/irc/api.py` & `FlexGet-3.6.8/flexget/components/irc/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/irc/cli.py` & `FlexGet-3.6.8/flexget/components/irc/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/irc/irc.py` & `FlexGet-3.6.8/flexget/components/irc/irc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/list_add.py` & `FlexGet-3.6.8/flexget/components/managed_lists/list_add.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/list_clear.py` & `FlexGet-3.6.8/flexget/components/managed_lists/list_clear.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/list_match.py` & `FlexGet-3.6.8/flexget/components/managed_lists/list_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/list_remove.py` & `FlexGet-3.6.8/flexget/components/managed_lists/list_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/couchpotato_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/couchpotato_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/api.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/cli.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/db.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/entry_list/entry_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/entry_list/entry_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/imdb_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/imdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/api.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/cli.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/db.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/movie_list/movie_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/movie_list/movie_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/api.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/cli.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/db.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/pending_list/pending_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/pending_list/pending_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/plex_watchlist.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/plex_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/radarr_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/radarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/cli.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/db.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/regexp_list/regexp_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/regexp_list/regexp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/sonarr_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/sonarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/subtitle_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/subtitle_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/thetvdb_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/thetvdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/managed_lists/lists/yaml_list.py` & `FlexGet-3.6.8/flexget/components/managed_lists/lists/yaml_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notification_framework.py` & `FlexGet-3.6.8/flexget/components/notify/notification_framework.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/bark.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/bark.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/cronitor.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/cronitor.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/discord.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/discord.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/email.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/gotify.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/gotify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/ifttt.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/ifttt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/join.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/join.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/matrix.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/matrix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/microsoftteams.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/microsoftteams.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/mqtt.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/mqtt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/notifymyandroid.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/notifymyandroid.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/ntfysh.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/ntfysh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/prowl.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/prowl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/pushalot.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/pushalot.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/pushbullet.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/pushbullet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/pushover.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/pushover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/pushsafer.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/pushsafer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/rapidpush.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/rapidpush.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/slack.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/sms_ru.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/sms_ru.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/telegram.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/toast.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/toast.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notifiers/xmpp.py` & `FlexGet-3.6.8/flexget/components/notify/notifiers/xmpp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/notify/notify.py` & `FlexGet-3.6.8/flexget/components/notify/notify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/parsing/parsers/parser_common.py` & `FlexGet-3.6.8/flexget/components/parsing/parsers/parser_common.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/parsing/parsers/parser_guessit.py` & `FlexGet-3.6.8/flexget/components/parsing/parsers/parser_guessit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/parsing/parsers/parser_internal.py` & `FlexGet-3.6.8/flexget/components/parsing/parsers/parser_internal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/parsing/plugin_parsing.py` & `FlexGet-3.6.8/flexget/components/parsing/plugin_parsing.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/pending_approval/api.py` & `FlexGet-3.6.8/flexget/components/pending_approval/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/pending_approval/cli.py` & `FlexGet-3.6.8/flexget/components/pending_approval/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/pending_approval/db.py` & `FlexGet-3.6.8/flexget/components/pending_approval/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/pending_approval/pending_approval.py` & `FlexGet-3.6.8/flexget/components/pending_approval/pending_approval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/rejected/api.py` & `FlexGet-3.6.8/flexget/components/rejected/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/rejected/cli.py` & `FlexGet-3.6.8/flexget/components/rejected/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/rejected/db.py` & `FlexGet-3.6.8/flexget/components/rejected/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/rejected/remember_rejected.py` & `FlexGet-3.6.8/flexget/components/rejected/remember_rejected.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/scheduler/api.py` & `FlexGet-3.6.8/flexget/components/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/scheduler/scheduler.py` & `FlexGet-3.6.8/flexget/components/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/seen/api.py` & `FlexGet-3.6.8/flexget/components/seen/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/seen/cli.py` & `FlexGet-3.6.8/flexget/components/seen/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/seen/db.py` & `FlexGet-3.6.8/flexget/components/seen/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/seen/seen.py` & `FlexGet-3.6.8/flexget/components/seen/seen.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/seen/seen_info_hash.py` & `FlexGet-3.6.8/flexget/components/seen/seen_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/seen/seen_movies.py` & `FlexGet-3.6.8/flexget/components/seen/seen_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/all_series.py` & `FlexGet-3.6.8/flexget/components/series/all_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/api.py` & `FlexGet-3.6.8/flexget/components/series/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/cli.py` & `FlexGet-3.6.8/flexget/components/series/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/configure_series.py` & `FlexGet-3.6.8/flexget/components/series/configure_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/db.py` & `FlexGet-3.6.8/flexget/components/series/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/gen_series.py` & `FlexGet-3.6.8/flexget/components/series/gen_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/internal_estimator.py` & `FlexGet-3.6.8/flexget/components/series/internal_estimator.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/metainfo_series.py` & `FlexGet-3.6.8/flexget/components/series/metainfo_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/next_series_episodes.py` & `FlexGet-3.6.8/flexget/components/series/next_series_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/next_series_seasons.py` & `FlexGet-3.6.8/flexget/components/series/next_series_seasons.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/series.py` & `FlexGet-3.6.8/flexget/components/series/series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/series_begin.py` & `FlexGet-3.6.8/flexget/components/series/series_begin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/series_premiere.py` & `FlexGet-3.6.8/flexget/components/series/series_premiere.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/series/series_remove.py` & `FlexGet-3.6.8/flexget/components/series/series_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/allyoulike.py` & `FlexGet-3.6.8/flexget/components/sites/sites/allyoulike.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/alpharatio.py` & `FlexGet-3.6.8/flexget/components/sites/sites/alpharatio.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/animeindex.py` & `FlexGet-3.6.8/flexget/components/sites/sites/animeindex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/anirena.py` & `FlexGet-3.6.8/flexget/components/sites/sites/anirena.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/archetorrent.py` & `FlexGet-3.6.8/flexget/components/sites/sites/archetorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/argenteam.py` & `FlexGet-3.6.8/flexget/components/sites/sites/argenteam.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/awesomehd.py` & `FlexGet-3.6.8/flexget/components/sites/sites/awesomehd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/bakabt.py` & `FlexGet-3.6.8/flexget/components/sites/sites/bakabt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/btn.py` & `FlexGet-3.6.8/flexget/components/sites/sites/btn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/cinemageddon.py` & `FlexGet-3.6.8/flexget/components/sites/sites/cinemageddon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/cpasbien.py` & `FlexGet-3.6.8/flexget/components/sites/sites/cpasbien.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/deadfrog.py` & `FlexGet-3.6.8/flexget/components/sites/sites/deadfrog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/descargas2020.py` & `FlexGet-3.6.8/flexget/components/sites/sites/descargas2020.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/ettv.py` & `FlexGet-3.6.8/flexget/components/sites/sites/ettv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/eztv.py` & `FlexGet-3.6.8/flexget/components/sites/sites/eztv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/filelist.py` & `FlexGet-3.6.8/flexget/components/sites/sites/filelist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/filelist_api.py` & `FlexGet-3.6.8/flexget/components/sites/sites/filelist_api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/frenchtorrentdb.py` & `FlexGet-3.6.8/flexget/components/sites/sites/frenchtorrentdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/fuzer.py` & `FlexGet-3.6.8/flexget/components/sites/sites/fuzer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/google_cse.py` & `FlexGet-3.6.8/flexget/components/sites/sites/google_cse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/hebits.py` & `FlexGet-3.6.8/flexget/components/sites/sites/hebits.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/hliang.py` & `FlexGet-3.6.8/flexget/components/sites/sites/hliang.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/horriblesubs.py` & `FlexGet-3.6.8/flexget/components/sites/sites/horriblesubs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/iptorrents.py` & `FlexGet-3.6.8/flexget/components/sites/sites/iptorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/koreus.py` & `FlexGet-3.6.8/flexget/components/sites/sites/koreus.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/limetorrents.py` & `FlexGet-3.6.8/flexget/components/sites/sites/limetorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/lostfilm.py` & `FlexGet-3.6.8/flexget/components/sites/sites/lostfilm.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/magnetdl.py` & `FlexGet-3.6.8/flexget/components/sites/sites/magnetdl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/morethantv.py` & `FlexGet-3.6.8/flexget/components/sites/sites/morethantv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/ncore.py` & `FlexGet-3.6.8/flexget/components/sites/sites/ncore.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/newtorrents.py` & `FlexGet-3.6.8/flexget/components/sites/sites/newtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/newznab.py` & `FlexGet-3.6.8/flexget/components/sites/sites/newznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/nnmclub.py` & `FlexGet-3.6.8/flexget/components/sites/sites/nnmclub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/nyaa.py` & `FlexGet-3.6.8/flexget/components/sites/sites/nyaa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/passthepopcorn.py` & `FlexGet-3.6.8/flexget/components/sites/sites/passthepopcorn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/piratebay.py` & `FlexGet-3.6.8/flexget/components/sites/sites/piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/ptn.py` & `FlexGet-3.6.8/flexget/components/sites/sites/ptn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/rarbg.py` & `FlexGet-3.6.8/flexget/components/sites/sites/rarbg.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/redirect.py` & `FlexGet-3.6.8/flexget/components/sites/sites/redirect.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/rlsbb.py` & `FlexGet-3.6.8/flexget/components/sites/sites/rlsbb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/rmz.py` & `FlexGet-3.6.8/flexget/components/sites/sites/rmz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/rss.py` & `FlexGet-3.6.8/flexget/components/sites/sites/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/rutracker.py` & `FlexGet-3.6.8/flexget/components/sites/sites/rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/serienjunkies.py` & `FlexGet-3.6.8/flexget/components/sites/sites/serienjunkies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/shortened.py` & `FlexGet-3.6.8/flexget/components/sites/sites/shortened.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/site_1337x.py` & `FlexGet-3.6.8/flexget/components/sites/sites/site_1337x.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/site_rutracker.py` & `FlexGet-3.6.8/flexget/components/sites/sites/site_rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/solidtorrents.py` & `FlexGet-3.6.8/flexget/components/sites/sites/solidtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/torrent_cache.py` & `FlexGet-3.6.8/flexget/components/sites/sites/torrent_cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/torrentday.py` & `FlexGet-3.6.8/flexget/components/sites/sites/torrentday.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/torrentleech.py` & `FlexGet-3.6.8/flexget/components/sites/sites/torrentleech.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/torrentz.py` & `FlexGet-3.6.8/flexget/components/sites/sites/torrentz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/wordpress.py` & `FlexGet-3.6.8/flexget/components/sites/sites/wordpress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/sites/yts.py` & `FlexGet-3.6.8/flexget/components/sites/sites/yts.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/urlrewrite.py` & `FlexGet-3.6.8/flexget/components/sites/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/urlrewrite_search.py` & `FlexGet-3.6.8/flexget/components/sites/urlrewrite_search.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/urlrewriting.py` & `FlexGet-3.6.8/flexget/components/sites/urlrewriting.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/sites/utils.py` & `FlexGet-3.6.8/flexget/components/sites/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/status/api.py` & `FlexGet-3.6.8/flexget/components/status/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/status/cli.py` & `FlexGet-3.6.8/flexget/components/status/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/status/db.py` & `FlexGet-3.6.8/flexget/components/status/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/status/status.py` & `FlexGet-3.6.8/flexget/components/status/status.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/thetvdb/api.py` & `FlexGet-3.6.8/flexget/components/thetvdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/thetvdb/api_tvdb.py` & `FlexGet-3.6.8/flexget/components/thetvdb/api_tvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/thetvdb/thetvdb_lookup.py` & `FlexGet-3.6.8/flexget/components/thetvdb/thetvdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/tmdb/api.py` & `FlexGet-3.6.8/flexget/components/tmdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/tmdb/api_tmdb.py` & `FlexGet-3.6.8/flexget/components/tmdb/api_tmdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/tmdb/tmdb_lookup.py` & `FlexGet-3.6.8/flexget/components/tmdb/tmdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/api.py` & `FlexGet-3.6.8/flexget/components/trakt/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/api_trakt.py` & `FlexGet-3.6.8/flexget/components/trakt/api_trakt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/cli.py` & `FlexGet-3.6.8/flexget/components/trakt/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/db.py` & `FlexGet-3.6.8/flexget/components/trakt/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/next_trakt_episodes.py` & `FlexGet-3.6.8/flexget/components/trakt/next_trakt_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/trakt_calendar.py` & `FlexGet-3.6.8/flexget/components/trakt/trakt_calendar.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/trakt_list.py` & `FlexGet-3.6.8/flexget/components/trakt/trakt_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/trakt/trakt_lookup.py` & `FlexGet-3.6.8/flexget/components/trakt/trakt_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/tvmaze/api.py` & `FlexGet-3.6.8/flexget/components/tvmaze/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/tvmaze/api_tvmaze.py` & `FlexGet-3.6.8/flexget/components/tvmaze/api_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/tvmaze/tvmaze_lookup.py` & `FlexGet-3.6.8/flexget/components/tvmaze/tvmaze_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/variables/api.py` & `FlexGet-3.6.8/flexget/components/variables/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/components/variables/variables.py` & `FlexGet-3.6.8/flexget/components/variables/variables.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/config_schema.py` & `FlexGet-3.6.8/flexget/config_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/db_schema.py` & `FlexGet-3.6.8/flexget/db_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/entry.py` & `FlexGet-3.6.8/flexget/entry.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/event.py` & `FlexGet-3.6.8/flexget/event.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ipc.py` & `FlexGet-3.6.8/flexget/ipc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/log.py` & `FlexGet-3.6.8/flexget/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/manager.py` & `FlexGet-3.6.8/flexget/manager.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/options.py` & `FlexGet-3.6.8/flexget/options.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugin.py` & `FlexGet-3.6.8/flexget/plugin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/check.py` & `FlexGet-3.6.8/flexget/plugins/cli/check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/cli_config.py` & `FlexGet-3.6.8/flexget/plugins/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/database.py` & `FlexGet-3.6.8/flexget/plugins/cli/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/debug_info.py` & `FlexGet-3.6.8/flexget/plugins/cli/debug_info.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/doc.py` & `FlexGet-3.6.8/flexget/plugins/cli/doc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/explain_sql.py` & `FlexGet-3.6.8/flexget/plugins/cli/explain_sql.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/filters.py` & `FlexGet-3.6.8/flexget/plugins/cli/filters.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/inject.py` & `FlexGet-3.6.8/flexget/plugins/cli/inject.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/perf_tests.py` & `FlexGet-3.6.8/flexget/plugins/cli/perf_tests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/performance.py` & `FlexGet-3.6.8/flexget/plugins/cli/performance.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/plugins.py` & `FlexGet-3.6.8/flexget/plugins/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/templates.py` & `FlexGet-3.6.8/flexget/plugins/cli/templates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/try_regexp.py` & `FlexGet-3.6.8/flexget/plugins/cli/try_regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/web.py` & `FlexGet-3.6.8/flexget/plugins/cli/web.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/wiki_qualities.py` & `FlexGet-3.6.8/flexget/plugins/cli/wiki_qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/cli/win32_service.py` & `FlexGet-3.6.8/flexget/plugins/cli/win32_service.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/clients/aria2.py` & `FlexGet-3.6.8/flexget/plugins/clients/aria2.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/clients/deluge.py` & `FlexGet-3.6.8/flexget/plugins/clients/deluge.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/clients/nzbget.py` & `FlexGet-3.6.8/flexget/plugins/clients/nzbget.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/clients/pyload.py` & `FlexGet-3.6.8/flexget/plugins/clients/pyload.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/clients/qbittorrent.py` & `FlexGet-3.6.8/flexget/plugins/clients/qbittorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/clients/rtorrent.py` & `FlexGet-3.6.8/flexget/plugins/clients/rtorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/clients/transmission.py` & `FlexGet-3.6.8/flexget/plugins/clients/transmission.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/daemon/web_server.py` & `FlexGet-3.6.8/flexget/plugins/daemon/web_server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/abort_if_exists.py` & `FlexGet-3.6.8/flexget/plugins/filter/abort_if_exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/accept_all.py` & `FlexGet-3.6.8/flexget/plugins/filter/accept_all.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/age.py` & `FlexGet-3.6.8/flexget/plugins/filter/age.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/best_quality.py` & `FlexGet-3.6.8/flexget/plugins/filter/best_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/content_filter.py` & `FlexGet-3.6.8/flexget/plugins/filter/content_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/content_size.py` & `FlexGet-3.6.8/flexget/plugins/filter/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/crossmatch.py` & `FlexGet-3.6.8/flexget/plugins/filter/crossmatch.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/delay.py` & `FlexGet-3.6.8/flexget/plugins/filter/delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/duplicates.py` & `FlexGet-3.6.8/flexget/plugins/filter/duplicates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/exists.py` & `FlexGet-3.6.8/flexget/plugins/filter/exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/exists_movie.py` & `FlexGet-3.6.8/flexget/plugins/filter/exists_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/exists_series.py` & `FlexGet-3.6.8/flexget/plugins/filter/exists_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/if_condition.py` & `FlexGet-3.6.8/flexget/plugins/filter/if_condition.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/limit_new.py` & `FlexGet-3.6.8/flexget/plugins/filter/limit_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/magnets.py` & `FlexGet-3.6.8/flexget/plugins/filter/magnets.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/only_new.py` & `FlexGet-3.6.8/flexget/plugins/filter/only_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/proper_movies.py` & `FlexGet-3.6.8/flexget/plugins/filter/proper_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/quality.py` & `FlexGet-3.6.8/flexget/plugins/filter/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/regexp.py` & `FlexGet-3.6.8/flexget/plugins/filter/regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/require_field.py` & `FlexGet-3.6.8/flexget/plugins/filter/require_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/rottentomatoes.py` & `FlexGet-3.6.8/flexget/plugins/filter/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/thetvdb.py` & `FlexGet-3.6.8/flexget/plugins/filter/thetvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/timeframe.py` & `FlexGet-3.6.8/flexget/plugins/filter/timeframe.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/unique.py` & `FlexGet-3.6.8/flexget/plugins/filter/unique.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/filter/upgrade.py` & `FlexGet-3.6.8/flexget/plugins/filter/upgrade.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/generic/cron_env.py` & `FlexGet-3.6.8/flexget/plugins/generic/cron_env.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/generic/db_vacuum.py` & `FlexGet-3.6.8/flexget/plugins/generic/db_vacuum.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/generic/log_start.py` & `FlexGet-3.6.8/flexget/plugins/generic/log_start.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/generic/urlfix.py` & `FlexGet-3.6.8/flexget/plugins/generic/urlfix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/generic/welcome.py` & `FlexGet-3.6.8/flexget/plugins/generic/welcome.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/anidb_list.py` & `FlexGet-3.6.8/flexget/plugins/input/anidb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/anilist.py` & `FlexGet-3.6.8/flexget/plugins/input/anilist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/apple_trailers.py` & `FlexGet-3.6.8/flexget/plugins/input/apple_trailers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/betaseries_list.py` & `FlexGet-3.6.8/flexget/plugins/input/betaseries_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/discover.py` & `FlexGet-3.6.8/flexget/plugins/input/discover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/filesystem.py` & `FlexGet-3.6.8/flexget/plugins/input/filesystem.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/filmweb_watchlist.py` & `FlexGet-3.6.8/flexget/plugins/input/filmweb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/from_piratebay.py` & `FlexGet-3.6.8/flexget/plugins/input/from_piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/from_task.py` & `FlexGet-3.6.8/flexget/plugins/input/from_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/from_telegram.py` & `FlexGet-3.6.8/flexget/plugins/input/from_telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/gazelle.py` & `FlexGet-3.6.8/flexget/plugins/input/gazelle.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/generate.py` & `FlexGet-3.6.8/flexget/plugins/input/generate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/html.py` & `FlexGet-3.6.8/flexget/plugins/input/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/input_csv.py` & `FlexGet-3.6.8/flexget/plugins/input/input_csv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/inputs.py` & `FlexGet-3.6.8/flexget/plugins/input/inputs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/json.py` & `FlexGet-3.6.8/flexget/plugins/input/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/kitsu.py` & `FlexGet-3.6.8/flexget/plugins/input/kitsu.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/letterboxd.py` & `FlexGet-3.6.8/flexget/plugins/input/letterboxd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/limit.py` & `FlexGet-3.6.8/flexget/plugins/input/limit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/medusa.py` & `FlexGet-3.6.8/flexget/plugins/input/medusa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/mock.py` & `FlexGet-3.6.8/flexget/plugins/input/mock.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/my_anime_list.py` & `FlexGet-3.6.8/flexget/plugins/input/my_anime_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/myepisodes_list.py` & `FlexGet-3.6.8/flexget/plugins/input/myepisodes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/next_sonarr_episodes.py` & `FlexGet-3.6.8/flexget/plugins/input/next_sonarr_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/npo_watchlist.py` & `FlexGet-3.6.8/flexget/plugins/input/npo_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/parameterize.py` & `FlexGet-3.6.8/flexget/plugins/input/parameterize.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/plex.py` & `FlexGet-3.6.8/flexget/plugins/input/plex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/pogcal.py` & `FlexGet-3.6.8/flexget/plugins/input/pogcal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/regexp_parse.py` & `FlexGet-3.6.8/flexget/plugins/input/regexp_parse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/rlslog.py` & `FlexGet-3.6.8/flexget/plugins/input/rlslog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/rottentomatoes_list.py` & `FlexGet-3.6.8/flexget/plugins/input/rottentomatoes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/rss.py` & `FlexGet-3.6.8/flexget/plugins/input/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/sceper.py` & `FlexGet-3.6.8/flexget/plugins/input/sceper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/sickbeard.py` & `FlexGet-3.6.8/flexget/plugins/input/sickbeard.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/tail.py` & `FlexGet-3.6.8/flexget/plugins/input/tail.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/text.py` & `FlexGet-3.6.8/flexget/plugins/input/text.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/torznab.py` & `FlexGet-3.6.8/flexget/plugins/input/torznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/input/twitterfeed.py` & `FlexGet-3.6.8/flexget/plugins/input/twitterfeed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/internal/api_bluray.py` & `FlexGet-3.6.8/flexget/plugins/internal/api_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/internal/api_rottentomatoes.py` & `FlexGet-3.6.8/flexget/plugins/internal/api_rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/internal/change_warn.py` & `FlexGet-3.6.8/flexget/plugins/internal/change_warn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/assume_quality.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/assume_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/bluray_lookup.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/bluray_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/content_size.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/media_id.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/media_id.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/metainfo_movie.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/metainfo_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/nfo_lookup.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/nfo_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/nzb_size.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/nzb_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/quality.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/rottentomatoes_lookup.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/rottentomatoes_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/subtitles_check.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/subtitles_check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/metainfo/task.py` & `FlexGet-3.6.8/flexget/plugins/metainfo/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/extension.py` & `FlexGet-3.6.8/flexget/plugins/modify/extension.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/headers.py` & `FlexGet-3.6.8/flexget/plugins/modify/headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/manipulate.py` & `FlexGet-3.6.8/flexget/plugins/modify/manipulate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/path_by_ext.py` & `FlexGet-3.6.8/flexget/plugins/modify/path_by_ext.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/path_by_space.py` & `FlexGet-3.6.8/flexget/plugins/modify/path_by_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/plugin_priority.py` & `FlexGet-3.6.8/flexget/plugins/modify/plugin_priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/regex_extract.py` & `FlexGet-3.6.8/flexget/plugins/modify/regex_extract.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/reorder_quality.py` & `FlexGet-3.6.8/flexget/plugins/modify/reorder_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/set_field.py` & `FlexGet-3.6.8/flexget/plugins/modify/set_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/sort_by.py` & `FlexGet-3.6.8/flexget/plugins/modify/sort_by.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/modify/sort_by_weight.py` & `FlexGet-3.6.8/flexget/plugins/modify/sort_by_weight.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/cfscraper.py` & `FlexGet-3.6.8/flexget/plugins/operate/cfscraper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/cookies.py` & `FlexGet-3.6.8/flexget/plugins/operate/cookies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/debug_db_sessions.py` & `FlexGet-3.6.8/flexget/plugins/operate/debug_db_sessions.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/debug_warnings.py` & `FlexGet-3.6.8/flexget/plugins/operate/debug_warnings.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/digest.py` & `FlexGet-3.6.8/flexget/plugins/operate/digest.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/disable.py` & `FlexGet-3.6.8/flexget/plugins/operate/disable.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/disable_phases.py` & `FlexGet-3.6.8/flexget/plugins/operate/disable_phases.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/domain_delay.py` & `FlexGet-3.6.8/flexget/plugins/operate/domain_delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/entry_trace.py` & `FlexGet-3.6.8/flexget/plugins/operate/entry_trace.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/formlogin.py` & `FlexGet-3.6.8/flexget/plugins/operate/formlogin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/free_space.py` & `FlexGet-3.6.8/flexget/plugins/operate/free_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/include.py` & `FlexGet-3.6.8/flexget/plugins/operate/include.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/interval.py` & `FlexGet-3.6.8/flexget/plugins/operate/interval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/log_filter.py` & `FlexGet-3.6.8/flexget/plugins/operate/log_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/manual.py` & `FlexGet-3.6.8/flexget/plugins/operate/manual.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/max_reruns.py` & `FlexGet-3.6.8/flexget/plugins/operate/max_reruns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/pathscrub.py` & `FlexGet-3.6.8/flexget/plugins/operate/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/priority.py` & `FlexGet-3.6.8/flexget/plugins/operate/priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/proxy.py` & `FlexGet-3.6.8/flexget/plugins/operate/proxy.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/rerun.py` & `FlexGet-3.6.8/flexget/plugins/operate/rerun.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/run_task.py` & `FlexGet-3.6.8/flexget/plugins/operate/run_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/sequence.py` & `FlexGet-3.6.8/flexget/plugins/operate/sequence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/sleep.py` & `FlexGet-3.6.8/flexget/plugins/operate/sleep.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/spy_headers.py` & `FlexGet-3.6.8/flexget/plugins/operate/spy_headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/template.py` & `FlexGet-3.6.8/flexget/plugins/operate/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/verbose.py` & `FlexGet-3.6.8/flexget/plugins/operate/verbose.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/verbose_details.py` & `FlexGet-3.6.8/flexget/plugins/operate/verbose_details.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/verify_ssl_certificates.py` & `FlexGet-3.6.8/flexget/plugins/operate/verify_ssl_certificates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/operate/version_checker.py` & `FlexGet-3.6.8/flexget/plugins/operate/version_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/download.py` & `FlexGet-3.6.8/flexget/plugins/output/download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/download_auth.py` & `FlexGet-3.6.8/flexget/plugins/output/download_auth.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/dump.py` & `FlexGet-3.6.8/flexget/plugins/output/dump.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/dump_config.py` & `FlexGet-3.6.8/flexget/plugins/output/dump_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/exec.py` & `FlexGet-3.6.8/flexget/plugins/output/exec.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/file_operations.py` & `FlexGet-3.6.8/flexget/plugins/output/file_operations.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/html.py` & `FlexGet-3.6.8/flexget/plugins/output/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/memusage.py` & `FlexGet-3.6.8/flexget/plugins/output/memusage.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/mock_output.py` & `FlexGet-3.6.8/flexget/plugins/output/mock_output.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/rss.py` & `FlexGet-3.6.8/flexget/plugins/output/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/rtorrent_magnet.py` & `FlexGet-3.6.8/flexget/plugins/output/rtorrent_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/sabnzbd.py` & `FlexGet-3.6.8/flexget/plugins/output/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/sns.py` & `FlexGet-3.6.8/flexget/plugins/output/sns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/subtitles.py` & `FlexGet-3.6.8/flexget/plugins/output/subtitles.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/subtitles_periscope.py` & `FlexGet-3.6.8/flexget/plugins/output/subtitles_periscope.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/subtitles_subliminal.py` & `FlexGet-3.6.8/flexget/plugins/output/subtitles_subliminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/symlink.py` & `FlexGet-3.6.8/flexget/plugins/output/symlink.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/output/utorrent.py` & `FlexGet-3.6.8/flexget/plugins/output/utorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/services/kodi_library.py` & `FlexGet-3.6.8/flexget/plugins/services/kodi_library.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/services/myepisodes.py` & `FlexGet-3.6.8/flexget/plugins/services/myepisodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/plugins/services/pogcal_acquired.py` & `FlexGet-3.6.8/flexget/plugins/services/pogcal_acquired.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/resources/flexget.png` & `FlexGet-3.6.8/flexget/resources/flexget.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/task.py` & `FlexGet-3.6.8/flexget/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/task_queue.py` & `FlexGet-3.6.8/flexget/task_queue.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/templates/task/default.template` & `FlexGet-3.6.8/flexget/templates/task/default.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/templates/task/html.template` & `FlexGet-3.6.8/flexget/templates/task/html.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/templates/task/rss.template` & `FlexGet-3.6.8/flexget/templates/task/rss.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/terminal.py` & `FlexGet-3.6.8/flexget/terminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/tray_icon.py` & `FlexGet-3.6.8/flexget/tray_icon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/__init__.py` & `FlexGet-3.6.8/flexget/ui/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/app.html` & `FlexGet-3.6.8/flexget/ui/v1/app/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/assets/images/header.png` & `FlexGet-3.6.8/flexget/ui/v1/app/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/favicon.ico` & `FlexGet-3.6.8/flexget/ui/v1/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/FontAwesome.otf` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.eot` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.svg` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.woff` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.eot` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.svg` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.ttf` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/fonts/ui-grid.woff` & `FlexGet-3.6.8/flexget/ui/v1/app/fonts/ui-grid.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/scripts/app.js` & `FlexGet-3.6.8/flexget/ui/v1/app/scripts/app.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/scripts/splash.js` & `FlexGet-3.6.8/flexget/ui/v1/app/scripts/splash.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/scripts/vendor.js` & `FlexGet-3.6.8/flexget/ui/v1/app/scripts/vendor.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/styles/app.css` & `FlexGet-3.6.8/flexget/ui/v1/app/styles/app.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/styles/splash.css` & `FlexGet-3.6.8/flexget/ui/v1/app/styles/splash.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/app/styles/vendor.css` & `FlexGet-3.6.8/flexget/ui/v1/app/styles/vendor.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/bower.json` & `FlexGet-3.6.8/flexget/ui/v1/bower.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/build.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/build.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/inject.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/inject.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/lint.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/lint.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/proxy.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/proxy.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/server.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/server.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/styles.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/styles.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/test.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/test.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/gulp/watch.js` & `FlexGet-3.6.8/flexget/ui/v1/gulp/watch.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/karma.conf.js` & `FlexGet-3.6.8/flexget/ui/v1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/package.json` & `FlexGet-3.6.8/flexget/ui/v1/package.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/specs.html` & `FlexGet-3.6.8/flexget/ui/v1/specs.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/app.html` & `FlexGet-3.6.8/flexget/ui/v1/src/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/app.module.js` & `FlexGet-3.6.8/flexget/ui/v1/src/app.module.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/app.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/app.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/assets/images/header.png` & `FlexGet-3.6.8/flexget/ui/v1/src/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error-dialog.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/error/error.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/error/error.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/exception/exception.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/exception/exception.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/exception/exception.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/exception/exception.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/_pagination.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/_pagination.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/pagination.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/pagination.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/router/router-helper.provider.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/router/router-helper.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/404/404.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/components/404/404.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.config.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.config.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.config.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/auth.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/auth.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/auth/login.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/components/auth/login.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/core/core.config.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/core/core.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/core/core.provider.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/core/core.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.config.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/database/database.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/components/database/database.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/home/home.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/components/home/home.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/_sidenav.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/_sidenav.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.semver.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.semver.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.provider.js` & `FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/construction.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/construction.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js` & `FlexGet-3.6.8/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/favicon.ico` & `FlexGet-3.6.8/flexget/ui/v1/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/config/config.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/config/config.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.filter.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.filter.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/execute/execute.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/execute/execute.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/history/history.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/history/history.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/log/log.tmpl.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/log/log.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/pending/pending.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/pending/pending.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/seen/seen.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/seen/seen.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.component.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.route.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.service.spec.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/series/series.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/series/series.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/loading-dialog.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/loading-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/server.config.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/server.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/server/server.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/server/server.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.component.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.route.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/plugins/status/status.tmpl.html` & `FlexGet-3.6.8/flexget/ui/v1/src/plugins/status/status.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/scss/_header.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/scss/flexget.scss` & `FlexGet-3.6.8/flexget/ui/v1/src/scss/flexget.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/src/services/schema.service.js` & `FlexGet-3.6.8/flexget/ui/v1/src/services/schema.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/config.js` & `FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/execute.js` & `FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/execute.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/history.js` & `FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/history.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/movie_list.js` & `FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/movie_list.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/seen.js` & `FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/seen.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/series.js` & `FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/series.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v1/tests-mock-data/states.js` & `FlexGet-3.6.8/flexget/ui/v1/tests-mock-data/states.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/__init__.py` & `FlexGet-3.6.8/flexget/ui/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map` & `FlexGet-3.6.8/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/ui/v2/dist/index.html` & `FlexGet-3.6.8/flexget/ui/v2/dist/index.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/bittorrent.py` & `FlexGet-3.6.8/flexget/utils/bittorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/cache.py` & `FlexGet-3.6.8/flexget/utils/cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/cached_input.py` & `FlexGet-3.6.8/flexget/utils/cached_input.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/database.py` & `FlexGet-3.6.8/flexget/utils/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/json.py` & `FlexGet-3.6.8/flexget/utils/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/lazy_dict.py` & `FlexGet-3.6.8/flexget/utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/log.py` & `FlexGet-3.6.8/flexget/utils/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/parsers/generic.py` & `FlexGet-3.6.8/flexget/utils/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/parsers/movie.py` & `FlexGet-3.6.8/flexget/utils/parsers/movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/parsers/parser.py` & `FlexGet-3.6.8/flexget/utils/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/parsers/series.py` & `FlexGet-3.6.8/flexget/utils/parsers/series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/pathscrub.py` & `FlexGet-3.6.8/flexget/utils/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/qualities.py` & `FlexGet-3.6.8/flexget/utils/qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/requests.py` & `FlexGet-3.6.8/flexget/utils/requests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/serialization.py` & `FlexGet-3.6.8/flexget/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/simple_persistence.py` & `FlexGet-3.6.8/flexget/utils/simple_persistence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/sqlalchemy_utils.py` & `FlexGet-3.6.8/flexget/utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/template.py` & `FlexGet-3.6.8/flexget/utils/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/utils/tools.py` & `FlexGet-3.6.8/flexget/utils/tools.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/flexget/webserver.py` & `FlexGet-3.6.8/flexget/webserver.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.6.7/pyproject.toml` & `FlexGet-3.6.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -86,40 +86,38 @@
 packaging = ">=21.3"
 pyparsing = ">=2.4.7"
 werkzeug = ">=2.2.3"
 zxcvbn-python = "^4.4.24"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=18.9b0"
-build = ">=0.9.0"
-click = ">=8.1.3"
 codacy-coverage = ">=1.2.18"
 coverage = ">=6.0"
 gitpython = ">=3.1.18"
 pre-commit = ">=2.9.0"
 pytest-cov = ">=3.0.0"
 pytest-runner = "^6.0.0"
 pytest-xdist = ">=2.4.0"
 pytest = ">=6.2.4"
 ruff = ">=0.0.261"
 sphinx = ">=5.0.0"
 sqlalchemy-stubs = "^0.4"
-twine = ">=3.6.0"
 vcrpy = ">=4.1.1"
 
+[tool.poetry.group.release.dependencies]
+build = ">=0.9.0"
+click = ">=8.1.3"
+twine = ">=3.6.0"
+
 [tool.poetry.group.plugin-test.dependencies]
 # These are optional dependencies for plugins that have tests in the test suite
 boto3 = ">=1.24.89"
 plexapi = ">=4.13.1"
-subliminal = ">= 2.0rc1"
-
-
-[tool.poetry.group.plugin-tests.dependencies]
 pysftp = "^0.2.9"
-
+subliminal = ">= 2.0rc1"
 
 [tool.poetry.group.docker.dependencies]
 transmission-rpc = "^4.1.4"
 qbittorrent-api = "^2023.3.44"
 deluge-client = "^1.9.0"
 cloudscraper = "^1.2.69"
```

### Comparing `FlexGet-3.6.7/requirements-docker.txt` & `FlexGet-3.6.8/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
 brotli==1.0.9 ; python_version >= "3.7" and python_version < "4.0"
 certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
 cheroot==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
 cherrypy==18.8.0 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
-cloudscraper==1.2.69 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0"
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
-deluge-client==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
 feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
 flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
 flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
 flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 flask==2.2.5 ; python_version >= "3.7" and python_version < "4.0"
@@ -52,27 +50,24 @@
 pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
 pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
 pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4"
 pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
-qbittorrent-api==2023.3.44 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
-requests-toolbelt==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
 rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4"
 sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
 sqlalchemy==1.4.45 ; python_version >= "3.7" and python_version < "4.0"
 tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
-transmission-rpc==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
 tzdata==2022.7 ; python_version >= "3.7" and python_version < "4"
 tzlocal==4.2 ; python_version >= "3.7" and python_version < "4"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
 werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
 win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
```

### Comparing `FlexGet-3.6.7/requirements.txt` & `FlexGet-3.6.8/dev-requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,66 @@
-aniso8601==9.0.1 ; python_version >= "3.7" and python_version < "4.0"
-apscheduler==3.9.1.post1 ; python_version >= "3.7" and python_version < "4"
+alabaster==0.7.12 ; python_version >= "3.7" and python_version < "4.0"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
-autocommand==2.2.2 ; python_version >= "3.7" and python_version < "4.0"
-babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
-backports-zoneinfo==0.2.1 ; python_version >= "3.7" and python_version < "3.9"
-beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
-brotli==1.0.9 ; python_version >= "3.7" and python_version < "4.0"
+babel==2.11.0 ; python_version >= "3.7" and python_version < "4.0"
+black==22.12.0 ; python_version >= "3.7" and python_version < "4.0"
 certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
+cfgv==3.3.1 ; python_version >= "3.7" and python_version < "4.0"
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
-cheroot==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
-cherrypy==18.8.0 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
-colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0"
-commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
-feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
-flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
-flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
-flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
-flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
-flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
-flask==2.2.5 ; python_version >= "3.7" and python_version < "4.0"
-greenlet==2.0.1 ; python_version >= "3.7" and platform_machine == "aarch64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "ppc64le" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "x86_64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "amd64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "AMD64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "win32" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "WIN32" and python_version < "4.0"
-guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
-html5lib==1.1 ; python_version >= "3.7" and python_version < "4.0"
+codacy-coverage==1.3.11 ; python_version >= "3.7" and python_version < "4.0"
+colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32" or python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
+coverage==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
+coverage[toml]==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
+distlib==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
+docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
+exceptiongroup==1.0.4 ; python_version >= "3.7" and python_version < "3.11"
+execnet==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
+filelock==3.8.2 ; python_version >= "3.7" and python_version < "4.0"
+gitdb==4.0.10 ; python_version >= "3.7" and python_version < "4.0"
+gitpython==3.1.29 ; python_version >= "3.7" and python_version < "4.0"
+identify==2.5.9 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4"
+imagesize==1.4.1 ; python_version >= "3.7" and python_version < "4.0"
 importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
-importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
-inflect==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
-itsdangerous==2.1.2 ; python_version >= "3.7" and python_version < "4.0"
-jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
-jaraco-collections==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
-jaraco-context==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
-jaraco-functools==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
-jaraco-text==3.11.0 ; python_version >= "3.7" and python_version < "4.0"
+iniconfig==1.1.1 ; python_version >= "3.7" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.7" and python_version < "4.0"
-jsonschema==4.17.3 ; python_version >= "3.7" and python_version < "4.0"
-loguru==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 markupsafe==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
-more-itertools==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
+multidict==6.0.3 ; python_version >= "3.7" and python_version < "4.0"
+mypy-extensions==0.4.3 ; python_version >= "3.7" and python_version < "4.0"
+mypy==0.991 ; python_version >= "3.7" and python_version < "4.0"
+nodeenv==1.7.0 ; python_version >= "3.7" and python_version < "4.0"
 packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
-pkgutil-resolve-name==1.3.10 ; python_version >= "3.7" and python_version < "3.9"
-plumbum==1.8.0 ; python_version >= "3.7" and python_version < "4.0"
-portend==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
-psutil==5.9.4 ; python_version >= "3.7" and python_version < "4.0"
-pydantic==1.10.2 ; python_version >= "3.7" and python_version < "4.0"
+pathspec==0.10.3 ; python_version >= "3.7" and python_version < "4.0"
+platformdirs==2.6.0 ; python_version >= "3.7" and python_version < "4.0"
+pluggy==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
+pre-commit==2.20.0 ; python_version >= "3.7" and python_version < "4.0"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
-pynzb==0.1.0 ; python_version >= "3.7" and python_version < "4.0"
-pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "4.0"
-pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
-pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
-python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
-pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4"
-pytz==2022.6 ; python_version >= "3.7" and python_version < "4"
-pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
+pytest-cov==4.0.0 ; python_version >= "3.7" and python_version < "4.0"
+pytest-runner==6.0.0 ; python_version >= "3.7" and python_version < "4.0"
+pytest-xdist==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
+pytest==7.2.0 ; python_version >= "3.7" and python_version < "4.0"
+pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
-rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
-rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
-rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
-setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4"
-sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
-six==1.16.0 ; python_version >= "3.7" and python_version < "4"
-soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
-sqlalchemy==1.4.45 ; python_version >= "3.7" and python_version < "4.0"
-tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
+ruff==0.0.261 ; python_version >= "3.7" and python_version < "4.0"
+setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
+six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
+smmap==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
+snowballstemmer==2.2.0 ; python_version >= "3.7" and python_version < "4.0"
+sphinx==5.3.0 ; python_version >= "3.7" and python_version < "4.0"
+sphinxcontrib-applehelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
+sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
+sphinxcontrib-htmlhelp==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
+sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
+sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
+sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.7" and python_version < "4.0"
+sqlalchemy-stubs==0.4 ; python_version >= "3.7" and python_version < "4.0"
+toml==0.10.2 ; python_version >= "3.7" and python_version < "4.0"
+tomli==2.0.1 ; python_version >= "3.7" and python_full_version < "3.11.0a7"
+typed-ast==1.5.4 ; python_version < "3.8" and python_version >= "3.7"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
-tzdata==2022.7 ; python_version >= "3.7" and python_version < "4"
-tzlocal==4.2 ; python_version >= "3.7" and python_version < "4"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4"
-webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
-werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
-win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
-zc-lockfile==2.0 ; python_version >= "3.7" and python_version < "4.0"
+vcrpy==4.2.1 ; python_version >= "3.7" and python_version < "4.0"
+virtualenv==20.17.1 ; python_version >= "3.7" and python_version < "4.0"
+wrapt==1.14.1 ; python_version >= "3.7" and python_version < "4.0"
+yarl==1.8.2 ; python_version >= "3.7" and python_version < "4.0"
 zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.10"
-zxcvbn-python==4.4.24 ; python_version >= "3.7" and python_version < "4.0"
```

