# Comparing `tmp/ajenti.plugin.traffic-0.7.tar.gz` & `tmp/ajenti.plugin.traffic-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ajenti.plugin.traffic-0.7.tar", last modified: Fri Sep 18 15:18:05 2015, max compression
+gzip compressed data, was "dist/ajenti.plugin.traffic-0.8.tar", last modified: Wed Sep 23 10:25:24 2015, max compression
```

## Comparing `ajenti.plugin.traffic-0.7.tar` & `ajenti.plugin.traffic-0.8.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/README
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      510 2015-09-18 15:14:49.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/plugin.yml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       27 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      648 2015-09-18 13:48:58.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/widget.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      577 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      879 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      563 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/he/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/he/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      492 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      791 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      478 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      567 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      869 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      553 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sw/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      792 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      518 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      817 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      504 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/th/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/th/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      483 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      782 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      469 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/vi/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      489 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      788 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      475 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      570 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      872 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      556 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/de/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/de/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      492 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      791 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      478 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-PT/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      499 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      798 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bn/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      792 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/da/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/da/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      492 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      791 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      478 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fa/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      486 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      785 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      472 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      526 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      825 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      512 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      589 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      891 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      575 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-TW/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      501 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      800 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      487 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      559 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      861 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      545 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/nl/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      491 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      790 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      477 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      538 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      840 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      524 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/en/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/en/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      124 2015-09-11 21:12:16.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/en/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      468 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/en/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      151 2015-09-11 21:44:43.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/en/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      547 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      849 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      533 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/my/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/my/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      486 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      785 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      472 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      569 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      871 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      555 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hu/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      794 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/es-ES/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      795 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/af/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/af/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      794 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tr/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      797 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      480 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/no/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/no/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      794 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      568 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      870 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      554 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tzl/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      497 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      796 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      483 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fr/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      491 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      790 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      477 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-BR/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      510 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      809 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      589 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      891 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      575 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/et/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/et/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      494 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      793 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      480 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/it/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/it/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      792 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/el/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/el/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      491 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      790 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      477 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fy-NL/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      795 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      519 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      818 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      505 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.mo
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      852 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/app.pot
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bg/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      794 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ko/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      784 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      471 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fi/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      792 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ka/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      494 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      793 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      480 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ja/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      487 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      786 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      473 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/id/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/id/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      489 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      788 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      475 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tlh-AA/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      498 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      797 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      484 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sv-SE/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      795 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ca/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      792 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      550 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      852 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      536 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-CN/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      500 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.po~
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      799 2015-09-18 13:51:29.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.po
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.js
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      486 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.mo
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/partial/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      933 2015-09-18 13:48:49.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/partial/widget.html
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      265 2015-09-18 13:48:33.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/partial/widget.config.html
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/js/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/js/module.coffee
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/js/controllers/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      872 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/js/controllers/widget.controller.coffee
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/build/
--rwxrwxrwx   0 eugene    (1000) eugene    (1000)     1151 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/build/all.js
--rwxrwxrwx   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:15:41.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/build/all.css
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       13 2015-09-01 16:35:22.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/.last-upload
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/requirements.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      412 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/views.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/ajenti.plugin.traffic.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       22 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/ajenti.plugin.traffic.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/ajenti.plugin.traffic.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/ajenti.plugin.traffic.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      255 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/ajenti.plugin.traffic.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    10942 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/ajenti.plugin.traffic.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      255 2015-09-18 15:18:05.000000 ajenti.plugin.traffic-0.7/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/requirements.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      183 2015-09-18 15:18:04.000000 ajenti.plugin.traffic-0.7/MANIFEST.in
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:23.000000 ajenti.plugin.traffic-0.8/README
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      510 2015-09-23 10:22:38.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/plugin.yml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       27 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      648 2015-09-18 13:48:58.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/widget.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      577 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      899 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      563 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/he/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/he/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      492 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      814 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      478 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      567 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      889 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      553 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sw/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      815 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      518 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      840 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      504 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/th/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/th/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      483 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      805 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      469 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/vi/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      489 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      811 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      475 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      570 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      892 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      556 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/de/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      492 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      814 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      478 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-PT/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      499 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      821 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bn/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      815 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/da/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/da/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      492 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      814 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      478 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fa/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      486 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      808 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      472 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      526 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      848 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      512 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      589 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      911 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      575 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-TW/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      501 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      823 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      487 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      559 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      881 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      545 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/nl/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      491 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      813 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      477 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      538 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      860 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      524 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/en/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      124 2015-09-11 21:12:16.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/en/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      468 2015-09-18 13:51:28.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/en/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      151 2015-09-11 21:44:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/en/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      547 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      869 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      533 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/my/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/my/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      486 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      808 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      472 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      569 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      891 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      555 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hu/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      817 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/es-ES/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      818 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/af/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/af/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      817 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tr/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      817 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      480 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/no/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/no/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      817 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      568 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      890 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      554 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tzl/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      497 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      819 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      483 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fr/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      491 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      813 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      477 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-BR/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      510 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      832 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      589 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      911 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      575 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/et/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/et/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      494 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      816 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      480 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/it/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      837 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       72 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/el/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/el/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      491 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      813 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      477 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fy-NL/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      818 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      519 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      841 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      505 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.mo
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      852 2015-09-18 13:51:27.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/app.pot
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bg/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      495 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      817 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      481 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ko/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      485 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      807 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      471 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fi/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      815 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ka/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      494 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      816 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      480 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ja/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      487 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      809 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      473 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/id/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      489 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      811 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      475 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tlh-AA/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      498 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      820 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      484 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sv-SE/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      818 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      482 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ca/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      493 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      815 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      479 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      550 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      872 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      536 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-CN/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      500 2015-09-17 09:55:47.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.po~
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      822 2015-09-23 10:11:43.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.po
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       50 2015-09-23 10:23:40.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.js
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      486 2015-09-14 21:23:48.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.mo
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/partial/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      933 2015-09-18 13:48:49.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/partial/widget.html
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      265 2015-09-18 13:48:33.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/partial/widget.config.html
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/js/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/js/module.coffee
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/js/controllers/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      872 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/js/controllers/widget.controller.coffee
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/build/
+-rwxrwxrwx   0 eugene    (1000) eugene    (1000)     1151 2015-09-23 10:23:41.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/build/all.js
+-rwxrwxrwx   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:23:41.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/build/all.css
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       13 2015-09-18 15:18:10.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/.last-upload
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/requirements.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      412 2015-08-28 18:01:53.000000 ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/views.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      496 2015-09-23 10:25:23.000000 ajenti.plugin.traffic-0.8/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti.plugin.traffic.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       22 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti.plugin.traffic.egg-info/top_level.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti.plugin.traffic.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti.plugin.traffic.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      255 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti.plugin.traffic.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    10942 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/ajenti.plugin.traffic.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      255 2015-09-23 10:25:24.000000 ajenti.plugin.traffic-0.8/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2015-09-23 10:25:23.000000 ajenti.plugin.traffic-0.8/requirements.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      183 2015-09-23 10:25:23.000000 ajenti.plugin.traffic-0.8/MANIFEST.in
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/widget.py` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/widget.py`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Arabic\n"
-"Language: ar_SA\n"
+"Language-Team: Slovenian\n"
+"Language: sl_SI\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
-"&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5);\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 1 : n%100==2 ? 2 : n%100==3 || n%100==4 ? 3 : 0);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: ar\n"
+"X-Crowdin-Language: sl\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ar/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Hebrew\n"
-"Language: he_IL\n"
+"Language-Team: Persian\n"
+"Language: fa_IR\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: he\n"
+"X-Crowdin-Language: fa\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Russian\n"
 "Language: ru_RU\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: ru\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
