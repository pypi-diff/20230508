# Comparing `tmp/ajenti.plugin.cron-0.5.tar.gz` & `tmp/ajenti.plugin.cron-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ajenti.plugin.cron-0.5.tar", last modified: Tue Jun 28 14:14:01 2022, max compression
+gzip compressed data, was "ajenti.plugin.cron-0.6.tar", last modified: Mon May  8 04:11:10 2023, max compression
```

## Comparing `ajenti.plugin.cron-0.5.tar` & `ajenti.plugin.cron-0.6.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/
--rw-r--r--   0 eugene     (503) staff       (20)      174 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/MANIFEST.in
--rw-r--r--   0 eugene     (503) staff       (20)      263 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/PKG-INFO
--rw-r--r--   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/README
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti.plugin.cron.egg-info/
--rw-r--r--   0 eugene     (503) staff       (20)      263 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti.plugin.cron.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (503) staff       (20)     5785 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti.plugin.cron.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (503) staff       (20)        1 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti.plugin.cron.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (503) staff       (20)       12 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti.plugin.cron.egg-info/requires.txt
--rw-r--r--   0 eugene     (503) staff       (20)       19 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti.plugin.cron.egg-info/top_level.txt
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/
--rw-r--r--   0 eugene     (503) staff       (20)       58 2021-03-22 09:28:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/README.md
--rw-r--r--   0 eugene     (503) staff       (20)      138 2020-06-25 15:00:56.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/__init__.py
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/af/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/af/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4087 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.po
--rw-r--r--   0 eugene     (503) staff       (20)     4137 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/app.pot
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ar/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ar/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     2115 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4695 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/be/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/be/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4223 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bg/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bg/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bg/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4087 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bg/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bn/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bn/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4085 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bs/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bs/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4159 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ca/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ca/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4085 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/cs/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/cs/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4110 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/da/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/da/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4084 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/de/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/de/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1060 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4503 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/el/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/el/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4083 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/en/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/en/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     4137 2020-10-26 09:25:26.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/en/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/eo/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/eo/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4087 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/es-ES/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4088 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/et/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/et/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4086 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fa/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fa/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fa/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4085 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fa/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fi/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fi/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4085 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fr/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fr/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1145 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4547 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fy-NL/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4088 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/he/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/he/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4134 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hr/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hr/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4160 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hu/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hu/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4087 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/id/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/id/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4081 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/it/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/it/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1076 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4520 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ja/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ja/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4079 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ka/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ka/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4086 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ko/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ko/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4077 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lt/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lt/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4188 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lv/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lv/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4118 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/my/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/my/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4078 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/nl/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/nl/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4083 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/no/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/no/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4087 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pl/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pl/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1146 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4663 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-BR/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1106 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4523 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-PT/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4091 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ro/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ro/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1186 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4571 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ru/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ru/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     2705 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ru/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4982 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ru/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sk/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sk/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4111 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sl/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sl/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4139 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4170 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr-CS/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4170 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sv-SE/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1057 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4480 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sw/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sw/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4085 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/th/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/th/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4075 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tlh-AA/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4090 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tr/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tr/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     1158 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4470 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tzl/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4089 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/uk/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/uk/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)     2959 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     5051 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/vi/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/vi/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/vi/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4081 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/vi/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-CN/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-CN/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-CN/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4092 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-CN/LC_MESSAGES/app.po
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-TW/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/
--rw-r--r--   0 eugene     (503) staff       (20)      629 2022-06-28 14:12:59.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/app.js
--rw-r--r--   0 eugene     (503) staff       (20)     4093 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/app.po
--rw-r--r--   0 eugene     (503) staff       (20)      469 2020-06-25 15:00:56.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/main.py
--rw-r--r--   0 eugene     (503) staff       (20)     1213 2021-03-22 09:28:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/manager.py
--rw-r--r--   0 eugene     (503) staff       (20)      449 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/plugin.yml
--rw-r--r--   0 eugene     (503) staff       (20)       12 2020-06-25 15:00:56.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/requirements.txt
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/build/
--rwxrwxrwx   0 eugene     (503) staff       (20)        0 2022-06-28 14:13:12.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/build/all.css
--rwxrwxrwx   0 eugene     (503) staff       (20)     2851 2022-06-28 14:13:12.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/build/all.js
--rwxrwxrwx   0 eugene     (503) staff       (20)        0 2022-06-28 14:13:12.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/build/all.vendor.css
--rwxrwxrwx   0 eugene     (503) staff       (20)        0 2022-06-28 14:13:12.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/build/all.vendor.js
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/js/
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/js/controllers/
--rw-r--r--   0 eugene     (503) staff       (20)     2381 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/js/controllers/index.controller.es
--rw-r--r--   0 eugene     (503) staff       (20)      126 2020-10-26 09:25:26.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/js/module.es
--rw-r--r--   0 eugene     (503) staff       (20)      213 2020-10-26 09:25:26.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/js/routing.es
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/partial/
--rw-r--r--   0 eugene     (503) staff       (20)     9437 2020-06-25 15:00:56.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/partial/index.html
--rw-r--r--   0 eugene     (503) staff       (20)     2280 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.5/ajenti_plugin_cron/views.py
--rw-r--r--   0 eugene     (503) staff       (20)       12 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/requirements.txt
--rw-r--r--   0 eugene     (503) staff       (20)       38 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/setup.cfg
--rw-r--r--   0 eugene     (503) staff       (20)      551 2022-06-28 14:14:01.000000 ajenti.plugin.cron-0.5/setup.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.432544 ajenti.plugin.cron-0.6/
+-rw-r--r--   0 eugene     (501) staff       (20)      174 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/MANIFEST.in
+-rw-r--r--   0 eugene     (501) staff       (20)      216 2023-05-08 04:11:10.432399 ajenti.plugin.cron-0.6/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/README
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.415835 ajenti.plugin.cron-0.6/ajenti.plugin.cron.egg-info/
+-rw-r--r--   0 eugene     (501) staff       (20)      216 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/ajenti.plugin.cron.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)     5785 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/ajenti.plugin.cron.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/ajenti.plugin.cron.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       12 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/ajenti.plugin.cron.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       19 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/ajenti.plugin.cron.egg-info/top_level.txt
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.416860 ajenti.plugin.cron-0.6/ajenti_plugin_cron/
+-rw-r--r--   0 eugene     (501) staff       (20)       58 2021-03-22 09:28:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/README.md
+-rw-r--r--   0 eugene     (501) staff       (20)      138 2020-06-25 15:00:56.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/__init__.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.417033 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.406007 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/af/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.417334 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/af/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4145 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.po
+-rw-r--r--   0 eugene     (501) staff       (20)     4198 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/app.pot
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.406159 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ar/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.417645 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     2137 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4747 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.406311 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/be/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.417974 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/be/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4281 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.406457 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bg/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.418223 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     2844 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bg/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4912 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bg/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.406609 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bn/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.418517 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4143 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.406776 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bs/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.418808 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bs/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4217 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.406923 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ca/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.419124 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4143 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.407067 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/cs/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.419602 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4168 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.407216 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/da/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.419920 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/da/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4142 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.407397 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/de/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.420196 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/de/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1128 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4618 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.407575 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/el/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.420473 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/el/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4141 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.407729 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/en/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.420614 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/en/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     4198 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/en/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.407879 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/eo/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.420940 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4145 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.408036 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/es-ES/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.421249 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1090 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4543 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.408177 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/et/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.421486 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/et/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4144 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.408341 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fa/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.421736 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     2433 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fa/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4772 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fa/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.408490 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fi/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.421972 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4143 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.408637 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fr/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.422204 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1221 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4662 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.408796 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fy-NL/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.422436 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4146 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.408950 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/he/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.422718 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/he/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4192 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.409118 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hr/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.422960 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4218 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.409277 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hu/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.423241 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4145 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.409437 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/id/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.423550 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/id/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4139 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.409594 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/it/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.423843 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/it/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1108 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4570 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.409742 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ja/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.424128 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4137 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.409893 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ka/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.424406 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4144 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.410051 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ko/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.424669 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4135 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.410202 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lt/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.424935 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4246 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.410353 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lv/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.425213 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4176 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.410514 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/my/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.425489 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/my/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4136 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.410669 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/nl/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.425769 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4141 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.410928 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/no/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.426056 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/no/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4145 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.411100 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pl/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.426322 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1181 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4716 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.411273 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-BR/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.426608 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1137 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4572 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.411418 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-PT/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.426872 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4149 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.411556 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ro/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.427148 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1213 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4620 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.411939 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ru/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.427426 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     2697 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ru/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     5024 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ru/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.412083 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sk/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.427704 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4169 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.412228 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sl/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.427980 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4197 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.412520 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.428535 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4228 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.412373 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr-CS/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.428256 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4228 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.412670 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sv-SE/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.428833 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1083 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4528 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.412824 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sw/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.429110 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4143 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.412977 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/th/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.429392 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/th/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4133 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.413130 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tlh-AA/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.429665 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4148 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.413282 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tr/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.429946 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1194 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4524 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.413435 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tzl/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.430214 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4147 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.413588 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/uk/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.430492 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     2963 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     5097 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.413758 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/vi/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.430765 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/vi/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4139 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/vi/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.413905 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-CN/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.431041 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-CN/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)     1000 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-CN/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4319 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-CN/LC_MESSAGES/app.po
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.414056 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-TW/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.431318 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/
+-rw-r--r--   0 eugene     (501) staff       (20)      669 2023-05-08 04:10:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/app.js
+-rw-r--r--   0 eugene     (501) staff       (20)     4151 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/app.po
+-rw-r--r--   0 eugene     (501) staff       (20)      469 2020-06-25 15:00:56.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/main.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1213 2021-03-22 09:28:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/manager.py
+-rw-r--r--   0 eugene     (501) staff       (20)      449 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/plugin.yml
+-rw-r--r--   0 eugene     (501) staff       (20)       12 2020-06-25 15:00:56.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/requirements.txt
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.414488 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.431752 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/build/
+-rwxrwxrwx   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:50.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/build/all.css
+-rwxrwxrwx   0 eugene     (501) staff       (20)     2851 2023-05-08 04:10:50.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/build/all.js
+-rwxrwxrwx   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:50.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/build/all.vendor.css
+-rwxrwxrwx   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:50.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/build/all.vendor.js
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.431956 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/js/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.432069 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/js/controllers/
+-rw-r--r--   0 eugene     (501) staff       (20)     2381 2022-06-28 14:12:43.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/js/controllers/index.controller.es
+-rw-r--r--   0 eugene     (501) staff       (20)      126 2020-10-26 09:25:26.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/js/module.es
+-rw-r--r--   0 eugene     (501) staff       (20)      213 2020-10-26 09:25:26.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/js/routing.es
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:11:10.432175 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/partial/
+-rw-r--r--   0 eugene     (501) staff       (20)     9680 2023-05-08 04:08:59.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/partial/index.html
+-rw-r--r--   0 eugene     (501) staff       (20)     2279 2022-07-23 18:15:53.000000 ajenti.plugin.cron-0.6/ajenti_plugin_cron/views.py
+-rw-r--r--   0 eugene     (501) staff       (20)       12 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/requirements.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       38 2023-05-08 04:11:10.432581 ajenti.plugin.cron-0.6/setup.cfg
+-rw-r--r--   0 eugene     (501) staff       (20)      551 2023-05-08 04:11:10.000000 ajenti.plugin.cron-0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ajenti.plugin.cron-0.5/ajenti.plugin.cron.egg-info/SOURCES.txt` & `ajenti.plugin.cron-0.6/ajenti.plugin.cron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Afrikaans\n"
-"Language: af_ZA\n"
+"Language-Team: Klingon\n"
+"Language: tlh_AA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: af\n"
+"X-Crowdin-Language: tlh-AA\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/app.pot` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,130 +1,131 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-25 21:20+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
+"Last-Translator: \n"
+"Language-Team: Serbian (Cyrillic)\n"
+"Language: sr_SP\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"X-Crowdin-Project: ajenti\n"
+"X-Crowdin-Project-ID: 18127\n"
+"X-Crowdin-Language: sr\n"
+"X-Crowdin-File: /2.0/cron.po\n"
+"X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
@@ -152,7 +153,8 @@
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
 msgstr ""
