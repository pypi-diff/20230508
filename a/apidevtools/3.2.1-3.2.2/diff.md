# Comparing `tmp/apidevtools-3.2.1.tar.gz` & `tmp/apidevtools-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.2.1.tar", last modified: Wed May  3 11:57:54 2023, max compression
+gzip compressed data, was "apidevtools-3.2.2.tar", last modified: Mon May  8 01:32:51 2023, max compression
```

## Comparing `apidevtools-3.2.1.tar` & `apidevtools-3.2.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.912418 apidevtools-3.2.1/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3400 2023-05-03 11:57:54.911419 apidevtools-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.1/README.md
--rw-rw-rw-   0        0        0     1774 2023-05-03 11:56:08.000000 apidevtools-3.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 11:57:54.912418 apidevtools-3.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.640179 apidevtools-3.2.1/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.659180 apidevtools-3.2.1/src/apidevtools/
--rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.1/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.2.1/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.692183 apidevtools-3.2.1/src/apidevtools/media/
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.1/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.2.1/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.1/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.737222 apidevtools-3.2.1/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.1/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.1/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.749220 apidevtools-3.2.1/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.781220 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4793 2023-05-01 17:19:11.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3287 2023-03-21 21:53:42.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6651 2023-05-03 11:55:37.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2087 2023-05-03 02:07:38.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.798252 apidevtools-3.2.1/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.1/src/apidevtools/simpleorm/types/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.812321 apidevtools-3.2.1/src/apidevtools/template/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/__init__.py
--rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/create.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.636180 apidevtools-3.2.1/src/apidevtools/template/template/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.813321 apidevtools-3.2.1/src/apidevtools/template/template/api/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.820420 apidevtools-3.2.1/src/apidevtools/template/template/api/build/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/build/__init__.py
--rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/build/compose.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.837421 apidevtools-3.2.1/src/apidevtools/template/template/api/src/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/app.py
--rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/const.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.866418 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/
--rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/__init__.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/auth.py
--rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/item.py
--rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/user.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.893420 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/
--rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/__init__.py
--rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/auth.py
--rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/item.py
--rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/user.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.910419 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/
--rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/__init__.py
--rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/item.py
--rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/user.py
--rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.2.1/src/apidevtools/template/template.zip
--rw-rw-rw-   0        0        0     1155 2023-04-16 14:10:32.000000 apidevtools-3.2.1/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:57:54.678213 apidevtools-3.2.1/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3400 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-03 11:57:54.000000 apidevtools-3.2.1/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.476144 apidevtools-3.2.2/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3400 2023-05-08 01:32:51.475144 apidevtools-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.2/README.md
+-rw-rw-rw-   0        0        0     1774 2023-05-08 01:32:36.000000 apidevtools-3.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 01:32:51.476144 apidevtools-3.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.408144 apidevtools-3.2.2/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.411144 apidevtools-3.2.2/src/apidevtools/
+-rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.2/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.2.2/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.433169 apidevtools-3.2.2/src/apidevtools/media/
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.2/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.2.2/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.2/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.436143 apidevtools-3.2.2/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.2/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.2/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.440143 apidevtools-3.2.2/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.445144 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4793 2023-05-01 17:19:11.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3392 2023-05-08 01:29:46.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6745 2023-05-08 01:31:17.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2087 2023-05-03 02:07:38.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.448143 apidevtools-3.2.2/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.2/src/apidevtools/simpleorm/types/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.456143 apidevtools-3.2.2/src/apidevtools/template/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/create.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.403144 apidevtools-3.2.2/src/apidevtools/template/template/
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.457143 apidevtools-3.2.2/src/apidevtools/template/template/api/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.459152 apidevtools-3.2.2/src/apidevtools/template/template/api/build/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/build/__init__.py
+-rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/build/compose.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.462149 apidevtools-3.2.2/src/apidevtools/template/template/api/src/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/__init__.py
+-rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/app.py
+-rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/const.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.466143 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/
+-rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/__init__.py
+-rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/auth.py
+-rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/item.py
+-rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/user.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.470158 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/
+-rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/auth.py
+-rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/item.py
+-rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/user.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.474144 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/
+-rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/__init__.py
+-rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/item.py
+-rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/user.py
+-rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.2.2/src/apidevtools/template/template.zip
+-rw-rw-rw-   0        0        0     1155 2023-04-16 14:10:32.000000 apidevtools-3.2.2/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 01:32:51.430143 apidevtools-3.2.2/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3400 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2079 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-08 01:32:51.000000 apidevtools-3.2.2/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.2.1/LICENSE.txt` & `apidevtools-3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/PKG-INFO` & `apidevtools-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.1
+Version: 3.2.2
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.1/README.md` & `apidevtools-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/pyproject.toml` & `apidevtools-3.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.2.1"
+version = "3.2.2"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "All in one tools for API development."
```

### Comparing `apidevtools-3.2.1/src/apidevtools/logman.py` & `apidevtools-3.2.2/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/media/imgproc.py` & `apidevtools-3.2.2/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/media/telegraph.py` & `apidevtools-3.2.2/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/security/encryptor.py` & `apidevtools-3.2.2/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/security/hasher.py` & `apidevtools-3.2.2/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,27 +34,30 @@
         except Exception as error:
             self.logger.error(error)
             return False
 
     async def execute(self, query: str, args: tuple[Any, ...] = ()) -> bool:
         try:
             await self.pool.execute(query, args) if len(args) else await self.pool.executescript(query)