@@ -24,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ru/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Swahili\n"
-"Language: sw_KE\n"
+"Language-Team: Indonesian\n"
+"Language: id_ID\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: sw\n"
+"X-Crowdin-Language: id\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/cs/LC_MESSAGES/app.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Czech\n"
 "Language: cs_CZ\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: cs\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/th/LC_MESSAGES/app.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Thai\n"
 "Language: th_TH\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: th\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Vietnamese\n"
-"Language: vi_VN\n"
+"Language-Team: Finnish\n"
+"Language: fi_FI\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: vi\n"
+"X-Crowdin-Language: fi\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 06:06-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Belarusian\n"
 "Language: be_BY\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: be\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
@@ -24,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/be/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/de/LC_MESSAGES/app.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: German\n"
 "Language: de_DE\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: de\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Portuguese\n"
-"Language: pt_PT\n"
+"Language-Team: Bulgarian\n"
+"Language: bg_BG\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: pt-PT\n"
+"X-Crowdin-Language: bg\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Bengali\n"
-"Language: bn_BD\n"
+"Language-Team: Japanese\n"
+"Language: ja_JP\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: bn\n"
+"X-Crowdin-Language: ja\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Danish\n"
-"Language: da_DK\n"
+"Language-Team: Korean\n"
+"Language: ko_KR\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: da\n"
+"X-Crowdin-Language: ko\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fa/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Persian\n"
-"Language: fa_IR\n"
+"Language-Team: Lithuanian\n"
+"Language: lt_LT\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: fa\n"
+"X-Crowdin-Language: lt\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Latvian\n"
 "Language: lv_LV\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==0 ? 0 : n%10==1 && n%100!=11 ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: lv\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lv/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Serbian (Cyrillic)\n"