+
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "\u0623\u0636\u0641",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "\u0625\u0644\u063a\u0627\u0621 \u0627\u0644\u0623\u0645\u0631",
     "Command": "\u0623\u0645\u0631",
     "Comment": "\u062a\u0639\u0644\u064a\u0642",
     "Day (month)": "\u0627\u0644\u064a\u0648\u0645 (\u0627\u0644\u0634\u0647\u0631)",
     "Day (week)": "\u0627\u0644\u064a\u0648\u0645 (\u0627\u0644\u0623\u0633\u0628\u0648\u0639)",
     "Day of the month": "\u064a\u0648\u0645 \u0645\u0646 \u0627\u0644\u0634\u0647\u0631",
     "Day of the week": "\u064a\u0648\u0645 \u0645\u0646 \u0627\u0644\u0623\u0633\u0628\u0648\u0639",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ar/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
 "Language-Team: Arabic\n"
 "Language: ar_SA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: ar\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "أضف"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr "إلغاء الأمر"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr "أمر"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr "تعليق"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr "اليوم (الشهر)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr "اليوم (الأسبوع)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr "يوم من الشهر"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr "يوم من الأسبوع"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr "المتغيرات البيئية"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr "ساعة"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr "وظائف"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr "دقيقة"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr "تغيير"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr "شهر"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr "الاسم"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "موافق"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr "حفظ"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr "مميز"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr "لا توجد وظيفة محصورة."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr "ولا توجد مهمة خاصة."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr "لا توجد مجموعة من المتغيرات."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr "القيمة"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Cron"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/be/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
 "Language-Team: Belarusian\n"
 "Language: be_BY\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || n%10>=5 && n%10<=9 || n%100>=11 && n%100<=14 ? 2 : 3);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: be\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bg/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bg/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Bulgarian\n"