+            await self.pool.commit()
             return True
         except Exception as error:
             self.logger.error(error)
             return False
 
     async def columns(self, tablename: str) -> list[str]:
         cursor: _aiosqlite.Cursor = await self.pool.execute(f'SELECT * FROM {tablename}')
         return list(map(lambda x: x[0], cursor.description))
 
     async def fetchall(self, query: str, args: tuple[Any, ...] = ()) -> list[MutableMapping]:
         try:
             cursor: _aiosqlite.Cursor = await self.pool.execute(query, args)
-            return [{cursor.description[i][0]: value for i, value in enumerate(row)} for row in await cursor.fetchall()]
+            result = [{cursor.description[i][0]: value for i, value in enumerate(row)} for row in await cursor.fetchall()]
+            await self.pool.commit()
+            return result
         except Exception as error:
             self.logger.error(error)
             return []
 
     async def _constructor__select_relations(
             self, relation: Relation
     ) -> tuple[str, tuple[Any, ...]]:
```

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     def __init__(self, connector: Connector, logger: Logger = loguru.logger):
         self.connector: Connector = connector
         self.logger: Logger = logger
 
     async def create_pool(self) -> bool:
         try:
             is_created = await self.connector.create_pool()
-            self.logger.info(f'`ORM.connector` pool created')
+            self.logger.info(f'`ORM.connector: {self.connector.__class__.__name__}` pool created')
             return is_created
         except Exception as error:
             self.logger.error(error)
             return False
 
     async def close_pool(self) -> bool:
         try:
             is_closed = await self.connector.close_pool()
-            self.logger.info(f'`ORM.connector` pool closed')
+            self.logger.info(f'`ORM.connector: {self.connector.__class__.__name__}` pool closed')
             return is_closed
         except Exception as error:
             self.logger.error(f'{error}')
             return False
 
     async def execute(self, query: str, args: tuple[Any, ...] = ()) -> Any:
         return await self.connector.execute(query, args)
@@ -37,15 +37,15 @@
     async def select(
             self,
             query: str, args: tuple[Any, ...] = (), record_t: RecordType = dict[str, Any],
             *, rel_depth: int = 0
     ) -> Records:
         records = Records(await self.connector.fetchall(query, args), record_t)
         if rel_depth and _is_dict(record_t):
-            self.logger.warning(f'`ORM.select(rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
+            self.logger.warning(f'`ORM.select(..., rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
         for index, record in enumerate(await records.all()) if not _is_dict(record_t) and rel_depth else ():
             for relation in record.relations():
                 query, args = await self.connector._constructor__select_relations(relation)
                 instances = await (await self.select(query, args, relation.rel_schema_t, rel_depth=rel_depth - 1)).all()
                 records, record = await self.__attach_instances(records, record, relation, instances, index)
         return records
 
@@ -62,15 +62,15 @@
             instance: Instance, where: dict[str, Any], record_t: RecordType = dict[str, Any], tablename: str = None,
             *, rel_depth: int = 0
     ) -> Records:
         instance, tablename = await self.__parse_parameters(instance, tablename)
         query, args = await self.connector._constructor__update_instances(instance, tablename, where)
         records = Records(await self.connector.fetchall(query, args), record_t)
         if rel_depth and _is_dict(record_t):
-            self.logger.warning(f'`ORM.update(rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
+            self.logger.warning(f'`ORM.update(..., rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
         for index, record in enumerate(await records.all()) if not _is_dict(record_t) and rel_depth else ():
             for relation in record.relations():
                 query, args = await self.connector._constructor__select_relations(relation)
                 instances = await (await self.select(query, args, relation.rel_schema_t, rel_depth=rel_depth - 1)).all()
                 records, record = await self.__attach_instances(records, record, relation, instances, index)
         return records
 
@@ -79,17 +79,17 @@
             instance: Instance, record_t: RecordType = dict[str, Any], tablename: str = None,
             *, rel_depth: int = 0, del_depth: int = INF
     ) -> Records:
         instance, tablename = await self.__parse_parameters(instance, tablename)
         query, args = await self.connector._constructor__select_instances(instance, tablename)
         records = await self.select(query, args, record_t)
         if del_depth and _is_dict(record_t):
-            self.logger.warning(f'`ORM.delete(del_depth={del_depth})` but `record_t` is not `Schema` ({record_t})')
+            self.logger.warning(f'`ORM.delete(..., del_depth={del_depth})` but `record_t` is not `Schema` ({record_t})')
         if rel_depth and _is_dict(record_t):
-            self.logger.warning(f'`ORM.delete(rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
+            self.logger.warning(f'`ORM.delete(..., rel_depth={rel_depth})` but `record_t` is not `Schema` ({record_t})')
         for index, record in enumerate(await records.all()) if not _is_dict(record_t) and del_depth else ():
             for relation in record.relations():
                 instances = await (await self.delete(
                     relation.where, relation.rel_schema_t, relation.rel_schema_t.__tablename__, del_depth=del_depth - 1
                 )).all()
                 if rel_depth:
                     records, record = await self.__attach_instances(records, record, relation, instances, index)
```

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.2.2/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/create.py` & `apidevtools-3.2.2/src/apidevtools/template/create.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/app.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/app.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/const.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/const.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/auth.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/item.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/crud/user.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/crud/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/auth.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/item.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/routers/user.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/routers/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template/api/src/schemas/user.py` & `apidevtools-3.2.2/src/apidevtools/template/template/api/src/schemas/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/template/template.zip` & `apidevtools-3.2.2/src/apidevtools/template/template.zip`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools/utils.py` & `apidevtools-3.2.2/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.1/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.2.2/src/apidevtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.1
+Version: 3.2.2
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.1/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.2.2/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