-"Language: sr_SP\n"
+"Language-Team: Ukrainian\n"
+"Language: uk_UA\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 3 : n%10==1 && n%100!=11 ? 0 : n"
-"%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: sr\n"
+"X-Crowdin-Language: uk\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/bn/LC_MESSAGES/app.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Chinese Traditional\n"
-"Language: zh_TW\n"
+"Language-Team: Bengali\n"
+"Language: bn_BD\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: zh-TW\n"
+"X-Crowdin-Language: bn\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Lithuanian\n"
-"Language: lt_LT\n"
+"Language-Team: Croatian\n"
+"Language: hr_HR\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && (n"
-"%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: lt\n"
+"X-Crowdin-Language: hr\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/lt/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Dutch\n"
-"Language: nl_NL\n"
+"Language-Team: Slovak\n"
+"Language: sk_SK\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: nl\n"
+"X-Crowdin-Language: sk\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sw/LC_MESSAGES/app.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 06:07-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Romanian\n"
-"Language: ro_RO\n"
+"Language-Team: Swahili\n"
+"Language: sw_KE\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100>0 && n"
-"%100<20)) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: ro\n"
+"X-Crowdin-Language: sw\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ro/LC_MESSAGES/app.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Slovenian\n"
-"Language: sl_SI\n"
+"Language-Team: Romanian\n"
+"Language: ro_RO\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 1 : n%100==2 ? 2 : n%100==3 || n"
-"%100==4 ? 3 : 0);\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100>0 && n%100<20)) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: sl\n"
+"X-Crowdin-Language: ro\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sl/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/my/LC_MESSAGES/app.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Burmese\n"
 "Language: my_MM\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: my\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Ukrainian\n"
-"Language: uk_UA\n"
+"Language-Team: Serbian (Latin)\n"
+"Language: sr_CS\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 3 : n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: uk\n"
+"X-Crowdin-Language: sr-CS\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/uk/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Hungarian\n"
-"Language: hu_HU\n"
+"Language-Team: Estonian\n"
+"Language: et_EE\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: hu\n"
+"X-Crowdin-Language: et\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/es-ES/LC_MESSAGES/app.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Spanish\n"
 "Language: es_ES\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: es-ES\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/af/LC_MESSAGES/app.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Afrikaans\n"
 "Language: af_ZA\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: af\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tr/LC_MESSAGES/app.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Turkish\n"
 "Language: tr_TR\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: tr\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
@@ -24,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hu/LC_MESSAGES/app.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Norwegian\n"
-"Language: no_NO\n"
+"Language-Team: Hungarian\n"
+"Language: hu_HU\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: no\n"
+"X-Crowdin-Language: hu\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr/LC_MESSAGES/app.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Croatian\n"
-"Language: hr_HR\n"
+"Language-Team: Serbian (Cyrillic)\n"
+"Language: sr_SP\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 3 : n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: hr\n"
+"X-Crowdin-Language: sr\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/hr/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Talossan\n"
-"Language: tzl_TZL\n"
+"Language-Team: Frisian\n"
+"Language: fy_NL\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: tzl\n"
+"X-Crowdin-Language: fy-NL\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/fr/LC_MESSAGES/app.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: French\n"
 "Language: fr_FR\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: fr\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-PT/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Portuguese, Brazilian\n"