-"Language: bg_BG\n"
+"Language-Team: Czech\n"
+"Language: cs_CZ\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 3;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: bg\n"
+"X-Crowdin-Language: cs\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Bengali\n"
-"Language: bn_BD\n"
+"Language-Team: Slovenian\n"
+"Language: sl_SI\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 1 : n%100==2 ? 2 : n%100==3 || n%100==4 ? 3 : 0);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: bn\n"
+"X-Crowdin-Language: sl\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Bosnian\n"
-"Language: bs_BA\n"
+"Language-Team: Serbian (Latin)\n"
+"Language: sr_CS\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: bs\n"
+"X-Crowdin-Language: sr-CS\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bn/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Catalan\n"
-"Language: ca_ES\n"
+"Language-Team: Bengali\n"
+"Language: bn_BD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: ca\n"
+"X-Crowdin-Language: bn\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/cs/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Czech\n"
-"Language: cs_CZ\n"
+"Language-Team: Hebrew\n"
+"Language: he_IL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 3;\n"
+"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n%100==4 ? 2 : 3;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: cs\n"
+"X-Crowdin-Language: he\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Danish\n"
-"Language: da_DK\n"
+"Language-Team: Slovak\n"
+"Language: sk_SK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 3;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: da\n"
+"X-Crowdin-Language: sk\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "Hinzuf\u00fcgen",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "<i class=\\\"fas fa-plus-circle\\\"></i>\\n",
     "Cancel": "Abbrechen",
     "Command": "Befehl",
     "Comment": "Kommentar",
     "Day (month)": "Tag (Monat)",
     "Day (week)": "Tag (Woche)",
     "Day of the month": "Tag des Monats",
     "Day of the week": "Wochentag",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/de/LC_MESSAGES/app.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,130 +1,132 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
 "Language-Team: German\n"
 "Language: de_DE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: de\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Hinzufügen"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Hinzufügen"
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr "Abbrechen"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr "Befehl"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr "Kommentar"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr "Tag (Monat)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr "Tag (Woche)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr "Tag des Monats"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr "Wochentag"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr "Umgebungsvariablen"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr "Stunde"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr "Aufträge"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr "Minute"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr "Ändern"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr "Monat"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr "Name"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr "Speichern"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr "Besondere"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr "Es gibt keinen Cronjob."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr "Es gibt keine besondere Aufgabe."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr "Es gibt keine Umgebungsvariablen."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr "Wert"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Cron"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Greek\n"
-"Language: el_GR\n"
+"Language-Team: Croatian\n"
+"Language: hr_HR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: el\n"
+"X-Crowdin-Language: hr\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/en/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,131 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
+"Last-Translator: \n"
+"Language-Team: Talossan\n"
+"Language: tzl_TZL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Crowdin-Project: ajenti\n"
+"X-Crowdin-Project-ID: 18127\n"
+"X-Crowdin-Language: tzl\n"
+"X-Crowdin-File: /2.0/cron.po\n"
+"X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
@@ -152,7 +153,8 @@
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
 msgstr ""
+
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Esperanto\n"
-"Language: eo_UY\n"
+"Language-Team: Japanese\n"
+"Language: ja_JP\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: eo\n"
+"X-Crowdin-Language: ja\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Spanish\n"
-"Language: es_ES\n"
+"Language-Team: Thai\n"
+"Language: th_TH\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: es-ES\n"
+"X-Crowdin-Language: th\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Estonian\n"
-"Language: et_EE\n"
+"Language-Team: Norwegian\n"
+"Language: no_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: et\n"
+"X-Crowdin-Language: no\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fa/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fa/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Persian\n"
-"Language: fa_IR\n"
+"Language-Team: Dutch\n"
+"Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: fa\n"
+"X-Crowdin-Language: nl\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/vi/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Finnish\n"
-"Language: fi_FI\n"
+"Language-Team: Vietnamese\n"
+"Language: vi_VN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: fi\n"
+"X-Crowdin-Language: vi\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "Ajouter",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "<i class=\\\"fas fa-plus-circle\\\"></i>\\n",
     "Cancel": "Annuler",
     "Command": "Commande",
     "Comment": "Commentaire",
     "Day (month)": "Jour (mois)",
     "Day (week)": "Jour (semaine)",
     "Day of the month": "Jour du mois",
     "Day of the week": "Jour de la semaine",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,159 +1,160 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: French\n"
-"Language: fr_FR\n"
+"Language-Team: Turkish\n"
+"Language: tr_TR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: fr\n"
+"X-Crowdin-Language: tr\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Ajouter"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Vazgeç"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr "Commande"
+msgstr "Komut"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr "Commentaire"
+msgstr "Yorum"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr "Jour (mois)"
+msgstr "Gün (ay)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr "Jour (semaine)"
+msgstr "Gün (hafta)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr "Jour du mois"
+msgstr "Ayın günü"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr "Jour de la semaine"
+msgstr "Haftanın günü"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr "Variables d'environnement"
+msgstr "Ortam değişkenleri"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr "Heure"
+msgstr "Saat"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr "Tâches"
+msgstr "İşler"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr "Minute"
+msgstr "Dakika"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr "Modifier"
+msgstr "Düzenle"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr "Mois"
+msgstr "Ay"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr "Nom"
+msgstr "İsim"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
-msgstr "OK"
+msgstr "Tamam"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr "Sauvegarder"
+msgstr "Kaydet"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr "Spécial"
+msgstr "Özel"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr "Il n'y a pas de tâche cron."
+msgstr "Zamanlanmış görev yok."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr "Il n'y a pas de tâche spéciale."
+msgstr "Özel görev yok."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr "Il n'y a pas d'environnement de variables."
+msgstr "Değişken ortam kümesi yoktur."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr "Valeur"
+msgstr "Değer"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
-msgstr "Cron"
+msgstr "Zamanlama"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr "tâche normale"
+msgstr "normal görev"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr "tâche spéciale"
+msgstr "özel görev"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr "variable d'environnement"
+msgstr "ortam değişkeni"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr "Souhaitez-vous vraiment supprimer cette entrée ?"
+msgstr "Bu girişi gerçekten kalıcı olarak silmek istiyor musunuz?"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr "Supprimer"
+msgstr "Sil"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr "Crontab enregistré avec succès !"
+msgstr "Crontab başarıyla kaydedildi!"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr "Échec de l'enregistrement du crontab"
+msgstr "Crontab kaydedilemedi"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ca/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Frisian\n"
-"Language: fy_NL\n"
+"Language-Team: Catalan\n"
+"Language: ca_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: fy-NL\n"
+"X-Crowdin-Language: ca\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/he/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-CN/LC_MESSAGES/app.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Hebrew\n"
-"Language: he_IL\n"
+"Language-Team: Chinese Simplified\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n%100==4 ? 2 : 3;\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: he\n"
+"X-Crowdin-Language: zh-CN\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr ""
+msgstr "取消 "
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr ""
+msgstr "命令"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr ""
+msgstr "备注"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr ""
+msgstr "天 (月)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr ""
+msgstr "天 (周)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr ""
+msgstr "月份中的天"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr ""
+msgstr "每周的某日"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr ""
+msgstr "环境变量"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr ""
+msgstr "时"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr ""
+msgstr "任务"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr ""
+msgstr "分钟"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr ""
+msgstr "修改"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr ""
+msgstr "月"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr ""
+msgstr "名称"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
-msgstr ""
+msgstr "确定"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr ""
+msgstr "保存"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr ""
+msgstr "杂项"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr ""
+msgstr "没有定时任务"
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr ""
+msgstr "没有特殊的任务。"
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hr/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Croatian\n"
-"Language: hr_HR\n"
+"Language-Team: Swahili\n"
+"Language: sw_KE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: hr\n"
+"X-Crowdin-Language: sw\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/hu/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
 "Language-Team: Hungarian\n"
 "Language: hu_HU\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: hu\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Indonesian\n"
