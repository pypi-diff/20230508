# Comparing `tmp/pineboo-1.0.4.4.tar.gz` & `tmp/pineboo-1.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pineboo-1.0.4.4.tar", last modified: Mon May  8 08:45:18 2023, max compression
+gzip compressed data, was "pineboo-1.0.4.5.tar", last modified: Mon May  8 09:15:03 2023, max compression
```

## Comparing `pineboo-1.0.4.4.tar` & `pineboo-1.0.4.5.tar`

### file list

```diff
@@ -1,736 +1,736 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.397082 pineboo-1.0.4.4/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1078 2019-07-27 10:21:43.000000 pineboo-1.0.4.4/LICENSE.mit
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-05-08 08:45:18.397082 pineboo-1.0.4.4/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4673 2023-04-04 09:45:23.000000 pineboo-1.0.4.4/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.285078 pineboo-1.0.4.4/pineboo.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-05-08 08:45:18.000000 pineboo-1.0.4.4/pineboo.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28782 2023-05-08 08:45:18.000000 pineboo-1.0.4.4/pineboo.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-08 08:45:18.000000 pineboo-1.0.4.4/pineboo.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      386 2023-05-08 08:45:18.000000 pineboo-1.0.4.4/pineboo.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      584 2023-05-08 08:45:18.000000 pineboo-1.0.4.4/pineboo.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-08 08:45:18.000000 pineboo-1.0.4.4/pineboo.egg-info/top_level.txt
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.285078 pineboo-1.0.4.4/pineboolib/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      179 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.285078 pineboo-1.0.4.4/pineboolib/application/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1515 2023-05-08 08:43:34.000000 pineboo-1.0.4.4/pineboolib/application/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.285078 pineboo-1.0.4.4/pineboolib/application/acls/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       20 2019-09-08 08:23:19.000000 pineboo-1.0.4.4/pineboolib/application/acls/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9234 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/acls/pnaccesscontrol.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7411 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/acls/pnaccesscontrolfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9900 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/acls/pnaccesscontrollists.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1554 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/acls/pnboolflagstate.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.285078 pineboo-1.0.4.4/pineboolib/application/acls/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      269 2020-08-26 10:35:25.000000 pineboo-1.0.4.4/pineboolib/application/acls/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24411 2023-05-01 19:58:35.000000 pineboo-1.0.4.4/pineboolib/application/acls/tests/test_acls.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      970 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/acls/tests/test_pnaccesscontrol.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9013 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/connections.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.289078 pineboo-1.0.4.4/pineboolib/application/database/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      210 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.289078 pineboo-1.0.4.4/pineboolib/application/database/orm/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       43 2020-05-06 20:13:13.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5021 2022-06-12 18:52:01.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/alembic_tools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    38000 2023-05-01 19:58:35.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/basemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6348 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/dummy_cursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1083 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/dummy_signal.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.293078 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-06-24 11:26:48.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12845 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_basemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2510 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_bytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4361 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_consistency.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3575 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_dummycursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4074 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_query_orm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4354 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_relationships.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5465 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_sessions.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4746 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_signals.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2524 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_thread_session.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1736 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1080 2020-10-15 10:56:54.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_view.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10720 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/orm/utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8355 2023-04-30 08:30:37.000000 pineboo-1.0.4.4/pineboolib/application/database/pnbuffer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22022 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/pnconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17300 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/pnconnectionmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    40279 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/pncursortablemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2020-06-29 10:01:24.000000 pineboo-1.0.4.4/pineboolib/application/database/pngroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2020-01-10 07:21:12.000000 pineboo-1.0.4.4/pineboolib/application/database/pnparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1340 2021-03-09 11:41:24.000000 pineboo-1.0.4.4/pineboolib/application/database/pnsignals.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   122196 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/pnsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5770 2023-04-18 17:17:33.000000 pineboo-1.0.4.4/pineboolib/application/database/pnsqldriversmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    30551 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/pnsqlquery.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.293078 pineboo-1.0.4.4/pineboolib/application/database/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-12-02 11:03:25.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5986 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnbuffer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8510 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4011 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnconnection_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8048 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pncursortablemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      413 2019-08-28 09:29:35.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pngroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      600 2019-08-28 09:29:35.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    42304 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1170 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnsqldriversmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28221 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3072 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15831 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/database/utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1475 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/file.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11435 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/load_script.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/metadata/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2019-07-30 14:11:28.000000 pineboo-1.0.4.4/pineboolib/application/metadata/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4940 2021-01-20 09:16:39.000000 pineboo-1.0.4.4/pineboolib/application/metadata/pnaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/metadata/pncompoundkeymetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    33263 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/metadata/pnfieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7344 2021-08-22 09:38:16.000000 pineboo-1.0.4.4/pineboolib/application/metadata/pnrelationmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25771 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/metadata/pntablemetadata.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/metadata/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-03 08:33:48.000000 pineboo-1.0.4.4/pineboolib/application/metadata/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1217 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pnaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2311 2020-02-05 09:39:18.000000 pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16137 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pnfieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4190 2021-08-23 10:27:07.000000 pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pnrelationmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7444 2021-01-21 09:59:47.000000 pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pntablemetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2862 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/module.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4141 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/moduleactions.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       47 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/modules_tree.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      122 2019-07-31 07:36:22.000000 pineboo-1.0.4.4/pineboolib/application/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10703 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/packager/pnpackager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1947 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/packager/pnunpacker.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/packager/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-01-21 10:44:31.000000 pineboo-1.0.4.4/pineboolib/application/packager/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1763 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/packager/tests/test_pnpackager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1519 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/packager/tests/test_pnunpaker.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/parsers/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       70 2019-07-29 14:08:13.000000 pineboo-1.0.4.4/pineboolib/application/parsers/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       56 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14822 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/kparsertools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    43978 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/kut2fpdf.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      291 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10578 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       50 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14324 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/pnmtdparser.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5405 2023-05-01 19:58:35.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.297078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1885 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-05-04 11:53:39.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      587 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/flex.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31580 2023-04-28 10:51:35.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/flscriptparse.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3400 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/lextab.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28374 2023-05-01 18:19:35.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/postparse.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8675 2023-05-01 18:19:35.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/pyconvert.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    91798 2023-05-04 11:53:36.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/pytnyzer.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      502 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16732 2023-05-01 18:19:35.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6174 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/token_rules.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      101 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    49421 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/qt3ui.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       33 2020-04-23 09:34:52.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    34668 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/pnapplication.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      371 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/pncore.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/process.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26642 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/projectmodule.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2021-03-30 10:58:34.000000 pineboo-1.0.4.4/pineboolib/application/proxy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6876 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/qsadictmodules.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/qsatypes/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-08-01 20:49:12.000000 pineboo-1.0.4.4/pineboolib/application/qsatypes/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7965 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/qsatypes/date.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20094 2023-05-01 19:58:35.000000 pineboo-1.0.4.4/pineboolib/application/qsatypes/sysbasetype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/qsatypes/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-06 06:55:22.000000 pineboo-1.0.4.4/pineboolib/application/qsatypes/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1853 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/qsatypes/tests/test_date.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5455 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/qsatypes/tests/test_sysbasetype.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3461 2021-03-29 11:28:24.000000 pineboo-1.0.4.4/pineboolib/application/safeqsa.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/signatures/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-12-25 17:46:05.000000 pineboo-1.0.4.4/pineboolib/application/signatures/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6312 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/signatures/pdf_digest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8187 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/signatures/pdf_qr.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/signatures/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      286 2021-01-18 11:51:09.000000 pineboo-1.0.4.4/pineboolib/application/signatures/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3440 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/signatures/tests/test_signatures.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9298 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/signatures/xml_digest.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/staticloader/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-10-04 20:53:14.000000 pineboo-1.0.4.4/pineboolib/application/staticloader/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14695 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/staticloader/pnmodulesstaticloader.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/staticloader/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      289 2020-09-07 08:35:55.000000 pineboo-1.0.4.4/pineboolib/application/staticloader/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2491 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/staticloader/tests/test_static_loader.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.301078 pineboo-1.0.4.4/pineboolib/application/staticloader/ui/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-08-17 12:14:19.000000 pineboo-1.0.4.4/pineboolib/application/staticloader/ui/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7299 2020-03-10 09:40:23.000000 pineboo-1.0.4.4/pineboolib/application/staticloader/ui/static_loader.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.305079 pineboo-1.0.4.4/pineboolib/application/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      287 2019-10-09 06:29:09.000000 pineboo-1.0.4.4/pineboolib/application/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2020-06-10 19:38:58.000000 pineboo-1.0.4.4/pineboolib/application/tests/test_application.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1350 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/tests/test_load_script.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1309 2020-09-21 07:02:30.000000 pineboo-1.0.4.4/pineboolib/application/tests/test_process.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1259 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/tests/test_projectmodule.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2020-09-04 08:27:19.000000 pineboo-1.0.4.4/pineboolib/application/tests/test_proxy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16925 2023-04-07 15:43:24.000000 pineboo-1.0.4.4/pineboolib/application/tests/test_types.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1319 2020-09-07 08:35:55.000000 pineboo-1.0.4.4/pineboolib/application/tests/test_xmlaction.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.305079 pineboo-1.0.4.4/pineboolib/application/translator/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-04-05 08:54:23.000000 pineboo-1.0.4.4/pineboolib/application/translator/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5405 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/translator/pntranslator.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.305079 pineboo-1.0.4.4/pineboolib/application/translator/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       34 2020-12-01 12:01:44.000000 pineboo-1.0.4.4/pineboolib/application/translator/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      802 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/translator/test/test_pntranslator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22047 2023-04-09 14:08:33.000000 pineboo-1.0.4.4/pineboolib/application/types.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.305079 pineboo-1.0.4.4/pineboolib/application/utils/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      182 2019-07-31 08:47:54.000000 pineboo-1.0.4.4/pineboolib/application/utils/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1548 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/utils/check_dependencies.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2245 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/utils/convert_flaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/utils/date_conversion.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6310 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/utils/flfiles_dir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1120 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/utils/geometry.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1949 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/utils/mobilemode.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2258 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/application/utils/modules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1626 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/utils/path.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4727 2020-11-25 10:48:38.000000 pineboo-1.0.4.4/pineboolib/application/utils/service.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23030 2023-05-01 19:58:35.000000 pineboo-1.0.4.4/pineboolib/application/utils/sql_tools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1307 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/utils/xpm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15051 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/application/xmlaction.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.309079 pineboo-1.0.4.4/pineboolib/core/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      268 2021-03-29 11:28:24.000000 pineboo-1.0.4.4/pineboolib/core/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8761 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/decorators.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      746 2020-10-16 07:17:25.000000 pineboo-1.0.4.4/pineboolib/core/exceptions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.309079 pineboo-1.0.4.4/pineboolib/core/fonts/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/core/fonts/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.309079 pineboo-1.0.4.4/pineboolib/core/fonts/noto_sans/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-03-09 09:55:39.000000 pineboo-1.0.4.4/pineboolib/core/fonts/noto_sans/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2578 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/garbage_collector.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.309079 pineboo-1.0.4.4/pineboolib/core/images/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/core/images/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.325079 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      960 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Pi-symbol.svg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)  1464366 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi.psd
--rw-rw-r--   0 aulla     (1000) aulla     (1000)  9487782 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2.xcf
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   476635 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50853 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2_256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   147180 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2_512.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50737 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi_1024.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi_256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29321 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi_512.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/core/images/icono_pi/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.341080 pineboo-1.0.4.4/pineboolib/core/images/icons/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/__init__.py
--rwxrwxr-x   0 aulla     (1000) aulla     (1000)      892 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/about.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1230 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/aboutqt.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      853 2019-10-01 07:14:24.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/cancel.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/consola.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      669 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/date.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2199 2019-09-30 08:28:48.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/delete.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2562 2019-10-01 07:14:24.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2069 2019-09-30 08:28:48.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/edit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2237 2020-01-15 08:29:51.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/edit_file.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2020-01-15 08:29:51.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/edit_file_xml.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      934 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/estilo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      870 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/exit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/flfielddb.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      691 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/fltable-clean.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/fltable-data.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/fltable-filter.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      727 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/fltable-odf.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      459 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/folder.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      615 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/folder_update.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      563 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/font.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-bottom.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-first.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-home.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-jump.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-last.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-next.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-previous.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-top.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/go-up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      601 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-add.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1624 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-bold.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-cancel.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1682 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-clear.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      723 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-copy.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-cut.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2049 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-delete.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2104 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-find-and-replace.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1636 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-find.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1256 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-fullscreen.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-back-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-back-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-forward-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-forward-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-bottom.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-first-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-first-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-last-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-last-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-top.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-home.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-indent-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-indent-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1338 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-italic.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-jump-to-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-jump-to-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-center.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      517 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-fill.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      515 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-left.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-right.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-forward-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-forward-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-next-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-next-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      481 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-pause.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1028 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-play-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-previous-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-previous-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1266 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-record.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-rewind-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-rewind-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-stop.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1008 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-new.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-open.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1027 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-paste.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1719 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-print-preview.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1013 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-print.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1115 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-properties.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1502 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-redo-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-refresh.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      317 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-remove.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1837 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-save-as.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1971 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-save.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      631 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-select-all.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-stop.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1445 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-strikethrough.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-underline.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1601 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-undo-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-unindent-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-unindent-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      911 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/help_index.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1854 2019-09-30 08:28:48.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/insert.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      711 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/lock.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      579 2019-10-01 07:14:24.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/ok.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1997 2019-09-30 08:28:48.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/paste.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-128.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      857 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-16.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1406 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-24.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1941 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-32.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2991 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-48.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3482 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-57.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3243 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-64.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-72.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19949 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-128.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1216 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-16.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1720 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-24.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    52103 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2568 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-32.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4552 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-48.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7028 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-64.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17588 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-09-30 08:28:48.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/print.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      885 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/reload.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22869 2022-07-06 21:01:18.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/signed_stamp.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1930 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_ebcomportamiento.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1571 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flareas.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2952 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_fldumpdb.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1133 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flgroups.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1871 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flloadmod.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2404 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flloadmodpkg.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1335 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flmodules.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2010 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flmrproper.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2334 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flreinit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2771 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flreloadbatch.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flreloadlast.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2194 2019-10-02 12:19:59.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flusers.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    35029 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/terminal.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      638 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/unlock.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2635 2019-10-01 07:14:24.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2019-09-30 08:28:48.000000 pineboo-1.0.4.4/pineboolib/core/images/icons/zoom.png
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.341080 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    72306 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/dbadmin240.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   187209 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/dbadmin480.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    71281 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/quick240.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   185547 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/quick480.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       52 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/readme
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    66162 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/splash.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   109093 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/core/images/splashscreen/splash.svg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1150 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/message_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      426 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/system.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.341080 pineboo-1.0.4.4/pineboolib/core/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-09-21 07:02:47.000000 pineboo-1.0.4.4/pineboolib/core/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1215 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/test/test_settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      211 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/translate.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.345080 pineboo-1.0.4.4/pineboolib/core/utils/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      114 2019-07-28 13:56:09.000000 pineboo-1.0.4.4/pineboolib/core/utils/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3203 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/core/utils/check_dependencies.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3140 2020-03-10 08:41:03.000000 pineboo-1.0.4.4/pineboolib/core/utils/logging.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      540 2019-07-28 13:56:09.000000 pineboo-1.0.4.4/pineboolib/core/utils/singleton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3720 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/core/utils/struct.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.345080 pineboo-1.0.4.4/pineboolib/core/utils/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       46 2019-08-04 20:13:49.000000 pineboo-1.0.4.4/pineboolib/core/utils/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2331 2020-03-09 12:29:25.000000 pineboo-1.0.4.4/pineboolib/core/utils/tests/test_utils_base.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1819 2020-09-21 06:32:29.000000 pineboo-1.0.4.4/pineboolib/core/utils/tests/test_version.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15945 2023-04-19 12:18:00.000000 pineboo-1.0.4.4/pineboolib/core/utils/utils_base.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4686 2021-03-08 21:10:30.000000 pineboo-1.0.4.4/pineboolib/core/utils/version.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.349080 pineboo-1.0.4.4/pineboolib/fllegacy/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      111 2019-07-31 21:01:09.000000 pineboo-1.0.4.4/pineboolib/fllegacy/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.349080 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       77 2019-07-31 16:14:18.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      349 2019-11-28 09:34:37.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqboolflagstate.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      580 2020-11-10 11:32:00.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqformdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13444 2022-07-05 09:51:12.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqods.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      521 2020-03-09 11:54:38.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2019-07-31 20:16:08.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsettings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      337 2019-11-18 12:56:58.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqshttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsignalmapper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      241 2019-07-31 20:16:08.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsmtpclient.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1531 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18185 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      273 2019-11-28 09:34:37.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      255 2019-07-31 20:16:08.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      734 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqssproject.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      343 2020-09-14 10:30:41.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqutil.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.349080 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-29 15:57:47.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1300 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1201 2020-12-01 12:01:57.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1907 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      554 2020-04-21 15:32:44.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1194 2020-08-07 17:51:40.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      953 2020-02-11 09:11:31.000000 pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      358 2019-09-19 09:51:37.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      171 2020-04-02 16:10:18.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flapplication.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      446 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flcheckbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12411 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flcodbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29167 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fldatatable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fldateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2319 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fldoublevalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2020-08-24 08:14:25.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flfastcgi.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   143143 2023-05-08 08:40:13.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31497 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flformdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    34481 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flformrecorddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14097 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flformsearchdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      185 2019-08-01 06:59:07.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flgroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1361 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flintvalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fljasperengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      103 2020-08-19 14:34:59.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fljasperviewer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5497 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fllineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3892 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fllistviewitem.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    52856 2023-04-19 12:33:57.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28979 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flmanagermodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4403 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flnetwork.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      196 2019-08-17 07:43:18.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4300 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flpixmapview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3702 2020-08-24 09:53:53.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flposprinter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13824 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flreportengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22476 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flreportviewer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      403 2019-11-14 09:39:09.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flscripteditor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5273 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flserialport.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1620 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flsettings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13515 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flsmtpclient.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      895 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flspinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      267 2020-03-05 11:36:30.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flsqlconnections.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2019-08-17 07:43:18.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2019-08-17 07:43:18.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fltable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   108501 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      875 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fltimeedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1092 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/fluintvalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    41598 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1876 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flvar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      549 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      315 2019-08-13 07:00:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/flworkspace.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.349080 pineboo-1.0.4.4/pineboolib/fllegacy/forms/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    48049 2020-12-24 07:51:30.000000 pineboo-1.0.4.4/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       67 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/forms/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67146 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/systype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.353080 pineboo-1.0.4.4/pineboolib/fllegacy/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2019-12-02 11:03:25.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1455 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flcodbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1664 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_fldatatable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      991 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_fldateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8825 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      939 2020-09-21 06:32:29.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flform.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2286 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flformrecorddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3065 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flformsearch.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2289 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      902 2020-12-22 09:37:36.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flreportengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12536 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8666 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1592 2020-09-01 07:21:14.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-09-01 07:21:14.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_smtp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8560 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_systype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.357080 pineboo-1.0.4.4/pineboolib/interfaces/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      331 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/interfaces/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      172 2019-07-31 18:05:01.000000 pineboo-1.0.4.4/pineboolib/interfaces/cursoraccessmode.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      228 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/interfaces/dgi_schema.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10886 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/interfaces/iconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5925 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/interfaces/ifieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2999 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/interfaces/imainwindow.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5542 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/interfaces/imanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/interfaces/isession.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    21668 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/interfaces/isqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50296 2023-05-08 08:42:41.000000 pineboo-1.0.4.4/pineboolib/interfaces/isqldriver.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3292 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/interfaces/itablemetadata.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.357080 pineboo-1.0.4.4/pineboolib/loader/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       92 2019-08-04 07:50:46.000000 pineboo-1.0.4.4/pineboolib/loader/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/connection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1546 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/dgi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.357080 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      104 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      716 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/conn_dialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15802 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/dlgconnect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24027 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/dlgconnect.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.357080 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       57 2020-12-02 18:09:30.000000 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2544 2020-11-09 16:02:09.000000 pineboo-1.0.4.4/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2870 2023-04-20 16:01:15.000000 pineboo-1.0.4.4/pineboolib/loader/init_project.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18283 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/loader/main.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5772 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/loader/options.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1311 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/preload.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17570 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/projectconfig.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.357080 pineboo-1.0.4.4/pineboolib/loader/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      477 2019-08-05 15:23:25.000000 pineboo-1.0.4.4/pineboolib/loader/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2495 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/tests/test_connection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      827 2021-03-08 11:35:13.000000 pineboo-1.0.4.4/pineboolib/loader/tests/test_main.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/tests/test_projectconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3682 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/loader/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.357080 pineboo-1.0.4.4/pineboolib/plugins/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       23 2019-08-18 15:38:56.000000 pineboo-1.0.4.4/pineboolib/plugins/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/custom_widgets/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      282 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/custom_widgets/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/custom_widgets/flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/custom_widgets/fltable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/custom_widgets/fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/custom_widgets/pncore.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/dgi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       19 2019-08-18 15:38:56.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_fcgi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-08-18 15:38:56.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_fcgi/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2848 2020-03-24 12:23:10.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-18 15:38:56.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2019-08-18 15:38:56.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-08-18 15:38:56.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2014 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9496 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2190 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1452 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      604 2020-04-02 16:10:18.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4643 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5507 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_schema.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/mainform/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      177 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       78 2019-07-30 09:20:57.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55893 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/eneboo.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4184 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/mainform.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.361081 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-11-04 08:30:07.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5085 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.365081 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       82 2019-07-30 09:20:57.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    49501 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1500 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.365081 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      280 2019-11-04 08:30:07.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3263 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.365081 pineboo-1.0.4.4/pineboolib/plugins/sql/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-18 13:55:56.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      483 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/flmysql_innodb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12024 2023-04-19 12:33:54.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/flmysql_myisam.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11877 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/flpymssql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      825 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/flpyodbc.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13367 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/flqpsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11393 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/flsqlite.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.365081 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       31 2020-09-17 10:11:16.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2172 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flmysql_innodb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2958 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flmysql_myisam.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2861 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flpymssql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flpyodbc.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4517 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flsqlite.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2095 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_qpsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9177 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_stress.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2019-07-27 10:21:43.000000 pineboo-1.0.4.4/pineboolib/py.typed
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.373081 pineboo-1.0.4.4/pineboolib/q3widgets/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       94 2019-09-27 15:43:59.000000 pineboo-1.0.4.4/pineboolib/q3widgets/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1761 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/checkbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      142 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/combobox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1398 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/dateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3877 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/dialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1634 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/filedialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      482 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/groupbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      118 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/line.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1061 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/lineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3570 2023-04-28 10:51:28.000000 pineboo-1.0.4.4/pineboolib/q3widgets/messagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2758 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/numberedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      443 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/picture.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      134 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/pixmap.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1109 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      887 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1541 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qbytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      774 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qcheckbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2176 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qcombobox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qdataview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2262 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qdateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      147 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qdatetime.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1663 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qdialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      237 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      316 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qeventloop.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1138 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qframe.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3328 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qgroupbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      656 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qhboxlayout.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qhbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17321 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qhttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      231 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qiconset.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2061 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qlabel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      144 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qlayoutwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1099 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qline.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1767 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qlineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5684 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qlistview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      173 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qlistviewwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      445 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qmainwindow.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      137 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qmenu.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qmessagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1668 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qobject.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qpopupmenu.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3111 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qpushbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1975 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qradiobutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      149 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qspinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12608 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qtable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1741 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qtabwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2013 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qtextedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      463 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qtextstream.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      926 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qtimeedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      404 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qtoolbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2255 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qtoolbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      654 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qvboxlayout.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qvbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1231 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/qwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      184 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/radiobutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/rect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/size.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/spinbox.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.377081 pineboo-1.0.4.4/pineboolib/q3widgets/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      278 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2019-12-19 10:11:59.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_dateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1411 2020-12-02 18:08:18.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_messagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qbytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2638 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qhttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      719 2019-09-27 15:43:59.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qpushbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1163 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qradiobuttons.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1131 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qtabwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1046 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qtextstream.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      532 2020-09-21 08:32:33.000000 pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_spinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/textedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/q3widgets/timeedit.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.377081 pineboo-1.0.4.4/pineboolib/qsa/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       95 2019-08-02 07:28:39.000000 pineboo-1.0.4.4/pineboolib/qsa/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5934 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/qsa/decorators.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1321 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/emptyscript.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7457 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/formdbwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2035 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/input.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1439 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/object_class.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11935 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/pncontrolsfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8336 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/qsa.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.377081 pineboo-1.0.4.4/pineboolib/qsa/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      496 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      744 2020-06-22 11:35:54.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/test_class.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4169 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/test_classes.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17795 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/test_knownbugs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6680 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/test_orm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1563 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/test_query_values.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1716 2023-05-01 18:19:33.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/test_require.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7893 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/qsa/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20373 2023-05-01 18:19:35.000000 pineboo-1.0.4.4/pineboolib/qsa/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.377081 pineboo-1.0.4.4/pineboolib/system_module/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/system_module/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.381081 pineboo-1.0.4.4/pineboolib/system_module/forms/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9153 2019-09-30 08:28:05.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/FLWidgetMasterTable.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28933 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/ebcomportamiento.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1368 2019-10-01 07:14:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/flareas.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2994 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/flfiles.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8007 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/flgroups.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16760 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/flmodulos.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3150 2020-07-06 10:29:58.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/fltest.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1214 2019-10-01 07:14:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/flusers.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8877 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/master.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10189 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/master_copy.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9932 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/master_print.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11619 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/master_print_copy.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11760 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/forms/sys.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.381081 pineboo-1.0.4.4/pineboolib/system_module/models/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2020-04-27 09:01:43.000000 pineboo-1.0.4.4/pineboolib/system_module/models/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1441 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flareas_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3270 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flfiles_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1238 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flgroups_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/fllarge_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1313 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flmetadata_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3296 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flmodules_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1292 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flseqs_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1007 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flserial_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1023 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flsettings_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2369 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/fltest2_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1769 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/models/fltest3_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1859 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/fltest4_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2296 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/models/fltest5_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2659 2020-10-13 15:24:00.000000 pineboo-1.0.4.4/pineboolib/system_module/models/fltest_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3548 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flupdates_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1450 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flusers_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1718 2020-07-16 10:23:10.000000 pineboo-1.0.4.4/pineboolib/system_module/models/flvar_model.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.381081 pineboo-1.0.4.4/pineboolib/system_module/queries/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/system_module/queries/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      636 2020-10-15 10:53:48.000000 pineboo-1.0.4.4/pineboolib/system_module/queries/fltest2.qry
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.385081 pineboo-1.0.4.4/pineboolib/system_module/scripts/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15186 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/ebcomportamiento.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      234 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/fldumpdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      859 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flfiles.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flloadmod.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      246 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flloadmodpkg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      427 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flmasterareas.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18788 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flmodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flmrproper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      238 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flreinit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3958 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flreloadbatch.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6038 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/flreloadlast.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/fltest6.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4351 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/sys.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.385081 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-03-26 18:29:13.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1104 2020-09-17 09:48:31.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2155 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flfiles.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2020-09-09 10:25:36.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4238 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flmodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      843 2020-09-09 10:25:36.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flmrproper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      851 2020-09-09 10:25:36.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flreinit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4322 2023-05-08 08:40:00.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_reload_last.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1564 2019-09-26 11:40:44.000000 pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_sys.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2411 2020-12-05 19:13:31.000000 pineboo-1.0.4.4/pineboolib/system_module/sys.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6505 2019-08-23 10:35:06.000000 pineboo-1.0.4.4/pineboolib/system_module/sys.xpm
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.397082 pineboo-1.0.4.4/pineboolib/system_module/translations/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-09-17 09:33:15.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 08:45:07.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.ca.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 08:45:09.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.de.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 08:45:05.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.en.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    68138 2023-05-08 08:45:03.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.es.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 08:45:11.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.fr.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 08:45:14.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.gl.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 08:45:16.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.it.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 08:45:18.000000 pineboo-1.0.4.4/pineboolib/system_module/translations/sys.pt.ts
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 08:45:18.397082 pineboo-1.0.4.4/pymodules/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2020-11-25 08:02:11.000000 pineboo-1.0.4.4/pymodules/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      283 2023-05-08 08:45:18.397082 pineboo-1.0.4.4/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4086 2023-04-04 09:45:24.000000 pineboo-1.0.4.4/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.707493 pineboo-1.0.4.5/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1078 2019-07-27 10:21:43.000000 pineboo-1.0.4.5/LICENSE.mit
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-05-08 09:15:03.707493 pineboo-1.0.4.5/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4673 2023-04-04 09:45:23.000000 pineboo-1.0.4.5/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.619489 pineboo-1.0.4.5/pineboo.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-05-08 09:15:03.000000 pineboo-1.0.4.5/pineboo.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28782 2023-05-08 09:15:03.000000 pineboo-1.0.4.5/pineboo.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-08 09:15:03.000000 pineboo-1.0.4.5/pineboo.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      386 2023-05-08 09:15:03.000000 pineboo-1.0.4.5/pineboo.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      584 2023-05-08 09:15:03.000000 pineboo-1.0.4.5/pineboo.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-08 09:15:03.000000 pineboo-1.0.4.5/pineboo.egg-info/top_level.txt
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.619489 pineboo-1.0.4.5/pineboolib/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      179 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.619489 pineboo-1.0.4.5/pineboolib/application/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1578 2023-05-08 09:14:26.000000 pineboo-1.0.4.5/pineboolib/application/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.623489 pineboo-1.0.4.5/pineboolib/application/acls/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       20 2019-09-08 08:23:19.000000 pineboo-1.0.4.5/pineboolib/application/acls/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9234 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/acls/pnaccesscontrol.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7411 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/acls/pnaccesscontrolfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9900 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/acls/pnaccesscontrollists.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1554 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/acls/pnboolflagstate.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.623489 pineboo-1.0.4.5/pineboolib/application/acls/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      269 2020-08-26 10:35:25.000000 pineboo-1.0.4.5/pineboolib/application/acls/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24411 2023-05-01 19:58:35.000000 pineboo-1.0.4.5/pineboolib/application/acls/tests/test_acls.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      970 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/acls/tests/test_pnaccesscontrol.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9013 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/connections.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.623489 pineboo-1.0.4.5/pineboolib/application/database/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      210 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.623489 pineboo-1.0.4.5/pineboolib/application/database/orm/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       43 2020-05-06 20:13:13.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5021 2022-06-12 18:52:01.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/alembic_tools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    38000 2023-05-01 19:58:35.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/basemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6348 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/dummy_cursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1083 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/dummy_signal.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.627490 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-06-24 11:26:48.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12845 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_basemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2510 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_bytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4361 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_consistency.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3575 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_dummycursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4074 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_query_orm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4354 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_relationships.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5465 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_sessions.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4746 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_signals.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2524 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_thread_session.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1736 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1080 2020-10-15 10:56:54.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_view.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10720 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/orm/utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8355 2023-04-30 08:30:37.000000 pineboo-1.0.4.5/pineboolib/application/database/pnbuffer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22022 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/pnconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17300 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/pnconnectionmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    40279 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/pncursortablemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2020-06-29 10:01:24.000000 pineboo-1.0.4.5/pineboolib/application/database/pngroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2020-01-10 07:21:12.000000 pineboo-1.0.4.5/pineboolib/application/database/pnparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1340 2021-03-09 11:41:24.000000 pineboo-1.0.4.5/pineboolib/application/database/pnsignals.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   122196 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/pnsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5770 2023-04-18 17:17:33.000000 pineboo-1.0.4.5/pineboolib/application/database/pnsqldriversmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    30551 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/pnsqlquery.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.627490 pineboo-1.0.4.5/pineboolib/application/database/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-12-02 11:03:25.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5986 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnbuffer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8510 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4011 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnconnection_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8048 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pncursortablemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      413 2019-08-28 09:29:35.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pngroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      600 2019-08-28 09:29:35.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    42304 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1170 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnsqldriversmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28221 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3072 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15831 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/database/utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1475 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/file.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11435 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/load_script.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.627490 pineboo-1.0.4.5/pineboolib/application/metadata/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2019-07-30 14:11:28.000000 pineboo-1.0.4.5/pineboolib/application/metadata/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4940 2021-01-20 09:16:39.000000 pineboo-1.0.4.5/pineboolib/application/metadata/pnaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/metadata/pncompoundkeymetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    33263 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/metadata/pnfieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7344 2021-08-22 09:38:16.000000 pineboo-1.0.4.5/pineboolib/application/metadata/pnrelationmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25771 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/metadata/pntablemetadata.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.627490 pineboo-1.0.4.5/pineboolib/application/metadata/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-03 08:33:48.000000 pineboo-1.0.4.5/pineboolib/application/metadata/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1217 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pnaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2311 2020-02-05 09:39:18.000000 pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16137 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pnfieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4190 2021-08-23 10:27:07.000000 pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pnrelationmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7444 2021-01-21 09:59:47.000000 pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pntablemetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2862 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/module.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4141 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/moduleactions.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       47 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/modules_tree.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.627490 pineboo-1.0.4.5/pineboolib/application/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      122 2019-07-31 07:36:22.000000 pineboo-1.0.4.5/pineboolib/application/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10703 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/packager/pnpackager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1947 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/packager/pnunpacker.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.627490 pineboo-1.0.4.5/pineboolib/application/packager/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-01-21 10:44:31.000000 pineboo-1.0.4.5/pineboolib/application/packager/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1763 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/packager/tests/test_pnpackager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1519 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/packager/tests/test_pnunpaker.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.627490 pineboo-1.0.4.5/pineboolib/application/parsers/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       70 2019-07-29 14:08:13.000000 pineboo-1.0.4.5/pineboolib/application/parsers/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       56 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14822 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/kparsertools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    43978 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/kut2fpdf.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      291 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10578 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       50 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14324 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/pnmtdparser.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5405 2023-05-01 19:58:35.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1885 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-05-04 11:53:39.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      587 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/flex.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31580 2023-04-28 10:51:35.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/flscriptparse.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3400 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/lextab.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28374 2023-05-01 18:19:35.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/postparse.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8675 2023-05-01 18:19:35.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/pyconvert.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    91788 2023-05-08 09:14:18.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/pytnyzer.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      502 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16732 2023-05-01 18:19:35.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6174 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/token_rules.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      101 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    49421 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/qt3ui.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       33 2020-04-23 09:34:52.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    34668 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/pnapplication.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      371 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/pncore.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/process.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26692 2023-05-08 09:05:01.000000 pineboo-1.0.4.5/pineboolib/application/projectmodule.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2021-03-30 10:58:34.000000 pineboo-1.0.4.5/pineboolib/application/proxy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6876 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/qsadictmodules.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/qsatypes/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-08-01 20:49:12.000000 pineboo-1.0.4.5/pineboolib/application/qsatypes/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7965 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/qsatypes/date.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20094 2023-05-01 19:58:35.000000 pineboo-1.0.4.5/pineboolib/application/qsatypes/sysbasetype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/qsatypes/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-06 06:55:22.000000 pineboo-1.0.4.5/pineboolib/application/qsatypes/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1853 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/qsatypes/tests/test_date.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5455 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/qsatypes/tests/test_sysbasetype.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3461 2021-03-29 11:28:24.000000 pineboo-1.0.4.5/pineboolib/application/safeqsa.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/signatures/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-12-25 17:46:05.000000 pineboo-1.0.4.5/pineboolib/application/signatures/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6312 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/signatures/pdf_digest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8187 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/signatures/pdf_qr.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/signatures/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      286 2021-01-18 11:51:09.000000 pineboo-1.0.4.5/pineboolib/application/signatures/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3440 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/signatures/tests/test_signatures.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9298 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/signatures/xml_digest.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/staticloader/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-10-04 20:53:14.000000 pineboo-1.0.4.5/pineboolib/application/staticloader/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14695 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/staticloader/pnmodulesstaticloader.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/staticloader/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      289 2020-09-07 08:35:55.000000 pineboo-1.0.4.5/pineboolib/application/staticloader/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2491 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/staticloader/tests/test_static_loader.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.631490 pineboo-1.0.4.5/pineboolib/application/staticloader/ui/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-08-17 12:14:19.000000 pineboo-1.0.4.5/pineboolib/application/staticloader/ui/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7299 2020-03-10 09:40:23.000000 pineboo-1.0.4.5/pineboolib/application/staticloader/ui/static_loader.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/application/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      287 2019-10-09 06:29:09.000000 pineboo-1.0.4.5/pineboolib/application/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2020-06-10 19:38:58.000000 pineboo-1.0.4.5/pineboolib/application/tests/test_application.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1350 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/tests/test_load_script.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1309 2020-09-21 07:02:30.000000 pineboo-1.0.4.5/pineboolib/application/tests/test_process.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1259 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/tests/test_projectmodule.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2020-09-04 08:27:19.000000 pineboo-1.0.4.5/pineboolib/application/tests/test_proxy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16925 2023-04-07 15:43:24.000000 pineboo-1.0.4.5/pineboolib/application/tests/test_types.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1319 2020-09-07 08:35:55.000000 pineboo-1.0.4.5/pineboolib/application/tests/test_xmlaction.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/application/translator/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-04-05 08:54:23.000000 pineboo-1.0.4.5/pineboolib/application/translator/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5405 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/translator/pntranslator.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/application/translator/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       34 2020-12-01 12:01:44.000000 pineboo-1.0.4.5/pineboolib/application/translator/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      802 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/translator/test/test_pntranslator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22047 2023-04-09 14:08:33.000000 pineboo-1.0.4.5/pineboolib/application/types.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/application/utils/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      182 2019-07-31 08:47:54.000000 pineboo-1.0.4.5/pineboolib/application/utils/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1548 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/utils/check_dependencies.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2245 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/utils/convert_flaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/utils/date_conversion.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6310 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/utils/flfiles_dir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1120 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/utils/geometry.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1949 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/utils/mobilemode.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2258 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/application/utils/modules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1626 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/utils/path.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4727 2020-11-25 10:48:38.000000 pineboo-1.0.4.5/pineboolib/application/utils/service.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    23030 2023-05-01 19:58:35.000000 pineboo-1.0.4.5/pineboolib/application/utils/sql_tools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1307 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/utils/xpm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15051 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/application/xmlaction.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/core/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      268 2021-03-29 11:28:24.000000 pineboo-1.0.4.5/pineboolib/core/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8761 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/decorators.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      746 2020-10-16 07:17:25.000000 pineboo-1.0.4.5/pineboolib/core/exceptions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/core/fonts/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/core/fonts/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/core/fonts/noto_sans/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-03-09 09:55:39.000000 pineboo-1.0.4.5/pineboolib/core/fonts/noto_sans/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2578 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/garbage_collector.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.635490 pineboo-1.0.4.5/pineboolib/core/images/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/core/images/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.647491 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      960 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Pi-symbol.svg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)  1464366 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi.psd
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)  9487782 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2.xcf
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   476635 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50853 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2_256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   147180 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2_512.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50737 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi_1024.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi_256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29321 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi_512.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/core/images/icono_pi/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.663491 pineboo-1.0.4.5/pineboolib/core/images/icons/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/__init__.py
+-rwxrwxr-x   0 aulla     (1000) aulla     (1000)      892 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/about.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1230 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/aboutqt.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      853 2019-10-01 07:14:24.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/cancel.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/consola.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      669 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/date.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2199 2019-09-30 08:28:48.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/delete.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2562 2019-10-01 07:14:24.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2069 2019-09-30 08:28:48.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/edit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2237 2020-01-15 08:29:51.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/edit_file.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2020-01-15 08:29:51.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/edit_file_xml.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      934 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/estilo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      870 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/exit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/flfielddb.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      691 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/fltable-clean.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/fltable-data.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/fltable-filter.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      727 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/fltable-odf.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      459 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/folder.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      615 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/folder_update.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      563 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/font.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-bottom.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-first.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-home.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-jump.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-last.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-next.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-previous.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-top.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/go-up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      601 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-add.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1624 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-bold.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-cancel.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1682 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-clear.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      723 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-copy.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-cut.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2049 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-delete.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2104 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-find-and-replace.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1636 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-find.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1256 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-fullscreen.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-back-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-back-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-forward-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-forward-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-bottom.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-first-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-first-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-last-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-last-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-top.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-home.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-indent-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-indent-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1338 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-italic.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-jump-to-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-jump-to-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-center.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      517 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-fill.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      515 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-left.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-right.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-forward-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-forward-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-next-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-next-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      481 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-pause.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1028 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-play-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-previous-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-previous-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1266 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-record.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-rewind-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-rewind-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-stop.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1008 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-new.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-open.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1027 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-paste.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1719 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-print-preview.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1013 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-print.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1115 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-properties.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1502 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-redo-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-refresh.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      317 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-remove.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1837 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-save-as.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1971 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-save.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      631 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-select-all.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-stop.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1445 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-strikethrough.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-underline.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1601 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-undo-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-unindent-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-unindent-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      911 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/help_index.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1854 2019-09-30 08:28:48.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/insert.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      711 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/lock.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      579 2019-10-01 07:14:24.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/ok.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1997 2019-09-30 08:28:48.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/paste.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-128.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      857 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-16.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1406 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-24.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1941 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-32.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2991 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-48.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3482 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-57.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3243 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-64.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-72.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19949 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-128.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1216 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-16.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1720 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-24.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    52103 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2568 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-32.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4552 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-48.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7028 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-64.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17588 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-09-30 08:28:48.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/print.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      885 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/reload.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22869 2022-07-06 21:01:18.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/signed_stamp.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1930 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_ebcomportamiento.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1571 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flareas.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2952 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_fldumpdb.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1133 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flgroups.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1871 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flloadmod.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2404 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flloadmodpkg.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1335 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flmodules.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2010 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flmrproper.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2334 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flreinit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2771 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flreloadbatch.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flreloadlast.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2194 2019-10-02 12:19:59.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flusers.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    35029 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/terminal.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      638 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/unlock.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2635 2019-10-01 07:14:24.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2019-09-30 08:28:48.000000 pineboo-1.0.4.5/pineboolib/core/images/icons/zoom.png
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.667492 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    72306 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/dbadmin240.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   187209 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/dbadmin480.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    71281 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/quick240.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   185547 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/quick480.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       52 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/readme
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    66162 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/splash.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   109093 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/core/images/splashscreen/splash.svg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1150 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/message_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      426 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/system.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.667492 pineboo-1.0.4.5/pineboolib/core/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-09-21 07:02:47.000000 pineboo-1.0.4.5/pineboolib/core/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1215 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/test/test_settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      211 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/translate.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.667492 pineboo-1.0.4.5/pineboolib/core/utils/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      114 2019-07-28 13:56:09.000000 pineboo-1.0.4.5/pineboolib/core/utils/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3203 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/core/utils/check_dependencies.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3140 2020-03-10 08:41:03.000000 pineboo-1.0.4.5/pineboolib/core/utils/logging.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      540 2019-07-28 13:56:09.000000 pineboo-1.0.4.5/pineboolib/core/utils/singleton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3720 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/core/utils/struct.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.667492 pineboo-1.0.4.5/pineboolib/core/utils/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       46 2019-08-04 20:13:49.000000 pineboo-1.0.4.5/pineboolib/core/utils/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2331 2020-03-09 12:29:25.000000 pineboo-1.0.4.5/pineboolib/core/utils/tests/test_utils_base.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1819 2020-09-21 06:32:29.000000 pineboo-1.0.4.5/pineboolib/core/utils/tests/test_version.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15945 2023-04-19 12:18:00.000000 pineboo-1.0.4.5/pineboolib/core/utils/utils_base.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4686 2021-03-08 21:10:30.000000 pineboo-1.0.4.5/pineboolib/core/utils/version.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.675492 pineboo-1.0.4.5/pineboolib/fllegacy/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      111 2019-07-31 21:01:09.000000 pineboo-1.0.4.5/pineboolib/fllegacy/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.675492 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       77 2019-07-31 16:14:18.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      349 2019-11-28 09:34:37.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqboolflagstate.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      580 2020-11-10 11:32:00.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqformdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13444 2022-07-05 09:51:12.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqods.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      521 2020-03-09 11:54:38.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2019-07-31 20:16:08.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsettings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      337 2019-11-18 12:56:58.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqshttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsignalmapper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      241 2019-07-31 20:16:08.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsmtpclient.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1531 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18185 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      273 2019-11-28 09:34:37.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      255 2019-07-31 20:16:08.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      734 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqssproject.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      343 2020-09-14 10:30:41.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqutil.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.675492 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-29 15:57:47.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1300 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1201 2020-12-01 12:01:57.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1907 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      554 2020-04-21 15:32:44.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1194 2020-08-07 17:51:40.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      953 2020-02-11 09:11:31.000000 pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      358 2019-09-19 09:51:37.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      171 2020-04-02 16:10:18.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flapplication.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      446 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flcheckbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12411 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flcodbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29167 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fldatatable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fldateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2319 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fldoublevalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2020-08-24 08:14:25.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flfastcgi.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   143143 2023-05-08 08:40:13.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31497 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flformdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    34481 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flformrecorddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14097 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flformsearchdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      185 2019-08-01 06:59:07.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flgroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1361 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flintvalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fljasperengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      103 2020-08-19 14:34:59.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fljasperviewer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5497 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fllineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3892 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fllistviewitem.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    52856 2023-04-19 12:33:57.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28979 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flmanagermodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4403 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flnetwork.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      196 2019-08-17 07:43:18.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4300 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flpixmapview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3702 2020-08-24 09:53:53.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flposprinter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13824 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flreportengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22476 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flreportviewer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      403 2019-11-14 09:39:09.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flscripteditor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5273 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flserialport.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1620 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flsettings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13515 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flsmtpclient.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      895 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flspinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      267 2020-03-05 11:36:30.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flsqlconnections.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2019-08-17 07:43:18.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2019-08-17 07:43:18.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fltable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   108501 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      875 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fltimeedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1092 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/fluintvalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    41598 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1876 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flvar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      549 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      315 2019-08-13 07:00:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/flworkspace.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.675492 pineboo-1.0.4.5/pineboolib/fllegacy/forms/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    48049 2020-12-24 07:51:30.000000 pineboo-1.0.4.5/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       67 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/forms/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67146 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/systype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.679492 pineboo-1.0.4.5/pineboolib/fllegacy/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2019-12-02 11:03:25.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1455 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flcodbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1664 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_fldatatable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      991 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_fldateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8825 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      939 2020-09-21 06:32:29.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flform.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2286 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flformrecorddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3065 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flformsearch.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2289 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      902 2020-12-22 09:37:36.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flreportengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12536 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8666 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1592 2020-09-01 07:21:14.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-09-01 07:21:14.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_smtp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8560 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_systype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.679492 pineboo-1.0.4.5/pineboolib/interfaces/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      331 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/interfaces/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      172 2019-07-31 18:05:01.000000 pineboo-1.0.4.5/pineboolib/interfaces/cursoraccessmode.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      228 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/interfaces/dgi_schema.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10886 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/interfaces/iconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5925 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/interfaces/ifieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2999 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/interfaces/imainwindow.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5542 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/interfaces/imanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/interfaces/isession.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    21668 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/interfaces/isqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50296 2023-05-08 08:42:41.000000 pineboo-1.0.4.5/pineboolib/interfaces/isqldriver.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3292 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/interfaces/itablemetadata.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.679492 pineboo-1.0.4.5/pineboolib/loader/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       92 2019-08-04 07:50:46.000000 pineboo-1.0.4.5/pineboolib/loader/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/connection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1546 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/dgi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.679492 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      104 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      716 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/conn_dialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15802 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/dlgconnect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24027 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/dlgconnect.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       57 2020-12-02 18:09:30.000000 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2544 2020-11-09 16:02:09.000000 pineboo-1.0.4.5/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2870 2023-04-20 16:01:15.000000 pineboo-1.0.4.5/pineboolib/loader/init_project.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18283 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/loader/main.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5772 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/loader/options.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1311 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/preload.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17570 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/projectconfig.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/loader/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      477 2019-08-05 15:23:25.000000 pineboo-1.0.4.5/pineboolib/loader/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2495 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/tests/test_connection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      827 2021-03-08 11:35:13.000000 pineboo-1.0.4.5/pineboolib/loader/tests/test_main.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/tests/test_projectconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3682 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/loader/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       23 2019-08-18 15:38:56.000000 pineboo-1.0.4.5/pineboolib/plugins/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/custom_widgets/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      282 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/custom_widgets/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/custom_widgets/flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/custom_widgets/fltable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/custom_widgets/fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/custom_widgets/pncore.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/dgi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       19 2019-08-18 15:38:56.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_fcgi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-08-18 15:38:56.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_fcgi/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2848 2020-03-24 12:23:10.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-18 15:38:56.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2019-08-18 15:38:56.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-08-18 15:38:56.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2014 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9496 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2190 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1452 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      604 2020-04-02 16:10:18.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4643 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5507 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_schema.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/mainform/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      177 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       78 2019-07-30 09:20:57.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55893 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/eneboo.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4184 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/mainform.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-11-04 08:30:07.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5085 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       82 2019-07-30 09:20:57.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    49501 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1500 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.683492 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      280 2019-11-04 08:30:07.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3263 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.687492 pineboo-1.0.4.5/pineboolib/plugins/sql/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-18 13:55:56.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      483 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/flmysql_innodb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12024 2023-04-19 12:33:54.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/flmysql_myisam.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11877 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/flpymssql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      825 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/flpyodbc.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13367 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/flqpsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11393 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/flsqlite.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.687492 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       31 2020-09-17 10:11:16.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2172 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flmysql_innodb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2958 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flmysql_myisam.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2861 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flpymssql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flpyodbc.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4517 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flsqlite.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2095 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_qpsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9177 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_stress.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2019-07-27 10:21:43.000000 pineboo-1.0.4.5/pineboolib/py.typed
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.695493 pineboo-1.0.4.5/pineboolib/q3widgets/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       94 2019-09-27 15:43:59.000000 pineboo-1.0.4.5/pineboolib/q3widgets/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1761 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/checkbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      142 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/combobox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1398 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/dateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3877 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/dialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1634 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/filedialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      482 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/groupbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      118 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/line.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1061 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/lineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3570 2023-04-28 10:51:28.000000 pineboo-1.0.4.5/pineboolib/q3widgets/messagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2758 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/numberedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      443 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/picture.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      134 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/pixmap.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1109 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      887 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1541 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qbytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      774 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qcheckbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2176 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qcombobox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qdataview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2262 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qdateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      147 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qdatetime.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1663 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qdialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      237 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      316 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qeventloop.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1138 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qframe.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3328 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qgroupbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      656 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qhboxlayout.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qhbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17321 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qhttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      231 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qiconset.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2061 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qlabel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      144 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qlayoutwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1099 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qline.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1767 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qlineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5684 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qlistview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      173 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qlistviewwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      445 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qmainwindow.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      137 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qmenu.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qmessagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1668 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qobject.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qpopupmenu.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3111 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qpushbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1975 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qradiobutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      149 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qspinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12608 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qtable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1741 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qtabwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2013 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qtextedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      463 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qtextstream.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      926 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qtimeedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      404 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qtoolbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2255 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qtoolbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      654 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qvboxlayout.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qvbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1231 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/qwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      184 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/radiobutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/rect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/size.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/spinbox.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.695493 pineboo-1.0.4.5/pineboolib/q3widgets/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      278 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2019-12-19 10:11:59.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_dateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1411 2020-12-02 18:08:18.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_messagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qbytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2638 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qhttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      719 2019-09-27 15:43:59.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qpushbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1163 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qradiobuttons.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1131 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qtabwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1046 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qtextstream.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      532 2020-09-21 08:32:33.000000 pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_spinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/textedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/q3widgets/timeedit.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.695493 pineboo-1.0.4.5/pineboolib/qsa/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       95 2019-08-02 07:28:39.000000 pineboo-1.0.4.5/pineboolib/qsa/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5934 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/qsa/decorators.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1321 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/emptyscript.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7457 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/formdbwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2035 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/input.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1439 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/object_class.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11935 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/pncontrolsfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8336 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/qsa.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.695493 pineboo-1.0.4.5/pineboolib/qsa/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      496 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      744 2020-06-22 11:35:54.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/test_class.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4169 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/test_classes.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17795 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/test_knownbugs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6680 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/test_orm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1563 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/test_query_values.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1716 2023-05-01 18:19:33.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/test_require.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7893 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/qsa/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20373 2023-05-01 18:19:35.000000 pineboo-1.0.4.5/pineboolib/qsa/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.699493 pineboo-1.0.4.5/pineboolib/system_module/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/system_module/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.699493 pineboo-1.0.4.5/pineboolib/system_module/forms/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9153 2019-09-30 08:28:05.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/FLWidgetMasterTable.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28933 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/ebcomportamiento.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1368 2019-10-01 07:14:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/flareas.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2994 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/flfiles.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8007 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/flgroups.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16760 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/flmodulos.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3150 2020-07-06 10:29:58.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/fltest.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1214 2019-10-01 07:14:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/flusers.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8877 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/master.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10189 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/master_copy.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9932 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/master_print.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11619 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/master_print_copy.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11760 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/forms/sys.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.703493 pineboo-1.0.4.5/pineboolib/system_module/models/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2020-04-27 09:01:43.000000 pineboo-1.0.4.5/pineboolib/system_module/models/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1441 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flareas_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3270 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flfiles_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1238 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flgroups_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/fllarge_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1313 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flmetadata_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3296 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flmodules_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1292 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flseqs_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1007 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flserial_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1023 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flsettings_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2369 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/fltest2_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1769 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/models/fltest3_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1859 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/fltest4_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2296 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/models/fltest5_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2659 2020-10-13 15:24:00.000000 pineboo-1.0.4.5/pineboolib/system_module/models/fltest_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3548 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flupdates_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1450 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flusers_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1718 2020-07-16 10:23:10.000000 pineboo-1.0.4.5/pineboolib/system_module/models/flvar_model.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.703493 pineboo-1.0.4.5/pineboolib/system_module/queries/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/system_module/queries/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      636 2020-10-15 10:53:48.000000 pineboo-1.0.4.5/pineboolib/system_module/queries/fltest2.qry
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.703493 pineboo-1.0.4.5/pineboolib/system_module/scripts/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15186 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/ebcomportamiento.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      234 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/fldumpdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      859 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flfiles.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flloadmod.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      246 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flloadmodpkg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      427 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flmasterareas.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18788 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flmodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flmrproper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      238 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flreinit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3958 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flreloadbatch.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6038 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/flreloadlast.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/fltest6.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4351 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/sys.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.703493 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-03-26 18:29:13.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1104 2020-09-17 09:48:31.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2155 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flfiles.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2020-09-09 10:25:36.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4238 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flmodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      843 2020-09-09 10:25:36.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flmrproper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      851 2020-09-09 10:25:36.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flreinit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4322 2023-05-08 08:40:00.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_reload_last.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1564 2019-09-26 11:40:44.000000 pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_sys.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2411 2020-12-05 19:13:31.000000 pineboo-1.0.4.5/pineboolib/system_module/sys.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6505 2019-08-23 10:35:06.000000 pineboo-1.0.4.5/pineboolib/system_module/sys.xpm
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.707493 pineboo-1.0.4.5/pineboolib/system_module/translations/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-09-17 09:33:15.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 09:14:55.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.ca.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 09:14:56.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.de.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 09:14:53.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.en.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    68138 2023-05-08 09:14:51.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.es.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 09:14:58.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.fr.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 09:15:00.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.gl.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 09:15:01.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.it.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-08 09:15:03.000000 pineboo-1.0.4.5/pineboolib/system_module/translations/sys.pt.ts
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-08 09:15:03.707493 pineboo-1.0.4.5/pymodules/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2020-11-25 08:02:11.000000 pineboo-1.0.4.5/pymodules/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      283 2023-05-08 09:15:03.707493 pineboo-1.0.4.5/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4086 2023-04-04 09:45:24.000000 pineboo-1.0.4.5/setup.py
```

### Comparing `pineboo-1.0.4.4/LICENSE.mit` & `pineboo-1.0.4.5/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/PKG-INFO` & `pineboo-1.0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pineboo
-Version: 1.0.4.4
+Version: 1.0.4.5
 Summary: ERP replacement for Eneboo written in Python
 Home-page: https://github.com/deavid/pineboo
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo accounting sales warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pineboo-1.0.4.4/README.rst` & `pineboo-1.0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboo.egg-info/PKG-INFO` & `pineboo-1.0.4.5/pineboo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pineboo
-Version: 1.0.4.4
+Version: 1.0.4.5
 Summary: ERP replacement for Eneboo written in Python
 Home-page: https://github.com/deavid/pineboo
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo accounting sales warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pineboo-1.0.4.4/pineboo.egg-info/SOURCES.txt` & `pineboo-1.0.4.5/pineboo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboo.egg-info/requires.txt` & `pineboo-1.0.4.5/pineboo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/__init__.py` & `pineboo-1.0.4.5/pineboolib/application/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Application package for resources.
 
 This package holds all functions and classes that are like side resources.
 """
 
 from pineboolib.application.projectmodule import Project
+from pineboolib.core import settings
 from typing import Dict, List, Any
 
 PROJECT = Project()
 
 SERIALIZE_LIST: Dict[int, List[str]] = {}
 FILE_CLASSES: Dict[str, str] = {}
 ID_SESSION: str = ""
 
-PINEBOO_VER = "1.0.4.4"
+PINEBOO_VER = "1.0.4.5"
 
 SHOW_CURSOR_EVENTS: bool = False  # Enable show pnsqlcursor actions debug.
 SHOW_CONNECTION_EVENTS: bool = False  # Enable show debug when connection is closed.
 SHOW_NESTED_WARNING: bool = False  # Enable show nested debug.
 VIRTUAL_DB: bool = True  # Enable :memory: database on pytest.
 LOG_SQL: bool = False  # Enable sqlalchemy logs.
 USE_WEBSOCKET_CHANNEL: bool = False  # Enable websockets features.
@@ -25,12 +26,12 @@
 RECOVERING_CONNECTIONS: bool = False  # Recovering state.
 AUTO_RELOAD_BAD_CONNECTIONS: bool = False  # Auto reload bad conecctions.
 DEVELOPER_MODE: bool = True  # Skip some bugs, critical in production.
 USE_REPORT_VIEWER: bool = True  # Enable internal report viewer.
 ENABLE_ACLS: bool = True  # Enable acls usage.
 USE_INTERACTIVE_GUI: bool = True  # Enable interactiveGUI value.
 ENABLE_CALL_EXCEPTIONS: bool = True  # Enable QSA calls exceptions.
-PARSE_PROJECT_ON_INIT: bool = True  # Parse all projects on init.
+PARSE_PROJECT_ON_INIT: bool = settings.CONFIG.value("ebcomportamiento/parseProject", False)
 USE_ALTER_TABLE_LEGACY: bool = True
 PERSISTENT: Dict[str, Any] = {}
 USE_FLFILES_FOLDER_AS_STATIC_LOAD: bool = True
 TESTING_MODE: bool = False  # True when testing_mode else False
```

### Comparing `pineboo-1.0.4.4/pineboolib/application/acls/pnaccesscontrol.py` & `pineboo-1.0.4.5/pineboolib/application/acls/pnaccesscontrol.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/acls/pnaccesscontrolfactory.py` & `pineboo-1.0.4.5/pineboolib/application/acls/pnaccesscontrolfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/acls/pnaccesscontrollists.py` & `pineboo-1.0.4.5/pineboolib/application/acls/pnaccesscontrollists.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/acls/pnboolflagstate.py` & `pineboo-1.0.4.5/pineboolib/application/acls/pnboolflagstate.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/acls/tests/test_acls.py` & `pineboo-1.0.4.5/pineboolib/application/acls/tests/test_acls.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/acls/tests/test_pnaccesscontrol.py` & `pineboo-1.0.4.5/pineboolib/application/acls/tests/test_pnaccesscontrol.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/connections.py` & `pineboo-1.0.4.5/pineboolib/application/connections.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/alembic_tools.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/alembic_tools.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/basemodel.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/basemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/dummy_cursor.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/dummy_cursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/dummy_signal.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/dummy_signal.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_basemodel.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_bytearray.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_bytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_consistency.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_consistency.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_dummycursor.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_dummycursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_query_orm.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_query_orm.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_relationships.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_relationships.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_sessions.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_signals.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_thread_session.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_thread_session.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_utils.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/tests/test_view.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/orm/utils.py` & `pineboo-1.0.4.5/pineboolib/application/database/orm/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnbuffer.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnbuffer.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnconnection.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnconnectionmanager.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnconnectionmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pncursortablemodel.py` & `pineboo-1.0.4.5/pineboolib/application/database/pncursortablemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pngroupbyquery.py` & `pineboo-1.0.4.5/pineboolib/application/database/pngroupbyquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnparameterquery.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnparameterquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnsignals.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnsignals.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnsqlcursor.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnsqlcursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnsqldriversmanager.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnsqldriversmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/pnsqlquery.py` & `pineboo-1.0.4.5/pineboolib/application/database/pnsqlquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnbuffer.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnbuffer.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnconnection.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnconnection_manager.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnconnection_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pncursortablemodel.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pncursortablemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnparameterquery.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnparameterquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnsqlcursor.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnsqlcursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnsqldriversmanager.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnsqldriversmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_pnsqlquery.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_pnsqlquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/tests/test_utils.py` & `pineboo-1.0.4.5/pineboolib/application/database/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/database/utils.py` & `pineboo-1.0.4.5/pineboolib/application/database/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/file.py` & `pineboo-1.0.4.5/pineboolib/application/file.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/load_script.py` & `pineboo-1.0.4.5/pineboolib/application/load_script.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/pnaction.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/pnaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/pncompoundkeymetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/pncompoundkeymetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/pnfieldmetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/pnfieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/pnrelationmetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/pnrelationmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/pntablemetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/pntablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pnaction.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pnaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pnfieldmetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pnfieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pnrelationmetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pnrelationmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/metadata/tests/test_pntablemetadata.py` & `pineboo-1.0.4.5/pineboolib/application/metadata/tests/test_pntablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/module.py` & `pineboo-1.0.4.5/pineboolib/application/module.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/moduleactions.py` & `pineboo-1.0.4.5/pineboolib/application/moduleactions.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/packager/pnpackager.py` & `pineboo-1.0.4.5/pineboolib/application/packager/pnpackager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/packager/pnunpacker.py` & `pineboo-1.0.4.5/pineboolib/application/packager/pnunpacker.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/packager/tests/test_pnpackager.py` & `pineboo-1.0.4.5/pineboolib/application/packager/tests/test_pnpackager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/packager/tests/test_pnunpaker.py` & `pineboo-1.0.4.5/pineboolib/application/packager/tests/test_pnunpaker.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/kparsertools.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/kparsertools.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/kut2fpdf.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/kut2fpdf.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/pnmtdparser.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/pnmtdparser.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/flex.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/flex.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/flscriptparse.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/flscriptparse.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/lextab.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/lextab.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/postparse.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/postparse.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/pyconvert.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/pyconvert.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/pytnyzer.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/pytnyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         return "True"
     elif name == "null":
         return "None"
     elif name == "unknown":
         return "None"
     elif name == "undefined":
         return "None"
-    elif name in ("this", "form"):
+    elif name == "this":
         return "self"
     elif name == "NaN":
         return 'float("nan")'
 
     elif name == "startsWith":
         name = "startswith"
     elif name == "endsWith":
```

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_qsa/token_rules.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_qsa/token_rules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/qt3ui.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/qt3ui.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py` & `pineboo-1.0.4.5/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/pnapplication.py` & `pineboo-1.0.4.5/pineboolib/application/pnapplication.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/process.py` & `pineboo-1.0.4.5/pineboolib/application/process.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/projectmodule.py` & `pineboo-1.0.4.5/pineboolib/application/projectmodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         self.tmpdir = settings.CONFIG.value("ebcomportamiento/temp_dir", "")
         self.parser = None
 
         self.no_python_cache = settings.CONFIG.value("ebcomportamiento/noPythonCache", False)
         self.apppath = utils_base.filedir("..")
         self.delete_base_cache = settings.CONFIG.value("ebcomportamiento/keep_general_cache", False)
         self.delete_cache = settings.CONFIG.value("ebcomportamiento/deleteCache", False)
+        application.PARSE_PROJECT_ON_INIT = settings.CONFIG.value(
+            "ebcomportamiento/parseProject", False
+        )
         self.actions = {}
         self.files = {}
         self.areas = {}
         self.modules = {}
         self.db_admin_mode = settings.CONFIG.value("application/dbadmin_enabled", False)
 
         import pathlib
@@ -156,17 +159,15 @@
 
     def init_conn(self, connection: "pnconnection.PNConnection") -> bool:
         """Initialize project with a connection."""
         # if self._conn is not None:
         #    del self._conn
         #    self._conn = None
 
-        self.parse_project = settings.CONFIG.value(
-            "ebcomportamiento/parseProject", application.PARSE_PROJECT_ON_INIT
-        )
+        self.parse_project = application.PARSE_PROJECT_ON_INIT
 
         return self.conn_manager.setMainConn(connection)
 
     def init_dgi(self, dgi: "dgi_schema.dgi_schema") -> None:
         """Load and associate the defined DGI onto this project."""
         # FIXME: Actually, DGI should be loaded here, or kind of.
```

### Comparing `pineboo-1.0.4.4/pineboolib/application/proxy.py` & `pineboo-1.0.4.5/pineboolib/application/proxy.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/qsadictmodules.py` & `pineboo-1.0.4.5/pineboolib/application/qsadictmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/qsatypes/date.py` & `pineboo-1.0.4.5/pineboolib/application/qsatypes/date.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/qsatypes/sysbasetype.py` & `pineboo-1.0.4.5/pineboolib/application/qsatypes/sysbasetype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/qsatypes/tests/test_date.py` & `pineboo-1.0.4.5/pineboolib/application/qsatypes/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/qsatypes/tests/test_sysbasetype.py` & `pineboo-1.0.4.5/pineboolib/application/qsatypes/tests/test_sysbasetype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/safeqsa.py` & `pineboo-1.0.4.5/pineboolib/application/safeqsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/signatures/pdf_digest.py` & `pineboo-1.0.4.5/pineboolib/application/signatures/pdf_digest.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/signatures/pdf_qr.py` & `pineboo-1.0.4.5/pineboolib/application/signatures/pdf_qr.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/signatures/tests/test_signatures.py` & `pineboo-1.0.4.5/pineboolib/application/signatures/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/signatures/xml_digest.py` & `pineboo-1.0.4.5/pineboolib/application/signatures/xml_digest.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/staticloader/pnmodulesstaticloader.py` & `pineboo-1.0.4.5/pineboolib/application/staticloader/pnmodulesstaticloader.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/staticloader/tests/test_static_loader.py` & `pineboo-1.0.4.5/pineboolib/application/staticloader/tests/test_static_loader.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/staticloader/ui/static_loader.ui` & `pineboo-1.0.4.5/pineboolib/application/staticloader/ui/static_loader.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/tests/test_application.py` & `pineboo-1.0.4.5/pineboolib/application/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/tests/test_load_script.py` & `pineboo-1.0.4.5/pineboolib/application/tests/test_load_script.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/tests/test_process.py` & `pineboo-1.0.4.5/pineboolib/application/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/tests/test_projectmodule.py` & `pineboo-1.0.4.5/pineboolib/application/tests/test_projectmodule.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/tests/test_proxy.py` & `pineboo-1.0.4.5/pineboolib/application/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/tests/test_types.py` & `pineboo-1.0.4.5/pineboolib/application/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/tests/test_xmlaction.py` & `pineboo-1.0.4.5/pineboolib/application/tests/test_xmlaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/translator/pntranslator.py` & `pineboo-1.0.4.5/pineboolib/application/translator/pntranslator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/translator/test/test_pntranslator.py` & `pineboo-1.0.4.5/pineboolib/application/translator/test/test_pntranslator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/types.py` & `pineboo-1.0.4.5/pineboolib/application/types.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/check_dependencies.py` & `pineboo-1.0.4.5/pineboolib/application/utils/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/convert_flaction.py` & `pineboo-1.0.4.5/pineboolib/application/utils/convert_flaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/date_conversion.py` & `pineboo-1.0.4.5/pineboolib/application/utils/date_conversion.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/flfiles_dir.py` & `pineboo-1.0.4.5/pineboolib/application/utils/flfiles_dir.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/geometry.py` & `pineboo-1.0.4.5/pineboolib/application/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/mobilemode.py` & `pineboo-1.0.4.5/pineboolib/application/utils/mobilemode.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/modules.py` & `pineboo-1.0.4.5/pineboolib/application/utils/modules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/path.py` & `pineboo-1.0.4.5/pineboolib/application/utils/path.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/service.py` & `pineboo-1.0.4.5/pineboolib/application/utils/service.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/sql_tools.py` & `pineboo-1.0.4.5/pineboolib/application/utils/sql_tools.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/utils/xpm.py` & `pineboo-1.0.4.5/pineboolib/application/utils/xpm.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/application/xmlaction.py` & `pineboo-1.0.4.5/pineboolib/application/xmlaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/decorators.py` & `pineboo-1.0.4.5/pineboolib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/exceptions.py` & `pineboo-1.0.4.5/pineboolib/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/garbage_collector.py` & `pineboo-1.0.4.5/pineboolib/core/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Pi-symbol.svg` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Pi-symbol.svg`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi.psd` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi.psd`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2.xcf` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2.xcf`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2_256.png` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2_256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi2_512.png` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi2_512.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi_1024.png` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi_1024.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi_256.png` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi_256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icono_pi/Symbol_pi_512.png` & `pineboo-1.0.4.5/pineboolib/core/images/icono_pi/Symbol_pi_512.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/about.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/about.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/aboutqt.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/aboutqt.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/cancel.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/consola.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/consola.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/date.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/date.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/delete.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/delete.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/down.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/down.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/edit.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/edit.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/edit_file.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/edit_file.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/edit_file_xml.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/edit_file_xml.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/estilo.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/estilo.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/exit.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/exit.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/fltable-clean.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/fltable-clean.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/fltable-data.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/fltable-data.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/fltable-odf.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/fltable-odf.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/folder_update.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/folder_update.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/font.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/font.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-bottom.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-bottom.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-down.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-down.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-first.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-first.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-home.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-home.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-jump.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-jump.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-last.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-last.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-next.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-next.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-previous.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-previous.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-top.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-top.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/go-up.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/go-up.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-add.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-add.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-bold.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-bold.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-cancel.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-cancel.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-clear.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-clear.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-copy.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-copy.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-cut.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-cut.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-delete.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-delete.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-find-and-replace.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-find-and-replace.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-find.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-find.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-fullscreen.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-fullscreen.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-back-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-back-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-back-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-back-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-down.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-down.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-forward-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-forward-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-forward-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-forward-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-go-up.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-go-up.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-bottom.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-bottom.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-first-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-first-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-first-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-first-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-last-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-last-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-last-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-last-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-goto-top.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-goto-top.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-home.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-home.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-indent-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-indent-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-indent-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-indent-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-italic.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-italic.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-jump-to-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-jump-to-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-jump-to-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-jump-to-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-center.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-center.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-fill.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-fill.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-left.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-left.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-justify-right.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-justify-right.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-forward-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-forward-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-forward-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-forward-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-next-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-next-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-next-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-next-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-play-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-play-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-previous-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-previous-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-previous-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-previous-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-record.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-record.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-rewind-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-rewind-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-rewind-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-rewind-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-media-stop.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-media-stop.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-new.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-new.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-open.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-open.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-paste.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-paste.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-print-preview.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-print-preview.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-print.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-print.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-properties.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-properties.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-redo-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-redo-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-refresh.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-refresh.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-save-as.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-save-as.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-save.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-save.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-select-all.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-select-all.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-stop.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-stop.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-strikethrough.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-strikethrough.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-underline.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-underline.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-undo-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-undo-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-unindent-ltr.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-unindent-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/gtk-unindent-rtl.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/gtk-unindent-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/help_index.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/help_index.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/insert.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/insert.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/lock.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/lock.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/ok.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/ok.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/paste.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/paste.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-128.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-128.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-16.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-16.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-24.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-24.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-256.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-32.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-32.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-48.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-48.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-57.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-57.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-64.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-64.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo-72.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo-72.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo-logo.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo-logo.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-128.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-128.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-16.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-16.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-24.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-24.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-256.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-32.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-32.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-48.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-48.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo-64.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo-64.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/pineboo2-logo.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/pineboo2-logo.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/print.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/print.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/reload.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/reload.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/signed_stamp.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/signed_stamp.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_ebcomportamiento.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_ebcomportamiento.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flareas.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flareas.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_fldumpdb.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_fldumpdb.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flgroups.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flgroups.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flloadmod.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flloadmod.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flloadmodpkg.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flloadmodpkg.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flmodules.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flmodules.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flmrproper.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flmrproper.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flreinit.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flreinit.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flreloadbatch.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flreloadbatch.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flreloadlast.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flreloadlast.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/sys_flusers.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/sys_flusers.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/terminal.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/terminal.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/unlock.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/unlock.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/up.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/up.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/icons/zoom.png` & `pineboo-1.0.4.5/pineboolib/core/images/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/splashscreen/dbadmin240.png` & `pineboo-1.0.4.5/pineboolib/core/images/splashscreen/dbadmin240.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/splashscreen/dbadmin480.png` & `pineboo-1.0.4.5/pineboolib/core/images/splashscreen/dbadmin480.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/splashscreen/quick240.png` & `pineboo-1.0.4.5/pineboolib/core/images/splashscreen/quick240.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/splashscreen/quick480.png` & `pineboo-1.0.4.5/pineboolib/core/images/splashscreen/quick480.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/splashscreen/splash.png` & `pineboo-1.0.4.5/pineboolib/core/images/splashscreen/splash.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/images/splashscreen/splash.svg` & `pineboo-1.0.4.5/pineboolib/core/images/splashscreen/splash.svg`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/message_manager.py` & `pineboo-1.0.4.5/pineboolib/core/message_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/settings.py` & `pineboo-1.0.4.5/pineboolib/core/settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/test/test_settings.py` & `pineboo-1.0.4.5/pineboolib/core/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/check_dependencies.py` & `pineboo-1.0.4.5/pineboolib/core/utils/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/logging.py` & `pineboo-1.0.4.5/pineboolib/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/singleton.py` & `pineboo-1.0.4.5/pineboolib/core/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/struct.py` & `pineboo-1.0.4.5/pineboolib/core/utils/struct.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/tests/test_utils_base.py` & `pineboo-1.0.4.5/pineboolib/core/utils/tests/test_utils_base.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/tests/test_version.py` & `pineboo-1.0.4.5/pineboolib/core/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/utils_base.py` & `pineboo-1.0.4.5/pineboolib/core/utils/utils_base.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/core/utils/version.py` & `pineboo-1.0.4.5/pineboolib/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqformdb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqformdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqods.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqods.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqs.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqs.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqsql.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/aqssproject.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/aqssproject.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flcodbar.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flcodbar.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fldatatable.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fldatatable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fldateedit.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fldateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fldoublevalidator.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fldoublevalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flfastcgi.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flfastcgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flfielddb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flfielddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flformdb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flformdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flformrecorddb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flformrecorddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flformsearchdb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flformsearchdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flintvalidator.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flintvalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fllineedit.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fllineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fllistviewitem.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fllistviewitem.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flmanager.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flmanagermodules.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flmanagermodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flnetwork.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flnetwork.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flpixmapview.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flpixmapview.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flposprinter.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flposprinter.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flreportengine.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flreportengine.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flreportviewer.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flreportviewer.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flserialport.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flserialport.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flsettings.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flsettings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flsmtpclient.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flsmtpclient.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flspinbox.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flspinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fltable.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fltable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fltabledb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fltabledb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fltimeedit.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fltimeedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/fluintvalidator.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/fluintvalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flutil.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flvar.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flvar.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/flwidget.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/flwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui` & `pineboo-1.0.4.5/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/systype.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/systype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flcodbar.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flcodbar.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_fldatatable.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_fldatatable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_fldateedit.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_fldateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flfielddb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flfielddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flform.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flform.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flformrecorddb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flformrecorddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flformsearch.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flformsearch.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flmanager.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flreportengine.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flreportengine.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_fltabledb.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_fltabledb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_flutil.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_flutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_settings.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_smtp.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/fllegacy/tests/test_systype.py` & `pineboo-1.0.4.5/pineboolib/fllegacy/tests/test_systype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/interfaces/iconnection.py` & `pineboo-1.0.4.5/pineboolib/interfaces/iconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/interfaces/ifieldmetadata.py` & `pineboo-1.0.4.5/pineboolib/interfaces/ifieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/interfaces/imainwindow.py` & `pineboo-1.0.4.5/pineboolib/interfaces/imainwindow.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/interfaces/imanager.py` & `pineboo-1.0.4.5/pineboolib/interfaces/imanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/interfaces/isqlcursor.py` & `pineboo-1.0.4.5/pineboolib/interfaces/isqlcursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/interfaces/isqldriver.py` & `pineboo-1.0.4.5/pineboolib/interfaces/isqldriver.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/interfaces/itablemetadata.py` & `pineboo-1.0.4.5/pineboolib/interfaces/itablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/connection.py` & `pineboo-1.0.4.5/pineboolib/loader/connection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/dgi.py` & `pineboo-1.0.4.5/pineboolib/loader/dgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/dlgconnect/conn_dialog.py` & `pineboo-1.0.4.5/pineboolib/loader/dlgconnect/conn_dialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/dlgconnect/dlgconnect.py` & `pineboo-1.0.4.5/pineboolib/loader/dlgconnect/dlgconnect.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/dlgconnect/dlgconnect.ui` & `pineboo-1.0.4.5/pineboolib/loader/dlgconnect/dlgconnect.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py` & `pineboo-1.0.4.5/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/init_project.py` & `pineboo-1.0.4.5/pineboolib/loader/init_project.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/main.py` & `pineboo-1.0.4.5/pineboolib/loader/main.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/options.py` & `pineboo-1.0.4.5/pineboolib/loader/options.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/preload.py` & `pineboo-1.0.4.5/pineboolib/loader/preload.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/projectconfig.py` & `pineboo-1.0.4.5/pineboolib/loader/projectconfig.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/tests/test_connection.py` & `pineboo-1.0.4.5/pineboolib/loader/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/tests/test_main.py` & `pineboo-1.0.4.5/pineboolib/loader/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/tests/test_projectconfig.py` & `pineboo-1.0.4.5/pineboolib/loader/tests/test_projectconfig.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/loader/utils.py` & `pineboo-1.0.4.5/pineboolib/loader/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/dgi/dgi_schema.py` & `pineboo-1.0.4.5/pineboolib/plugins/dgi/dgi_schema.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/eneboo.py` & `pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/eneboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/mainform.ui` & `pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/mainform.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py` & `pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py` & `pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui` & `pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py` & `pineboo-1.0.4.5/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/flmysql_myisam.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/flmysql_myisam.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/flpymssql.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/flpymssql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/flpyodbc.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/flpyodbc.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/flqpsql.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/flqpsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/flsqlite.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/flsqlite.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flmysql_innodb.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flmysql_innodb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flmysql_myisam.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flmysql_myisam.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flpymssql.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flpymssql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flpyodbc.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flpyodbc.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_flsqlite.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_flsqlite.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_qpsql.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_qpsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/plugins/sql/tests/test_stress.py` & `pineboo-1.0.4.5/pineboolib/plugins/sql/tests/test_stress.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/checkbox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/dateedit.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/dateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/dialog.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/filedialog.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/filedialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/lineedit.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/lineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/messagebox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/messagebox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/numberedit.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/numberedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qaction.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qbuttongroup.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qbytearray.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qbytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qcheckbox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qcheckbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qcombobox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qcombobox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qdateedit.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qdateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qdialog.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qdialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qframe.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qframe.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qgroupbox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qgroupbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qhboxlayout.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qhboxlayout.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qhttp.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qhttp.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qlabel.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qlabel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qline.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qline.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qlineedit.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qlineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qlistview.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qlistview.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qobject.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qobject.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qpushbutton.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qpushbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qradiobutton.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qradiobutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qtable.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qtable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qtabwidget.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qtabwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qtextedit.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qtextedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qtimeedit.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qtimeedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qtoolbutton.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qtoolbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qvboxlayout.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qvboxlayout.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/qwidget.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/qwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/spinbox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_messagebox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_messagebox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qbytearray.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qbytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qhttp.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qhttp.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qpushbutton.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qpushbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qradiobuttons.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qradiobuttons.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qtabwidget.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qtabwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_qtextstream.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_qtextstream.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/q3widgets/tests/test_spinbox.py` & `pineboo-1.0.4.5/pineboolib/q3widgets/tests/test_spinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/decorators.py` & `pineboo-1.0.4.5/pineboolib/qsa/decorators.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/emptyscript.py` & `pineboo-1.0.4.5/pineboolib/qsa/emptyscript.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/formdbwidget.py` & `pineboo-1.0.4.5/pineboolib/qsa/formdbwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/input.py` & `pineboo-1.0.4.5/pineboolib/qsa/input.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/object_class.py` & `pineboo-1.0.4.5/pineboolib/qsa/object_class.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/pncontrolsfactory.py` & `pineboo-1.0.4.5/pineboolib/qsa/pncontrolsfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/qsa.py` & `pineboo-1.0.4.5/pineboolib/qsa/qsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/tests/test_class.py` & `pineboo-1.0.4.5/pineboolib/qsa/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/tests/test_classes.py` & `pineboo-1.0.4.5/pineboolib/qsa/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/tests/test_knownbugs.py` & `pineboo-1.0.4.5/pineboolib/qsa/tests/test_knownbugs.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/tests/test_orm.py` & `pineboo-1.0.4.5/pineboolib/qsa/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/tests/test_query_values.py` & `pineboo-1.0.4.5/pineboolib/qsa/tests/test_query_values.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/tests/test_require.py` & `pineboo-1.0.4.5/pineboolib/qsa/tests/test_require.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/tests/test_utils.py` & `pineboo-1.0.4.5/pineboolib/qsa/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/qsa/utils.py` & `pineboo-1.0.4.5/pineboolib/qsa/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/FLWidgetMasterTable.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/FLWidgetMasterTable.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/ebcomportamiento.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/ebcomportamiento.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/flareas.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/flareas.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/flfiles.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/flfiles.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/flgroups.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/flgroups.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/flmodulos.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/flmodulos.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/fltest.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/fltest.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/flusers.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/flusers.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/master.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/master.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/master_copy.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/master_copy.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/master_print.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/master_print.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/master_print_copy.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/master_print_copy.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/forms/sys.ui` & `pineboo-1.0.4.5/pineboolib/system_module/forms/sys.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flareas_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flareas_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flfiles_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flfiles_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flgroups_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flgroups_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/fllarge_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/fllarge_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flmetadata_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flmetadata_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flmodules_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flmodules_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flseqs_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flseqs_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flserial_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flserial_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flsettings_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flsettings_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/fltest2_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/fltest2_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/fltest3_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/fltest3_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/fltest4_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/fltest4_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/fltest5_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/fltest5_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/fltest_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/fltest_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flupdates_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flupdates_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flusers_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flusers_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/models/flvar_model.py` & `pineboo-1.0.4.5/pineboolib/system_module/models/flvar_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/queries/fltest2.qry` & `pineboo-1.0.4.5/pineboolib/system_module/queries/fltest2.qry`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/ebcomportamiento.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/ebcomportamiento.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/flfiles.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/flfiles.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/flloadmod.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/flloadmod.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/flmodules.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/flmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/flreloadbatch.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/flreloadbatch.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/flreloadlast.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/flreloadlast.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/sys.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/sys.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flfiles.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flfiles.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flmodules.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flmrproper.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flmrproper.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_flreinit.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_flreinit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_reload_last.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_reload_last.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/scripts/tests/test_sys.py` & `pineboo-1.0.4.5/pineboolib/system_module/scripts/tests/test_sys.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/sys.xml` & `pineboo-1.0.4.5/pineboolib/system_module/sys.xml`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/sys.xpm` & `pineboo-1.0.4.5/pineboolib/system_module/sys.xpm`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.ca.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.ca.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.de.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.de.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.en.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.en.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.es.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.es.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.fr.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.fr.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.gl.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.gl.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.it.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.it.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/pineboolib/system_module/translations/sys.pt.ts` & `pineboo-1.0.4.5/pineboolib/system_module/translations/sys.pt.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.4/setup.py` & `pineboo-1.0.4.5/setup.py`

 * *Files identical despite different names*