-"Language: pt_BR\n"
+"Language-Team: Portuguese\n"
+"Language: pt_PT\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: pt-BR\n"
+"X-Crowdin-Language: pt-PT\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/vi/LC_MESSAGES/app.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Serbian (Latin)\n"
-"Language: sr_CS\n"
+"Language-Team: Vietnamese\n"
+"Language: vi_VN\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1 ? 3 : n%10==1 && n%100!=11 ? 0 : n"
-"%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: sr-CS\n"
+"X-Crowdin-Language: vi\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sr-CS/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/et/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Estonian\n"
-"Language: et_EE\n"
+"Language-Team: Greek\n"
+"Language: el_GR\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: et\n"
+"X-Crowdin-Language: el\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 06:06-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Italian\n"
-"Language: it_IT\n"
+"Language-Team: Georgian\n"
+"Language: ka_GE\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: it\n"
+"X-Crowdin-Language: ka\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/el/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Greek\n"
-"Language: el_GR\n"
+"Language-Team: Chinese Simplified\n"
+"Language: zh_CN\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: el\n"
+"X-Crowdin-Language: zh-CN\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fy-NL/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/da/LC_MESSAGES/app.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Frisian\n"
-"Language: fy_NL\n"
+"Language-Team: Danish\n"
+"Language: da_DK\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: fy-NL\n"
+"X-Crowdin-Language: da\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sk/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Slovak\n"
-"Language: sk_SK\n"
+"Language-Team: Polish\n"
+"Language: pl_PL\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: sk\n"
+"X-Crowdin-Language: pl\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/app.pot` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/app.pot`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/bg/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Bulgarian\n"
-"Language: bg_BG\n"
+"Language-Team: Swedish\n"
+"Language: sv_SE\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: bg\n"
+"X-Crowdin-Language: sv-SE\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ko/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/it/LC_MESSAGES/app.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Korean\n"
-"Language: ko_KR\n"
+"Language-Team: Italian\n"
+"Language: it_IT\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: ko\n"
+"X-Crowdin-Language: it\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
-msgstr ""
+msgstr "/ s"
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
-msgstr ""
+msgstr "Interfaccia"
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
-msgstr ""
+msgstr "Traffico"
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/fi/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pt-BR/LC_MESSAGES/app.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Finnish\n"
-"Language: fi_FI\n"
+"Language-Team: Portuguese, Brazilian\n"
+"Language: pt_BR\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: fi\n"
+"X-Crowdin-Language: pt-BR\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ka/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Georgian\n"
-"Language: ka_GE\n"
+"Language-Team: Klingon\n"
+"Language: tlh_AA\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: ka\n"
+"X-Crowdin-Language: tlh-AA\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ja/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/no/LC_MESSAGES/app.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Japanese\n"
-"Language: ja_JP\n"
+"Language-Team: Norwegian\n"
+"Language: no_NO\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: ja\n"
+"X-Crowdin-Language: no\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/id/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/he/LC_MESSAGES/app.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Indonesian\n"
-"Language: id_ID\n"
+"Language-Team: Hebrew\n"
+"Language: he_IL\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: id\n"
+"X-Crowdin-Language: he\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/tlh-AA/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/zh-TW/LC_MESSAGES/app.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Klingon\n"
-"Language: tlh_AA\n"
+"Language-Team: Chinese Traditional\n"
+"Language: zh_TW\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: tlh-AA\n"
+"X-Crowdin-Language: zh-TW\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/sv-SE/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/nl/LC_MESSAGES/app.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Swedish\n"
-"Language: sv_SE\n"
+"Language-Team: Dutch\n"
+"Language: nl_NL\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: sv-SE\n"
+"X-Crowdin-Language: nl\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/ca/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:44-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
 "Language-Team: Catalan\n"
 "Language: ca_ES\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Language: ca\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
@@ -23,7 +24,8 @@
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.po~` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.po~`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.mo` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/pl/LC_MESSAGES/app.mo`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/locale/zh-CN/LC_MESSAGES/app.po` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/locale/tzl/LC_MESSAGES/app.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2015-09-18 15:51+0200\n"
-"PO-Revision-Date: 2015-09-17 05:55-0400\n"
+"PO-Revision-Date: 2015-09-23 05:45-0400\n"
 "Last-Translator: eugenepankov <john.pankov@gmail.com>\n"
-"Language-Team: Chinese Simplified\n"
-"Language: zh_CN\n"
+"Language-Team: Talossan\n"
+"Language: tzl_TZL\n"
+"MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: crowdin.com\n"
 "X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Language: zh-CN\n"
+"X-Crowdin-Language: tzl\n"
 "X-Crowdin-File: /2.0/traffic.po\n"
 
 #: plugins/traffic/resources/partial/widget.html:11
 #: plugins/traffic/resources/partial/widget.html:22
 msgid "/s"
 msgstr ""
 
 #: plugins/traffic/resources/partial/widget.config.html:3
 msgid "Interface"
 msgstr ""
 
 #: plugins/traffic/widget.py:11
 msgid "Traffic"
 msgstr ""
+
```

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/partial/widget.html` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/partial/widget.html`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/js/controllers/widget.controller.coffee` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/js/controllers/widget.controller.coffee`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti_plugin_traffic/resources/build/all.js` & `ajenti.plugin.traffic-0.8/ajenti_plugin_traffic/resources/build/all.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.traffic-0.7/ajenti.plugin.traffic.egg-info/SOURCES.txt` & `ajenti.plugin.traffic-0.8/ajenti.plugin.traffic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