-"Language: id_ID\n"
+"Language-Team: Lithuanian\n"
+"Language: lt_LT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && (n%100>19 || n%100<11) ? 0 : (n%10>=2 && n%10<=9) && (n%100>19 || n%100<11) ? 1 : n%1!=0 ? 2: 3);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: id\n"
+"X-Crowdin-Language: lt\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "Aggiungi",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "Annulla",
     "Command": "Comando",
     "Comment": "Commento",
     "Day (month)": "Giorni (mese)",
     "Day (week)": "Giorni (settimana)",
     "Day of the month": "Giorno del mese",
     "Day of the week": "Giorno della settimana",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,159 +1,160 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Italian\n"
-"Language: it_IT\n"
+"Language-Team: Portuguese, Brazilian\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: it\n"
+"X-Crowdin-Language: pt-BR\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Aggiungi"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Cancelar"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr "Comando"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr "Commento"
+msgstr "Comentário"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr "Giorni (mese)"
+msgstr "Dia (mês)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr "Giorni (settimana)"
+msgstr "Dia (semana)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr "Giorno del mese"
+msgstr "Dia do mês"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr "Giorno della settimana"
+msgstr "Dia da semana"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr "Variabili ambientali"
+msgstr "Variáveis de ambiente"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr "Ora"
+msgstr "Hora"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr "Lavori"
+msgstr "Tarefas"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr "Minuto"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr "Modifica"
+msgstr "Alterar"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr "Mese"
+msgstr "Mês"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr "Nome"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr "Salva"
+msgstr "Salvar"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr "Speciale"
+msgstr "Especial"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr "Nessun cronjob."
+msgstr "Não há cronjob."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr "Nessun'attività speciale."
+msgstr "Não há nenhuma tarefa especial."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr "Nessuna variabile ambientale impostata."
+msgstr "Não há nenhum ambiente de variáveis definido."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr "Valore"
+msgstr "Valor"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Cron"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr "attività normale"
+msgstr "tarefa normal"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr "attività speciale"
+msgstr "tarefa especial"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr "variabile ambientale"
+msgstr "variável de ambiente"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr "Sei sicuro di voler eliminare permanentemente questa voce?"
+msgstr "Você realmente quer excluir esta entrada permanentemente?"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr "Elimina"
+msgstr "Excluir"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr "Crontab salvata correttamente !"
+msgstr "Crontab salva com sucesso!"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr "Impossibile salvare la crontab"
+msgstr "Falha ao salvar crontab"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ja/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/da/LC_MESSAGES/app.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Japanese\n"
-"Language: ja_JP\n"
+"Language-Team: Danish\n"
+"Language: da_DK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: ja\n"
+"X-Crowdin-Language: da\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Georgian\n"
-"Language: ka_GE\n"
+"Language-Team: Korean\n"
+"Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: ka\n"
+"X-Crowdin-Language: ko\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ko/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fi/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Korean\n"
-"Language: ko_KR\n"
+"Language-Team: Finnish\n"
+"Language: fi_FI\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: ko\n"
+"X-Crowdin-Language: fi\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lt/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/el/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Lithuanian\n"
-"Language: lt_LT\n"
+"Language-Team: Greek\n"
+"Language: el_GR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && (n%100>19 || n%100<11) ? 0 : (n%10>=2 && n%10<=9) && (n%100>19 || n%100<11) ? 1 : n%1!=0 ? 2: 3);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: lt\n"
+"X-Crowdin-Language: el\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/et/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Latvian\n"
-"Language: lv_LV\n"
+"Language-Team: Estonian\n"
+"Language: et_EE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==0 ? 0 : n%10==1 && n%100!=11 ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: lv\n"
+"X-Crowdin-Language: et\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/my/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
 "Language-Team: Burmese\n"
 "Language: my_MM\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: my\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/nl/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/id/LC_MESSAGES/app.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Dutch\n"
-"Language: nl_NL\n"
+"Language-Team: Indonesian\n"
+"Language: id_ID\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: nl\n"
+"X-Crowdin-Language: id\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/no/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/af/LC_MESSAGES/app.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Norwegian\n"
-"Language: no_NO\n"
+"Language-Team: Afrikaans\n"
+"Language: af_ZA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: no\n"
+"X-Crowdin-Language: af\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "Dodaj",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "Anuluj",
     "Command": "Komenda",
     "Comment": "Komentarz",
     "Day (month)": "Dzie\u0144 (miesi\u0105c)",
     "Day (week)": "Dzie\u0144 (tydzie\u0144)",
     "Day of the month": "Dzie\u0144 miesi\u0105ca",
     "Day of the week": "Dzie\u0144 tygodnia",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pl/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
 "Language-Team: Polish\n"
 "Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: pl\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Dodaj"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr "Anuluj"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr "Komenda"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr "Komentarz"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr "Dzień (miesiąc)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr "Dzień (tydzień)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr "Dzień miesiąca"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr "Dzień tygodnia"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr "Zmienne środowiskowe"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr "Godzina"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr "Zadania"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr "Minuta"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr "Modyfikuj"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr "Miesiąc"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr "Nazwa"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr "Zapisz"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr "Specjalne"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr "Brak zadania cron."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr "Nie ma specjalnego zadania."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr "Nie ma ustawionych zmiennych."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr "Wartość"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Cron"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "Adicionar",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "Cancelar",
     "Command": "Comando",
     "Comment": "Coment\u00e1rio",
     "Day (month)": "Dia (m\u00eas)",
     "Day (week)": "Dia (semana)",
     "Day of the month": "Dia do m\u00eas",
     "Day of the week": "Dia da semana",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-BR/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,159 +1,160 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Portuguese, Brazilian\n"
