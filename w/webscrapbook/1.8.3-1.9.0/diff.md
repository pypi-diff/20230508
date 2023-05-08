# Comparing `tmp/webscrapbook-1.8.3.tar.gz` & `tmp/webscrapbook-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapbook-1.8.3.tar", last modified: Wed Mar  8 13:50:16 2023, max compression
+gzip compressed data, was "webscrapbook-1.9.0.tar", last modified: Sun Mar 26 13:48:00 2023, max compression
```

## Comparing `webscrapbook-1.8.3.tar` & `webscrapbook-1.9.0.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.520142 webscrapbook-1.8.3/
--rw-rw-rw-   0        0        0     1092 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5234 2023-03-08 13:50:16.520142 webscrapbook-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     3985 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/README.md
--rw-rw-rw-   0        0        0      494 2023-03-08 13:50:16.520142 webscrapbook-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0     2543 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.455736 webscrapbook-1.8.3/tests/
--rw-rw-rw-   0        0        0   265291 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_app_actions.py
--rw-rw-rw-   0        0        0    21842 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_app_config.py
--rw-rw-rw-   0        0        0    46945 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_app_helpers.py
--rw-rw-rw-   0        0        0    24380 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_cli.py
--rw-rw-rw-   0        0        0    11308 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_init.py
--rw-rw-rw-   0        0        0     7653 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_locales.py
--rw-rw-rw-   0        0        0    45991 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_book.py
--rw-rw-rw-   0        0        0   136912 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_cache.py
--rw-rw-rw-   0        0        0    35991 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_check.py
--rw-rw-rw-   0        0        0    31914 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_convert_file2wsb.py
--rw-rw-rw-   0        0        0    58056 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_convert_items.py
--rw-rw-rw-   0        0        0    58963 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_convert_migrate.py
--rw-rw-rw-   0        0        0    26916 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_convert_sb2wsb.py
--rw-rw-rw-   0        0        0    23247 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_convert_wsb2file.py
--rw-rw-rw-   0        0        0    51839 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_convert_wsb2sb.py
--rw-rw-rw-   0        0        0    24094 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_exporter.py
--rw-rw-rw-   0        0        0    24746 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_host.py
--rw-rw-rw-   0        0        0    58506 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_importer.py
--rw-rw-rw-   0        0        0    86635 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_scrapbook_indexer.py
--rw-rw-rw-   0        0        0    13455 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_server.py
--rw-rw-rw-   0        0        0    83786 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_util.py
--rw-rw-rw-   0        0        0    19327 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/tests/test_util_html.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.461732 webscrapbook-1.8.3/webscrapbook/
--rw-rw-rw-   0        0        0     9042 2023-03-08 13:49:02.000000 webscrapbook-1.8.3/webscrapbook/__init__.py
--rw-rw-rw-   0        0        0      165 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/__main__.py
--rw-rw-rw-   0        0        0    66332 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/app.py
--rw-rw-rw-   0        0        0    41782 2023-03-08 13:07:35.000000 webscrapbook-1.8.3/webscrapbook/cli.py
--rw-rw-rw-   0        0        0     3217 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/locales.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.469749 webscrapbook-1.8.3/webscrapbook/resources/
--rw-rw-rw-   0        0        0      144 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/resources/app.py
--rw-rw-rw-   0        0        0      948 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/resources/config.ini
--rw-rw-rw-   0        0        0    11907 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/resources/config.md
--rw-rw-rw-   0        0        0     1505 2021-12-07 15:19:04.000000 webscrapbook-1.8.3/webscrapbook/resources/mimetypes.md
--rw-rw-rw-   0        0        0      128 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/resources/serve.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.477737 webscrapbook-1.8.3/webscrapbook/scrapbook/
--rw-rw-rw-   0        0        0        0 2021-12-07 15:19:04.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/__init__.py
--rw-rw-rw-   0        0        0    12822 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/book.py
--rw-rw-rw-   0        0        0    38152 2023-03-08 13:39:28.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/cache.py
--rw-rw-rw-   0        0        0    27605 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/check.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.481735 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/
--rw-rw-rw-   0        0        0        0 2021-12-07 15:19:04.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/__init__.py
--rw-rw-rw-   0        0        0    12576 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/file2wsb.py
--rw-rw-rw-   0        0        0    13623 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/items.py
--rw-rw-rw-   0        0        0    41527 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/migrate.py
--rw-rw-rw-   0        0        0    15877 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/sb2wsb.py
--rw-rw-rw-   0        0        0     5902 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/wsb2file.py
--rw-rw-rw-   0        0        0    25939 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/convert/wsb2sb.py
--rw-rw-rw-   0        0        0     6619 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/exporter.py
--rw-rw-rw-   0        0        0    15228 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/host.py
--rw-rw-rw-   0        0        0    15255 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/importer.py
--rw-rw-rw-   0        0        0    39353 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/scrapbook/indexer.py
--rw-rw-rw-   0        0        0     2356 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/server.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.429941 webscrapbook-1.8.3/webscrapbook/themes/
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.431925 webscrapbook-1.8.3/webscrapbook/themes/default/
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.431925 webscrapbook-1.8.3/webscrapbook/themes/default/locales/
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.483725 webscrapbook-1.8.3/webscrapbook/themes/default/locales/ar/
--rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/locales/ar/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.483725 webscrapbook-1.8.3/webscrapbook/themes/default/locales/en/
--rw-rw-rw-   0        0        0     7705 2023-03-08 13:49:02.000000 webscrapbook-1.8.3/webscrapbook/themes/default/locales/en/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.485727 webscrapbook-1.8.3/webscrapbook/themes/default/locales/es/
--rw-rw-rw-   0        0        0     8763 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/locales/es/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.485727 webscrapbook-1.8.3/webscrapbook/themes/default/locales/fa/
--rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/locales/fa/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.485727 webscrapbook-1.8.3/webscrapbook/themes/default/locales/he/
--rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/locales/he/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.489208 webscrapbook-1.8.3/webscrapbook/themes/default/locales/zh/
--rw-rw-rw-   0        0        0     7843 2023-03-08 13:49:02.000000 webscrapbook-1.8.3/webscrapbook/themes/default/locales/zh/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.489208 webscrapbook-1.8.3/webscrapbook/themes/default/locales/zh_cn/
--rw-rw-rw-   0        0        0     7860 2023-03-08 13:49:02.000000 webscrapbook-1.8.3/webscrapbook/themes/default/locales/zh_cn/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.506148 webscrapbook-1.8.3/webscrapbook/themes/default/static/
--rw-rw-rw-   0        0        0      281 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/collapse.png
--rw-rw-rw-   0        0        0      728 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/comment.png
--rw-rw-rw-   0        0        0      877 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/common.css
--rw-rw-rw-   0        0        0     4140 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/common.js
--rw-rw-rw-   0        0        0     1055 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/edit.css
--rw-rw-rw-   0        0        0     1563 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/edit.js
--rw-rw-rw-   0        0        0     2438 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/editx.js
--rw-rw-rw-   0        0        0      279 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/expand.png
--rw-rw-rw-   0        0        0      523 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/external.png
--rw-rw-rw-   0        0        0      752 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/fclose.png
--rw-rw-rw-   0        0        0      449 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/file.png
--rw-rw-rw-   0        0        0      790 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/fopen.png
--rw-rw-rw-   0        0        0     3810 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/index-ex.css
--rw-rw-rw-   0        0        0    60629 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/index-ex.js
--rw-rw-rw-   0        0        0     2210 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/index.css
--rw-rw-rw-   0        0        0     2156 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/index.js
--rw-rw-rw-   0        0        0      502 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/item.png
--rw-rw-rw-   0        0        0      387 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/link.png
--rw-rw-rw-   0        0        0      445 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/note.png
--rw-rw-rw-   0        0        0      515 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/postit.png
--rw-rw-rw-   0        0        0      661 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/search.png
--rw-rw-rw-   0        0        0      807 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/static/toggle.png
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.516148 webscrapbook-1.8.3/webscrapbook/themes/default/templates/
--rw-rw-rw-   0        0        0      482 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/base.html
--rw-rw-rw-   0        0        0      632 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/cli.html
--rw-rw-rw-   0        0        0     1053 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/edit.html
--rw-rw-rw-   0        0        0      965 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/editx.html
--rw-rw-rw-   0        0        0     5632 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/index.html
--rw-rw-rw-   0        0        0      510 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/maff_index.html
--rw-rw-rw-   0        0        0      490 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/markdown.html
--rw-rw-rw-   0        0        0      568 2021-12-07 15:19:05.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_frame.html
--rw-rw-rw-   0        0        0     1751 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_index.html
--rw-rw-rw-   0        0        0    12917 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_map.html
--rw-rw-rw-   0        0        0    26419 2023-03-08 13:49:02.000000 webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_search.html
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.518148 webscrapbook-1.8.3/webscrapbook/util/
--rw-rw-rw-   0        0        0       74 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/util/__init__.py
--rw-rw-rw-   0        0        0     5867 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/util/css.py
--rw-rw-rw-   0        0        0    15308 2023-02-28 12:33:22.000000 webscrapbook-1.8.3/webscrapbook/util/html.py
--rw-rw-rw-   0        0        0    52535 2023-03-08 13:07:35.000000 webscrapbook-1.8.3/webscrapbook/util/util.py
-drwxrwxrwx   0        0        0        0 2023-03-08 13:50:16.465741 webscrapbook-1.8.3/webscrapbook.egg-info/
--rw-rw-rw-   0        0        0     5234 2023-03-08 13:50:16.000000 webscrapbook-1.8.3/webscrapbook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3809 2023-03-08 13:50:16.000000 webscrapbook-1.8.3/webscrapbook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 13:50:16.000000 webscrapbook-1.8.3/webscrapbook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-03-08 13:50:16.000000 webscrapbook-1.8.3/webscrapbook.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      255 2023-03-08 13:50:16.000000 webscrapbook-1.8.3/webscrapbook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-08 13:50:16.000000 webscrapbook-1.8.3/webscrapbook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/
+-rw-rw-rw-   0        0        0     1092 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5422 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4173 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/README.md
+-rw-rw-rw-   0        0        0      494 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2543 2023-03-26 06:42:51.000000 webscrapbook-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.010047 webscrapbook-1.9.0/tests/
+-rw-rw-rw-   0        0        0   265526 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_app_actions.py
+-rw-rw-rw-   0        0        0    21865 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_app_config.py
+-rw-rw-rw-   0        0        0    46945 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_app_helpers.py
+-rw-rw-rw-   0        0        0    24358 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0    11308 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_init.py
+-rw-rw-rw-   0        0        0     7653 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_locales.py
+-rw-rw-rw-   0        0        0    45991 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_book.py
+-rw-rw-rw-   0        0        0   136912 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_cache.py
+-rw-rw-rw-   0        0        0    35991 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_check.py
+-rw-rw-rw-   0        0        0    31914 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_file2wsb.py
+-rw-rw-rw-   0        0        0    58056 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_items.py
+-rw-rw-rw-   0        0        0    58963 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_migrate.py
+-rw-rw-rw-   0        0        0    26916 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_sb2wsb.py
+-rw-rw-rw-   0        0        0    23247 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_wsb2file.py
+-rw-rw-rw-   0        0        0    51845 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/tests/test_scrapbook_convert_wsb2sb.py
+-rw-rw-rw-   0        0        0    24094 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_exporter.py
+-rw-rw-rw-   0        0        0    24746 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_host.py
+-rw-rw-rw-   0        0        0    58506 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_importer.py
+-rw-rw-rw-   0        0        0    86635 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_scrapbook_indexer.py
+-rw-rw-rw-   0        0        0    13455 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_server.py
+-rw-rw-rw-   0        0        0    83786 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_util.py
+-rw-rw-rw-   0        0        0    19327 2023-03-26 13:10:54.000000 webscrapbook-1.9.0/tests/test_util_html.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.025675 webscrapbook-1.9.0/webscrapbook/
+-rw-rw-rw-   0        0        0     9042 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/__main__.py
+-rw-rw-rw-   0        0        0    68272 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/app.py
+-rw-rw-rw-   0        0        0    42102 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/cli.py
+-rw-rw-rw-   0        0        0     3217 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/locales.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/resources/
+-rw-rw-rw-   0        0        0      144 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/resources/app.py
+-rw-rw-rw-   0        0        0      948 2023-03-26 12:46:27.000000 webscrapbook-1.9.0/webscrapbook/resources/config.ini
+-rw-rw-rw-   0        0        0    12038 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/resources/config.md
+-rw-rw-rw-   0        0        0     1505 2021-12-07 15:19:04.000000 webscrapbook-1.9.0/webscrapbook/resources/mimetypes.md
+-rw-rw-rw-   0        0        0      128 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/resources/serve.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/scrapbook/
+-rw-rw-rw-   0        0        0        0 2021-12-07 15:19:04.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/__init__.py
+-rw-rw-rw-   0        0        0    12822 2023-03-26 13:19:57.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/book.py
+-rw-rw-rw-   0        0        0    38152 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/cache.py
+-rw-rw-rw-   0        0        0    27605 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/check.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/
+-rw-rw-rw-   0        0        0        0 2021-12-07 15:19:04.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/__init__.py
+-rw-rw-rw-   0        0        0    12576 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/file2wsb.py
+-rw-rw-rw-   0        0        0    13623 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/items.py
+-rw-rw-rw-   0        0        0    41527 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/migrate.py
+-rw-rw-rw-   0        0        0    15877 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/sb2wsb.py
+-rw-rw-rw-   0        0        0     5902 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2file.py
+-rw-rw-rw-   0        0        0    25939 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2sb.py
+-rw-rw-rw-   0        0        0     6619 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/exporter.py
+-rw-rw-rw-   0        0        0    15228 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/host.py
+-rw-rw-rw-   0        0        0    15255 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/importer.py
+-rw-rw-rw-   0        0        0    39353 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/scrapbook/indexer.py
+-rw-rw-rw-   0        0        0     2356 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/server.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:47:59.956670 webscrapbook-1.9.0/webscrapbook/themes/
+drwxrwxrwx   0        0        0        0 2023-03-26 13:47:59.956670 webscrapbook-1.9.0/webscrapbook/themes/default/
+drwxrwxrwx   0        0        0        0 2023-03-26 13:47:59.956670 webscrapbook-1.9.0/webscrapbook/themes/default/locales/
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.041299 webscrapbook-1.9.0/webscrapbook/themes/default/locales/ar/
+-rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/ar/messages.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/en/
+-rw-rw-rw-   0        0        0     7705 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/en/messages.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/es/
+-rw-rw-rw-   0        0        0     8763 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/es/messages.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/fa/
+-rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/fa/messages.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/he/
+-rw-rw-rw-   0        0        0       36 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/he/messages.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh/
+-rw-rw-rw-   0        0        0     7843 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh/messages.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.056923 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh_cn/
+-rw-rw-rw-   0        0        0     7860 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh_cn/messages.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.072546 webscrapbook-1.9.0/webscrapbook/themes/default/static/
+-rw-rw-rw-   0        0        0      281 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/collapse.png
+-rw-rw-rw-   0        0        0      728 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/comment.png
+-rw-rw-rw-   0        0        0      877 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/common.css
+-rw-rw-rw-   0        0        0     4140 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/common.js
+-rw-rw-rw-   0        0        0     1055 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.css
+-rw-rw-rw-   0        0        0     1563 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.js
+-rw-rw-rw-   0        0        0     2438 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/editx.js
+-rw-rw-rw-   0        0        0      279 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/expand.png
+-rw-rw-rw-   0        0        0      523 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/external.png
+-rw-rw-rw-   0        0        0      752 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/fclose.png
+-rw-rw-rw-   0        0        0      449 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/file.png
+-rw-rw-rw-   0        0        0      790 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/fopen.png
+-rw-rw-rw-   0        0        0     3810 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.css
+-rw-rw-rw-   0        0        0    60629 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.js
+-rw-rw-rw-   0        0        0     2210 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index.css
+-rw-rw-rw-   0        0        0     2156 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/index.js
+-rw-rw-rw-   0        0        0      502 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/item.png
+-rw-rw-rw-   0        0        0      387 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/link.png
+-rw-rw-rw-   0        0        0      445 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/note.png
+-rw-rw-rw-   0        0        0      515 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/postit.png
+-rw-rw-rw-   0        0        0      661 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/search.png
+-rw-rw-rw-   0        0        0      807 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/static/toggle.png
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/webscrapbook/themes/default/templates/
+-rw-rw-rw-   0        0        0      482 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/base.html
+-rw-rw-rw-   0        0        0      632 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/cli.html
+-rw-rw-rw-   0        0        0     1053 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/edit.html
+-rw-rw-rw-   0        0        0      965 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/editx.html
+-rw-rw-rw-   0        0        0     5632 2023-03-26 13:24:56.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/index.html
+-rw-rw-rw-   0        0        0      510 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/maff_index.html
+-rw-rw-rw-   0        0        0      490 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/markdown.html
+-rw-rw-rw-   0        0        0      568 2021-12-07 15:19:05.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_frame.html
+-rw-rw-rw-   0        0        0     1751 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_index.html
+-rw-rw-rw-   0        0        0    12917 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_map.html
+-rw-rw-rw-   0        0        0    26419 2023-03-08 13:49:02.000000 webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_search.html
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.088171 webscrapbook-1.9.0/webscrapbook/util/
+-rw-rw-rw-   0        0        0      120 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/util/__init__.py
+-rw-rw-rw-   0        0        0     5867 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/util/css.py
+-rw-rw-rw-   0        0        0    15308 2023-02-28 12:33:22.000000 webscrapbook-1.9.0/webscrapbook/util/html.py
+-rw-rw-rw-   0        0        0    52535 2023-03-26 12:46:59.000000 webscrapbook-1.9.0/webscrapbook/util/util.py
+-rw-rw-rw-   0        0        0      568 2023-03-26 13:47:18.000000 webscrapbook-1.9.0/webscrapbook/util/zipstream.py
+drwxrwxrwx   0        0        0        0 2023-03-26 13:48:00.025675 webscrapbook-1.9.0/webscrapbook.egg-info/
+-rw-rw-rw-   0        0        0     5422 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3840 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      255 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-03-26 13:47:59.000000 webscrapbook-1.9.0/webscrapbook.egg-info/top_level.txt
```

### Comparing `webscrapbook-1.8.3/LICENSE.txt` & `webscrapbook-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/PKG-INFO` & `webscrapbook-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 1.8.3
+Version: 1.9.0
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -102,20 +102,22 @@
 
 > This step can be skipped if you want PyWebScrapBook default data structure instead. See [doc wiki](https://github.com/danny0838/webscrapbook/wiki/Backend) for more details.
 
 Run the generated `.wsb/serve.py` to start the server, or run below command from CLI:
 
     wsb serve
 
+> Alternatively, a backend server can be run with a specialized WSGI server, such as mod_wsgi, uWSGI, or Gunicorn, by providing the generated application script `.wsb/app.py` to it.
+
 ### Open archive file directly
 
 The `wsbview` executable supports opening an archive page (HTZ or MAFF) to view in the browser.
 
 Run `which wsbview` (or `where wsbview` in Windows) from CLI to get the path of `wsbview` executable, and set default application of MAFF/HTZ file to that executable to open them directly in the browser with double-click.
 
 ### Configuration
 
-Run `wsb config -be` to edit configs for CWD. For documentation about configs, run `wsb help config`, or [read online](https://github.com/danny0838/PyWebScrapBook/blob/master/webscrapbook/resources/config.md).
+Run `wsb config -be` to edit configs for CWD. For documentation about configs, run `wsb help config`, or [read it online](https://github.com/danny0838/PyWebScrapBook/blob/master/webscrapbook/resources/config.md).
 
 ### Further documentation
 
 For more tips about how to configure PyWebScrapBook alongside WebScrapBook, visit [the documentation wiki for WebScrapBook](https://github.com/danny0838/webscrapbook/wiki/Backend).
```

### Comparing `webscrapbook-1.8.3/README.md` & `webscrapbook-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,20 +73,22 @@
 
 > This step can be skipped if you want PyWebScrapBook default data structure instead. See [doc wiki](https://github.com/danny0838/webscrapbook/wiki/Backend) for more details.
 
 Run the generated `.wsb/serve.py` to start the server, or run below command from CLI:
 
     wsb serve
 
+> Alternatively, a backend server can be run with a specialized WSGI server, such as mod_wsgi, uWSGI, or Gunicorn, by providing the generated application script `.wsb/app.py` to it.
+
 ### Open archive file directly
 
 The `wsbview` executable supports opening an archive page (HTZ or MAFF) to view in the browser.
 
 Run `which wsbview` (or `where wsbview` in Windows) from CLI to get the path of `wsbview` executable, and set default application of MAFF/HTZ file to that executable to open them directly in the browser with double-click.
 
 ### Configuration
 
-Run `wsb config -be` to edit configs for CWD. For documentation about configs, run `wsb help config`, or [read online](https://github.com/danny0838/PyWebScrapBook/blob/master/webscrapbook/resources/config.md).
+Run `wsb config -be` to edit configs for CWD. For documentation about configs, run `wsb help config`, or [read it online](https://github.com/danny0838/PyWebScrapBook/blob/master/webscrapbook/resources/config.md).
 
 ### Further documentation
 
 For more tips about how to configure PyWebScrapBook alongside WebScrapBook, visit [the documentation wiki for WebScrapBook](https://github.com/danny0838/webscrapbook/wiki/Backend).
```

### Comparing `webscrapbook-1.8.3/setup.py` & `webscrapbook-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_app_actions.py` & `webscrapbook-1.9.0/tests/test_app_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,18 @@
     def assert_file_equal(self, *datas, is_move=False):
         """Assert if file datas are equivalent.
 
         Args:
             *datas: compatible data format with get_file_data()
             is_move: requires strict equivalent of stat
         """
+        # Such bits may be changed by the API when copying among ZIP files,
+        # and we don't really care about them.
+        excluded_flag_bits = 1 << 3
+
         datas = [self.get_file_data(data, follow_symlinks=not is_move) for data in datas]
         for i in range(1, len(datas)):
             self.assertEqual(datas[0]['bytes'], datas[i]['bytes'])
             if (
                 is_move
                 and isinstance(datas[0]['stat'], os.stat_result)
                 and isinstance(datas[i]['stat'], os.stat_result)
@@ -144,15 +148,15 @@
                     }
                 else:
                     stat0 = {
                         'mtime': zip_timestamp(datas[0]['stat']),
                         'compress_type': datas[0]['stat'].compress_type,
                         'comment': datas[0]['stat'].comment,
                         'extra': datas[0]['stat'].extra,
-                        'flag_bits': datas[0]['stat'].flag_bits,
+                        'flag_bits': datas[0]['stat'].flag_bits & ~excluded_flag_bits,
                         'internal_attr': datas[0]['stat'].internal_attr,
                         'external_attr': datas[0]['stat'].external_attr,
                     }
 
             if isinstance(datas[i]['stat'], os.stat_result):
                 if isinstance(datas[0]['stat'], os.stat_result):
                     stati = {
@@ -173,15 +177,15 @@
                     }
                 else:
                     stati = {
                         'mtime': zip_timestamp(datas[i]['stat']),
                         'compress_type': datas[i]['stat'].compress_type,
                         'comment': datas[i]['stat'].comment,
                         'extra': datas[i]['stat'].extra,
-                        'flag_bits': datas[i]['stat'].flag_bits,
+                        'flag_bits': datas[i]['stat'].flag_bits & ~excluded_flag_bits,
                         'internal_attr': datas[i]['stat'].internal_attr,
                         'external_attr': datas[i]['stat'].external_attr,
                     }
 
             for i in stat0:
                 with self.subTest(i=i):
                     if i == 'mtime':
@@ -238,15 +242,15 @@
 
     @mock.patch('webscrapbook.app.abort', side_effect=abort)
     def test_permission_check2(self, mock_abort):
         zip_filename = os.path.join(tmpdir, 'archive.zip')
         try:
             with zipfile.ZipFile(zip_filename, 'w'):
                 pass
-            with app.test_client() as c, mock.patch('zipfile.ZipFile', side_effect=PermissionError('Forbidden')):
+            with app.test_client() as c, mock.patch('zipfile.ZipFile.__init__', side_effect=PermissionError('Forbidden')):
                 c.get('/archive.zip!/')
                 mock_abort.assert_called_once_with(403)
         finally:
             try:
                 os.remove(zip_filename)
             except FileNotFoundError:
                 pass
@@ -977,15 +981,15 @@
 
     @mock.patch('webscrapbook.app.abort', side_effect=abort)
     def test_permission_check2(self, mock_abort):
         zip_filename = os.path.join(tmpdir, 'archive.zip')
         try:
             with zipfile.ZipFile(zip_filename, 'w'):
                 pass
-            with app.test_client() as c, mock.patch('zipfile.ZipFile', side_effect=PermissionError('Forbidden')):
+            with app.test_client() as c, mock.patch('zipfile.ZipFile.__init__', side_effect=PermissionError('Forbidden')):
                 c.get('/archive.zip!/', query_string={'a': 'list', 'f': 'json'})
                 mock_abort.assert_called_once_with(403)
         finally:
             try:
                 os.remove(zip_filename)
             except FileNotFoundError:
                 pass
@@ -1421,15 +1425,15 @@
 
     @mock.patch('webscrapbook.app.abort', side_effect=abort)
     def test_permission_check2(self, mock_abort):
         zip_filename = os.path.join(tmpdir, 'archive.zip')
         try:
             with zipfile.ZipFile(zip_filename, 'w'):
                 pass
-            with app.test_client() as c, mock.patch('zipfile.ZipFile', side_effect=PermissionError('Forbidden')):
+            with app.test_client() as c, mock.patch('zipfile.ZipFile.__init__', side_effect=PermissionError('Forbidden')):
                 c.get('/archive.zip!/', query_string={'a': 'source'})
                 mock_abort.assert_called_once_with(403)
         finally:
             try:
                 os.remove(zip_filename)
             except FileNotFoundError:
                 pass
@@ -1688,15 +1692,15 @@
 
     @mock.patch('webscrapbook.app.abort', side_effect=abort)
     def test_permission_check2(self, mock_abort):
         zip_filename = os.path.join(tmpdir, 'archive.zip')
         try:
             with zipfile.ZipFile(zip_filename, 'w'):
                 pass
-            with app.test_client() as c, mock.patch('zipfile.ZipFile', side_effect=PermissionError('Forbidden')):
+            with app.test_client() as c, mock.patch('zipfile.ZipFile.__init__', side_effect=PermissionError('Forbidden')):
                 c.get('/archive.zip!/', query_string={'a': 'download'})
                 mock_abort.assert_called_once_with(403)
         finally:
             try:
                 os.remove(zip_filename)
             except FileNotFoundError:
                 pass
@@ -1735,15 +1739,15 @@
 
             with app.test_client() as c:
                 r = c.get('/中文', query_string={'a': 'download'})
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''%E4%B8%AD%E6%96%87.zip; filename="%E4%B8%AD%E6%96%87.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(fh) as zh:
                 self.assert_file_equal(
                     {'file': os.path.join(root, 'subdir')},
                     {'zip': zh, 'filename': 'subdir/'},
@@ -1775,15 +1779,15 @@
             # i=['subdir/bar.txt']
             with app.test_client() as c:
                 r = c.get('/中文', query_string={'a': 'download', 'i': 'subdir/bar.txt'})
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''%E4%B8%AD%E6%96%87.zip; filename="%E4%B8%AD%E6%96%87.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(fh) as zh:
                 with self.assertRaises(KeyError):
                     zh.getinfo('subdir/')
                 self.assert_file_equal(
@@ -1796,15 +1800,15 @@
             # i=['foo.txt']
             with app.test_client() as c:
                 r = c.get('/中文', query_string={'a': 'download', 'i': 'foo.txt'})
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''%E4%B8%AD%E6%96%87.zip; filename="%E4%B8%AD%E6%96%87.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(fh) as zh:
                 with self.assertRaises(KeyError):
                     zh.getinfo('subdir/')
                 with self.assertRaises(KeyError):
@@ -1817,15 +1821,15 @@
             # i=['subdir/bar.txt', 'foo.txt']
             with app.test_client() as c:
                 r = c.get('/中文', query_string=[('a', 'download'), ('i', 'subdir/bar.txt'), ('i', 'foo.txt')])
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''%E4%B8%AD%E6%96%87.zip; filename="%E4%B8%AD%E6%96%87.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(fh) as zh:
                 with self.assertRaises(KeyError):
                     zh.getinfo('subdir/')
                 self.assert_file_equal(
@@ -1887,15 +1891,15 @@
 
             with app.test_client() as c:
                 r = c.get('/archive.zip!/explicit_dir', query_string={'a': 'download'}, buffered=True)
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''explicit_dir.zip; filename="explicit_dir.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(zip_filename) as zh:
                 with zipfile.ZipFile(fh) as zh2:
                     self.assert_file_equal(
                         {'zip': zh, 'filename': 'explicit_dir/subdir/'},
@@ -1912,15 +1916,15 @@
 
             with app.test_client() as c:
                 r = c.get('/archive.zip!/implicit_dir', query_string={'a': 'download'}, buffered=True)
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''implicit_dir.zip; filename="implicit_dir.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(zip_filename) as zh:
                 with zipfile.ZipFile(fh) as zh2:
                     self.assert_file_equal(
                         {'zip': zh, 'filename': 'implicit_dir/subdir/foo.txt'},
@@ -1951,15 +1955,15 @@
             # i=['subdir/foo.txt']
             with app.test_client() as c:
                 r = c.get('/archive.zip!/explicit_dir', query_string={'a': 'download', 'i': 'subdir/foo.txt'}, buffered=True)
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''explicit_dir.zip; filename="explicit_dir.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(zip_filename) as zh:
                 with zipfile.ZipFile(fh) as zh2:
                     with self.assertRaises(KeyError):
                         zh2.getinfo('subdir/')
@@ -1973,15 +1977,15 @@
             # i=['bar.txt']
             with app.test_client() as c:
                 r = c.get('/archive.zip!/explicit_dir', query_string={'a': 'download', 'i': 'bar.txt'}, buffered=True)
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''explicit_dir.zip; filename="explicit_dir.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(zip_filename) as zh:
                 with zipfile.ZipFile(fh) as zh2:
                     with self.assertRaises(KeyError):
                         zh2.getinfo('subdir/')
@@ -1995,15 +1999,15 @@
             # i=['subdir/foo.txt', 'bar.txt']
             with app.test_client() as c:
                 r = c.get('/archive.zip!/explicit_dir', query_string=[('a', 'download'), ('i', 'subdir/foo.txt'), ('i', 'bar.txt')], buffered=True)
 
             self.assertEqual(r.status_code, 200)
             self.assertEqual(r.headers['Content-Type'], 'application/zip')
             self.assertEqual(r.headers['Content-Disposition'], '''attachment; filename*=UTF-8''explicit_dir.zip; filename="explicit_dir.zip"''')
-            self.assertNotEqual(r.headers['Content-Length'], '0')
+            self.assertIsNone(r.headers.get('Content-Length'))
             self.assertEqual(r.headers['Cache-Control'], 'no-store')
             self.assertEqual(r.headers['Content-Security-Policy'], "frame-ancestors 'none';")
             fh = io.BytesIO(r.data)
             with zipfile.ZipFile(zip_filename) as zh:
                 with zipfile.ZipFile(fh) as zh2:
                     with self.assertRaises(KeyError):
                         zh2.getinfo('subdir/')
@@ -2145,15 +2149,15 @@
             c.get('/temp.html', query_string={'a': 'edit'})
             mock_abort.assert_called_once_with(403)
 
     @mock.patch('webscrapbook.app.abort', side_effect=abort)
     def test_permission_check2(self, mock_abort):
         with zipfile.ZipFile(self.test_zip, 'w'):
             pass
-        with app.test_client() as c, mock.patch('zipfile.ZipFile', side_effect=PermissionError('Forbidden')):
+        with app.test_client() as c, mock.patch('zipfile.ZipFile.__init__', side_effect=PermissionError('Forbidden')):
             c.get('/temp.maff!/index.html', query_string={'a': 'edit'})
             mock_abort.assert_called_once_with(403)
 
     @mock.patch('webscrapbook.app.render_template', return_value='')
     def test_file_utf8(self, mock_template):
         with open(self.test_file, 'wb') as fh:
             fh.write('你好𧌒蟲'.encode('UTF-8'))
@@ -2283,15 +2287,15 @@
 
     @mock.patch('webscrapbook.app.abort', side_effect=abort)
     def test_permission_check(self, mock_abort):
         zip_filename = os.path.join(tmpdir, 'archive.zip')
         try:
             with zipfile.ZipFile(zip_filename, 'w'):
                 pass
-            with app.test_client() as c, mock.patch('zipfile.ZipFile', side_effect=PermissionError('Forbidden')):
+            with app.test_client() as c, mock.patch('zipfile.ZipFile.__init__', side_effect=PermissionError('Forbidden')):
                 c.get('/archive.zip!/index.html', query_string={'a': 'editx'})
                 mock_abort.assert_called_once_with(403)
         finally:
             try:
                 os.remove(zip_filename)
             except FileNotFoundError:
                 pass
```

### Comparing `webscrapbook-1.8.3/tests/test_app_config.py` & `webscrapbook-1.9.0/tests/test_app_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 from flask import request
 
 from webscrapbook import WSB_CONFIG, WSB_DIR
 from webscrapbook import app as wsbapp
 from webscrapbook.app import make_app
 
-from . import ROOT_DIR, TEMP_DIR
+from . import PROG_DIR, ROOT_DIR, TEMP_DIR
+
+THEMES_DIR = os.path.join(PROG_DIR, 'themes')
 
 
 def setUpModule():
     """Set up a temp directory for testing."""
     global _tmpdir, tmpdir
     _tmpdir = tempfile.TemporaryDirectory(prefix='config-', dir=TEMP_DIR)
     tmpdir = os.path.realpath(os.path.join(_tmpdir.name, 'd'))
@@ -107,15 +109,15 @@
 theme = default
 """)
 
         make_app(server_root)
         self.assertListEqual([os.path.normcase(i) for i in mock_loader.call_args[0][0]], [
             os.path.normcase(os.path.join(server_root, WSB_DIR, 'themes', 'default', 'templates')),
             os.path.normcase(os.path.abspath(os.path.join(server_root, 'wsb', 'themes', 'default', 'templates'))),
-            os.path.normcase(os.path.abspath(os.path.join(__file__, '..', '..', 'webscrapbook', 'themes', 'default', 'templates'))),
+            os.path.normcase(os.path.abspath(os.path.join(THEMES_DIR, 'default', 'templates'))),
         ])
 
     def test_root(self):
         with open(server_config, 'w', encoding='UTF-8') as fh:
             fh.write("""[app]
 root = subdir
 """)
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
 # @FIXME: Some cases have an unclosed file issue. Although adding #
 buffered=True temporarily suppresses it, a further investigation # for a
 possible leak of the source code is pending. import os import shutil import
 tempfile import unittest from base64 import b64encode from functools import
 partial from unittest import mock from flask import request from webscrapbook
 import WSB_CONFIG, WSB_DIR from webscrapbook import app as wsbapp from
-webscrapbook.app import make_app from . import ROOT_DIR, TEMP_DIR def
-setUpModule(): """Set up a temp directory for testing.""" global _tmpdir,
-tmpdir _tmpdir = tempfile.TemporaryDirectory(prefix='config-', dir=TEMP_DIR)
-tmpdir = os.path.realpath(os.path.join(_tmpdir.name, 'd')) shutil.copytree
-(os.path.join(ROOT_DIR, 'test_app_config'), tmpdir) global server_root,
-server_config server_root = tmpdir server_config = os.path.join(server_root,
-WSB_DIR, WSB_CONFIG) os.makedirs(os.path.dirname(server_config), exist_ok=True)
-# mock out user config global mockings mockings = [ mock.patch
+webscrapbook.app import make_app from . import PROG_DIR, ROOT_DIR, TEMP_DIR
+THEMES_DIR = os.path.join(PROG_DIR, 'themes') def setUpModule(): """Set up a
+temp directory for testing.""" global _tmpdir, tmpdir _tmpdir =
+tempfile.TemporaryDirectory(prefix='config-', dir=TEMP_DIR) tmpdir =
+os.path.realpath(os.path.join(_tmpdir.name, 'd')) shutil.copytree(os.path.join
+(ROOT_DIR, 'test_app_config'), tmpdir) global server_root, server_config
+server_root = tmpdir server_config = os.path.join(server_root, WSB_DIR,
+WSB_CONFIG) os.makedirs(os.path.dirname(server_config), exist_ok=True) # mock
+out user config global mockings mockings = [ mock.patch
 ('webscrapbook.scrapbook.host.WSB_USER_DIR', os.path.join(tmpdir, 'wsb')),
 mock.patch('webscrapbook.WSB_USER_DIR', os.path.join(tmpdir, 'wsb')),
 mock.patch('webscrapbook.WSB_USER_CONFIG', tmpdir), ] for mocking in mockings:
 mocking.start() def tearDownModule(): """Cleanup the temp directory."""
 _tmpdir.cleanup() # stop mock for mocking in mockings: mocking.stop() def token
 (get): """Wrapper to quickly retrieve a token.""" return get('/', query_string=
 {'a': 'token'}).data.decode('UTF-8') class TestApp(unittest.TestCase): def
@@ -35,38 +36,37 @@
 (r.headers['WWW-Authenticate'], 'Basic realm="mywsb"') @mock.patch
 ('jinja2.FileSystemLoader') def test_theme(self, mock_loader): with open
 (server_config, 'w', encoding='UTF-8') as fh: fh.write("""[app] theme = default
 """) make_app(server_root) self.assertListEqual([os.path.normcase(i) for i in
 mock_loader.call_args[0][0]], [ os.path.normcase(os.path.join(server_root,
 WSB_DIR, 'themes', 'default', 'templates')), os.path.normcase(os.path.abspath
 (os.path.join(server_root, 'wsb', 'themes', 'default', 'templates'))),
-os.path.normcase(os.path.abspath(os.path.join(__file__, '..', '..',
-'webscrapbook', 'themes', 'default', 'templates'))), ]) def test_root(self):
-with open(server_config, 'w', encoding='UTF-8') as fh: fh.write("""[app] root =
-subdir """) os.makedirs(os.path.join(server_root, WSB_DIR, 'themes', 'default',
-'static')) with open(os.path.join(server_root, WSB_DIR, 'themes', 'default',
-'static', 'index.js'), 'w', encoding='UTF-8') as fh: fh.write('console.log
-("test");') app = make_app(server_root) app.testing = True with app.test_client
-() as c: get = partial(c.get, buffered=True) post = partial(c.post,
-buffered=True) r = get('/index.html') html = r.data.decode('UTF-8')
-self.assertEqual(html, 'Subdirectory Hello World! ä½ å¥½') # check if server
-dependent files are at the right path r = get('/index.js', query_string={'a':
-'static'}) self.assertEqual(r.data.decode('UTF-8'), 'console.log("test");') t =
-token(post) self.assertEqual(len(os.listdir(os.path.join(server_root, WSB_DIR,
-'server', 'tokens'))), 1) r = post('/', data={ 'token': t, 'a': 'lock', 'f':
-'json', 'name': 'test', }) self.assertTrue(os.path.lexists(os.path.join
-(server_root, WSB_DIR, 'locks', '098f6bcd4621d373cade4e832627b4f6.lock'))) def
-test_x_prefix(self): # allowed_x_prefix = 0 with open(server_config, 'w',
-encoding='UTF-8') as fh: fh.write("""[app] allowed_x_prefix = 0 """) app =
-make_app(server_root) app.testing = True with app.test_client() as c: get =
-partial(c.get, headers={ 'X-Forwarded-Prefix': '/scrap æ¸', }) # / r = get('/
-') html = r.data.decode('UTF-8') self.assertIn('href="/common.css?a=static"',
-html) self.assertIn('href="/index.css?a=static"', html) self.assertIn('src="/
-common.js?a=static"', html) self.assertIn('src="/index.js?a=static"', html)
-self.assertIn('
+os.path.normcase(os.path.abspath(os.path.join(THEMES_DIR, 'default',
+'templates'))), ]) def test_root(self): with open(server_config, 'w',
+encoding='UTF-8') as fh: fh.write("""[app] root = subdir """) os.makedirs
+(os.path.join(server_root, WSB_DIR, 'themes', 'default', 'static')) with open
+(os.path.join(server_root, WSB_DIR, 'themes', 'default', 'static', 'index.js'),
+'w', encoding='UTF-8') as fh: fh.write('console.log("test");') app = make_app
+(server_root) app.testing = True with app.test_client() as c: get = partial
+(c.get, buffered=True) post = partial(c.post, buffered=True) r = get('/
+index.html') html = r.data.decode('UTF-8') self.assertEqual(html, 'Subdirectory
+Hello World! ä½ å¥½') # check if server dependent files are at the right path r
+= get('/index.js', query_string={'a': 'static'}) self.assertEqual(r.data.decode
+('UTF-8'), 'console.log("test");') t = token(post) self.assertEqual(len
+(os.listdir(os.path.join(server_root, WSB_DIR, 'server', 'tokens'))), 1) r =
+post('/', data={ 'token': t, 'a': 'lock', 'f': 'json', 'name': 'test', })
+self.assertTrue(os.path.lexists(os.path.join(server_root, WSB_DIR, 'locks',
+'098f6bcd4621d373cade4e832627b4f6.lock'))) def test_x_prefix(self): #
+allowed_x_prefix = 0 with open(server_config, 'w', encoding='UTF-8') as fh:
+fh.write("""[app] allowed_x_prefix = 0 """) app = make_app(server_root)
+app.testing = True with app.test_client() as c: get = partial(c.get, headers=
+{ 'X-Forwarded-Prefix': '/scrap æ¸', }) # / r = get('/') html = r.data.decode
+('UTF-8') self.assertIn('href="/common.css?a=static"', html) self.assertIn
+('href="/index.css?a=static"', html) self.assertIn('src="/common.js?a=static"',
+html) self.assertIn('src="/index.js?a=static"', html) self.assertIn('
 ****** WebScrapBook/ ******
 ', html) self.assertIn('data-base="" data-path="/"', html) # /subdir/ r = get
 ('/subdir') self.assertEqual(r.status_code, 302) self.assertEqual(r.headers
 ['Location'], 'http://localhost/subdir/') # /subdir/ r = get('/subdir/') html =
 r.data.decode('UTF-8') self.assertIn('href="/common.css?a=static"', html)
 self.assertIn('href="/index.css?a=static"', html) self.assertIn('src="/
 common.js?a=static"', html) self.assertIn('src="/index.js?a=static"', html)
```

### Comparing `webscrapbook-1.8.3/tests/test_app_helpers.py` & `webscrapbook-1.9.0/tests/test_app_helpers.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_cli.py` & `webscrapbook-1.9.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import unittest
 import zipfile
 from unittest import mock
 from urllib.request import pathname2url
 
 from webscrapbook import WSB_DIR, cli
 
-from . import ROOT_DIR, TEMP_DIR
+from . import PROG_DIR, TEMP_DIR
 
-RESOURCE_DIR = os.path.join(ROOT_DIR, '..', 'webscrapbook', 'resources')
+RESOURCE_DIR = os.path.join(PROG_DIR, 'resources')
 
 
 def setUpModule():
     """Set up a temp directory for testing."""
     global _tmpdir, tmpdir
     _tmpdir = tempfile.TemporaryDirectory(prefix='cli-', dir=TEMP_DIR)
     tmpdir = os.path.realpath(_tmpdir.name)
```

### Comparing `webscrapbook-1.8.3/tests/test_init.py` & `webscrapbook-1.9.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_locales.py` & `webscrapbook-1.9.0/tests/test_locales.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_book.py` & `webscrapbook-1.9.0/tests/test_scrapbook_book.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_cache.py` & `webscrapbook-1.9.0/tests/test_scrapbook_cache.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_check.py` & `webscrapbook-1.9.0/tests/test_scrapbook_check.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_convert_file2wsb.py` & `webscrapbook-1.9.0/tests/test_scrapbook_convert_file2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_convert_items.py` & `webscrapbook-1.9.0/tests/test_scrapbook_convert_items.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_convert_migrate.py` & `webscrapbook-1.9.0/tests/test_scrapbook_convert_migrate.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_convert_sb2wsb.py` & `webscrapbook-1.9.0/tests/test_scrapbook_convert_sb2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_convert_wsb2file.py` & `webscrapbook-1.9.0/tests/test_scrapbook_convert_wsb2file.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_convert_wsb2sb.py` & `webscrapbook-1.9.0/tests/test_scrapbook_convert_wsb2sb.py`

 * *Files 0% similar despite different names*

```diff
@@ -994,19 +994,19 @@
 scrapbook.meta({
   "20200101000000000": {
     "index": "20200101000000000/index.html",
     "type": ""
   }
 })""")
 
-        input = """<html><body><scrapbook-linemarker data-scrapbook-id="20200101000000000" data-scrapbook-elem="linemarker" style="border-bottom: 2px dotted #FF0000;" class="first" title="inline annotation
+        input = """<html><body><b><scrapbook-linemarker data-scrapbook-id="20200101000000000" data-scrapbook-elem="linemarker" style="border-bottom: 2px dotted #FF0000;" class="first" title="inline annotation
 2nd line">Suspendisse eget</scrapbook-linemarker></b><scrapbook-linemarker data-scrapbook-id="20200101000000000" data-scrapbook-elem="linemarker" style="border-bottom: 2px dotted #FF0000;" class="last" title="inline annotation
 2nd line"> interdum quam, eu semper ipsum</scrapbook-linemarker>.<style data-scrapbook-elem="annotation-css">/* stylesheet */</style><script data-scrapbook-elem="annotation-loader">/* script */</script></body></html>"""  # noqa: E501
 
-        expected = """<html><body><span data-sb-id="20200101000000000" data-sb-obj="inline" class="scrapbook-inline" style="border-bottom: 2px dotted #FF0000;" title="inline annotation
+        expected = """<html><body><b><span data-sb-id="20200101000000000" data-sb-obj="inline" class="scrapbook-inline" style="border-bottom: 2px dotted #FF0000;" title="inline annotation
 2nd line">Suspendisse eget</span></b><span data-sb-id="20200101000000000" data-sb-obj="inline" class="scrapbook-inline" style="border-bottom: 2px dotted #FF0000;" title="inline annotation
 2nd line"> interdum quam, eu semper ipsum</span>.</body></html>"""  # noqa: E501
 
         index_dir = os.path.join(self.test_input, '20200101000000000')
         os.makedirs(index_dir, exist_ok=True)
         with open(os.path.join(index_dir, 'index.html'), 'w', encoding='UTF-8') as fh:
             fh.write(input)
```

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_exporter.py` & `webscrapbook-1.9.0/tests/test_scrapbook_exporter.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_host.py` & `webscrapbook-1.9.0/tests/test_scrapbook_host.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_importer.py` & `webscrapbook-1.9.0/tests/test_scrapbook_importer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_scrapbook_indexer.py` & `webscrapbook-1.9.0/tests/test_scrapbook_indexer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_server.py` & `webscrapbook-1.9.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_util.py` & `webscrapbook-1.9.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/tests/test_util_html.py` & `webscrapbook-1.9.0/tests/test_util_html.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/__init__.py` & `webscrapbook-1.9.0/webscrapbook/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 from collections import OrderedDict
 from configparser import ConfigParser
 from copy import deepcopy
 
 __all__ = ['WSB_EXTENSION_MIN_VERSION', 'WSB_USER_DIR', 'WSB_USER_CONFIG', 'WSB_DIR', 'WSB_CONFIG', 'config']
 
-__version__ = '1.8.3'
+__version__ = '1.9.0'
 __author__ = 'Danny Lin'
 __author_email__ = 'danny0838@gmail.com'
 __homepage__ = 'https://github.com/danny0838/PyWebScrapBook'
 __license__ = 'MIT'
 
 WSB_EXTENSION_MIN_VERSION = '0.79.0'
 WSB_USER_DIR = os.path.join(os.path.expanduser('~'), '.config', 'wsb')  # affected by $HOME
```

### Comparing `webscrapbook-1.8.3/webscrapbook/app.py` & `webscrapbook-1.9.0/webscrapbook/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,27 +51,33 @@
 host = LocalProxy(lambda: current_app.config['WEBSCRAPBOOK_HOST'])
 
 
 def static_url(path):
     return f'{quote_path(request.script_root)}/{quote_path(path)}?a=static'
 
 
+def apply_csp(response):
+    """Apply CSP, mostly for a static resource.
+    """
+    if host.config['app']['content_security_policy'] == 'strict':
+        response.headers.set('Content-Security-Policy', "connect-src 'none'; form-action 'none';")
+
+
 def static_file(filename, mimetype=None):
     """Output the specified file to the client.
 
     Args:
         filename: absolute path of the file to output.
     """
     if not os.path.isfile(filename):
         abort(404)
     response = flask.send_file(filename, conditional=True, mimetype=mimetype)
     response.headers.set('Accept-Ranges', 'bytes')
     response.headers.set('Cache-Control', 'no-cache')
-    if host.config['app']['content_security_policy'] == 'strict':
-        response.headers.set('Content-Security-Policy', "connect-src 'none'; form-action 'none';")
+    apply_csp(response)
     return response
 
 
 def zip_static_file(zh, subpath, mimetype=None):
     """Output the specified file in a ZIP to the client.
 
     Args:
@@ -99,19 +105,18 @@
 
     headers = {
         'Accept-Ranges': 'bytes',
         'Cache-Control': 'no-cache',
         'Last-Modified': last_modified,
         'ETag': etag,
     }
-    if host.config['app']['content_security_policy'] == 'strict':
-        headers['Content-Security-Policy'] = "connect-src 'none'; form-action 'none';"
 
     response = Response(fh, headers=headers, mimetype=mimetype)
     response.make_conditional(request.environ, accept_ranges=True, complete_length=info.file_size)
+    apply_csp(response)
     return response
 
 
 def stream_template(template_name, **context):
     current_app.update_template_context(context)
     t = current_app.jinja_env.get_template(template_name)
     return t.stream(context)
@@ -305,31 +310,31 @@
             # create a buffer for writing
             buffer = io.BytesIO()
             with zipfile.ZipFile(buffer, 'w') as zh:
                 yield zh
 
             # copy zip file
             for i in reversed(range(1, last + 1)):
-                zip0 = stack.pop()
+                zh0 = stack.pop()
                 with zipfile.ZipFile(buffer, 'a') as zh:
-                    zh.comment = zip0.comment
-                    for info in zip0.infolist():
+                    zh.comment = zh0.comment
+                    for info in zh0.infolist():
                         if filters and i == last:
                             if _open_archive_path_filter(info.filename, filters):
                                 filtered = True
                                 continue
 
                         try:
                             zh.getinfo(info.filename)
                         except KeyError:
                             pass
                         else:
                             continue
 
-                        zh.writestr(info, zip0.read(info),
+                        zh.writestr(info, zh0.read(info),
                                     compress_type=info.compress_type,
                                     compresslevel=None if info.compress_type == zipfile.ZIP_STORED else 9,
                                     )
 
                 if filters and not any(f == '' for f in filters) and not filtered:
                     raise KeyError('paths to filter do not exist')
 
@@ -618,16 +623,14 @@
             return http_response(status=304)
 
         headers = {
             'Cache-Control': 'no-cache',
             'Last-Modified': last_modified,
             'ETag': etag,
         }
-        if host.config['app']['content_security_policy'] == 'strict':
-            headers['Content-Security-Policy'] = "connect-src 'none'; form-action 'none';"
 
         # prepare content
         if zh:
             with zh.open(info) as fh:
                 body = fh.read().decode('UTF-8')
         else:
             with open(localpaths[0], 'r', encoding='UTF-8') as fh:
@@ -638,15 +641,17 @@
                            is_local=is_local_access(),
                            base=request.script_root,
                            path=request.path,
                            pathparts=request.paths,
                            content=commonmark.commonmark(body),
                            )
 
-    return http_response(body, headers=headers)
+    response = http_response(body, headers=headers)
+    apply_csp(response)
+    return response
 
 
 class Request(flask.Request):
     """Subclassed Request object for more useful properties.
     """
     @cached_property
     def paths(self):
@@ -791,15 +796,15 @@
 
                     # recheck if target exists
                     if os.path.lexists(targetpaths[0]):
                         abort(400, 'Found identical entry under the target directory.')
                 else:
                     abort(400, 'Found something at target.')
 
-        return func(sourcepaths=localpaths, targetpaths=targetpaths, *args, **kwargs)
+        return func(*args, sourcepaths=localpaths, targetpaths=targetpaths, **kwargs)
 
     return wrapper
 
 
 def action_unknown():
     """Default handler for an undefined action"""
     abort(400, 'Action not supported.')
@@ -934,74 +939,122 @@
     response.headers.set('Content-Type', 'text/plain; charset=' + quote(encoding))
     response.headers.set('Content-Disposition', 'inline')
 
     return response
 
 
 def action_download():
-    """Download a file or directory.
-
-    @TODO: support streaming ZIP output to prevent memory exhaustion for a large directory
-    """
+    """Download a file or directory."""
     if request.format:
         abort(400, 'Action not supported.')
 
     localpaths = request.localpaths
     filter = request.values.getlist('i')
 
     if len(localpaths) > 1:
+        streaming = False
         with open_archive_path(localpaths) as zh:
             try:
                 zh.getinfo(localpaths[-1])
             except KeyError:
                 base = localpaths[-1] + '/' if localpaths[-1] else ''
                 infos = [i for i in zh.infolist() if i.filename.startswith(base)]
 
                 # not exist
                 if base and not len(infos):
                     abort(404)
 
-                filter = set(filter)
-                filter_d = {f + '/' for f in filter}
-
-                # directory (explicit or implicit)
+                # directory (explicit or implicit): stream as ZIP
+                streaming = True
                 filename = (localpaths[-1] or os.path.basename(localpaths[-2])) + '.zip'
                 mimetype, _ = mimetypes.guess_type(filename)
-                fh = io.BytesIO()
-                with zipfile.ZipFile(fh, 'w') as zh2:
-                    cut = len(base)
-                    for info in infos:
-                        info.filename = info.filename[cut:]
+                cut = len(base)
 
-                        # exclude the directory itself
-                        if not info.filename:
-                            continue
+                # prepare paths to output
+                filter = set(filter)
+                filter_d = {f + '/' for f in filter}
+                paths = []
+                for info in infos:
+                    arcname = info.filename
+                    subpath = info.filename[cut:]
+
+                    # exclude the directory itself
+                    if not arcname:
+                        continue
+
+                    # apply the filter
+                    if filter:
+                        if subpath not in filter:
+                            if not any(subpath.startswith(f) for f in filter_d):
+                                continue
 
-                        # apply the filter
-                        if filter:
-                            if info.filename not in filter:
-                                if not any(info.filename.startswith(f) for f in filter_d):
-                                    continue
-
-                        zh2.writestr(info, zh.read(info))
-
-                fh.seek(0)
-                response = flask.send_file(fh, mimetype=mimetype)
-                response.headers.set('Cache-Control', 'no-store')
+                    paths.append((arcname, subpath))
             else:
                 filename = os.path.basename(request.localrealpath)
                 response = zip_static_file(zh, localpaths[-1], mimetype=request.localmimetype)
+
+        if streaming:
+            def gen():
+                zs = util.ZipStream()
+                with open_archive_path(localpaths) as zh,\
+                     zipfile.ZipFile(zs, 'w') as zf:
+                    for arcname, subpath in paths:
+                        info = zh.getinfo(arcname)
+                        with zh.open(info) as ih:
+                            info.filename = subpath
+                            with zf.open(info, 'w') as oh:
+                                for chunk in iter(lambda: ih.read(8192), b''):
+                                    oh.write(chunk)
+                                    yield zs.get()
+                yield zs.get()
+
+            response = Response(gen(), mimetype=mimetype)
+            response.headers.set('Cache-Control', 'no-store')
     else:
         if os.path.isdir(localpaths[0]):
             filename = os.path.basename(request.localrealpath) + '.zip'
             mimetype, _ = mimetypes.guess_type(filename)
-            fh = io.BytesIO()
-            util.zip_compress(fh, localpaths[0], '', filter=filter)
-            fh.seek(0)
-            response = flask.send_file(fh, mimetype=mimetype)
+
+            # prepare paths to output
+            filter = {os.path.normcase(os.path.join(localpaths[0], f)) for f in filter}
+            filter_d = {os.path.join(f, '') for f in filter}
+            cut = len(os.path.join(localpaths[0], ''))
+            paths = []
+            for root, dirs, files in os.walk(localpaths[0]):
+                for file in dirs + files:
+                    file = os.path.join(root, file)
+
+                    # apply the filter
+                    if filter:
+                        file_nc = os.path.normcase(file)
+                        if file_nc not in filter:
+                            if not any(file_nc.startswith(f) for f in filter_d):
+                                continue
+
+                    subpath = file[cut:]
+                    if os.path.isdir(file):
+                        subpath += '/'
+                    paths.append((file, subpath))
+
+            def gen():
+                zs = util.ZipStream()
+                with zipfile.ZipFile(zs, 'w') as zf:
+                    for file, subpath in paths:
+                        zinfo = zipfile.ZipInfo.from_file(file, subpath)
+                        if zinfo.is_dir():
+                            zf.writestr(zinfo, b'')
+                            yield zs.get()
+                        else:
+                            with open(file, 'rb') as ih, zf.open(zinfo, 'w') as oh:
+                                for chunk in iter(lambda: ih.read(8192), b''):
+                                    oh.write(chunk)
+                                    yield zs.get()
+                yield zs.get()
+
+            response = Response(gen(), mimetype=mimetype)
             response.headers.set('Cache-Control', 'no-store')
         else:
             filename = os.path.basename(request.localrealpath)
             response = static_file(localpaths[0])
 
     filename = quote_path(filename)
     response.headers.set('Content-Disposition',
@@ -1314,20 +1367,20 @@
 def action_mkdir():
     """Create a directory."""
     localpaths = request.localpaths
 
     if len(localpaths) > 1:
         try:
             zh = None
-            with open_archive_path(localpaths) as zip0:
-                if util.zip_has(zip0, localpaths[-1], type='file'):
+            with open_archive_path(localpaths) as zh0:
+                if util.zip_has(zh0, localpaths[-1], type='file'):
                     abort(400, 'Found a non-directory here.')
 
                 # skip if the folder already exists
-                if util.zip_has(zip0, localpaths[-1], type='dir'):
+                if util.zip_has(zh0, localpaths[-1], type='dir'):
                     return
 
                 # append for a non-nested zip
                 if len(localpaths) == 2:
                     zh = zipfile.ZipFile(localpaths[0], 'a')
 
             if zh is None:
@@ -1361,21 +1414,21 @@
 def action_mkzip():
     """Create a zip file."""
     localpaths = request.localpaths
 
     if len(localpaths) > 1:
         try:
             zh = None
-            with open_archive_path(localpaths) as zip0:
-                if util.zip_has(zip0, localpaths[-1], type='dir'):
+            with open_archive_path(localpaths) as zh0:
+                if util.zip_has(zh0, localpaths[-1], type='dir'):
                     abort(400, 'Found a non-file here.')
 
                 # append for a nonexistent path in a non-nested zip
                 if len(localpaths) == 2:
-                    if not util.zip_has(zip0, localpaths[-1], type='file'):
+                    if not util.zip_has(zh0, localpaths[-1], type='file'):
                         zh = zipfile.ZipFile(localpaths[0], 'a')
 
             if zh is None:
                 zh = open_archive_path(localpaths, 'w')
 
             with zh as zh:
                 info = zipfile.ZipInfo(localpaths[-1], time.localtime())
@@ -1415,21 +1468,21 @@
 def action_save():
     """Write a file with provided text or uploaded stream."""
     localpaths = request.localpaths
 
     if len(localpaths) > 1:
         try:
             zh = None
-            with open_archive_path(localpaths) as zip0:
-                if util.zip_has(zip0, localpaths[-1], type='dir'):
+            with open_archive_path(localpaths) as zh0:
+                if util.zip_has(zh0, localpaths[-1], type='dir'):
                     abort(400, 'Found a non-file here.')
 
                 # append for a nonexistent path in a non-nested zip
                 if len(localpaths) == 2:
-                    if not util.zip_has(zip0, localpaths[-1], type='file'):
+                    if not util.zip_has(zh0, localpaths[-1], type='file'):
                         zh = zipfile.ZipFile(localpaths[0], 'a')
 
             if zh is None:
                 zh = open_archive_path(localpaths, 'w')
 
             with zh as zh:
                 info = zipfile.ZipInfo(localpaths[-1], time.localtime())
```

### Comparing `webscrapbook-1.8.3/webscrapbook/cli.py` & `webscrapbook-1.9.0/webscrapbook/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -705,20 +705,21 @@
 
     # -- migrate
     parser_convert_migrate = parser_convert_sub.add_parser(
         'migrate',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""\
 Migrate a scrapbook to be compatible with the latest WebScrapBook version.
+- WebScrapBook < 0.115: Migrate old shadow root loader and content data.
+- WebScrapBook < 0.69: Migrate old canvas and shadow root loaders.
 
-This tool fixes incomplete conversion from legacy ScrapBook to WebScrapBook or
-migrate from older WebScrapBook to the latest.
-
-- Convert legacy annotations and resources at chrome://scrapbook/skin/* for all
-  web pages associated with an item.
+Also fix an incomplete conversion from legacy ScrapBook:
+- Convert legacy annotations to be compatible with latest WebScrapBook.
+- Convert legacy resources at chrome://scrapbook/skin/* to work in a browser
+  without legacy ScrapBook add-on installed.
 - Convert the index file of "postit" items for canonical wrapper and styling.
 """,
         help="""migrate to latest WebScrapBook""")
     parser_convert_migrate.add_argument(
         'input', action='store',
         help="""the input directory""")
     parser_convert_migrate.add_argument(
@@ -774,15 +775,15 @@
   "maff"         a ZIP archive with each page in an individial subfolder
   "single_file"  a single file with resources embedded in
 
 * Conversion between "folder", "htz", and "maff" is mostly lostless (as long as
   no multi-page or arbitrary metadata is included in the MAFF file), while
   conversion between "single_file" and other formats may lose information
   permanently, such as filename and in-depth captured pages. Also note that
-  some features are not supported for single_file.
+  some features are not supported for "single_file".
 
 Available TYPEs:
   ""         a captured web page
   "site"     an in-depth captured web page set
   "file"     a captured or uploaded file
   "image"    an image file captured by legacy ScrapBook
   "note"     a note
@@ -822,15 +823,18 @@
     # -- sb2wsb
     parser_convert_sb2wsb = parser_convert_sub.add_parser(
         'sb2wsb',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""\
 Convert a scrapbook from legacy ScrapBook to WebScrapBook.
 
-Fulltext cache is not converted and requires a manual rebuild.
+The conversion is safe and lossless, with a few caveats:
+- In-depth capture information is not converted and cannot be reused
+  for a merge capture.
+- Fulltext cache is not converted and requires a manual rebuild.
 
 Known supported legacy scrapbook implementations:
 - ScrapBook X (legacy Firefox Add-on)
 - ScrapBook (legacy Firefox Add-on)
 - ScrapBook Plus (legacy Firefox Add-on)
 - ScrapBee (Firefox Quantum Add-on)""",
         help="""convert from legacy ScrapBook to WebScrapBook""")
@@ -842,15 +846,15 @@
         help="""the output directory""")
     parser_convert_sb2wsb.add_argument(
         '--no-data-files', default=False, action='store_true',
         help="""do not convert data files (set this if there's something wrong
 with the conversion, and run "wsb convert migrate" afterwards for advanced options)""")
     parser_convert_sb2wsb.add_argument(
         '--no-backup', default=False, action='store_true',
-        help="""do not backup unneeded legacy scrapbook files""")
+        help="""do not copy legacy ScrapBook files not needed by WebScrapBook""")
     parser_convert_sb2wsb.add_argument(
         '--force', default=False, action='store_true',
         help="""overwrite everything in the output directory""")
     parser_convert_sb2wsb.add_argument(
         '--debug', default=False, action='store_true',
         help="""include debug output""")
```

### Comparing `webscrapbook-1.8.3/webscrapbook/locales.py` & `webscrapbook-1.9.0/webscrapbook/locales.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/resources/config.ini` & `webscrapbook-1.9.0/webscrapbook/resources/config.ini`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/resources/config.md` & `webscrapbook-1.9.0/webscrapbook/resources/config.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ## Overview
 WebScrapBook is an application that can host one or more directories, with
 each host containing one or more scrapbooks.
 
-A host has 3 levels of configuration:
+A WebScrapBook host for a diretory `<root>` has 3 levels of configuration:
 
 * default: written in the source code
 * user: at `~/.config/wsb/config.ini` and `~/.wsbconfig`
-* host: at `<host>/.wsb/config.ini`
+* host: at `<root>/.wsb/config.ini`
 
 with the latters overwriting the formers.
 
 A config file can be generated using the command `wsb config`. Run
 `wsb config --help` for more details.
 
 Configs are loaded only at process starting, and a config change won't affect
-an already running process. For example, a running webscrapbook server needs
+an already running process. For example, a running WebScrapBook host needs
 to be shut off and restarted to get new configs take effect.
 
 
 ## Configuration Format
 
 A WebScrapBook config file is written in "ini" format, which looks like:
 
@@ -52,17 +52,20 @@
 
 
 ## Available values
 
 
 ### `[app]` section
 
-The `[app]` section defines the behavior of WebScrapBook application (for the
-host), which follows WSGI specification and can be hosted by any WSGI server,
-such as the built-in server, `mod_wsgi` Apache module, `uWSGI`, or `Gunicorn`.
+The `[app]` section defines the behavior of the WSGI application of the host.
+
+The host can run with the built-in web server (as the `[server]` section says)
+or with a specialized WSGI server, such as mod_wsgi, uWSGI, or Gunicorn, by
+providing the `.wsb/app.py` script (which can be generated by `wsb config -ba`)
+to it.
 
 
 #### `name`
 
 The name of the served website, which is used as the site title, the label of
 the top level of breadcrumbs, etc.
 
@@ -307,15 +310,15 @@
 
 (default: `all`)
 
 
 ### `[server]` section
 
 The `[server]` section defines the behavior of the built-in HTTP server, which
-can be run by `wsb serve` command or by running the `serve.py` shortcut
+can be run by `wsb serve` command or by executing the `.wsb/serve.py` shortcut
 generated by `wsb config -ba`.
 
 
 #### `port`
 
 A port integer ranged from 0 to 65535 to host. Pick a port >= 1024 to avoid a
 conflict with system ports. Consider the default port (`80` for HTTP and `443`
```

### Comparing `webscrapbook-1.8.3/webscrapbook/resources/mimetypes.md` & `webscrapbook-1.9.0/webscrapbook/resources/mimetypes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/book.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/book.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/cache.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/cache.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/check.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/check.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/convert/file2wsb.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/file2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/convert/items.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/items.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/convert/migrate.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/migrate.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/convert/sb2wsb.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/sb2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/convert/wsb2file.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2file.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/convert/wsb2sb.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/convert/wsb2sb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/exporter.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/exporter.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/host.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/host.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/importer.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/importer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/scrapbook/indexer.py` & `webscrapbook-1.9.0/webscrapbook/scrapbook/indexer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/server.py` & `webscrapbook-1.9.0/webscrapbook/server.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/locales/en/messages.py` & `webscrapbook-1.9.0/webscrapbook/themes/default/locales/en/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/locales/es/messages.py` & `webscrapbook-1.9.0/webscrapbook/themes/default/locales/es/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/locales/zh/messages.py` & `webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/locales/zh_cn/messages.py` & `webscrapbook-1.9.0/webscrapbook/themes/default/locales/zh_cn/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/comment.png` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/comment.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/common.css` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/common.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/common.js` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/common.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/edit.css` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/edit.js` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/edit.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/editx.js` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/editx.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/external.png` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/external.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/fclose.png` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/fclose.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/fopen.png` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/fopen.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/index-ex.css` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/index-ex.js` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/index-ex.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/index.css` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/index.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/index.js` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/index.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/postit.png` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/postit.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/search.png` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/search.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/static/toggle.png` & `webscrapbook-1.9.0/webscrapbook/themes/default/static/toggle.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/cli.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/cli.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/edit.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/edit.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/editx.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/editx.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/index.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_frame.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_frame.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_index.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_map.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_map.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/themes/default/templates/static_search.html` & `webscrapbook-1.9.0/webscrapbook/themes/default/templates/static_search.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/util/css.py` & `webscrapbook-1.9.0/webscrapbook/util/css.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/util/html.py` & `webscrapbook-1.9.0/webscrapbook/util/html.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook/util/util.py` & `webscrapbook-1.9.0/webscrapbook/util/util.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-1.8.3/webscrapbook.egg-info/PKG-INFO` & `webscrapbook-1.9.0/webscrapbook.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 1.8.3
+Version: 1.9.0
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -102,20 +102,22 @@
 
 > This step can be skipped if you want PyWebScrapBook default data structure instead. See [doc wiki](https://github.com/danny0838/webscrapbook/wiki/Backend) for more details.
 
 Run the generated `.wsb/serve.py` to start the server, or run below command from CLI:
 
     wsb serve
 
+> Alternatively, a backend server can be run with a specialized WSGI server, such as mod_wsgi, uWSGI, or Gunicorn, by providing the generated application script `.wsb/app.py` to it.
+
 ### Open archive file directly
 
 The `wsbview` executable supports opening an archive page (HTZ or MAFF) to view in the browser.
 
 Run `which wsbview` (or `where wsbview` in Windows) from CLI to get the path of `wsbview` executable, and set default application of MAFF/HTZ file to that executable to open them directly in the browser with double-click.
 
 ### Configuration
 
-Run `wsb config -be` to edit configs for CWD. For documentation about configs, run `wsb help config`, or [read online](https://github.com/danny0838/PyWebScrapBook/blob/master/webscrapbook/resources/config.md).
+Run `wsb config -be` to edit configs for CWD. For documentation about configs, run `wsb help config`, or [read it online](https://github.com/danny0838/PyWebScrapBook/blob/master/webscrapbook/resources/config.md).
 
 ### Further documentation
 
 For more tips about how to configure PyWebScrapBook alongside WebScrapBook, visit [the documentation wiki for WebScrapBook](https://github.com/danny0838/webscrapbook/wiki/Backend).
```

### Comparing `webscrapbook-1.8.3/webscrapbook.egg-info/SOURCES.txt` & `webscrapbook-1.9.0/webscrapbook.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,8 +95,9 @@
 webscrapbook/themes/default/templates/static_frame.html
 webscrapbook/themes/default/templates/static_index.html
 webscrapbook/themes/default/templates/static_map.html
 webscrapbook/themes/default/templates/static_search.html
 webscrapbook/util/__init__.py
 webscrapbook/util/css.py
 webscrapbook/util/html.py
-webscrapbook/util/util.py
+webscrapbook/util/util.py
+webscrapbook/util/zipstream.py
```