-"Language: pt_BR\n"
+"Language-Team: Romanian\n"
+"Language: ro_RO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100>0 && n%100<20)) ? 1 : 2);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: pt-BR\n"
+"X-Crowdin-Language: ro\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Adicionar"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Anulare"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr "Comando"
+msgstr "Comandă"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr "Comentário"
+msgstr "Comentariu"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr "Dia (mês)"
+msgstr "Zi (lună)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr "Dia (semana)"
+msgstr "Zi (săptămână)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr "Dia do mês"
+msgstr "Ziua lunii"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr "Dia da semana"
+msgstr "Ziua săptămânii"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr "Variáveis de ambiente"
+msgstr "Variabile de mediu"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr "Hora"
+msgstr "Ora"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr "Tarefas"
+msgstr "Joburi"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr "Minuto"
+msgstr "Minut"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr "Alterar"
+msgstr "Modificare"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr "Mês"
+msgstr "Luna"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr "Nome"
+msgstr "Nume"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr "Salvar"
+msgstr "Salvare"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr "Especial"
+msgstr "Special"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr "Não há cronjob."
+msgstr "Nu există joburi."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr "Não há nenhuma tarefa especial."
+msgstr "Nu există sarcini speciale."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr "Não há nenhum ambiente de variáveis definido."
+msgstr "Nu există nici o variabilă de mediu setată."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr "Valor"
+msgstr "Valoare"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Cron"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr "tarefa normal"
+msgstr "sarcină normală"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr "tarefa especial"
+msgstr "sarcină specială"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr "variável de ambiente"
+msgstr "variabilă de mediu"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr "Você realmente quer excluir esta entrada permanentemente?"
+msgstr "Sunteţi sigur că doriţi să ştergeţi definitiv această intrare?"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr "Excluir"
+msgstr "Ștergere"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr "Crontab salva com sucesso!"
+msgstr "Crontab salvat cu succes!"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr "Falha ao salvar crontab"
+msgstr "Salvarea crontab a eșuat"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/pt-PT/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
 "Language-Team: Portuguese\n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: pt-PT\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "Ad\u0103ugare",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "Anulare",
     "Command": "Comand\u0103",
     "Comment": "Comentariu",
     "Day (month)": "Zi (lun\u0103)",
     "Day (week)": "Zi (s\u0103pt\u0103m\u00e2n\u0103)",
     "Day of the month": "Ziua lunii",
     "Day of the week": "Ziua s\u0103pt\u0103m\u00e2nii",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ro/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fa/LC_MESSAGES/app.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,159 +1,160 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Romanian\n"
-"Language: ro_RO\n"
+"Language-Team: Persian\n"
+"Language: fa_IR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100>0 && n%100<20)) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: ro\n"
+"X-Crowdin-Language: fa\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Adăugare"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr "Anulare"
+msgstr "لغو"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr "Comandă"
+msgstr "دستور"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr "Comentariu"
+msgstr "دیدگاه"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr "Zi (lună)"
+msgstr "روز (ماه)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr "Zi (săptămână)"
+msgstr "روز (هفته)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr "Ziua lunii"
+msgstr "روز از ماه"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr "Ziua săptămânii"
+msgstr "روز از هفته"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr "Variabile de mediu"
+msgstr "متغیرهای محیطی"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr "Ora"
+msgstr "ساعت"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr "Joburi"
+msgstr "مشاغل"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr "Minut"
+msgstr "دقیقه"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr "Modificare"
+msgstr "ویرایش"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr "Luna"
+msgstr "ماه"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr "Nume"
+msgstr "نام"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
-msgstr "OK"
+msgstr "تایید"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr "Salvare"
+msgstr "ذخیره"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr "Special"
+msgstr "ویژه"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr "Nu există joburi."
+msgstr "کرنجاب وجود ندارد."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr "Nu există sarcini speciale."
+msgstr "هیچ مورد خاصی وجود ندارد."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr "Nu există nici o variabilă de mediu setată."
+msgstr "هیچ مجموعه ای از متغیرهای محیطی وجود ندارد."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr "Valoare"
+msgstr "مقدار"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
-msgstr "Cron"
+msgstr "کرون"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr "sarcină normală"
+msgstr "مامویت معمولی"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr "sarcină specială"
+msgstr "ماموریت ویژه"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr "variabilă de mediu"
+msgstr "متغیر محیطی"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr "Sunteţi sigur că doriţi să ştergeţi definitiv această intrare?"
+msgstr "مطمئنید می‌خواهید برای همیشه این ورودی را حذف کنید؟"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr "Ștergere"
+msgstr "حذف"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr "Crontab salvat cu succes!"
+msgstr "Crontab با موفقیت ذخیره شد!"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr "Salvarea crontab a eșuat"
+msgstr "دخیره Crontab ناموفق بود"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ru/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ru/LC_MESSAGES/app.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "\u0414\u043e\u0431\u0430\u0432\u0438\u0442\u044c",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "\u041e\u0442\u043c\u0435\u043d\u0438\u0442\u044c",
     "Command": "\u041a\u043e\u043c\u0430\u043d\u0434\u0430",
     "Comment": "\u041a\u043e\u043c\u043c\u0435\u043d\u0442\u0430\u0440\u0438\u0439",
     "Day (month)": "\u0414\u0435\u043d\u044c (\u043c\u0435\u0441\u044f\u0446)",
     "Day (week)": "\u0414\u0435\u043d\u044c (\u043d\u0435\u0434\u0435\u043b\u044f)",
     "Day of the month": "\u0414\u0435\u043d\u044c \u043c\u0435\u0441\u044f\u0446\u0430",
     "Day of the week": "\u0414\u0435\u043d\u044c \u043d\u0435\u0434\u0435\u043b\u0438",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/ru/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,159 +1,160 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Russian\n"
-"Language: ru_RU\n"
+"Language-Team: Swedish\n"
+"Language: sv_SE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=((n%10==1 && n%100!=11) ? 0 : ((n%10 >= 2 && n%10 <=4 && (n%100 < 12 || n%100 > 14)) ? 1 : ((n%10 == 0 || (n%10 >= 5 && n%10 <=9)) || (n%100 >= 11 && n%100 <= 14)) ? 2 : 3));\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: ru\n"
+"X-Crowdin-Language: sv-SE\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Добавить"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr "Отменить"
+msgstr "Avbryt"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr "Команда"
+msgstr "Kommando"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr "Комментарий"
+msgstr "Kommentar"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr "День (месяц)"
+msgstr "Dag (månad)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr "День (неделя)"
+msgstr "Dag (vecka)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr "День месяца"
+msgstr "Dag i månaden"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr "День недели"
+msgstr "Veckodag"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr "Переменные окружения"
+msgstr "Miljövariabler"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr "Час"
+msgstr "Timme"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr "Работы"
+msgstr "Jobb"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr "Минуты"
+msgstr "Minut"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr "Изменить"
+msgstr "Ändra"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr "Месяц"
+msgstr "Månad"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr "Имя"
+msgstr "Namn"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr "Сохранить"
+msgstr "Spara"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr "Специальный"
+msgstr "Speciell"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr "Нет задач для cron."
+msgstr "Det finns inget cronjobb."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr "Нет специальной задачи."
+msgstr "Det finns ingen speciell uppgift."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr "Переменных окружения не установлено."
+msgstr "Det finns ingen variablermiljö satt."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr "Значение"
+msgstr "Värde"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Cron"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr "Обычная задача"
+msgstr "normal uppgift"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr "специальная задача"
+msgstr "speciell uppgift"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr "Переменная среды"
+msgstr "miljövariabel"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr "Вы действительно хотите удалить эту запись?"
+msgstr "Vill du verkligen permanent ta bort denna post?"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr "Удалить"
+msgstr "Ta bort"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr "Crontab успешно сохранен !"
+msgstr "Crontab har sparats!"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr "Не удалось сохранить crontab"
+msgstr "Det gick inte att spara crontab"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sk/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/app.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Slovak\n"
-"Language: sk_SK\n"
+"Language-Team: Chinese Traditional\n"
+"Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 3;\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: sk\n"
+"X-Crowdin-Language: zh-TW\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sl/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/eo/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Slovenian\n"
-"Language: sl_SI\n"
+"Language-Team: Esperanto\n"
+"Language: eo_UY\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 1 : n%100==2 ? 2 : n%100==3 || n%100==4 ? 3 : 0);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: sl\n"
+"X-Crowdin-Language: eo\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/bs/LC_MESSAGES/app.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Serbian (Cyrillic)\n"
-"Language: sr_SP\n"
+"Language-Team: Bosnian\n"
+"Language: bs_BA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: sr\n"
+"X-Crowdin-Language: bs\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sr-CS/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/ka/LC_MESSAGES/app.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Serbian (Latin)\n"
-"Language: sr_CS\n"
+"Language-Team: Georgian\n"
+"Language: ka_GE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: sr-CS\n"
+"X-Crowdin-Language: ka\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "L\u00e4gg till",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "Avbryt",
     "Command": "Kommando",
     "Comment": "Kommentar",
     "Day (month)": "Dag (m\u00e5nad)",
     "Day (week)": "Dag (vecka)",
     "Day of the month": "Dag i m\u00e5naden",
     "Day of the week": "Veckodag",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sv-SE/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/it/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,159 +1,160 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Swedish\n"
-"Language: sv_SE\n"
+"Language-Team: Italian\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: sv-SE\n"
+"X-Crowdin-Language: it\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Lägg till"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr "Avbryt"
+msgstr "Annulla"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr "Kommando"
+msgstr "Comando"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr "Kommentar"
+msgstr "Commento"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr "Dag (månad)"
+msgstr "Giorni (mese)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr "Dag (vecka)"
+msgstr "Giorni (settimana)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr "Dag i månaden"
+msgstr "Giorno del mese"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr "Veckodag"
+msgstr "Giorno della settimana"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr "Miljövariabler"
+msgstr "Variabili ambientali"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr "Timme"
+msgstr "Ora"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr "Jobb"
+msgstr "Lavori"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr "Minut"
+msgstr "Minuto"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr "Ändra"
+msgstr "Modifica"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr "Månad"
+msgstr "Mese"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr "Namn"
+msgstr "Nome"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr "Spara"
+msgstr "Salva"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr "Speciell"
+msgstr "Speciale"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr "Det finns inget cronjobb."
+msgstr "Nessun cronjob."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr "Det finns ingen speciell uppgift."
+msgstr "Nessun'attività speciale."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr "Det finns ingen variablermiljö satt."
+msgstr "Nessuna variabile ambientale impostata."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr "Värde"
+msgstr "Valore"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Cron"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr "normal uppgift"
+msgstr "attività normale"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr "speciell uppgift"
+msgstr "attività speciale"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr "miljövariabel"
+msgstr "variabile ambientale"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr "Vill du verkligen permanent ta bort denna post?"
+msgstr "Sei sicuro di voler eliminare permanentemente questa voce?"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr "Ta bort"
+msgstr "Elimina"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr "Crontab har sparats!"
+msgstr "Crontab salvata correttamente !"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr "Det gick inte att spara crontab"
+msgstr "Impossibile salvare la crontab"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/sw/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fy-NL/LC_MESSAGES/app.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Swahili\n"
-"Language: sw_KE\n"
+"Language-Team: Frisian\n"
+"Language: fy_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: sw\n"
+"X-Crowdin-Language: fy-NL\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/vi/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/th/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/lv/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Thai\n"
-"Language: th_TH\n"
+"Language-Team: Latvian\n"
+"Language: lv_LV\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=(n==0 ? 0 : n%10==1 && n%100!=11 ? 1 : 2);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: th\n"
+"X-Crowdin-Language: lv\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/zh-TW/LC_MESSAGES/app.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "",
     "Command": "",
     "Comment": "",
     "Day (month)": "",
     "Day (week)": "",
     "Day of the month": "",
     "Day of the week": "",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tlh-AA/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/es-ES/LC_MESSAGES/app.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,159 +1,160 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
-"Language-Team: Klingon\n"
-"Language: tlh_AA\n"
+"Language-Team: Spanish\n"
+"Language: es_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: tlh-AA\n"
+"X-Crowdin-Language: es-ES\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr ""
+msgstr "Cancelar"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr ""
+msgstr "Comando"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr ""
+msgstr "Comentario"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr ""
+msgstr "Día (mes)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr ""
+msgstr "Día (semana)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr ""
+msgstr "Día del mes"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr ""
+msgstr "Día de la semana"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr ""
+msgstr "Variables de entorno"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr ""
+msgstr "Hora"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr ""
+msgstr "Trabajos"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr ""
+msgstr "Minuto"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr ""
+msgstr "Modificar"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr ""
+msgstr "Mes"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr ""
+msgstr "Nombre"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
-msgstr ""
+msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr ""
+msgstr "Guardar"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr ""
+msgstr "Especial"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr ""
+msgstr "No hay cronjob."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr ""
+msgstr "No hay tareas especiales."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr ""
+msgstr "No se han establecido variabls de entorno."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr ""
+msgstr "Valor"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
-msgstr ""
+msgstr "Cron"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr ""
+msgstr "Tarea normal"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr ""
+msgstr "Tarea especial"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr ""
+msgstr "Variable de entorno"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr ""
+msgstr "¿Quiere eliminar permanentemente esta entrada?"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr ""
+msgstr "Eliminar"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr ""
+msgstr "Crontab guardado con éxito !"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr ""
+msgstr "Error al guardar la crontab"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "Ekle",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "Vazge\u00e7",
     "Command": "Komut",
     "Comment": "Yorum",
     "Day (month)": "G\u00fcn (ay)",
     "Day (week)": "G\u00fcn (hafta)",
     "Day of the month": "Ay\u0131n g\u00fcn\u00fc",
     "Day of the week": "Haftan\u0131n g\u00fcn\u00fc",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tr/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/fr/LC_MESSAGES/app.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,159 +1,161 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:29\n"
 "Last-Translator: \n"
-"Language-Team: Turkish\n"
-"Language: tr_TR\n"
+"Language-Team: French\n"
+"Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: tr\n"
+"X-Crowdin-Language: fr\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Ekle"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Ajouter"
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
-msgstr "Vazgeç"
+msgstr "Annuler"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
-msgstr "Komut"
+msgstr "Commande"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
-msgstr "Yorum"
+msgstr "Commentaire"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
-msgstr "Gün (ay)"
+msgstr "Jour (mois)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
-msgstr "Gün (hafta)"
+msgstr "Jour (semaine)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
-msgstr "Ayın günü"
+msgstr "Jour du mois"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
-msgstr "Haftanın günü"
+msgstr "Jour de la semaine"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
-msgstr "Ortam değişkenleri"
+msgstr "Variables d'environnement"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
-msgstr "Saat"
+msgstr "Heure"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
-msgstr "İşler"
+msgstr "Tâches"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
-msgstr "Dakika"
+msgstr "Minute"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
-msgstr "Düzenle"
+msgstr "Modifier"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
-msgstr "Ay"
+msgstr "Mois"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
-msgstr "İsim"
+msgstr "Nom"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
-msgstr "Tamam"
+msgstr "OK"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
-msgstr "Kaydet"
+msgstr "Sauvegarder"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
-msgstr "Özel"
+msgstr "Spécial"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
-msgstr "Zamanlanmış görev yok."
+msgstr "Il n'y a pas de tâche cron."
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
-msgstr "Özel görev yok."
+msgstr "Il n'y a pas de tâche spéciale."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
-msgstr "Değişken ortam kümesi yoktur."
+msgstr "Il n'y a pas d'environnement de variables."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
-msgstr "Değer"
+msgstr "Valeur"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
-msgstr "Zamanlama"
+msgstr "Cron"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:32
 msgid "normal task"
-msgstr "normal görev"
+msgstr "tâche normale"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:33
 msgid "special task"
-msgstr "özel görev"
+msgstr "tâche spéciale"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:34
 msgid "environment variable"
-msgstr "ortam değişkeni"
+msgstr "variable d'environnement"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:45
 msgid "Do you really want to permanently delete this entry?"
-msgstr "Bu girişi gerçekten kalıcı olarak silmek istiyor musunuz?"
+msgstr "Souhaitez-vous vraiment supprimer cette entrée ?"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:46
 msgid "Delete"
-msgstr "Sil"
+msgstr "Supprimer"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
-msgstr "Crontab başarıyla kaydedildi!"
+msgstr "Crontab enregistré avec succès !"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
-msgstr "Crontab kaydedilemedi"
+msgstr "Échec de l'enregistrement du crontab"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/tzl/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/en/LC_MESSAGES/app.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,132 @@
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: ajenti\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:28\n"
-"Last-Translator: \n"
-"Language-Team: Talossan\n"
-"Language: tzl_TZL\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: tzl\n"
-"X-Crowdin-File: /2.0/cron.po\n"
-"X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid ""
+"<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
@@ -152,8 +154,7 @@
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
 msgstr ""
-
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 {
     "": "",
-    "Add": "\u0414\u043e\u0434\u0430\u0442\u0438",
+    "<i class=\\\"fas fa-plus-circle\\\"></i>\\n": "",
     "Cancel": "\u0421\u043a\u0430\u0441\u0443\u0432\u0430\u0442\u0438",
     "Command": "\u041a\u043e\u043c\u0430\u043d\u0434\u0430",
     "Comment": "\u041a\u043e\u043c\u0435\u043d\u0442\u0430\u0440",
     "Day (month)": "\u0414\u0435\u043d\u044c (\u043c\u0456\u0441\u044f\u0446\u044c)",
     "Day (week)": "\u0414\u0435\u043d\u044c (\u0442\u0438\u0436\u0434\u0435\u043d\u044c)",
     "Day of the month": "\u0414\u0435\u043d\u044c \u043c\u0456\u0441\u044f\u0446\u044f",
     "Day of the week": "\u0414\u0435\u043d\u044c \u0442\u0438\u0436\u043d\u044f",
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/uk/LC_MESSAGES/app.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,130 +1,131 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: ajenti\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
+"POT-Creation-Date: 2023-04-30 15:01+0200\n"
+"PO-Revision-Date: 2023-05-07 10:30\n"
 "Last-Translator: \n"
 "Language-Team: Ukrainian\n"
 "Language: uk_UA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=((n%10==1 && n%100!=11) ? 0 : ((n%10 >= 2 && n%10 <=4 && (n%100 < 12 || n%100 > 14)) ? 1 : ((n%10 == 0 || (n%10 >= 5 && n%10 <=9)) || (n%100 >= 11 && n%100 <= 14)) ? 2 : 3));\n"
 "X-Crowdin-Project: ajenti\n"
 "X-Crowdin-Project-ID: 18127\n"
 "X-Crowdin-Language: uk\n"
 "X-Crowdin-File: /2.0/cron.po\n"
 "X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
-msgstr "Додати"
-
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid "<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
+msgstr ""
+
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr "Скасувати"
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr "Команда"
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr "Коментар"
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr "День (місяць)"
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr "День (тиждень)"
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr "День місяця"
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr "День тижня"
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr "Змінні середовища"
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr "Година"
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr "Завдання"
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr "Хвилина"
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr "Змінити"
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr "Місяць"
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr "Ім’я"
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr "ОК"
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr "Зберегти"
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr "Спеціальні"
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr "Немає планувань"
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr "Немає спеціальних завдань."
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr "Немає набору змінних середовища."
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr "Значення"
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr "Планувальник"
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/locale/vi/LC_MESSAGES/app.po` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/locale/app.pot`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,132 @@
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: ajenti\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-09-06 13:09+0200\n"
-"PO-Revision-Date: 2022-06-25 19:27\n"
-"Last-Translator: \n"
-"Language-Team: Vietnamese\n"
-"Language: vi_VN\n"
+"POT-Creation-Date: 2023-05-07 11:53+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Crowdin-Project: ajenti\n"
-"X-Crowdin-Project-ID: 18127\n"
-"X-Crowdin-Language: vi\n"
-"X-Crowdin-File: /2.0/cron.po\n"
-"X-Crowdin-File-ID: 60\n"
 
 #: plugins/cron/resources/partial/index.html:38
-#: plugins/cron/resources/partial/index.html:65
-#: plugins/cron/resources/partial/index.html:92
-msgid "Add"
+#: plugins/cron/resources/partial/index.html:68
+#: plugins/cron/resources/partial/index.html:98
+msgid ""
+"<i class=\"fas fa-plus-circle\"></i>\n"
+"                Add"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:129
-#: plugins/cron/resources/partial/index.html:145
-#: plugins/cron/resources/partial/index.html:161
+#: plugins/cron/resources/partial/index.html:138
+#: plugins/cron/resources/partial/index.html:154
+#: plugins/cron/resources/partial/index.html:170
 #: plugins/cron/resources/js/controllers/index.controller.es:47
 msgid "Cancel"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:121
-#: plugins/cron/resources/partial/index.html:137
+#: plugins/cron/resources/partial/index.html:130
+#: plugins/cron/resources/partial/index.html:146
 #: plugins/cron/resources/partial/index.html:15
-#: plugins/cron/resources/partial/index.html:46
+#: plugins/cron/resources/partial/index.html:49
 msgid "Command"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:125
-#: plugins/cron/resources/partial/index.html:141
-#: plugins/cron/resources/partial/index.html:157
+#: plugins/cron/resources/partial/index.html:134
+#: plugins/cron/resources/partial/index.html:150
+#: plugins/cron/resources/partial/index.html:166
 msgid "Comment"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:12
 msgid "Day (month)"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:14
 msgid "Day (week)"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:109
+#: plugins/cron/resources/partial/index.html:118
 msgid "Day of the month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:117
+#: plugins/cron/resources/partial/index.html:126
 msgid "Day of the week"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:67
+#: plugins/cron/resources/partial/index.html:73
 msgid "Environment variables"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:105
 #: plugins/cron/resources/partial/index.html:11
+#: plugins/cron/resources/partial/index.html:114
 msgid "Hour"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:5
 msgid "Jobs"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:10
-#: plugins/cron/resources/partial/index.html:101
+#: plugins/cron/resources/partial/index.html:110
 msgid "Minute"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:97
+#: plugins/cron/resources/partial/index.html:106
 msgid "Modify"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:113
+#: plugins/cron/resources/partial/index.html:122
 #: plugins/cron/resources/partial/index.html:13
 msgid "Month"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:149
-#: plugins/cron/resources/partial/index.html:72
+#: plugins/cron/resources/partial/index.html:158
+#: plugins/cron/resources/partial/index.html:78
 msgid "Name"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:130
-#: plugins/cron/resources/partial/index.html:146
-#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:139
+#: plugins/cron/resources/partial/index.html:155
+#: plugins/cron/resources/partial/index.html:171
 msgid "OK"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:167
+#: plugins/cron/resources/partial/index.html:176
 msgid "Save"
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:133
-#: plugins/cron/resources/partial/index.html:40
-#: plugins/cron/resources/partial/index.html:45
+#: plugins/cron/resources/partial/index.html:142
+#: plugins/cron/resources/partial/index.html:43
+#: plugins/cron/resources/partial/index.html:48
 msgid "Special"
 msgstr ""
 
 #: plugins/cron/resources/partial/index.html:7
 msgid "There is no cronjob."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:42
+#: plugins/cron/resources/partial/index.html:45
 msgid "There is no special task."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:69
+#: plugins/cron/resources/partial/index.html:75
 msgid "There is no variables environment set."
 msgstr ""
 
-#: plugins/cron/resources/partial/index.html:153
-#: plugins/cron/resources/partial/index.html:73
+#: plugins/cron/resources/partial/index.html:162
+#: plugins/cron/resources/partial/index.html:79
 msgid "Value"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:2
 #: plugins/cron/resources/js/controllers/index.controller.es:4
 msgid "Cron"
 msgstr ""
@@ -152,8 +154,7 @@
 #: plugins/cron/resources/js/controllers/index.controller.es:76
 msgid "Crontab successfully saved !"
 msgstr ""
 
 #: plugins/cron/resources/js/controllers/index.controller.es:79
 msgid "Failed to save crontab"
 msgstr ""
-
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/manager.py` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/manager.py`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/build/all.js` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/build/all.js`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/js/controllers/index.controller.es` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/js/controllers/index.controller.es`

 * *Files identical despite different names*

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/resources/partial/index.html` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/resources/partial/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,18 @@
                     <td style="width:1px;">
                         <button class="btn btn-default" ng:click="remove('normal_tasks', job)" title="Remove">
                                 <i class="fa fa-trash-o"></i>
                         </button>
                     </td>
                 </tr>
             </table>
-            <button class="btn btn-default" ng:click="add('normal_tasks')" translate>Add</button>
+            <button class="btn btn-default" ng:click="add('normal_tasks')" translate>
+                <i class="fas fa-plus-circle"></i>
+                Add
+            </button>
         </uib:tab>
         <uib:tab heading="{{'Special'|translate}}">
             <br/>
             <div ng:show="crontab.special_tasks.length == 0" class="alert alert-info" translate>There is no special task.</div>
             <table ng:show="crontab.special_tasks.length > 0" class="table">
                 <tr>
                     <th translate>Special</th>
@@ -58,15 +61,18 @@
                     <td style="width:1px;">
                         <button class="btn btn-default" ng:click="remove('special_tasks', job)" title="Remove">
                                 <i class="fa fa-trash-o"></i>
                         </button>
                     </td>
                 </tr>
             </table>
-            <button class="btn btn-default" ng:click="add('special_tasks')" translate>Add</button>
+            <button class="btn btn-default" ng:click="add('special_tasks')" translate>
+                <i class="fas fa-plus-circle"></i>
+                Add
+            </button>
         </uib:tab>
         <uib:tab heading="{{'Environment variables'|translate}}">
             <br/>
             <div ng:show="crontab.env_settings.length == 0" class="alert alert-info" translate>There is no variables environment set.</div>
             <table ng:show="crontab.env_settings.length > 0" class="table">
                 <tr>
                     <th translate>Name</th>
@@ -85,15 +91,18 @@
                     <td style="width:1px;">
                         <button class="btn btn-default" ng:click="remove('env_settings', var)" title="Remove">
                                 <i class="fa fa-trash-o"></i>
                         </button>
                     </td>
                 </tr>
             </table>
-            <button class="btn btn-default" ng:click="add('env_settings')" translate>Add</button>
+            <button class="btn btn-default" ng:click="add('env_settings')" translate>
+                <i class="fas fa-plus-circle"></i>
+                Add
+            </button>
         </uib:tab>
     </uib:tabset>
     <dialog ng:show="modifyJob">
         <div class="modal-header">
             <h4><span translate>Modify</span> {{translate[modifyJob.type]}}</h4>
         </div>
         <div class="modal-body scrollable">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 
 
 There is no cronjob.
 Minute        Hour        Day (month)         Month        Day (week)         Command
 {             {           {                   {            {                  {
 {job.minute}} {job.hour}} {job.day_of_month}} {job.month}} {job.day_of_week}} {job.command}}
-Add
+  Add
 There is no special task.
 Special         Command
 {{job.special}} {{job.command}}
-Add
+  Add
 There is no variables environment set.
 Name         Value
 {{var.name}} {{var.value}}
-Add
+  Add
 *** Modify {{translate[modifyJob.type]}} ***
 Minute
 [
 ]
 Hour
 [
 ]
```

### Comparing `ajenti.plugin.cron-0.5/ajenti_plugin_cron/views.py` & `ajenti.plugin.cron-0.6/ajenti_plugin_cron/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     @endpoint(api=True)
     def handle_api_save_crontab(self, http_context):
         """
         Store cron data from frontend in a cron file through CronManager.
 
         :param http_context: HttpContext
         :type http_context: HttpContext
-        :return: True if successfull
+        :return: True if successful
         :rtype: bool
         """
 
         def setTask(obj, values):
             for k,v in values.items():
                 setattr(obj, k, v)
             return obj
```

### Comparing `ajenti.plugin.cron-0.5/setup.py` & `ajenti.plugin.cron-0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 
 __requires = [dep.split('#')[0].strip() for dep in filter(None, open('requirements.txt').read().splitlines())] 
 
 setup(
     name='ajenti.plugin.cron',
-    version='0.5',
+    version='0.6',
     python_requires='>=3',
     install_requires=__requires,
     description='Cron',
     long_description='A Cron plugin for Ajenti panel',
     author='Arnaud Kientz',
     author_email='arnaud@linuxmuster.net',
     url='https://ajenti.org',
```

