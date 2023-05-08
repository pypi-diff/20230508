# Comparing `tmp/ApiLogicServer-8.3.6.tar.gz` & `tmp/ApiLogicServer-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ApiLogicServer-8.3.6.tar", last modified: Tue May  2 04:14:08 2023, max compression
+gzip compressed data, was "ApiLogicServer-8.4.0.tar", last modified: Mon May  8 02:38:24 2023, max compression
```

## Comparing `ApiLogicServer-8.3.6.tar` & `ApiLogicServer-8.4.0.tar`

### file list

```diff
@@ -1,777 +1,706 @@
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.728937 ApiLogicServer-8.3.6/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.507710 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/
--rw-r--r--   0 val        (502) staff       (20)    14816 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    54435 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/SOURCES.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/dependency_links.txt
--rw-r--r--   0 val        (502) staff       (20)       66 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/entry_points.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/not-zip-safe
--rw-r--r--   0 val        (502) staff       (20)      585 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/requires.txt
--rw-r--r--   0 val        (502) staff       (20)       21 2023-05-02 04:14:08.000000 ApiLogicServer-8.3.6/ApiLogicServer.egg-info/top_level.txt
--rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/LICENSE
--rw-r--r--   0 val        (502) staff       (20)      804 2023-05-02 03:36:56.000000 ApiLogicServer-8.3.6/MANIFEST.in
--rw-r--r--   0 val        (502) staff       (20)    14816 2023-05-02 04:14:08.728664 ApiLogicServer-8.3.6/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    13827 2023-05-02 04:03:01.000000 ApiLogicServer-8.3.6/README.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.509731 ApiLogicServer-8.3.6/api_logic_server_cli/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    60440 2023-05-02 04:02:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/api_logic_server.py
--rw-r--r--   0 val        (502) staff       (20)      124 2023-05-02 04:11:59.000000 ApiLogicServer-8.3.6/api_logic_server_cli/api_logic_server_info.yaml
--rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/cli.py
--rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_base.py
--rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_project.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.512921 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.517871 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5300 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    13709 2023-05-02 02:08:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     5290 2023-02-05 02:48:17.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
--rw-r--r--   0 val        (502) staff       (20)    11680 2023-05-02 02:02:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_logic_server_utils.py
--rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/model_creation_services.py
--rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.519954 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
--rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.520143 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
--rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
--rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
--rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
--rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
--rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
--rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
--rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.499500 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.522549 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
--rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
--rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
--rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
--rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.602635 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
--rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
--rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
--rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
--rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
--rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.607377 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
--rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.613021 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.613691 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/
--rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
--rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.614189 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
--rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
--rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.614374 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
--rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.499833 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.499878 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.614743 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.615321 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
--rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
--rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
--rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
--rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
--rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/create_admin.sh
--rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/fab_config.py
--rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/home.js
--rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/react_admin_component.js
--rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/ui_admin_creator.py
--rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/uri_info.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.638965 ApiLogicServer-8.3.6/api_logic_server_cli/database/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/Chinook_Sqlite.sqlite
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/__init__.py
--rw-r--r--   0 val        (502) staff       (20)   545792 2023-05-02 01:22:02.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/allocation.sqlite
--rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/authentication.sqlite
--rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/classicmodels.sqlite
--rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/new.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold-plus.sqlite
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/nw.sqlite
--rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests.sqlite
--rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests.yml
--rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests_nw.yml
--rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests_nw_1.yml
--rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests_typical.yml
--rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/database/todos.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.656863 ApiLogicServer-8.3.6/api_logic_server_cli/docs/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1251 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/API-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     2647 2022-12-29 01:51:24.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/API.md
--rw-r--r--   0 val        (502) staff       (20)     3222 2022-12-21 16:33:05.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Admin-Customization.md
--rw-r--r--   0 val        (502) staff       (20)    18275 2023-03-10 04:52:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Admin-Tour.md
--rw-r--r--   0 val        (502) staff       (20)      384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Architecture-What-Is.md
--rw-r--r--   0 val        (502) staff       (20)    12713 2022-11-22 02:48:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Architecture.md
--rw-r--r--   0 val        (502) staff       (20)    61944 2022-10-11 03:42:54.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave-Logic-Report.md
--rw-r--r--   0 val        (502) staff       (20)     3838 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave.md
--rw-r--r--   0 val        (502) staff       (20)     1994 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Create-ApiLogicProject.md
--rw-r--r--   0 val        (502) staff       (20)     5319 2022-12-21 20:29:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Classes.md
--rw-r--r--   0 val        (502) staff       (20)     2660 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Customization.md
--rw-r--r--   0 val        (502) staff       (20)     1114 2023-01-27 04:14:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Examples.md
--rw-r--r--   0 val        (502) staff       (20)      970 2022-10-03 02:15:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Keys.md
--rw-r--r--   0 val        (502) staff       (20)     3898 2023-01-06 02:59:38.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Multi.md
--rw-r--r--   0 val        (502) staff       (20)    13193 2023-03-12 01:14:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Database-Connectivity.md
--rw-r--r--   0 val        (502) staff       (20)     1241 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Execute.md
--rw-r--r--   0 val        (502) staff       (20)     3273 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-Frameworks.md
--rw-r--r--   0 val        (502) staff       (20)      527 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-Low-Code.md
--rw-r--r--   0 val        (502) staff       (20)     7036 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/FAQ-RETE.md
--rw-r--r--   0 val        (502) staff       (20)     1851 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/IDE-Customize.md
--rw-r--r--   0 val        (502) staff       (20)     7532 2023-01-20 15:50:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/IDE-Execute.md
--rw-r--r--   0 val        (502) staff       (20)     6368 2023-02-04 01:50:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Eval-x.md
--rw-r--r--   0 val        (502) staff       (20)     8093 2023-01-09 21:17:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Eval.md
--rw-r--r--   0 val        (502) staff       (20)     3390 2023-02-03 23:28:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Express-x.md
--rw-r--r--   0 val        (502) staff       (20)     3539 2022-08-23 15:56:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Express.md
--rw-r--r--   0 val        (502) staff       (20)      566 2022-11-30 17:57:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-psycopg2.md
--rw-r--r--   0 val        (502) staff       (20)      977 2022-11-17 04:40:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-pyodbc.md
--rw-r--r--   0 val        (502) staff       (20)     7135 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install.md
--rw-r--r--   0 val        (502) staff       (20)    13448 2023-02-05 02:54:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Internals-CLI.md
--rw-r--r--   0 val        (502) staff       (20)     6504 2022-12-01 16:51:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Internals.md
--rw-r--r--   0 val        (502) staff       (20)     3258 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Operation.md
--rw-r--r--   0 val        (502) staff       (20)    14729 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)    10325 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Why.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic.md
--rw-r--r--   0 val        (502) staff       (20)     4205 2022-08-28 15:23:33.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Manage-GitHub.md
--rw-r--r--   0 val        (502) staff       (20)     3796 2022-12-28 03:43:06.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Builders.md
--rw-r--r--   0 val        (502) staff       (20)     1957 2022-12-22 04:40:03.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-DevOps.md
--rw-r--r--   0 val        (502) staff       (20)     1930 2023-01-31 22:36:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Env.md
--rw-r--r--   0 val        (502) staff       (20)     4936 2022-11-24 20:38:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Execution.md
--rw-r--r--   0 val        (502) staff       (20)     2446 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Rebuild.md
--rw-r--r--   0 val        (502) staff       (20)     2104 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Project-Structure.md
--rw-r--r--   0 val        (502) staff       (20)      773 2022-09-18 04:42:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Sample-Database.md
--rw-r--r--   0 val        (502) staff       (20)     2227 2023-02-14 23:54:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Activation.md
--rw-------   0 val        (502) staff       (20)     1585 2023-01-21 01:47:08.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authentication-Provider.md
--rw-------   0 val        (502) staff       (20)     1470 2023-01-21 02:17:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authentication.md
--rw-r--r--   0 val        (502) staff       (20)     1922 2023-01-06 17:06:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Authorization.md
--rw-r--r--   0 val        (502) staff       (20)     5277 2023-01-21 01:31:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Security-Overview.md
--rw-r--r--   0 val        (502) staff       (20)      155 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech--Notes.md
--rw-r--r--   0 val        (502) staff       (20)      237 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-4GL.md
--rw-r--r--   0 val        (502) staff       (20)     7081 2022-11-24 00:40:19.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-CodeSpaces.md
--rw-r--r--   0 val        (502) staff       (20)     3053 2022-12-06 21:43:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
--rw-r--r--   0 val        (502) staff       (20)     3174 2022-12-06 18:38:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     5693 2022-12-05 19:50:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Conference.md
--rw-r--r--   0 val        (502) staff       (20)     3385 2022-11-07 18:45:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Docker.md
--rw-r--r--   0 val        (502) staff       (20)      815 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Install-Python.md
--rw-r--r--   0 val        (502) staff       (20)     1049 2022-10-03 16:52:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Proven.md
--rw-r--r--   0 val        (502) staff       (20)     2679 2022-12-07 04:30:27.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Python-311.md
--rw-r--r--   0 val        (502) staff       (20)     3728 2023-01-12 06:40:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-Python.md
--rw-r--r--   0 val        (502) staff       (20)     3019 2022-10-21 23:29:01.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-m1.md
--rw-r--r--   0 val        (502) staff       (20)     1644 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tech-mkdocs-material.md
--rw-r--r--   0 val        (502) staff       (20)    12291 2022-10-08 18:23:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Troubleshooting.md
--rw-r--r--   0 val        (502) staff       (20)    15277 2023-04-27 02:31:04.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Tutorial.md
--rw-r--r--   0 val        (502) staff       (20)     6697 2022-12-02 18:42:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Working-With-Docker.md
--rw-r--r--   0 val        (502) staff       (20)     4031 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.657168 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-08-30 03:14:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.657694 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/
--rw-r--r--   0 val        (502) staff       (20)     2362 2022-08-29 00:06:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/bulb-icon.svg
--rw-r--r--   0 val        (502) staff       (20)     3482 2022-08-30 03:46:01.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/assets/images/lightbulb.svg
--rw-r--r--   0 val        (502) staff       (20)    15440 2023-02-06 03:49:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/index.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.657946 ApiLogicServer-8.3.6/api_logic_server_cli/docs/stylesheets/
--rw-r--r--   0 val        (502) staff       (20)      634 2022-08-30 03:44:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/docs/stylesheets/extra.css
--rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/extended_builder.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.659685 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/
--rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
--rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/configZZ.py
--rw-r--r--   0 val        (502) staff       (20)       63 2022-10-01 16:17:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/db_typesZZ.txt
--rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/modelsZZ.py
--rw-r--r--   0 val        (502) staff       (20)      888 2023-04-23 22:57:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/nw_virtual_attrs.py
--rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
--rw-r--r--   0 val        (502) staff       (20)     1006 2023-04-21 23:18:04.000000 ApiLogicServer-8.3.6/api_logic_server_cli/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.663139 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-04-26 02:43:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.663923 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.664187 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.665917 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1127 2023-04-29 02:28:50.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
--rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1193 2023-04-29 01:03:03.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
--rw-r--r--   0 val        (502) staff       (20)     2444 2023-04-29 01:03:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.666439 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.667442 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     2053 2023-04-26 02:48:17.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/customize_api.py
--rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/expose_api_models.py
--rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/json_encoder.py
--rw-r--r--   0 val        (502) staff       (20)     2689 2023-04-29 21:17:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/readme_customize_api.md
--rw-r--r--   0 val        (502) staff       (20)    18920 2023-04-29 18:24:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api_logic_server_run.py
--rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.668241 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.669001 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/
--rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/env.py
--rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/readme.md
--rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.669173 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/versions/
--rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
--rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic.ini
--rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/bind_databases.py
--rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/default.env
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.669347 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.670416 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/
--rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
--rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
--rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
--rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
--rw-r--r--   0 val        (502) staff       (20)     1475 2023-04-21 23:01:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logging.yml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.670906 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/
--rw-r--r--   0 val        (502) staff       (20)      592 2023-04-26 02:47:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)     5953 2023-04-27 00:49:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
--rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/mypy.ini
--rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
--rw-r--r--   0 val        (502) staff       (20)     7196 2023-05-01 21:36:23.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.ps1
--rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.671676 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.672309 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.674009 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.674506 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.674759 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.501621 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.675474 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.675708 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
--rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
--rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.676388 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/
--rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
--rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
--rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677251 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677538 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authentication.py
--rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authorization.py
--rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677815 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/templates/
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/templates/index.html
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.677966 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.678483 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
--rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.678660 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.679034 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.679596 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
--rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
--rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
--rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.680395 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/basic/
--rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/basic/server_test.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.680927 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.681290 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
--rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/home.js
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.681550 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.683307 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.684635 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.684784 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/templates/
--rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/templates/content.html
--rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/util.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.686333 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/
--rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/py.py
--rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
--rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
--rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
--rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
--rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.686886 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-05-02 02:53:53.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.688462 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/
--rw-r--r--   0 val        (502) staff       (20)   670261 2023-05-02 02:18:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/db.png
--rw-r--r--   0 val        (502) staff       (20)  1035433 2023-05-02 02:18:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/logic-diagram.png
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.689976 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/logic/
--rw-r--r--   0 val        (502) staff       (20)     1398 2023-05-02 01:22:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)     7982 2023-05-02 04:11:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/readme-allocation.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.690104 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/test/
--rw-r--r--   0 val        (502) staff       (20)      583 2023-05-02 01:22:37.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/test/test.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.690670 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/
--rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.690901 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/
--rw-r--r--   0 val        (502) staff       (20)     8711 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/customize_api.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.691691 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/
--rw-r--r--   0 val        (502) staff       (20)    34142 2023-04-29 21:00:10.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
--rw-r--r--   0 val        (502) staff       (20)      650 2023-04-29 21:02:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.692616 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/
--rw-r--r--   0 val        (502) staff       (20)     2664 2023-05-01 21:01:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/customize_models.py
--rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/db_debug.py
--rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
--rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.692864 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/logic/
--rw-r--r--   0 val        (502) staff       (20)    10650 2023-04-23 00:10:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
--rw-r--r--   0 val        (502) staff       (20)      241 2023-04-29 21:06:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.693122 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/security/
--rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/security/declare_security.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.693341 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.693427 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.694015 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
--rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
--rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
--rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
--rw-r--r--   0 val        (502) staff       (20)      473 2023-04-23 23:42:07.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.695081 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
--rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
--rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
--rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
--rw-r--r--   0 val        (502) staff       (20)     4722 2023-04-23 23:41:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.695381 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
--rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.697007 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
--rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
--rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
--rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
--rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.697668 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.699152 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/
--rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
--rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
--rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
--rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
--rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
--rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
--rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
--rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
--rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
--rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
--rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.699309 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/
--rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.700192 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/
--rw-r--r--   0 val        (502) staff       (20)    17259 2023-04-24 23:38:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
--rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.700577 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/
--rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.702294 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/
--rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
--rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
--rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
--rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
--rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
--rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
--rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
--rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.703628 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
--rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
--rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
--rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
--rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
--rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
--rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
--rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
--rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
--rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.703770 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw_no_cust/
--rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.705211 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.706957 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/
--rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
--rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
--rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
--rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.gitignore
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.707251 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.710227 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
--rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
--rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
--rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
--rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
--rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
--rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
--rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.710840 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/
--rw-r--r--   0 val        (502) staff       (20)     5986 2023-04-13 16:51:25.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/launch.json
--rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/settings.json
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.712564 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.713627 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.713810 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
--rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
--rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.715365 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.715656 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
--rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
--rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
--rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
--rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
--rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
--rw-r--r--   0 val        (502) staff       (20)    21134 2023-04-14 00:57:12.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/readme.md
--rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/requirements.txt
--rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/sample_db.sqlite
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.717265 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/
--rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
--rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
--rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.721291 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    21445 2023-04-29 17:29:36.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
--rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.722688 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
--rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
--rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.723184 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
--rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.724239 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.725479 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
--rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
--rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
--rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
--rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.726084 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
--rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
--rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
--rwxr-xr-x   0 val        (502) staff       (20)    17236 2023-04-29 17:29:32.000000 ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-02 04:14:08.728259 ApiLogicServer-8.3.6/api_logic_server_cli/templates/
--rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/admin.yaml
--rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.md
--rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.txt
--rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/index.html
--rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/login_endpoint.txt
--rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.3.6/api_logic_server_cli/templates/login_endpoint_imports.txt
--rw-r--r--   0 val        (502) staff       (20)       38 2023-05-02 04:14:08.728977 ApiLogicServer-8.3.6/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)     3521 2023-04-26 19:16:06.000000 ApiLogicServer-8.3.6/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.729780 ApiLogicServer-8.4.0/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.552962 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/
+-rw-r--r--   0 val        (502) staff       (20)    14906 2023-05-08 02:38:24.000000 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    51376 2023-05-08 02:38:24.000000 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-05-08 02:38:24.000000 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (502) staff       (20)       66 2023-05-08 02:38:24.000000 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/entry_points.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-05-08 02:38:24.000000 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/not-zip-safe
+-rw-r--r--   0 val        (502) staff       (20)      585 2023-05-08 02:38:24.000000 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/requires.txt
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-05-08 02:38:24.000000 ApiLogicServer-8.4.0/ApiLogicServer.egg-info/top_level.txt
+-rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/LICENSE
+-rw-r--r--   0 val        (502) staff       (20)      804 2023-05-02 03:36:56.000000 ApiLogicServer-8.4.0/MANIFEST.in
+-rw-r--r--   0 val        (502) staff       (20)    14906 2023-05-08 02:38:24.729530 ApiLogicServer-8.4.0/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    13917 2023-05-08 01:36:48.000000 ApiLogicServer-8.4.0/README.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.555034 ApiLogicServer-8.4.0/api_logic_server_cli/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    60713 2023-05-08 01:36:18.000000 ApiLogicServer-8.4.0/api_logic_server_cli/api_logic_server.py
+-rw-r--r--   0 val        (502) staff       (20)      151 2023-05-08 01:22:49.000000 ApiLogicServer-8.4.0/api_logic_server_cli/api_logic_server_info.yaml
+-rw-r--r--   0 val        (502) staff       (20)    33430 2023-03-10 20:22:39.000000 ApiLogicServer-8.4.0/api_logic_server_cli/cli.py
+-rw-r--r--   0 val        (502) staff       (20)     1001 2023-04-02 18:24:38.000000 ApiLogicServer-8.4.0/api_logic_server_cli/cli_args_base.py
+-rw-r--r--   0 val        (502) staff       (20)     3184 2023-04-02 23:08:24.000000 ApiLogicServer-8.4.0/api_logic_server_cli/cli_args_project.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.558136 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-26 18:43:59.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-10 15:34:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.564141 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-11-10 15:35:23.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      189 2023-02-26 22:48:45.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2601 2022-11-18 17:28:18.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3049 2023-02-05 16:19:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5270 2023-05-06 02:48:51.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     7174 2023-02-10 20:33:17.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    13709 2023-05-02 02:08:40.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21342 2023-02-05 16:19:42.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    35378 2023-02-26 22:48:45.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4053 2023-01-18 01:12:07.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    20087 2023-02-05 19:25:01.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    37019 2023-02-26 23:03:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2274 2023-02-26 20:50:53.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2617 2023-03-12 04:54:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5260 2023-05-06 02:48:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py
+-rw-r--r--   0 val        (502) staff       (20)    11680 2023-05-02 02:02:21.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py
+-rw-r--r--   0 val        (502) staff       (20)    34401 2023-02-05 02:48:22.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/model_creation_services.py
+-rw-r--r--   0 val        (502) staff       (20)     6127 2023-01-18 01:12:06.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.566338 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store
+-rwxrwxrwx   0 val        (502) staff       (20)    15430 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.566498 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/
+-rwxrwxrwx   0 val        (502) staff       (20)  1145966 2023-01-15 08:58:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json
+-rwxrwxrwx   0 val        (502) staff       (20)     3870 2023-01-15 08:58:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico
+-rwxrwxrwx   0 val        (502) staff       (20)      692 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html
+-rwxrwxrwx   0 val        (502) staff       (20)     5347 2023-01-15 08:58:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png
+-rwxrwxrwx   0 val        (502) staff       (20)     9664 2023-01-15 08:58:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png
+-rwxrwxrwx   0 val        (502) staff       (20)      492 2023-01-15 08:58:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/manifest.json
+-rwxrwxrwx   0 val        (502) staff       (20)       67 2023-01-15 08:58:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/robots.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.545276 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.568907 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/
+-rwxrwxrwx   0 val        (502) staff       (20)    86781 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css
+-rwxrwxrwx   0 val        (502) staff       (20)   166928 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map
+-rwxrwxrwx   0 val        (502) staff       (20)      211 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css
+-rwxrwxrwx   0 val        (502) staff       (20)      516 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.634420 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/
+-rwxrwxrwx   0 val        (502) staff       (20)     1576 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3197 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9011 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    21905 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2921 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7103 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1004 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     2792 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7546 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17381 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    33520 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    71153 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14043 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    36857 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5595 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    14138 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6135 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    14288 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2280 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5953 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8068 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4407 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10552 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2156 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5783 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11957 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24504 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5499 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13356 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4187 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10856 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7001 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    17447 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3591 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8746 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3747 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9475 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3140 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7634 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4056 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9168 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8184 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18882 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4068 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9104 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    14317 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    32894 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3963 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9547 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3152 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8052 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8662 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    20172 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4982 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13442 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6569 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    15183 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2002 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4736 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2974 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7499 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1967 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5172 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5948 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    10454 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    23458 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1255 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     3229 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4128 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10303 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17096 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    31009 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7760 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    18142 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9800 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21207 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3420 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8828 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3820 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10430 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    41393 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   145206 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5605 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    13185 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8412 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19971 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9916 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    22155 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     6545 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16602 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4681 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11819 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3545 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8963 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3710 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9146 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1924 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4864 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11830 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3092 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8217 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2417 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6013 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7472 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    16988 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2342 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6267 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  3310604 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      576 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20) 10838575 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    35620 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   121512 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    17547 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    39845 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2594 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6567 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2814 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7255 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    18754 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    38065 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2736 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     7008 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2693 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6865 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3378 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8159 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2709 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6645 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4619 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10592 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4203 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    10608 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2559 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     6522 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5926 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    96741 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1840 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5116 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     8013 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    19497 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3725 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     9025 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3288 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8254 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2026 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     5528 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    13558 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    26650 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     9201 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    21765 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5069 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    11826 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    34921 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)   119930 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4669 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10814 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     4316 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    10868 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)    11414 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    24817 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     2622 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)     7016 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     5259 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)    13615 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     7391 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)    17258 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     1986 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     4960 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)     3230 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js
+-rwxrwxrwx   0 val        (502) staff       (20)      387 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)     8177 2023-01-15 08:59:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map
+-rwxrwxrwx   0 val        (502) staff       (20)  1384276 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js
+-rwxrwxrwx   0 val        (502) staff       (20)     3014 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt
+-rwxrwxrwx   0 val        (502) staff       (20)  5552838 2023-01-15 08:59:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.638630 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/
+-rwxrwxrwx   0 val        (502) staff       (20)    72504 2023-01-15 08:59:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.644377 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.645022 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/
+-rw-r--r--   0 val        (502) staff       (20)       55 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/.gitignore
+-rw-r--r--   0 val        (502) staff       (20)      389 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/README.rst
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.645460 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/
+-rw-r--r--   0 val        (502) staff       (20)      742 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)      276 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/models.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.645625 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/
+-rw-r--r--   0 val        (502) staff       (20)      124 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/templates/404.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.545593 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.545634 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.645908 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 val        (502) staff       (20)      483 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 val        (502) staff       (20)      727 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 val        (502) staff       (20)      938 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.646217 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/
+-rw-r--r--   0 val        (502) staff       (20)       64 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/babel.cfg
+-rw-r--r--   0 val        (502) staff       (20)      662 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot
+-rw-r--r--   0 val        (502) staff       (20)     3669 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py
+-rw-r--r--   0 val        (502) staff       (20)       68 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/run.py
+-rw-r--r--   0 val        (502) staff       (20)      556 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/create_admin.sh
+-rw-r--r--   0 val        (502) staff       (20)      624 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/fab_config.py
+-rw-r--r--   0 val        (502) staff       (20)     2683 2023-02-05 02:49:11.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/home.js
+-rw-r--r--   0 val        (502) staff       (20)     3121 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js
+-rw-r--r--   0 val        (502) staff       (20)    35694 2023-02-05 19:24:16.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/ui_admin_creator.py
+-rw-r--r--   0 val        (502) staff       (20)     2252 2023-03-12 01:14:25.000000 ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/uri_info.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.659855 ApiLogicServer-8.4.0/api_logic_server_cli/database/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-22 22:39:55.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)  1067008 2022-10-11 15:13:39.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)   545792 2023-05-02 01:22:02.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/allocation.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    45056 2023-01-19 01:03:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/authentication.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   413696 2022-12-26 21:41:55.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/classicmodels.sqlite
+-rw-r--r--   0 val        (502) staff       (20)      122 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)    16384 2023-03-07 00:17:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/new.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/nw-gold-plus.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-03-19 18:51:02.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)   496640 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/nw.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    32768 2023-03-08 04:23:41.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/table_filters_tests.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       53 2023-03-08 15:53:51.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/table_filters_tests.yml
+-rw-r--r--   0 val        (502) staff       (20)       23 2023-04-06 03:07:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/table_filters_tests_nw.yml
+-rw-r--r--   0 val        (502) staff       (20)       25 2023-04-06 03:06:34.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/table_filters_tests_nw_1.yml
+-rw-r--r--   0 val        (502) staff       (20)       21 2023-03-14 16:06:21.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/table_filters_tests_typical.yml
+-rw-r--r--   0 val        (502) staff       (20)    16384 2022-12-31 01:13:31.000000 ApiLogicServer-8.4.0/api_logic_server_cli/database/todos.sqlite
+-rw-r--r--   0 val        (502) staff       (20)    11824 2023-02-11 04:16:18.000000 ApiLogicServer-8.4.0/api_logic_server_cli/extended_builder.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.661783 ApiLogicServer-8.4.0/api_logic_server_cli/fragments/
+-rw-r--r--   0 val        (502) staff       (20)     1431 2023-02-05 02:48:13.000000 ApiLogicServer-8.4.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py
+-rw-r--r--   0 val        (502) staff       (20)     1956 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/fragments/configZZ.py
+-rw-r--r--   0 val        (502) staff       (20)       63 2022-10-01 16:17:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/fragments/db_typesZZ.txt
+-rw-r--r--   0 val        (502) staff       (20)    12053 2023-02-05 02:48:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/fragments/modelsZZ.py
+-rw-r--r--   0 val        (502) staff       (20)      888 2023-04-23 22:57:22.000000 ApiLogicServer-8.4.0/api_logic_server_cli/fragments/nw_virtual_attrs.py
+-rw-r--r--   0 val        (502) staff       (20)      870 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
+-rw-r--r--   0 val        (502) staff       (20)     1006 2023-04-21 23:18:04.000000 ApiLogicServer-8.4.0/api_logic_server_cli/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.664936 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-04-26 02:43:32.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.665623 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      444 2023-02-05 02:50:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 21:44:41.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-08 18:52:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      106 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.665874 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:37.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.667565 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:32:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1127 2023-04-29 02:28:50.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml
+-rw-r--r--   0 val        (502) staff       (20)     1306 2022-04-03 03:00:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1196 2022-04-03 03:00:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1205 2022-04-03 03:00:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1193 2023-04-29 01:03:03.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml
+-rw-r--r--   0 val        (502) staff       (20)     2444 2023-04-29 01:03:22.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.668058 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     6518 2023-04-13 16:38:20.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      437 2023-04-13 04:29:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.669147 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     2053 2023-04-26 02:48:17.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/customize_api.py
+-rw-r--r--   0 val        (502) staff       (20)      316 2023-01-23 01:07:06.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/expose_api_models.py
+-rw-r--r--   0 val        (502) staff       (20)      521 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/json_encoder.py
+-rw-r--r--   0 val        (502) staff       (20)     2689 2023-04-29 21:17:10.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/readme_customize_api.md
+-rw-r--r--   0 val        (502) staff       (20)    18920 2023-04-29 18:24:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api_logic_server_run.py
+-rw-r--r--   0 val        (502) staff       (20)     3131 2023-03-03 16:08:15.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.669987 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.670679 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/
+-rw-r--r--   0 val        (502) staff       (20)     2101 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/env.py
+-rw-r--r--   0 val        (502) staff       (20)     1967 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/readme.md
+-rw-r--r--   0 val        (502) staff       (20)      494 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/script.py.mako
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.670813 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/versions/
+-rw-r--r--   0 val        (502) staff       (20)       60 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     3027 2023-02-09 15:42:27.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic.ini
+-rw-r--r--   0 val        (502) staff       (20)      537 2023-01-28 17:53:13.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/bind_databases.py
+-rw-r--r--   0 val        (502) staff       (20)      469 2023-01-23 01:14:38.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      139 2022-12-21 03:23:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/default.env
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.670949 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.672145 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/
+-rw-r--r--   0 val        (502) staff       (20)     2381 2023-02-26 22:13:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     3643 2023-02-25 03:16:21.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
+-rw-r--r--   0 val        (502) staff       (20)      331 2023-04-02 15:52:20.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     2079 2023-04-02 16:35:31.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh
+-rw-r--r--   0 val        (502) staff       (20)      876 2023-01-07 21:19:34.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.672443 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/python-anywhere/
+-rw-r--r--   0 val        (502) staff       (20)     3820 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py
+-rw-r--r--   0 val        (502) staff       (20)     1475 2023-04-21 23:01:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/logging.yml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.672941 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/logic/
+-rw-r--r--   0 val        (502) staff       (20)      592 2023-04-26 02:47:32.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)     5953 2023-04-27 00:49:20.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
+-rw-r--r--   0 val        (502) staff       (20)      568 2023-03-04 03:52:49.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/mypy.ini
+-rw-r--r--   0 val        (502) staff       (20)     7435 2023-05-06 03:47:04.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)      801 2022-10-19 20:24:10.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/run.ps1
+-rwxr-xr-x   0 val        (502) staff       (20)     1040 2022-11-09 16:08:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/run.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.673568 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-15 01:50:41.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.674143 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-12-18 05:06:14.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-12-14 21:51:49.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.675859 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      173 2022-12-14 21:55:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      928 2022-12-19 03:03:12.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1803 2022-12-18 03:38:13.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      820 2022-12-16 14:20:29.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1392 2022-12-14 22:25:00.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1024 2022-12-16 15:01:05.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1619 2022-12-15 17:24:50.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      580 2022-12-19 03:03:11.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.676515 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.676782 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1493 2022-12-19 03:13:00.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     4355 2023-01-24 04:07:34.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)     2907 2023-01-24 04:07:34.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.547006 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.677659 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1215 2022-12-19 03:24:21.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     2262 2022-12-19 00:39:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      839 2022-12-18 03:49:32.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.677937 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/
+-rw-r--r--   0 val        (502) staff       (20)     2165 2023-02-15 02:24:49.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py
+-rw-r--r--   0 val        (502) staff       (20)      587 2023-01-23 01:02:25.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.678843 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/notes_temp/
+-rw-r--r--   0 val        (502) staff       (20)     1403 2023-01-12 23:08:16.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt
+-rw-r--r--   0 val        (502) staff       (20)     1156 2023-01-12 23:08:16.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt
+-rw-r--r--   0 val        (502) staff       (20)     1364 2023-01-12 23:29:28.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.679557 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.679831 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     4665 2022-12-19 03:03:12.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3425 2023-03-03 16:56:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/authentication.py
+-rw-r--r--   0 val        (502) staff       (20)     6004 2023-03-03 16:56:55.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/authorization.py
+-rw-r--r--   0 val        (502) staff       (20)     1705 2023-02-13 15:35:11.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.680093 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/templates/
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/templates/index.html
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.680241 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.680735 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     9969 2022-11-29 03:36:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py
+-rw-r--r--   0 val        (502) staff       (20)     1026 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.680894 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      414 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/about.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.681191 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      416 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     1518 2023-02-11 17:50:21.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.681969 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/
+-rw-r--r--   0 val        (502) staff       (20)      147 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro micro.md
+-rw-r--r--   0 val        (502) staff       (20)     3707 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md
+-rw-r--r--   0 val        (502) staff       (20)    65295 2022-10-11 03:42:40.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.682765 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)      735 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/basic/server_test.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.683242 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-01-22 20:09:13.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.683607 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)     6671 2023-03-19 18:44:09.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py
+-rw-r--r--   0 val        (502) staff       (20)     2750 2023-02-05 02:50:52.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/admin/home.js
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.683858 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-26 23:48:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.685674 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.686806 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.687060 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/templates/
+-rw-r--r--   0 val        (502) staff       (20)       26 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/templates/content.html
+-rw-r--r--   0 val        (502) staff       (20)     9076 2023-03-24 00:43:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/util.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.689081 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/
+-rwxr-xr-x   0 val        (502) staff       (20)     3116 2023-03-10 20:26:13.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/py.py
+-rw-r--r--   0 val        (502) staff       (20)      738 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
+-rw-r--r--   0 val        (502) staff       (20)      579 2023-03-03 02:36:32.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-02-05 02:50:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
+-rw-r--r--   0 val        (502) staff       (20)      698 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1
+-rw-r--r--   0 val        (502) staff       (20)      893 2023-02-05 02:50:58.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.689593 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-05-02 02:53:53.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     7733 2023-05-03 01:13:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/Logic-Allocation.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.548210 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/images/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.691338 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/images/allocation/
+-rw-r--r--   0 val        (502) staff       (20)   670261 2023-05-02 02:18:30.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/images/allocation/db.png
+-rw-r--r--   0 val        (502) staff       (20)  1035433 2023-05-02 02:18:30.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/images/allocation/logic-diagram.png
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.692857 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/logic/
+-rw-r--r--   0 val        (502) staff       (20)     1398 2023-05-02 01:22:37.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.693132 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/test/
+-rw-r--r--   0 val        (502) staff       (20)      583 2023-05-02 01:22:37.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/test/test.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.694072 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/
+-rw-r--r--   0 val        (502) staff       (20)    10244 2023-05-07 15:12:04.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)    15278 2023-05-07 14:43:29.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/Tutorial.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.694437 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/
+-rw-r--r--   0 val        (502) staff       (20)     8709 2023-05-06 02:58:04.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.695298 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/
+-rw-r--r--   0 val        (502) staff       (20)    34142 2023-04-29 21:00:10.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
+-rw-r--r--   0 val        (502) staff       (20)      650 2023-04-29 21:02:15.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.696174 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/database/
+-rw-r--r--   0 val        (502) staff       (20)     2664 2023-05-01 21:01:40.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py
+-rw-r--r--   0 val        (502) staff       (20)      312 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/database/db_debug.py
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-11-16 19:24:28.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
+-rw-r--r--   0 val        (502) staff       (20)       29 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/database/restore_sample_db.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.696439 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/logic/
+-rw-r--r--   0 val        (502) staff       (20)    10678 2023-05-06 02:54:13.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py
+-rw-r--r--   0 val        (502) staff       (20)      241 2023-05-07 04:56:34.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.696682 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/security/
+-rw-r--r--   0 val        (502) staff       (20)     1158 2023-02-14 15:54:30.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.696914 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.697010 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.697538 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/
+-rw-r--r--   0 val        (502) staff       (20)      187 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/about.feature
+-rw-r--r--   0 val        (502) staff       (20)      285 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/api.feature
+-rw-r--r--   0 val        (502) staff       (20)     1281 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature
+-rw-r--r--   0 val        (502) staff       (20)      473 2023-04-23 23:42:07.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/salary_change.feature
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.698693 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/
+-rw-r--r--   0 val        (502) staff       (20)      450 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/about.py
+-rw-r--r--   0 val        (502) staff       (20)     2130 2023-01-14 03:27:19.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py
+-rw-r--r--   0 val        (502) staff       (20)    16642 2023-02-16 04:52:22.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py
+-rw-r--r--   0 val        (502) staff       (20)     4722 2023-04-23 23:41:49.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.698985 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/
+-rw-r--r--   0 val        (502) staff       (20)     4356 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.700458 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     5794 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log
+-rw-r--r--   0 val        (502) staff       (20)     2568 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log
+-rw-r--r--   0 val        (502) staff       (20)     8481 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log
+-rw-r--r--   0 val        (502) staff       (20)     8445 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log
+-rw-r--r--   0 val        (502) staff       (20)     2561 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.701146 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.702935 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/
+-rw-r--r--   0 val        (502) staff       (20)     5070 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log
+-rw-r--r--   0 val        (502) staff       (20)     8652 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/BEGIN.log
+-rw-r--r--   0 val        (502) staff       (20)    16926 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log
+-rw-r--r--   0 val        (502) staff       (20)     6095 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log
+-rw-r--r--   0 val        (502) staff       (20)      840 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_self-reln_Dept-SubDep.log
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/GET_test_on_Order.log
+-rw-r--r--   0 val        (502) staff       (20)     1381 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log
+-rw-r--r--   0 val        (502) staff       (20)      831 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log
+-rw-r--r--   0 val        (502) staff       (20)     2256 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log
+-rw-r--r--   0 val        (502) staff       (20)     8405 2023-03-10 20:26:58.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py
+-rw-r--r--   0 val        (502) staff       (20)    13497 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py
+-rw-r--r--   0 val        (502) staff       (20)     1543 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.703132 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/
+-rw-r--r--   0 val        (502) staff       (20)     8196 2022-11-11 23:20:49.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.704136 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/admin/
+-rw-r--r--   0 val        (502) staff       (20)    17259 2023-04-24 23:38:28.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     3443 2023-02-05 02:51:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js
+-rw-r--r--   0 val        (502) staff       (20)     8798 2022-12-30 19:58:21.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.704570 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2022-11-11 23:17:05.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.706085 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/
+-rw-r--r--   0 val        (502) staff       (20)     6054 2008-04-22 03:46:52.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif
+-rw-r--r--   0 val        (502) staff       (20)     7324 2008-04-22 03:47:14.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif
+-rw-r--r--   0 val        (502) staff       (20)     7751 2008-04-22 03:47:30.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif
+-rw-r--r--   0 val        (502) staff       (20)     7022 2008-04-22 03:47:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif
+-rw-r--r--   0 val        (502) staff       (20)     6136 2008-04-22 03:47:58.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif
+-rw-r--r--   0 val        (502) staff       (20)     7268 2008-04-22 03:49:00.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif
+-rw-r--r--   0 val        (502) staff       (20)     7633 2008-04-22 03:49:44.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif
+-rw-r--r--   0 val        (502) staff       (20)     8469 2008-04-22 03:50:18.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.707438 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/
+-rw-r--r--   0 val        (502) staff       (20)     3719 2008-04-22 03:50:34.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3715 2008-04-22 03:48:32.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4425 2008-04-22 03:49:28.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg
+-rw-r--r--   0 val        (502) staff       (20)     5404 2008-04-22 03:51:58.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3778 2008-04-22 03:51:40.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3737 2008-04-22 03:50:00.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3750 2008-04-22 03:48:16.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg
+-rw-r--r--   0 val        (502) staff       (20)     3862 2008-04-22 03:48:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg
+-rw-r--r--   0 val        (502) staff       (20)     4375 2008-04-22 03:49:14.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.707599 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw_no_cust/
+-rw-r--r--   0 val        (502) staff       (20)     5431 2023-02-05 02:51:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.708908 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:04:24.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.710455 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.devcontainer/
+-rw-r--r--   0 val        (502) staff       (20)      446 2023-02-05 02:55:30.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.devcontainer/For_VSCode.dockerfile
+-rw-r--r--   0 val        (502) staff       (20)     1932 2023-02-05 02:52:45.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json
+-rw-r--r--   0 val        (502) staff       (20)      288 2023-01-25 20:14:39.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.devcontainer/setup.sh
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-01-25 20:14:39.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.gitignore
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.710693 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 06:05:31.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.713035 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-14 05:30:57.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)     1141 2023-02-14 05:35:26.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml
+-rw-r--r--   0 val        (502) staff       (20)     1162 2023-02-14 05:07:31.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml
+-rw-r--r--   0 val        (502) staff       (20)     1174 2023-02-14 05:17:54.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml
+-rw-r--r--   0 val        (502) staff       (20)     1148 2023-02-14 05:35:26.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml
+-rw-r--r--   0 val        (502) staff       (20)     1160 2023-02-14 05:35:26.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml
+-rw-r--r--   0 val        (502) staff       (20)     1142 2023-02-14 05:16:08.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml
+-rw-r--r--   0 val        (502) staff       (20)     1204 2023-02-14 05:54:42.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml
+-rw-r--r--   0 val        (502) staff       (20)     1386 2023-02-14 05:54:42.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.713508 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.vscode/
+-rw-r--r--   0 val        (502) staff       (20)     7535 2023-05-07 16:35:42.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.vscode/launch.json
+-rw-r--r--   0 val        (502) staff       (20)      100 2023-01-25 20:14:39.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.vscode/settings.json
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.715323 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-02-27 01:16:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.716443 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     1238 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3435 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3970 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     3439 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)     5965 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.716595 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/
+-rw-r--r--   0 val        (502) staff       (20)     2895 2023-02-28 05:23:15.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py
+-rw-r--r--   0 val        (502) staff       (20)     2058 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.718017 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.718247 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)     8571 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)    11838 2023-01-28 17:14:40.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py
+-rw-r--r--   0 val        (502) staff       (20)     1452 2023-02-27 23:00:55.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py
+-rw-r--r--   0 val        (502) staff       (20)     1400 2023-01-25 20:14:56.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml
+-rw-r--r--   0 val        (502) staff       (20)     3530 2023-02-28 05:20:39.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md
+-rw-r--r--   0 val        (502) staff       (20)     7699 2023-02-13 15:35:11.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py
+-rw-r--r--   0 val        (502) staff       (20)    22117 2023-05-07 05:28:10.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/readme.md
+-rw-r--r--   0 val        (502) staff       (20)       14 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/requirements.txt
+-rw-r--r--   0 val        (502) staff       (20)   522240 2023-04-02 02:53:45.000000 ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/sample_db.sqlite
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.719710 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/
+-rw-r--r--   0 val        (502) staff       (20)     6148 2023-01-22 18:56:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store
+-rw-r--r--   0 val        (502) staff       (20)      369 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/Readme.md
+-rw-r--r--   0 val        (502) staff       (20)        0 2023-01-03 23:29:33.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.722252 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      175 2023-01-03 23:29:48.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      191 2023-02-26 22:48:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     8054 2022-11-17 03:31:49.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    14080 2023-02-17 01:02:20.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    21445 2023-04-29 17:29:36.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)     1755 2023-02-01 19:08:47.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    53944 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt
+-rw-r--r--   0 val        (502) staff       (20)       54 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/requirements.txt
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.723703 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)     1850 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml
+-rw-r--r--   0 val        (502) staff       (20)     2593 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst
+-rw-r--r--   0 val        (502) staff       (20)     3865 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.724095 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      183 2022-08-15 21:21:51.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      203 2023-02-26 22:48:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)       87 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/pyproject.toml
+-rw-r--r--   0 val        (502) staff       (20)     1399 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)      196 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.725011 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.726205 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/
+-rw-r--r--   0 val        (502) staff       (20)      195 2022-08-15 21:21:51.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)      215 2023-02-26 22:48:46.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    32358 2023-02-05 16:19:43.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc
+-rw-r--r--   0 val        (502) staff       (20)    74447 2023-04-06 14:36:23.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc
+-rw-r--r--   0 val        (502) staff       (20)    58988 2023-04-06 14:31:39.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py
+-rw-r--r--   0 val        (502) staff       (20)     3252 2022-11-18 19:19:33.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.727023 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/
+-rw-r--r--   0 val        (502) staff       (20)    33384 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py
+-rw-r--r--   0 val        (502) staff       (20)      440 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tox.ini
+-rwxr-xr-x   0 val        (502) staff       (20)    17236 2023-04-29 17:29:32.000000 ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-05-08 02:38:24.729209 ApiLogicServer-8.4.0/api_logic_server_cli/templates/
+-rw-r--r--   0 val        (502) staff       (20)    14864 2023-03-29 21:47:30.000000 ApiLogicServer-8.4.0/api_logic_server_cli/templates/admin.yaml
+-rw-r--r--   0 val        (502) staff       (20)     1221 2023-03-29 20:25:21.000000 ApiLogicServer-8.4.0/api_logic_server_cli/templates/app_fiddle.md
+-rw-r--r--   0 val        (502) staff       (20)     3322 2023-04-13 17:12:40.000000 ApiLogicServer-8.4.0/api_logic_server_cli/templates/app_fiddle.txt
+-rw-r--r--   0 val        (502) staff       (20)     3765 2022-08-15 19:22:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/templates/index.html
+-rw-r--r--   0 val        (502) staff       (20)      900 2023-01-19 01:43:35.000000 ApiLogicServer-8.4.0/api_logic_server_cli/templates/login_endpoint.txt
+-rw-r--r--   0 val        (502) staff       (20)      205 2023-01-19 01:44:07.000000 ApiLogicServer-8.4.0/api_logic_server_cli/templates/login_endpoint_imports.txt
+-rw-r--r--   0 val        (502) staff       (20)       38 2023-05-08 02:38:24.729814 ApiLogicServer-8.4.0/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)     3521 2023-05-08 00:44:38.000000 ApiLogicServer-8.4.0/setup.py
```

### Comparing `ApiLogicServer-8.3.6/ApiLogicServer.egg-info/PKG-INFO` & `ApiLogicServer-8.4.0/ApiLogicServer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.3.6
+Version: 8.4.0
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -257,20 +257,21 @@
 * [Extensible Rules](https://dzone.com/articles/logic-bank-now-extensible-drive-95-automation-even) - defining new rule types, using Python
 * [Declarative](https://dzone.com/articles/agile-design-automation-how-are-rules-different-fr) - exploring _multi-statement_ declarative technology
 * [Automate Business Logic With Logic Bank](https://dzone.com/articles/automate-business-logic-with-logic-bank) - general introduction, discussions of extensibility, manageability and scalability
 * [Agile Design Automation With Logic Bank](https://dzone.com/articles/logical-data-indendence) - focuses on automation, design flexibility and agile iterations
 * [Instant Web Apps](https://dzone.com/articles/instant-db-web-apps) 
 
 
-
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+05/07/2023 - 08.04.00: safrs 3.0.4, tutorial demo notes, rm cli/docs, move pythonanywhere
+
 05/01/2023 - 08.03.06: allocation sample
 
 04/29/2023 - 08.03.03: restore missing debug info for open database failures
 
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
```

### Comparing `ApiLogicServer-8.3.6/ApiLogicServer.egg-info/SOURCES.txt` & `ApiLogicServer-8.4.0/ApiLogicServer.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -328,98 +328,27 @@
 api_logic_server_cli/database/nw.sqlite
 api_logic_server_cli/database/table_filters_tests.sqlite
 api_logic_server_cli/database/table_filters_tests.yml
 api_logic_server_cli/database/table_filters_tests_nw.yml
 api_logic_server_cli/database/table_filters_tests_nw_1.yml
 api_logic_server_cli/database/table_filters_tests_typical.yml
 api_logic_server_cli/database/todos.sqlite
-api_logic_server_cli/docs/.DS_Store
-api_logic_server_cli/docs/API-Customize.md
-api_logic_server_cli/docs/API.md
-api_logic_server_cli/docs/Admin-Customization.md
-api_logic_server_cli/docs/Admin-Tour.md
-api_logic_server_cli/docs/Architecture-What-Is.md
-api_logic_server_cli/docs/Architecture.md
-api_logic_server_cli/docs/Behave-Logic-Report.md
-api_logic_server_cli/docs/Behave.md
-api_logic_server_cli/docs/Create-ApiLogicProject.md
-api_logic_server_cli/docs/Data-Model-Classes.md
-api_logic_server_cli/docs/Data-Model-Customization.md
-api_logic_server_cli/docs/Data-Model-Examples.md
-api_logic_server_cli/docs/Data-Model-Keys.md
-api_logic_server_cli/docs/Data-Model-Multi.md
-api_logic_server_cli/docs/Database-Connectivity.md
-api_logic_server_cli/docs/Execute.md
-api_logic_server_cli/docs/FAQ-Frameworks.md
-api_logic_server_cli/docs/FAQ-Low-Code.md
-api_logic_server_cli/docs/FAQ-RETE.md
-api_logic_server_cli/docs/IDE-Customize.md
-api_logic_server_cli/docs/IDE-Execute.md
-api_logic_server_cli/docs/Install-Eval-x.md
-api_logic_server_cli/docs/Install-Eval.md
-api_logic_server_cli/docs/Install-Express-x.md
-api_logic_server_cli/docs/Install-Express.md
-api_logic_server_cli/docs/Install-psycopg2.md
-api_logic_server_cli/docs/Install-pyodbc.md
-api_logic_server_cli/docs/Install.md
-api_logic_server_cli/docs/Internals-CLI.md
-api_logic_server_cli/docs/Internals.md
-api_logic_server_cli/docs/Logic-Operation.md
-api_logic_server_cli/docs/Logic-Tutorial.md
-api_logic_server_cli/docs/Logic-Why.md
-api_logic_server_cli/docs/Logic.md
-api_logic_server_cli/docs/Manage-GitHub.md
-api_logic_server_cli/docs/Project-Builders.md
-api_logic_server_cli/docs/Project-DevOps.md
-api_logic_server_cli/docs/Project-Env.md
-api_logic_server_cli/docs/Project-Execution.md
-api_logic_server_cli/docs/Project-Rebuild.md
-api_logic_server_cli/docs/Project-Structure.md
-api_logic_server_cli/docs/Sample-Database.md
-api_logic_server_cli/docs/Security-Activation.md
-api_logic_server_cli/docs/Security-Authentication-Provider.md
-api_logic_server_cli/docs/Security-Authentication.md
-api_logic_server_cli/docs/Security-Authorization.md
-api_logic_server_cli/docs/Security-Overview.md
-api_logic_server_cli/docs/Tech--Notes.md
-api_logic_server_cli/docs/Tech-4GL.md
-api_logic_server_cli/docs/Tech-CodeSpaces.md
-api_logic_server_cli/docs/Tech-Conference-PyCon23-Talk.md
-api_logic_server_cli/docs/Tech-Conference-PyCon23-Tutorial.md
-api_logic_server_cli/docs/Tech-Conference.md
-api_logic_server_cli/docs/Tech-Docker.md
-api_logic_server_cli/docs/Tech-Install-Python.md
-api_logic_server_cli/docs/Tech-Proven.md
-api_logic_server_cli/docs/Tech-Python-311.md
-api_logic_server_cli/docs/Tech-Python.md
-api_logic_server_cli/docs/Tech-m1.md
-api_logic_server_cli/docs/Tech-mkdocs-material.md
-api_logic_server_cli/docs/Troubleshooting.md
-api_logic_server_cli/docs/Tutorial.md
-api_logic_server_cli/docs/Working-With-Docker.md
-api_logic_server_cli/docs/Working-with-Flask-AppBuilder.md
-api_logic_server_cli/docs/index.md
-api_logic_server_cli/docs/assets/.DS_Store
-api_logic_server_cli/docs/assets/images/bulb-icon.svg
-api_logic_server_cli/docs/assets/images/lightbulb.svg
-api_logic_server_cli/docs/stylesheets/extra.css
 api_logic_server_cli/fragments/Todo_modelsZZ.py.py
 api_logic_server_cli/fragments/configZZ.py
 api_logic_server_cli/fragments/db_typesZZ.txt
 api_logic_server_cli/fragments/modelsZZ.py
 api_logic_server_cli/fragments/nw_virtual_attrs.py
 api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py
 api_logic_server_cli/project_prototype/.DS_Store
 api_logic_server_cli/project_prototype/.gitignore
 api_logic_server_cli/project_prototype/api_logic_server_run.py
 api_logic_server_cli/project_prototype/config.py
 api_logic_server_cli/project_prototype/default.env
 api_logic_server_cli/project_prototype/logging.yml
 api_logic_server_cli/project_prototype/mypy.ini
-api_logic_server_cli/project_prototype/python_anywhere_wsgi.py
 api_logic_server_cli/project_prototype/readme.md
 api_logic_server_cli/project_prototype/requirements.txt
 api_logic_server_cli/project_prototype/run.ps1
 api_logic_server_cli/project_prototype/run.sh
 api_logic_server_cli/project_prototype/util.py
 api_logic_server_cli/project_prototype/.devcontainer/For_VSCode.dockerfile
 api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json
@@ -448,14 +377,15 @@
 api_logic_server_cli/project_prototype/database/alembic/script.py.mako
 api_logic_server_cli/project_prototype/database/alembic/versions/readme.md
 api_logic_server_cli/project_prototype/devops/git_push_new_project.sh
 api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile
 api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql
 api_logic_server_cli/project_prototype/devops/docker/build_image.dockerfile
 api_logic_server_cli/project_prototype/devops/docker/build_image.sh
+api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py
 api_logic_server_cli/project_prototype/logic/declare_logic.py
 api_logic_server_cli/project_prototype/logic/readme_declare_logic.md
 api_logic_server_cli/project_prototype/security/.DS_Store
 api_logic_server_cli/project_prototype/security/__init__.py
 api_logic_server_cli/project_prototype/security/declare_security.py
 api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store
 api_logic_server_cli/project_prototype/security/authentication_provider/__init__.py
@@ -519,20 +449,21 @@
 api_logic_server_cli/project_prototype/venv_setup/py.py
 api_logic_server_cli/project_prototype/venv_setup/readme_venv.md
 api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt
 api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh
 api_logic_server_cli/project_prototype/venv_setup/venv.ps1
 api_logic_server_cli/project_prototype/venv_setup/venv.sh
 api_logic_server_cli/project_prototype_allocation/.DS_Store
-api_logic_server_cli/project_prototype_allocation/readme-allocation.md
-api_logic_server_cli/project_prototype_allocation/images/db.png
-api_logic_server_cli/project_prototype_allocation/images/logic-diagram.png
+api_logic_server_cli/project_prototype_allocation/Logic-Allocation.md
+api_logic_server_cli/project_prototype_allocation/images/allocation/db.png
+api_logic_server_cli/project_prototype_allocation/images/allocation/logic-diagram.png
 api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py
 api_logic_server_cli/project_prototype_allocation/test/test.sh
 api_logic_server_cli/project_prototype_nw/.DS_Store
+api_logic_server_cli/project_prototype_nw/Tutorial.md
 api_logic_server_cli/project_prototype_nw/readme.md
 api_logic_server_cli/project_prototype_nw/api/customize_api.py
 api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json
 api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt
 api_logic_server_cli/project_prototype_nw/database/customize_models.py
 api_logic_server_cli/project_prototype_nw/database/db_debug.py
 api_logic_server_cli/project_prototype_nw/database/nw-gold.sqlite
```

### Comparing `ApiLogicServer-8.3.6/ApiLogicServer.egg-info/requires.txt` & `ApiLogicServer-8.4.0/ApiLogicServer.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 SQLAlchemy-Utils==0.38.2
 Werkzeug==2.2.3
 logicbankutils==0.6.0
 inflect==5.0.2
 itsdangerous==2.1.2
 Jinja2==3.1.2
 MarkupSafe==2.1.1
-safrs>=3.0.2
+safrs>=3.0.4
 Flask-Admin==1.5.7
 Flask-Cors==3.0.0
 Flask==2.2.2
 Flask-JWT-Extended==4.4.4
 Flask-Login==0.6.2
 Flask-OpenID==1.3.0
 python-dotenv==0.15.0
```

### Comparing `ApiLogicServer-8.3.6/LICENSE` & `ApiLogicServer-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/MANIFEST.in` & `ApiLogicServer-8.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/PKG-INFO` & `ApiLogicServer-8.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ApiLogicServer
-Version: 8.3.6
+Version: 8.4.0
 Summary: Create JSON:API and Web App from database, with LogicBank -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/ApiLogicServer
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://valhuber.github.io/ApiLogicServer/
 Platform: any
@@ -257,20 +257,21 @@
 * [Extensible Rules](https://dzone.com/articles/logic-bank-now-extensible-drive-95-automation-even) - defining new rule types, using Python
 * [Declarative](https://dzone.com/articles/agile-design-automation-how-are-rules-different-fr) - exploring _multi-statement_ declarative technology
 * [Automate Business Logic With Logic Bank](https://dzone.com/articles/automate-business-logic-with-logic-bank) - general introduction, discussions of extensibility, manageability and scalability
 * [Agile Design Automation With Logic Bank](https://dzone.com/articles/logical-data-indendence) - focuses on automation, design flexibility and agile iterations
 * [Instant Web Apps](https://dzone.com/articles/instant-db-web-apps) 
 
 
-
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+05/07/2023 - 08.04.00: safrs 3.0.4, tutorial demo notes, rm cli/docs, move pythonanywhere
+
 05/01/2023 - 08.03.06: allocation sample
 
 04/29/2023 - 08.03.03: restore missing debug info for open database failures
 
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
```

### Comparing `ApiLogicServer-8.3.6/README.md` & `ApiLogicServer-8.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -233,20 +233,21 @@
 * [Extensible Rules](https://dzone.com/articles/logic-bank-now-extensible-drive-95-automation-even) - defining new rule types, using Python
 * [Declarative](https://dzone.com/articles/agile-design-automation-how-are-rules-different-fr) - exploring _multi-statement_ declarative technology
 * [Automate Business Logic With Logic Bank](https://dzone.com/articles/automate-business-logic-with-logic-bank) - general introduction, discussions of extensibility, manageability and scalability
 * [Agile Design Automation With Logic Bank](https://dzone.com/articles/logical-data-indendence) - focuses on automation, design flexibility and agile iterations
 * [Instant Web Apps](https://dzone.com/articles/instant-db-web-apps) 
 
 
-
 [^1]:
     See the [FAQ for Low Code](FAQ-Low-Code)
 
 ### Change Log
 
+05/07/2023 - 08.04.00: safrs 3.0.4, tutorial demo notes, rm cli/docs, move pythonanywhere
+
 05/01/2023 - 08.03.06: allocation sample
 
 04/29/2023 - 08.03.03: restore missing debug info for open database failures
 
 04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, LogicBank 1.8.4, project readme updates
 
 04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65)
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/api_logic_server.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/api_logic_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 '''
 ApiLogicServer CLI: given a database url, create [and run] customizable ApiLogicProject.
     * Basically clones prototype project, and creates:
         * database/models.py for SQLAlchemy, using modified sqlacodegen & safrs metadata
         * ui/admin/admin.yaml for the Admin App     - using introspected models.py
         * api/expose_api_models.py for a safrs api  - using introspected models.py
     * Special provisions for NW Sample, to show customizations.
-    * See end for key module map quick links...
+    * See end for key_module_map() quick links
 
 Called from api_logic_server_cli.py, by instantiating the ProjectRun object.
 '''
 
-__version__ = "08.03.06"
+__version__ = "08.04.00"
 recent_changes = \
     f'\n\nRecent Changes:\n' +\
+    "\t05/07/2023 - 08.04.00: safrs 3.0.4, tutorial nutshell demo, rm cli/docs, move pythonanywhere \n"\
     "\t05/01/2023 - 08.03.06: allocation sample \n"\
     "\t04/29/2023 - 08.03.03: connect error reporting, startup logging \n"\
     "\t04/26/2023 - 08.03.00: virt attrs (Issue 56), safrs 3.0.2, readme updates, LogicBank 1.8.4 \n"\
     "\t04/13/2023 - 08.02.00: integratedConsole, logic logging (66), table relns fix (65) \n"\
     "\t04/06/2023 - 08.01.24: create_image, bugfix for excluded table relationships \n"\
     "\t03/23/2023 - 08.01.15: cloud debug additions, issue 59, 62-4, table filters \n"\
     "\t03/05/2023 - 08.01.04: python 3.11.2, Werkzeug==2.2.3, mypy initial, logicbank 1.8.3 \n"\
@@ -208,27 +209,30 @@
     else:
         shutil.copyfile(src, dest)
 
 
 def create_nw_tutorial(project_name, api_logic_server_dir_str):
     """ copy tutorial from docs, and link to it from readme.md 
     
-    alert 2 copies
-    * /Users/val/dev/Org-ApiLogicServer/Docs/docs/Tutorial.md
-    * /Users/val/dev/ApiLogicServer/Docs/api_logic_server_cli/docs/Tutorial.md <=
+    Alert: 2 copies:
+    * ~/dev/ApiLogicServer/api_logic_server_cli/project_prototype_nw/Tutorial.md
+    * ~/dev/Org-ApiLogicServer/Docs/docs/Tutorial.md
+    * cli version is master -->
+    * cp api_logic_server_cli/project_prototype_nw/Tutorial.md ../Org-ApiLogicServer/Docs/docs/Tutorial.md
     """
 
-
+    """
     tutorial_file_proj = open(project_name + '/Tutorial.md', 'w')
     tutorial_file_docs_path = Path(api_logic_server_dir_str).\
         joinpath('docs/Tutorial.md')
     tutorial_file_docs = open(tutorial_file_docs_path)
     tutorial_readme = tutorial_file_docs.read()
     tutorial_file_proj.write(tutorial_readme)
     tutorial_file_proj.close()
+    """
 
     project_readme_file_path = project_name + '/readme.md'  # brief 'go read tutorial' - add std readme
     standard_readme_file_path = str(Path(api_logic_server_dir_str).\
         joinpath('project_prototype').joinpath("readme.md"))
     with open(project_readme_file_path, 'a') as project_readme_file:
         with open(standard_readme_file_path) as standard_readme_file:
             project_readme_file.write(standard_readme_file.read())
@@ -537,15 +541,15 @@
     create_utils.replace_string_in_file(search_for="api_logic_server_port",
                            replace_with=replace_port,
                            in_file=in_file)
     log.debug(f' d.   Updated customize_api_py with port={project.port} and host={project.host}')
     full_path = project.project_directory_actual
     create_utils.replace_string_in_file(search_for="python_anywhere_path",
                            replace_with=full_path,
-                           in_file=f'{project.project_directory}/python_anywhere_wsgi.py')
+                           in_file=f'{project.project_directory}/devops/python-anywhere/python_anywhere_wsgi.py')
     log.debug(f' e.   Updated python_anywhere_wsgi.py with {full_path}')
 
 
 def fix_build_docker_image(msg, project: Project):
     """  d.   Fixing devops/docker/build_image.sh - project name """
     log.debug(msg)  #  d.   Fixing devops/docker/build_image.sh - project name
     replace_port = f':{project.port}' if project.port else ""
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/cli.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/cli.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_base.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/cli_args_base.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/cli_args_project.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/cli_args_project.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_expose_api_models_creator.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf118df63 (Sun Feb  5 02:48:17 2023 UTC)
-files sz: 5290
+moddate:  0x10c05564 (Sat May  6 02:48:48 2023 UTC)
+files sz: 5260
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -229,15 +229,15 @@
                       44 LOAD_ATTR                1 (port)
                       54 JUMP_FORWARD             1 (to 58)
                  >>   56 LOAD_CONST               2 ('None')
                  >>   58 STORE_FAST               2 (port_replace)
          
           40          60 LOAD_FAST                1 (result_apis)
          
-          41          62 LOAD_CONST               3 ('\n\ndef expose_models(api, method_decorators = []):  # th \n')
+          41          62 LOAD_CONST               3 ('\n\ndef expose_models(api, method_decorators = []): \n')
          
           40          64 BINARY_OP               13 (+=)
                       68 STORE_FAST               1 (result_apis)
          
           45          70 LOAD_FAST                1 (result_apis)
                       72 LOAD_CONST               4 ('    """\n')
                       74 BINARY_OP               13 (+=)
@@ -245,15 +245,15 @@
          
           46          80 LOAD_FAST                1 (result_apis)
                       82 LOAD_CONST               5 ('        Declare API - on existing SAFRSAPI \n')
                       84 BINARY_OP               13 (+=)
                       88 STORE_FAST               1 (result_apis)
          
           47          90 LOAD_FAST                1 (result_apis)
-                      92 LOAD_CONST               6 ('            This exposes each model (note: end point names are table names) \n')
+                      92 LOAD_CONST               6 ('            This exposes each model - API automation\n')
                       94 BINARY_OP               13 (+=)
                       98 STORE_FAST               1 (result_apis)
          
           48         100 LOAD_FAST                1 (result_apis)
                      102 LOAD_CONST               7 ('            Including get (filtering, pagination, related data access) \n')
                      104 BINARY_OP               13 (+=)
                      108 STORE_FAST               1 (result_apis)
@@ -544,18 +544,18 @@
          
          102     >> 1480 LOAD_CONST              13 (None)
                     1482 RETURN_VALUE
          consts
             ' create strings for ui/basic_web_app/views.py and api/expose_api_models.py '
             ''
             'None'
-            '\n\ndef expose_models(api, method_decorators = []):  # th \n'
+            '\n\ndef expose_models(api, method_decorators = []): \n'
             '    """\n'
             '        Declare API - on existing SAFRSAPI \n'
-            '            This exposes each model (note: end point names are table names) \n'
+            '            This exposes each model - API automation\n'
             '            Including get (filtering, pagination, related data access) \n'
             '            And post/patch/update (including logic enforcement) \n'
             '        You typically do not customize this file \n'
             '            See https://apilogicserver.github.io/Docs/Tutorial/#customize-and-debug \n'
             'TRANSFERFUNDx'
             'special table'
             None
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/api_logic_server_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/model_creation_services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/multi_db_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/ui_admin_creator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/__pycache__/uri_info.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/api_expose_api_models_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,21 +34,21 @@
                     # + "From: " + sys.argv[0] + "\n\n"
                     + "Using Python: " + sys.version + "\n\n"
                     + "At: " + str(datetime.datetime.date()) + "\n\n"
                     + '"""\n\n')
     '''
     port_replace = model_creation_services.project.port if model_creation_services.project.port else "None"
     result_apis += \
-        f'\n\ndef expose_models(api, method_decorators = []):  # th \n'
+        f'\n\ndef expose_models(api, method_decorators = []): \n'
     # result_apis += '    my_host = HOST\n'
     # result_apis += '    if HOST == "0.0.0.0":\n'
     # result_apis += '        my_host = "localhost"  # override default HOST for pc"\n'
     result_apis += '    """\n'
     result_apis += '        Declare API - on existing SAFRSAPI \n'
-    result_apis += '            This exposes each model (note: end point names are table names) \n'
+    result_apis += '            This exposes each model - API automation\n'
     result_apis += '            Including get (filtering, pagination, related data access) \n'
     result_apis += '            And post/patch/update (including logic enforcement) \n'
     result_apis += '        You typically do not customize this file \n'
     result_apis += '            See https://apilogicserver.github.io/Docs/Tutorial/#customize-and-debug \n'
     result_apis += '    """\n'
 
     sys.path.append(model_creation_services.project.os_cwd)
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/api_logic_server_utils.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/api_logic_server_utils.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/model_creation_services.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/model_creation_services.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/multi_db_utilsZZ.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/data/customer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/favicon.ico`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo192.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/logo512.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/695.2b02568d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/css/main.a0c288b7.css.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1022.0747a719.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1062.9e2b1e6c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1069.16bec71d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1074.2c3d927c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1251.10ac0097.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1258.94dead34.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1295.179239a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1324.be7507c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1431.d02260cd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1532.41e3c0c8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1619.31b6d6e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1690.e74e47c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/1989.ee922c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2154.5c399961.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2402.e66e47e8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2478.4e6b45fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2526.c4309069.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/254.1bc22866.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2611.8815ae2b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2880.029aa44e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2900.14a00390.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/2909.28b39275.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3003.57cfe277.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/312.3d69e408.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3126.99b58416.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3323.b47b9b1e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3668.cd0becc2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/369.0237ca8c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3698.750e43d6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3766.d8eddcd9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3907.7b2efd62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/3955.f5434704.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4040.613bd8c0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4333.61aa216a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/464.522c11f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4877.7cebca37.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4900.19572072.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/4969.ccedbf9b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5133.71af5a54.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/52.22a03ee6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5328.77d62d48.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5342.e36bdc43.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5419.3d10c516.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5507.c29076d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5540.d957a974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5558.d0dc5575.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5571.ad570057.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/5672.f0c2440f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/608.84469af3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6289.a7c21fba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6304.ce792f5f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6384.8f33f789.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6403.77f38472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/651.bf520a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6717.805e1882.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/695.a9cefc11.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/6965.381dbe04.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7117.b2e9eb70.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7294.6813eb1f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7299.20100701.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7436.4e91a3a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7497.f56048e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7499.b216e9da.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7615.f5af9bae.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7713.6d02efa2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/787.d5293104.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7894.f8f70466.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/7952.29e2c950.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8184.741e3d56.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8272.99aef5a5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8347.649393e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/839.87662037.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8501.ea0cd3a2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/8861.01a110f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/907.7b650179.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9186.73a41896.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9200.d0bc8746.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9214.5198dfc3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9335.43329da2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9357.e2f466b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9361.e7bbdd03.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9381.9495a14c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9432.e84dc193.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9687.e1a38d25.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9845.3bb55d3c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/9902.bfcd7f60.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/js/main.1eb04138.js.map`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/safrs-react-admin-npm-build/static/media/codicon.b797181c93b3755f4fa1.ttf`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/app/views.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/basic_web_app/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/create_admin.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/create_admin.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/fab_config.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/fab_config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/home.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/templates/react_admin_component.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/templates/react_admin_component.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/ui_admin_creator.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/ui_admin_creator.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/create_from_model/uri_info.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/create_from_model/uri_info.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/Chinook_Sqlite.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/Chinook_Sqlite.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/allocation.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/allocation.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/authentication.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/authentication.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/classicmodels.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/classicmodels.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/new.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/new.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold-plus.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/nw-gold-plus.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/nw-gold.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/nw-gold.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/nw.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/nw.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/table_filters_tests.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/table_filters_tests.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/database/todos.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/database/todos.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/docs/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/.DS_Store`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
-00000050: 0000 0001 0000 1000 0074 0073 6c67 3153  .........t.slg1S
+00000040: 0000 0000 0000 0002 0000 0000 0000 000c  ................
+00000050: 0000 0001 0000 1000 0065 0073 6c67 3153  .........e.slg1S
 00000060: 636f 6d70 0000 0000 0000 0000 0000 0000  comp............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,39 +26,39 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0008 0000 0006  ................
-00000210: 0061 0073 0073 0065 0074 0073 6c67 3153  .a.s.s.e.t.slg1S
-00000220: 636f 6d70 0000 0000 0000 2ed8 0000 0006  comp............
-00000230: 0061 0073 0073 0065 0074 0073 6d6f 4444  .a.s.s.e.t.smoDD
-00000240: 626c 6f62 0000 0008 360f f210 dc5e c441  blob....6....^.A
-00000250: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-00000260: 6d6f 6444 626c 6f62 0000 0008 360f f210  modDblob....6...
-00000270: dc5e c441 0000 0006 0061 0073 0073 0065  .^.A.....a.s.s.e
-00000280: 0074 0073 7068 3153 636f 6d70 0000 0000  .t.sph1Scomp....
-00000290: 0000 4000 0000 000b 0073 0074 0079 006c  ..@......s.t.y.l
-000002a0: 0065 0073 0068 0065 0065 0074 0073 6c67  .e.s.h.e.e.t.slg
-000002b0: 3153 636f 6d70 0000 0000 0000 027a 0000  1Scomp.......z..
-000002c0: 000b 0073 0074 0079 006c 0065 0073 0068  ...s.t.y.l.e.s.h
-000002d0: 0065 0065 0074 0073 6d6f 4444 626c 6f62  .e.e.t.smoDDblob
-000002e0: 0000 0008 8122 c90f df5e c441 0000 000b  ....."...^.A....
-000002f0: 0073 0074 0079 006c 0065 0073 0068 0065  .s.t.y.l.e.s.h.e
-00000300: 0065 0074 0073 6d6f 6444 626c 6f62 0000  .e.t.smodDblob..
-00000310: 0008 8122 c90f df5e c441 0000 000b 0073  ..."...^.A.....s
-00000320: 0074 0079 006c 0065 0073 0068 0065 0065  .t.y.l.e.s.h.e.e
-00000330: 0074 0073 7068 3153 636f 6d70 0000 0000  .t.sph1Scomp....
-00000340: 0000 1000 0000 0000 0000 0000 0000 0000  ................
-00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 000c 0000 0006  ................
+00000210: 0069 006d 0061 0067 0065 0073 6c67 3153  .i.m.a.g.e.slg1S
+00000220: 636f 6d70 0000 0000 001a 06de 0000 0006  comp............
+00000230: 0069 006d 0061 0067 0065 0073 6d6f 4444  .i.m.a.g.e.smoDD
+00000240: 626c 6f62 0000 0008 2fea 2a3b 5500 c541  blob..../.*;U..A
+00000250: 0000 0006 0069 006d 0061 0067 0065 0073  .....i.m.a.g.e.s
+00000260: 6d6f 6444 626c 6f62 0000 0008 2fea 2a3b  modDblob..../.*;
+00000270: 5500 c541 0000 0006 0069 006d 0061 0067  U..A.....i.m.a.g
+00000280: 0065 0073 7068 3153 636f 6d70 0000 0000  .e.sph1Scomp....
+00000290: 001a 1000 0000 0005 006c 006f 0067 0069  .........l.o.g.i
+000002a0: 0063 6c67 3153 636f 6d70 0000 0000 0000  .clg1Scomp......
+000002b0: 0576 0000 0005 006c 006f 0067 0069 0063  .v.....l.o.g.i.c
+000002c0: 6d6f 4444 626c 6f62 0000 0008 4f26 423e  moDDblob....O&B>
+000002d0: 5500 c541 0000 0005 006c 006f 0067 0069  U..A.....l.o.g.i
+000002e0: 0063 6d6f 6444 626c 6f62 0000 0008 4f26  .cmodDblob....O&
+000002f0: 423e 5500 c541 0000 0005 006c 006f 0067  B>U..A.....l.o.g
+00000300: 0069 0063 7068 3153 636f 6d70 0000 0000  .i.cph1Scomp....
+00000310: 0000 1000 0000 0004 0074 0065 0073 0074  .........t.e.s.t
+00000320: 6c67 3153 636f 6d70 0000 0000 0000 0247  lg1Scomp.......G
+00000330: 0000 0004 0074 0065 0073 0074 6d6f 4444  .....t.e.s.tmoDD
+00000340: 626c 6f62 0000 0008 ad90 c8ae 4e00 c541  blob........N..A
+00000350: 0000 0004 0074 0065 0073 0074 6d6f 6444  .....t.e.s.tmodD
+00000360: 626c 6f62 0000 0008 ad90 c8ae 4e00 c541  blob........N..A
+00000370: 0000 0004 0074 0065 0073 0074 7068 3153  .....t.e.s.tph1S
+00000380: 636f 6d70 0000 0000 0000 1000 0000 0000  comp............
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave-Logic-Report.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Sample.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,100 @@
+# Behave Creates Executable Test Suite, Documentation
 
-# Behave Logic Report
+You can optionally use the Behave test framework to (here is an [Agile Approach for using Behave](https://github.com/valhuber/ApiLogicServer/wiki/Logic:-Tutorial)):
+
+1. **Create and Run an Executable Test Suite:** in your IDE, create test definitions (similar to what is shown in the report below), and Python code to execute tests.  You can then execute your test suite with 1 command.
+
+2. **Requirements and Test Documentation:** as shown below, you can then create a wiki report that documents your requirements, and the tests (**Scenarios**) that confirm their proper operation.
+
+   * **Integrated Logic Documentation:** the report integrates your logic, including a logic report showing your logic (rules and Python), and a Logic Log that shows exactly how the rules executed.  Logic Doc is transparent to business users, so can further contribute to Agile Collaboration.
+
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/behave-summary.png?raw=true"  height="600"></figure>
+
+[Behave](https://behave.readthedocs.io/en/stable/tutorial.html) is a framework for defining and executing tests.  It is based on [TDD (Test Driven Development)](http://dannorth.net/introducing-bdd/), an Agile approach for defining system requirements as executable tests.
+
+&nbsp;&nbsp;
+
+# Using Behave
+
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/TDD-ide.png?raw=true"></figure>
+
+Behave is pre-installed with API Logic Server.  Use it as shown above:
+
+1. Create `.feature` files to define ***Scenarios*** (aka tests) for ***Features*** (aka Stories)
+
+2. Code `.py` files to implement Scenario tests
+
+3. Run Test Suite: Launch Configuration `Behave Run`.  This runs all your Scenarios, and produces a summary report of your Features and the test results.
+
+4. Report: Launch Configuration `Behave Report` to create the wiki file shown at the top of this page.
+
+These steps are further defined, below.  Explore the samples in the sample project.
+
+&nbsp;&nbsp;
+
+## 1. Create `.feature` file to define Scenario
+
+Feature (aka Story) files are designed to promote IT / business user collaboration.  
+
+&nbsp;&nbsp;
+
+## 2. Code `.py` file to implement test
 
-This is the sample project from API Logic Server, based on the Northwind database (sqlite database located in the `database` folder - no installation required):
+Implement your tests in Python.  Here, the tests are largely _read existing data_, _run transaction_, and _test results_, using the API.  You can obtain the URLs from the swagger.
 
-<figure><img src="https://github.com/valhuber/LogicBank/raw/main/images/nw.png"></figure>
+Key points:
 
->  The sample Scenarios below were chosen to illustrate the basic patterns of using rules.  Open the disclosure box (_"Tests - and their logic..."_) to see the implementation and notes.
+* Link your scenario / implementations with annotations, as shown for _Order Placed with excessive quantity_.
+
+* Include the `test_utils.prt()` call; be sure to use specify the scenario name as the 2nd argument.  This is what drives the name of the Logic Log file, discussed below.
+
+* Optionally, include a Python docstring on your `when` implementation as shown above, delimited by `"""` strings (see _"Familiar logic pattern"_ in the screen shot, above). If provided, this will be written into the wiki report.
+
+* Important: the system assumes the following line identifies the scenario_name; be sure to include it.
+
+&nbsp;&nbsp;
+
+## 3. Run Test Suite: Launch Configuration `Behave Run`
+
+You can now execute your Test Suite.  Run the `Behave Run` Launch Configuration, and Behave will run all of the tests, producing the outputs (`behave.log` and `<scenario.logs>` shown above.
+
+* Windows users will need to run `Windows Behave Run`
+
+* You can run just 1 scenario using `Behave Scenario`
+
+* You can set breakpoints in your tests
+
+The server must be running for these tests.  Use the Launch Configuration `ApiLogicServer`, or `python api_logic_server_run.py`.  The latter does not run the debugger, which you may find more convenient since changes to your test code won't restart the server.
+
+&nbsp;&nbsp;
+
+## 4. Report: Launch Configuration `Behave Report'
+
+Run this to create the wiki reports from the logs in step 3.
 
 
 &nbsp;
+&nbsp;
 
----
 
 
+# Behave Logic Report
+&nbsp;
+&nbsp;
 ## Feature: About Sample  
   
 &nbsp;
 &nbsp;
 ### Scenario: Transaction Processing
 &emsp;  Scenario: Transaction Processing  
 &emsp;&emsp;    Given Sample Database  
 &emsp;&emsp;    When Transactions are submitted  
 &emsp;&emsp;    Then Enforce business policies with Logic (rules + code)  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -91,45 +159,43 @@
 &emsp;  Scenario: Good Order Custom Service  
 &emsp;&emsp;    Given Customer Account: ALFKI  
 &emsp;&emsp;    When Good Order Placed  
 &emsp;&emsp;    Then Logic adjusts Balance (demo: chain up)  
 &emsp;&emsp;    Then Logic adjusts Products Reordered  
 &emsp;&emsp;    Then Logic sends email to salesrep  
 &emsp;&emsp;    Then Logic adjusts aggregates down on delete order  
-<details markdown>
-
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
 **Logic Doc** for scenario: Good Order Custom Service
    
 We place an Order with an Order Detail.  It's one transaction.
 
-
 Note how the `Order.OrderTotal` and `Customer.Balance` are *adjusted* as Order Details are processed.
 Similarly, the `Product.UnitsShipped` is adjusted, and used to recompute `UnitsInStock`
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/declare-logic.png?raw=true"></figure>
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/declare-logic.png?raw=true"></figure>
 
 > **Key Takeaway:** sum/count aggregates (e.g., `Customer.Balance`) automate ***chain up*** multi-table transactions.
 
 **Events - Extensible Logic**
 
 Inspect the log for __Hi, Andrew - Congratulate Nancy on their new order__. 
 
 The `congratulate_sales_rep` event illustrates logic 
 [Extensibility](https://github.com/valhuber/LogicBank/wiki/Rule-Extensibility) 
 - using Python to provide logic not covered by rules, 
 like non-database operations such as sending email or messages.
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/send-email.png?raw=true"></figure>
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/send-email.png?raw=true"></figure>
 
 There are actually multiple kinds of events:
 
 * *Before* row logic
 * *After* row logic
 * On *commit,* after all row logic has completed (as here), so that your code "sees" the full logic results
 
@@ -190,15 +256,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Bad Order Custom Service
 &emsp;  Scenario: Bad Order Custom Service  
 &emsp;&emsp;    Given Customer Account: ALFKI  
 &emsp;&emsp;    When Order Placed with excessive quantity  
 &emsp;&emsp;    Then Rejected per Check Credit  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -261,15 +327,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Alter Item Qty to exceed credit
 &emsp;  Scenario: Alter Item Qty to exceed credit  
 &emsp;&emsp;    Given Customer Account: ALFKI  
 &emsp;&emsp;    When Order Detail Quantity altered very high  
 &emsp;&emsp;    Then Rejected per Check Credit  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -319,15 +385,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Alter Required Date - adjust logic pruned
 &emsp;  Scenario: Alter Required Date - adjust logic pruned  
 &emsp;&emsp;    Given Customer Account: ALFKI  
 &emsp;&emsp;    When Order RequiredDate altered (2013-10-13)  
 &emsp;&emsp;    Then Balance not adjusted  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -369,15 +435,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Set Shipped - adjust logic reuse
 &emsp;  Scenario: Set Shipped - adjust logic reuse  
 &emsp;&emsp;    Given Customer Account: ALFKI  
 &emsp;&emsp;    When Order ShippedDate altered (2013-10-13)  
 &emsp;&emsp;    Then Balance reduced 1086  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -385,15 +451,15 @@
    
 We set `Order.ShippedDate`.
 
 This cascades to the Order Details, per the `derive=models.OrderDetail.ShippedDate` rule.
 
 This chains to adjust the `Product.UnitsShipped` and recomputes `UnitsInStock`, as above
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/order-shipped-date.png?raw=true"></figure>
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/order-shipped-date.png?raw=true"></figure>
 
 
 > **Key Takeaway:** parent references (e.g., `OrderDetail.ShippedDate`) automate ***chain-down*** multi-table transactions.
 
 > **Key Takeaway:** Automatic Reuse (_design one, solve many_)
 
 
@@ -449,15 +515,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Reset Shipped - adjust logic reuse
 &emsp;  Scenario: Reset Shipped - adjust logic reuse  
 &emsp;&emsp;    Given Shipped Order  
 &emsp;&emsp;    When Order ShippedDate set to None  
 &emsp;&emsp;    Then Logic adjusts Balance by -1086  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -519,15 +585,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Clone Existing Order
 &emsp;  Scenario: Clone Existing Order  
 &emsp;&emsp;    Given Shipped Order  
 &emsp;&emsp;    When Cloning Existing Order  
 &emsp;&emsp;    Then Logic Copies ClonedFrom OrderDetails  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -541,15 +607,15 @@
 
 1. `place_order.feature` defines the test
 
 2. `place_order.py` implements the test.  It uses the API to Post an Order, setting `CloneFromOrder` to trigger the copy logic
 
 3. `declare_logic.py` implements the logic, by invoking `logic_row.copy_children()`.  `which` defines which children to copy, here just `OrderDetailList`
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/clone-order.png?raw=true"></figure>
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/clone-order.png?raw=true"></figure>
 
 `CopyChildren` For more information, [see here](https://github.com/valhuber/LogicBank/wiki/Copy-Children)
 
     Useful in row event handlers to copy multiple children types to self from copy_from children.
 
     child-spec := < ‘child-list-name’ | < ‘child-list-name = parent-list-name’ >
     child-list-spec := [child-spec | (child-spec, child-list-spec)]
@@ -619,15 +685,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Audit Salary Change
 &emsp;  Scenario: Audit Salary Change  
 &emsp;&emsp;    Given Employee 5 (Buchanan) - Salary 95k  
 &emsp;&emsp;    When Patch Salary to 200k  
 &emsp;&emsp;    Then Salary_audit row created  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
 
 
@@ -638,15 +704,15 @@
 1. **Discouraged:** you can implement auditing with events.  But auditing is a common pattern, and this can lead to repetitive, tedious code
 2. **Preferred:** approaches use [extensible rules](https://github.com/valhuber/LogicBank/wiki/Rule-Extensibility#generic-event-handlers).
 
 Generic event handlers can also reduce redundant code, illustrated in the time/date stamping `handle_all` logic.
 
 This is due to the `copy_row` rule.  Contrast this to the *tedious* `audit_by_event` alternative:
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/salary_change.png?raw=true"></figure>
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/salary_change.png?raw=true"></figure>
 
 > **Key Takeaway:** use **extensible own rule types** to automate pattern you identify; events can result in tedious amounts of code.
 
 
 
 &nbsp;
 &nbsp;
@@ -674,15 +740,15 @@
 &nbsp;
 &nbsp;
 ### Scenario: Raise Must be Meaningful
 &emsp;  Scenario: Raise Must be Meaningful  
 &emsp;&emsp;    Given Employee 5 (Buchanan) - Salary 95k  
 &emsp;&emsp;    When Patch Salary to 96k  
 &emsp;&emsp;    Then Reject - Raise too small  
-<details markdown>
+<details>
 <summary>Tests - and their logic - are transparent.. click to see Logic</summary>
 
 
 &nbsp;
 &nbsp;
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Behave.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/reports/Behave Logic Report Intro.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Behave Creates Executable Test Suite, Documentation
 
-You can optionally use the Behave test framework to (here is an [Agile Approach for using Behave](../Logic:-Tutorial)):
+You can optionally use the Behave test framework to:
 
 1. **Create and Run an Executable Test Suite:** in your IDE, create test definitions (similar to what is shown in the report below), and Python code to execute tests.  You can then execute your test suite with 1 command.
 
 2. **Requirements and Test Documentation:** as shown below, you can then create a wiki report that documents your requirements, and the tests (**Scenarios**) that confirm their proper operation.
 
-   * **Integrated Logic Documentation:** the report integrates your logic, including a logic report showing your logic (rules and Python), and a Logic Log that shows exactly how the rules executed.  Logic Doc is transparent to business users, so can further contribute to Agile Collaboration.
+   * **Logic Documentation:** the report integrates your logic, including a logic report showing your logic (rules and Python), and a Logic Log that shows exactly how the rules executed.  Logic Doc can further contribute to Agile Collaboration.
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/behave-summary.png?raw=true"  height="600"></figure>
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/behave-summary.png?raw=true"  height="600"></figure>
 
 [Behave](https://behave.readthedocs.io/en/stable/tutorial.html) is a framework for defining and executing tests.  It is based on [TDD (Test Driven Development)](http://dannorth.net/introducing-bdd/), an Agile approach for defining system requirements as executable tests.
 
 &nbsp;&nbsp;
 
 # Using Behave
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/TDD-ide.png?raw=true"></figure>
+<figure><img src="https://github.com/valhuber/ApiLogicServer/wiki/images/behave/TDD-ide.png?raw=true"></figure>
 
 Behave is pre-installed with API Logic Server.  Use it as shown above:
 
 1. Create `.feature` files to define ***Scenarios*** (aka tests) for ***Features*** (aka Stories)
 
 2. Code `.py` files to implement Scenario tests
 
@@ -67,11 +67,7 @@
 The server must be running for these tests.  Use the Launch Configuration `ApiLogicServer`, or `python api_logic_server_run.py`.  The latter does not run the debugger, which you may find more convenient since changes to your test code won't restart the server.
 
 &nbsp;&nbsp;
 
 ## 4. Report: Launch Configuration `Behave Report'
 
 Run this to create the wiki reports from the logs in step 3.
-
-
-&nbsp;
-&nbsp;
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Data-Model-Multi.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/readme.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,111 @@
-API Logic Server enables you to create projects that support multiple databases, as follows:
+# 1. Basic App: Flask / SQLAlchemy -- manually coded app
 
-1. Create the project, specifying your "main" database
+This is a manually coded server providing a few APIs for [this database]().
 
-2. Use the `ApiLogicServer add-db` command for each additional database
+It is the smallest example of a typical project for a modern database API server.
 
-    * See the example below
+&nbsp;
+
+## Background - Key Tools
+
+Creating an API Server requires 2 basic tools: a Framework, and database access.
+
+&nbsp;
+
+### Framework - Flask
+
+A framework is a "your code goes here" library, provding backend functions to handle api calls, html calls, etc.  The framework provides key basic functions such as:
+
+* listening for incoming calls, and **invoking your code** (your 'handler')
+
+* providing **access to url parameters and request data**
+
+* enabling you to **return a response** in a designated format, such as html or json
+
+A popular framework in Python is ***Flask***, illustrated in this application.
 
 &nbsp;
 
-## Example
+### Data Access - SQLAlchemy ORM
+
+In your handler, you may need to read or write database data.  You can use raw SQL, or an ORM (Object Relational Manager) such as SQLAlchemy.  ORMs can facilitate database access:
+
+* **use Objects** (instead of dictionaries), which provide IDE services such as code completion to simplify coding and reduce errors
+
+* simplified **access to related data** (e.g., a simple way to get the OrderDetails for an Order)
+
+* other services, such as support for type hierarchies
+
+There are 2 common aspects for using an ORM:
+
+* provide **data model classes** - these are used to read/write data, and can also be used to create / update the database structure (add tables and columns)
+
+* use **data access** - verbs to read/write data
 
-SQLAlchemy supports multiple databases by using the `bind_key` which is [supported by Flask](https://flask-sqlalchemy.palletsprojects.com/en/3.0.x/binds/){:target="_blank" rel="noopener"}.  It is leveraged in creating Api Logic Projects when you add databases like this:
+---
 
-```bash
-cd YourApiLogicProject
-ApiLogicServer add-db --db-url=todo --bind_key=Todo
-``` 
+&nbsp;
+
+## Exploring the App
 
 &nbsp;
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/model/multi-db.png?raw=true"></figure>
+### App Structure
+
+Long before you use the Flask/SQLAlchemy tools, you need to create project structure.  You can explore [```1. Basic_App```](../1.%20Basic_App/):
+
+* `api` - a directory for api code
+
+* `database` - a directory for SQLAlchemy artifacts
 
-Observe:
+There are also important devops artifacts:
 
-1. Model files are created (prefixed by your `bind-key`) for each table in your `db-url`.  Note:
-    * The `bind-key` is inserted into the table class.
-    * Sqlite databases are copied to your database folder, simplifying source control.
-    * This example uses the shorthand for sqlite databases: `todo`, `classicmodels`, `chinook` and `nw`.  These are included in the install, so you can experiment with them.
-2. The `config.py` file is altered per your `db-url`
-    * You can use environment variables to override these assignments, to avoid placing passwords in projects.
-3. The `bind_databases.py` file is created to bind the `bind_key` to the database url.   This enables SQLAlchemy to access the proper database.
+* `.devcontainer/` - files here enable your project to be run in docker images, and to package your application as an image
+
+* `config.py` - use this to set up key configuration parameters, including code to override them with environment variables
 
 &nbsp;
 
-## Internals
+### Server
 
-The example above will result in the following log:
+See [```flask_basic.py```](../1.%20Basic_App/flask_basic.py) to see how to establish a Flask server.  It's this program you ran to start the server.
 
-```bash
-ApiLogicServer 6.90.08 Creation Log:
-1. Not Deleting Existing Project
-2. Using Existing Project
-.. ..Adding Database [Todo] to existing project
-.. .. ..Copying sqlite database to: database/Todo_db.sqlite
-.. .. ..From /Users/val/dev/ApiLogicServer/api_logic_server_cli/database/todos.sqlite
-.. ..Updating config.py file with SQLALCHEMY_DATABASE_URI_TODO...
-.. ..Updating database/bind_databases.py with SQLALCHEMY_DATABASE_URI_TODO...
-3. Create/verify database/Todo_models.py, then use that to create api/ and ui/ models
- a.  Create Models - create database/Todo_models.py, using sqlcodegen
-.. .. ..For database:  sqlite:////Users/val/dev/servers/ApiLogicProject/database/Todo_db.sqlite
-.. .. ..Setting bind_key = Todo
-.. .. ..Create resource_list - dynamic import database/Todo_models.py, inspect 2 classes in <project>/database
- b.  Create api/expose_api_models.py from models
- c.  Create ui/admin/admin.yaml from models
-.. .. ..WARNING - no relationships detected - add them to your database or model
-.. .. ..  See https://github.com/valhuber/LogicBank/wiki/Managing-Rules#database-design
-.. .. ..Write /Users/val/dev/servers/ApiLogicProject/ui/admin/Todo_admin.yaml
- d.  Create ui/basic_web_app -- declined
-4. Final project fixup
- b.   Update api_logic_server_run.py with project_name=/Users/val/dev/servers/ApiLogicProject and api_name, host, port
- c.   Fixing api/expose_services - port, host
- d.   Updated customize_api_py with port=5656 and host=localhost
- e.   Updated python_anywhere_wsgi.py with /Users/val/dev/servers/ApiLogicProject
-```
+&nbsp;
 
-Notes:
+### API
 
-1. In step 2:
-    1. Updating `config.py` file with the location of the new database
-    2. Updating `database/bind_databases.py` to open this database for SQLAlchemy access
-2. In Step 3:
-    1. Creating a `models.py` file; note:
-        * The additional superclasses,
-        * Inclusion of your designated `bind_key`, for step 1.2
-3. Note the shorthand for sqlite versions of `todo`, `classicmodels`, `chinook`.  These are included in the install.
+Explore [```api/end_points.py```](../1.%20Basic_App/api/end_points.py) for examples of handling api calls.  See `def order():`.
 
 &nbsp;
 
-## Runtime Support
+### Data Access
+
+There are 2 aspects to explore for SQLAlchemy:
+
+* See [```database/models.py```](../1.%20Basic_App/database/models.py) for examples of defining objects (models) for database rows.  These correspond to the tables in your database.
 
-### API support
+* See [```api/end_points.py```](../1.%20Basic_App/api/end_points.py) for examples of SQLAlchemy calls.  See `def order():`.
 
-Tables in your new databases are available through swagger.
+&nbsp;
+
+## Appendix
 
 &nbsp;
 
-### Admin support
+### API
+
+An API is a set of endpoints, accessible via the web, that clients (e.g, mobile apps) can invoke by providing:
+
+* **a command:** such as GET, POST or PATCH
+
+* **a URL:** this identifies the server, the endpoint (e.g, Order), and the arguments (e.g. the OrderNumber)
+
+* **a payload:** data being sent to the server (e.g, to be saved), typically in `json` format (not provided for GET commands)
+
+* **a header:** typically identifying the authenticated user
+
+&nbsp;
 
-An admin app is built for the table in your new database.  Access it via a url that prefixes the `bind-key`, such as `http://localhost:5656/admin/Todo_admin/` (note the trailing slash).
+### API Server
 
+A server that implements an API.  In the context of this tutorial, it's a Flask server, using SQLAlchemy for data access.
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Install-Eval-x.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/readme.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,162 @@
-The fastest way to explore API Logic Server - *with __no install__* - is to follow this guide to create, explore and customize a project using Codespaces.
+# Setup and Run
 
-<details markdown>
+To run your project, the system requires various runtime systems for data access, api, and logic.  These are included with API Logic Server ([architecture doc here](https://apilogicserver.github.io/Docs/Architecture-What-Is/)).  So, to run your project ([instructions here](#setup-instructions)):
 
-<summary>What is API Logic Server</summary>
-
-API Logic Server creates __customizable database web app projects:__
-
-* Creation is __Instant:__ create _executable_ projects from your database, with a _single_ command.  Projects are __Highly Functional,__ providing:
-
-    * __API:__ an endpoint for each table, with filtering, sorting, pagination and related data access
-
-    * __Admin UI:__ multi-page / multi-table apps, with page navigations, automatic joins and declarative hide/show
-
-* __Projects are Customizable, using _your IDE_:__ such as VSCode, PyCharm, etc, for familiar edit/debug services
-
-* __Business Logic Automation:__ using unique spreadsheet-like rules, extensible with Python :trophy:
-
-Follow the steps below to be up and running in about a minute - no install, no configuration.  You can run the created project to explore its functionality, and how to customize it in VSCode.
+1.  __Establish your Python Environment__ to activate these runtime systems
+2. __Run__
 
 &nbsp;
 
-<details markdown>
-
-<summary>Why Does It Matter: Faster, Simpler, Modern Architecture</summary>
-
-<details markdown>
-
-<summary>Frameworks are too slow, Low Code is not dev-friendly</summary>
-
-We looked at approaches for building database systems:   
-
-* __Frameworks:__ Frameworks like Flask or Django enable you to build a single endpoint or _Hello World_ page, but a __multi-endpoint__ API and __multi-page__ application would take __weeks__ or more.
-
-* __Low Code Tools:__ these are great for building great UIs, but
-
-    * Want a multi-page app, _instantly_ -- __no layout required each screen__
-    * Want to __preserve standard dev tools__ (VSCode, PyCharm, git, etc) - propietary IDEs are not dev-friendly
-
-And neither provides an answer for __backend business logic__ (it's nearly half the effort).
-
-</details>
-
-<details markdown>
-
-<summary>API Logic Server - dev-friendly low-code automation</summary>
-
+# Key Customization Files
 
-API Logic Server is a low-code, developer-friendly approach that leverages automation to dramatically improve web app development:
+Your project is ready to run, but it's likely you'll want to customize it - declare logic, new endpoints, etc.
 
-* Automation makes it __faster:__ _moments_, instead of weeks or months.  Unblock UI Dev, and engage business users - _early_ - to reduce misunderstandings.  _Customize_ with __standard IDEs.__
+The ___Key Customization Files___ listed in the table below are created as stubs, intended for you to add customizations that extend
+the created API, Logic and Web App.
 
-* Automation makes it __simpler:__ this reduces the risk of architectural errors, e.g., APIs without pagination.
+* Since they are separate files, the project can be
+[rebuilt](https://apilogicserver.github.io/Docs/Project-Rebuild/) (e.g., synchronized with a revised schema), preserving your customizations.
 
-* Automation ensures a __modern software architecture:__ _container-ready_, _API-based_, with _shared logic_ over UIs and APIs (no more logic in UI controllers), in maintainable _models_.
+Please see the `nw` sample for examples of typical customizations.  You can open it in GitHub (use Shift + "." to view in project mode) - [click here](https://github.com/ApiLogicServer/demo).
 
-</details>
+| Directory | Usage                         | Key Customization File             | Typical Customization                                                                 |
+|:-------------- |:------------------------------|:-----------------------------------|:--------------------------------------------------------------------------------------|
+| ```api``` | **JSON:API**<br>*Ready to Run*                    | ```api/customize_api.py```         | Add new end points / services                                                         |
+| ```ui``` | **Multi-Page Admin App**<br>*Ready to Run*  | ```ui/admin/admin.yaml```          | Control field display - order, captions etc.                                          |
+| ```database``` | SQLAlchemy Data Model Classes | ```database/customize_models.py``` | Add derived attributes, and relationships missing in the schema                       |
+| ```logic``` | **Transactional Logic**<br>spreadsheet-like rules   | ```logic/declare_logic.py```       | Declare multi-table derivations, constraints, and Python events such as send mail / messages |
+| ```security``` | Authentication, Authorization   | ```security/declare_security.py```          | Control login, role-based row access         |
+| ```tests``` | Behave Test Suite              | ```tests/api_logic_server_behave/features```          | Declare and implement [Behave Tests](https://apilogicserver.github.io/Docs/Behave/)                                          |
 
-</details>
+&nbsp;
 
-</details>
+# Project Information
 
+This API Logic Project was created with the `ApiLogicServer create` command.
+For information on Managing API Logic Projects, [click here](https://apilogicserver.github.io/Docs/Project-Structure).
 
+| About                    | Info                               |
+|:-------------------------|:-----------------------------------|
+| Created                  | creation-date                      |
+| API Logic Server Version | api_logic_server_version           |
+| Created in directory     | api_logic_server_project_directory |
+| API Name                 | api_logic_server_api_name          |
+| Execution begins with    | `api_logic_server_run.py`          |
 
 &nbsp;
 
-## 1. Open in Codespaces
-
-No install is required - this runs in the cloud, via your Browser, courtesy Codespaces.  Use your existing GitHub account (no signup is required), and:
+# Setup Instructions
 
-1. [__Click here__](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=593459232){:target="_blank" rel="noopener"} to open the *Create Codespace* page.
+Setup your Python environment, according to whether you did a *local install*, or *Docker*.  Choose the appropriate section, then run.
 
-2. Configure as desired, and click __Create codespace__.
+&nbsp;
 
->  This process takes about a minute.  Wait until you see the port created.
+## Establish Your Python Environment - Local Install
 
-<details markdown>
+You `requirements.txt` has already been created, so...
 
-<summary>What Is Happening</summary>
+```bash title="Install API Logic Server in a Virtual Environment"
+python -m venv venv                        # may require python3 -m venv venv
+venv\Scripts\activate                      # mac/linux: source venv/bin/activate
+python -m pip install -r requirements.txt  # accept "new Virtual environment"
+```
 
-You will now see 3 projects - open in VSCode, _in the Browser._  But that's just what you _see..._
+Notes:
 
-Behind the scenes, Codespaces has requisitioned a cloud machine, and loaded the template - with a _complete development environment_ - Python, your dependencies, git, etc.
+* See also the `venv_setup` directory in this API Logic Project.
 
-You are attached to this machine in your Browser, running VSCode.
+* If using SqlServer, install `pyodbc`.  Not required for docker-based projects.  For local installs, see the [Quick Start](https://apilogicserver.github.io/Docs/Install-pyodbc/).
 
-These instructions are now visible in VS Code, to minimize window switching.
+&nbsp;
 
+## Establish Your Python Environment - Docker
 
-> :trophy: Pretty remarkable.
+Your runtime systems are part of Dev Container, which you probably activated when you [opened the project](https://apilogicserver.github.io/Docs/IDE-Execute/).  
+ * If you did not accept the "Open in Container" option when you started VSCode, use __View > Command Palette > Remote-Containers: Reopen in Container__.
 
-</details>
+&nbsp;
 
-<details markdown>
+## Run
 
-<summary>Verify it worked</summary>
+To run your project
 
-VSCode will open in your Browser, and the project will perform various initialization tasks.  After about 1 minute, verify as follows:
+![Start Project](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/tutorial/2-apilogicproject-nutshell.png?raw=true)
 
-1. Port is created
-2. Port made public
-3. 3 Sample projects created
-3. `readme` opened, showing next step
+As shown above:
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/git-codespaces/verify-codespaces-tutorial.png?raw=true"></figure>
+1. Use the pre-supplied Run Configuration; use either:
+    * `**ApiLogicServer - No Security (e.g., for behave tests** to run *with security* (recommended initially)
+    * `**ApiLogicServer** to run [with security](https://apilogicserver.github.io/Docs/Security-Swagger/)
+2. Click the url in the console to start the Admin App
+    * Use it to explore your data (shown below)
+    * And your API (via Swagger)
 
-</details>
+![Admin App](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/ui-admin/run-admin-app.png?raw=true)
 
-These instructions will continue in Codespaces in the `readme.md` (double-click it if it does not open automatically).
 
 &nbsp;
 
-## 4. Explore the Readme
-
-[Open the Readme](readme.md) to explore the sample project.
-
-<details markdown>
-
-<summary>Tutorial Overview</summary>
-
-The Tutorial will enable you to explore 2 key aspects:
-
-* __Initial Automation__ - API and UI creation are automated from the data model. So, later, you'd see this level of automation for your own databases.
+# Appendix: Key Technologies
 
-* __Customization and Debugging__ - this sample also includes customizations for extending the API and declaring logic, and how to use VSCode to debug these.  The Tutorial will clearly identify such pre-built customizations.
-
-</details>
+API Logic Server is based on the projects shown below.
+Consult their documentation for important information.
 
 &nbsp;
 
-Extensive [product documentation is available here](https://valhuber.github.io/ApiLogicServer/) - checkout the [FAQs](https://valhuber.github.io/ApiLogicServer/FAQ-Frameworks/).
+### SARFS JSON:API Server
 
-&nbsp;
+[SAFRS: Python OpenAPI & JSON:API Framework](https://github.com/thomaxxl/safrs)
 
-# API Logic Server Background
+SAFRS is an acronym for SqlAlchemy Flask-Restful Swagger.
+The purpose of this framework is to help python developers create
+a self-documenting JSON API for sqlalchemy database objects and relationships.
 
-### Motivation
+These objects are serialized to JSON and 
+created, retrieved, updated and deleted through the JSON API.
+Optionally, custom resource object methods can be exposed and invoked using JSON.
 
-We looked at approaches for building database systems:  
+Class and method descriptions and examples can be provided
+in yaml syntax in the code comments.
 
-<br/>
+The description is parsed and shown in the swagger web interface.
+The result is an easy-to-use
+swagger/OpenAPI and JSON:API compliant API implementation.
 
-__Frameworks__
+&nbsp;
 
-Frameworks like Flask or Django enable you to build a single endpoint or _Hello World_ page, but a __multi-endpoint__ API and __multi-page__ application would take __weeks__ or more.
+### LogicBank
+[Transaction Logic for SQLAlchemy Object Models](https://apilogicserver.github.io/Docs/Logic-Why/)
 
-<br/>
+Use Logic Bank to govern SQLAlchemy update transaction logic - 
+multi-table derivations, constraints, and actions such as sending mail or messages. Logic consists of _both:_
 
-__Low Code Tools__
+*   **Rules - 40X** more concise using a spreadsheet-like paradigm, and
 
-These are great for building great UIs, but
+*   **Python - control and extensibility,** using standard tools and techniques
 
-* Want a multi-page app -- __without requiring detail layout for each screen__
-* Want to __preserve standard dev tools__ - VSCode, PyCharm, git, etc
-* Need an answer for __backend logic__ (it's nearly half the effort)
+Logic Bank is based on SQLAlchemy - it handles `before_flush` events to enforce your logic.
+Your logic therefore applies to any SQLAlchemy-based access - JSON:Api, Admin App, etc.
 
 &nbsp;
 
-### Our Approach: Instant, Standards-based Customization, Logic Automation
-
-API Logic Server is an open source Python project.  It runs as a standard Python (`pip`) install, or under Docker. It consists of:
-
-* a set of runtimes (api, user interface, data access) for project execution, plus 
+### SQLAlchemy
 
-* a CLI (Command Language Interface) to create executable projects with a single command
+[Object Relational Mapping for Python](https://docs.sqlalchemy.org/en/13/).
 
-Then,
+SQLAlchemy provides Python-friendly database access for Python.
 
-* Customize your projects in standard IDEs such as VSCode or PyCharm
+It is used by JSON:Api, Logic Bank, and the Admin App.
 
-* Declare multi-table derivation and constraint logic using spreadsheet-like rules
-
-    * :trophy: 40X more concise than code
-    * Extend with Python
-
-
-> :bulb: API Logic Server reads your schema, and creates an executable, customizable project.
+SQLAlchemy processing is based on Python `model` classes,
+created automatically by API Logic Server from your database,
+and saved in the `database` directory.
 
 &nbsp;
 
+### Admin App
+
+This generated project also contains a React Admin app:
+* Multi-page - including page transitions to "drill down"
+* Multi-table - master / details (with tab sheets)
+* Intelligent layout - favorite fields first, predictive joins, etc
+* Logic Aware - updates are monitored by business logic
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/docs/Logic-Tutorial.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/Tutorial.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,274 +1,317 @@
-# Automation + Collaboration: Fast, Right
+## About this Detailed Tutorial
 
-**Automated App Creation** (Working Software Now) enables **Collaboration** to uncover **Automated Rules.**
+This Detailed Tutorial is designed for these scenarios:
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/introduction.png?raw=true"></figure>
+* You are using **codespaces** / VSCode, open to either the [tutorial project](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=593459232), or [app_fiddle](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=594296622).
 
-This page explains how [API Logic Server](https://github.com/valhuber/ApiLogicServer/blob/main/README.md) Automation, coupled with an [Agile (TDD - Test Driven Development) Process](http://dannorth.net/introducing-bdd/), can dramatically improve Time to Market and reduce Requirements Risk:
-  
-1. **Automated App Creation:** API Logic Server creates an API Logic Project with a single command.  The project implements an **Admin App** and underlying API.
+* You are using a **local install** (pip install) version of API Logic Server, and have reviewed the [tutorial readme](https://github.com/ApiLogicServer/tutorial#readme).
 
-1. **Customer Collaboration:** the Admin App (Working Software, _Now_) drives collaboration, resulting in *Features* (Stories), *Scenarios* (tests), and *Logic Designs* that define how data is computed, validated, and processed (e.g., issues email or messages, auditing, etc.).
+* You are using a **docker version** of API Logic Server, and have reviewed the [tutorial readme](https://github.com/ApiLogicServer/tutorial#readme).
 
-1. **Automated Logic:** the Logic Design often translates directly into ***Executable* Rules,** which can be entered as customizations into the created API Logic Project.
+   * Projects are pre-configured for VS Code with `.devcontainer` and `launch configurations,` so these instructions are oriented around VS Code.
 
-2. **Transparency:** the [Behave Logic Report](#behave-logic-report) documents the functionality of the system: Features (Stories) and Scenarios (tests) that confirm its operation.  The report includes the underlying Rules, extending transparency to the implementation level.
+* You are reviewing the docs, and want to get a sense of the software
 
-&nbsp;&nbsp;
+In this tutorial, we will explore:
+
+* **create** - we will briefly review what actually happens during the create process.
 
-> **Key Takeaway:** automation drives Time to Market by providing working software rapidly; this drives agile collaboration to define systems that meet actual needs, reducing requirements risk.
+* **run** - we will first run the Admin App and the JSON:API.  These will illustrate how automation creates an app and API from a data model.  You can then infer what you'd get for one of your databases.
 
-> **Virtuous Cycle:** the collaboration uncovers Logic Designs, which can be declared as spreadsheet-like rules for API Logic Server automation.
+* **customize** - we will then explore some customizations already done for the API and logic, and how to debug them.
 
 &nbsp;&nbsp;
 
-# Resources
+---
+
+## Key Underlying Concepts
+This tutorial illustrates some key concepts:
+
+### _Declarative Models_, not code
+Observe that the files for the Admin App and API are models that describe _what, not how_.  This makes it much easier to understand than large amounts of generated code.
+
+### Preserve Customizations
+The system is designed to enable `rebuild`, so you can iterate the data model - _without losing your customizations._  In general, such customizations are kept in separate files from the model files.  So, the model files can be rebuilt without affecting customization files.
 
-After you've reviewed the [logic background](../Logic:-Rules-plus-Python), use this page to learn how to use logic.  Key resources:
-1. [Rule Summary](https://github.com/valhuber/LogicBank/wiki/Examples)
-2. [Sample Database](../Sample-Database)
-3. [Behave](https://behave.readthedocs.io/en/stable/tutorial.html) is a framework for defining and executing tests.  It is based on [TDD (Test Driven Development)](http://dannorth.net/introducing-bdd/), an Agile approach for defining system requirements as executable tests.
-  * Here are some [details for using Behave with API Logic Server](../Working-With-Behave).
+### Logic Automation
+A unique feature of API Logic Server is provision for spreadsheet-like rules, customizable with Python.  Rules address update logic (multi-table derivations and constraints), and security (authorization).
 
 &nbsp;&nbsp;
 
-# Process Overview
+---
 
-The diagram below provides more detail on the development process, further explained in the sections below.
+## Create
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/TDD-process.png?raw=true"></figure>
+[![Using VS Code](https://github.com/valhuber/apilogicserver/wiki/images//creates-and-runs-video.jpg?raw=true?raw=true)](https://youtu.be/tOojjEAct4M "Using VS Code with the ApiLogicServer container - click for video")
 
-&nbsp;&nbsp;
+The diagram above summarizes the create / run / customize process.  When you issue the `ApiLogicServer create` CLI command, the system reads your schema and creates a customizable API Logic Project.
+
+> It's a video - click to view.
 
-## 1. Create Api Logic Project
+&nbsp;
 
-API Logic Server is used once you have a preliminary database design.  Use your existing procedures for database design.  Include at least minimal test data.
+## Create and establish Python Environment
 
-Then (presuming API Logic Server [is installed](https://github.com/valhuber/ApiLogicServer/blob/main/README.md)), create the project with this command, using `venv` based installs:
+After creation, you must establish your Python environment:
 
-```
-ApiLogicServer create  --db_url= --project_name=
-```
+* This is already complete for Codespace users
+* Other users - please  see [Quick Start > Express Install](https://valhuber.github.io/ApiLogicServer/IDE-Execute/).  Note there are different instructions, depending on how your install / IDE.
 
-or, like this, using docker-based installs:
-```
-ApiLogicServer create --db_url= --project_name=/localhost/ApiLogicProject
-```
 
 &nbsp;&nbsp;
 
-#### 1a. Creates **Admin App**
+## Start the Server and Admin App
 
-The Agile objective of collaboration is typically best-served with _running_ screens.  The problem is, it takes quite a long time to create the API and screens to reach this point.  And this work can be wasted if there were misunderstandings.
+> Stop any running servers that might still be running from the readme - &nbsp;&nbsp;(square red button at top in "Show me how", below).
 
-Ideally, User Interface creation would be automatic.
+Now (see *Show me how*, below, for details):
 
-So, the API Logic Server `create` command above builds first-cut screens, automatically from the data model.  
+1. Start the server with **Run and Debug >> *2. API Logic Project: Instant, Open***, and then 
+2. Start the Browser at localhost:5656 by **clicking the url shown in the console log.**
 
-The app shown below [(more detail here)](https://github.com/valhuber/ApiLogicServer#admin-app-multi-page-multi-table-automatic-joins) is suitable for initial _business user collaboration_ (further discussed below), and basic _back office_ data maintenance.
+<details markdown>
 
-You can [customize it](https://github.com/valhuber/ApiLogicServer#admin-app-customization) by editing a simple `yaml`file (e.g, field captions, ordering etc.)
+<summary> Show me how </summary>
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/ui-admin/run-admin-app.png?raw=true"></figure>
+&nbsp;
 
-&nbsp;&nbsp;
+To run the ApiLogicProject app:
 
->  **Key Takeaway:** Admin App Automation enables collaboration, instantly.
+1. Start the Server:
 
-&nbsp;&nbsp;
+    1. Click **Run and Debug**
+    2. Use the dropdown to select **3. API Logic Project: Logic**, and
+    3. Click the green button to start the server
+<br><br>
 
-#### 1b. Also creates **API**
+2. Start the Browser at localhost:5656 by **clicking the url shown in the console log.**
 
-It is not difficult to create a single endpoint API.  The problem is that it's quite a bit more work to create an endpoint for each table, with support for related data, pagination, filtering and sorting.
+<figure><img src="https://github.com/ApiLogicServer/Docs/blob/main/docs/images/tutorial/2-apilogicproject.png?raw=true"></figure>
 
-Ideally, API creation would be automatic.
+</details>
 
-So, the API Logic Server `create` command above builds such an API instantly, suitable for _application integration_, and creating _custom User Interfaces_.  The API enforces the business logic described below.
+&nbsp;
 
-The [created project is customizable,](https://github.com/valhuber/ApiLogicServer/blob/main/README.md#customize-and-debug) using a standard IDE.
+---
 
-&nbsp;&nbsp;
+## Run
 
->  **Key Takeaway:** automatic API creation, with support for related data, pagination, filtering and sorting.
+With the server started and the Admin App open in your Browser, we are ready to explore the Admin App and the API.
 
-&nbsp;&nbsp;
+&nbsp;
 
-## 2. Collaborate using **Admin App**
+### Admin App: Multi-Page, Multi-Table, Automatic Joins
 
-As noted above, running screens are an excellent way to engage business user collaboration, and ensure the system meets actual user needs.  Such collaboration typically leads in two important directions, described below.
+After starting the server and browser, explore the Admin App in your browser:
 
-&nbsp;&nbsp;
+1. Navigate to `Customer`
+      * Depending on your screen size, you may need to hit the "hamburger menu" (top left) to see the left menu<br/><br/>
+2. Click the first Customer row  to see Customer Details
+3. Observe the `Placed Order List` tab at the bottom
+4. Click the first Order row
+5. Observe the `Order Detail List` tab at the bottom
+6. Observe the elements shown in the diagram
 
-#### 2a. Iterate Data Model
+      * Multi-Page - 2 pages for each table (list, with search, and display)
+      * Multi-Table - database relationships (typically from foreign keys) used to build master/detail pages
+      * Automatic Joins - the Order Detail table contains `ProductId`, but the system has joined in the `Product Name`.  You can edit the `admin.yaml` file to control such behavior.
 
-You may discover that the data model is incorrect (_"Wait!  Customers have multiple addresses!!"_).  
+7. __Leave the server and browser running__
 
-In a conventional system, this would mean revising the API and App.  However, since these are created instantly through automation, such iterations are trivial.  Just rebuild.
+<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/ui-admin/run-admin-app.png?raw=true"></figure>
 
 &nbsp;&nbsp;
 
-#### 2b. Define Behave Scenarios
+  > **Key Take-away:** instant multi-page / multi-table admin apps, suitable for **back office, and instant agile collaboration.**
 
-Running screens also spark insight about the Features ("Place Order") and Scenarios ("Check Credit"): _"When the customer places an order, we need to reject it if it exceeds the credit limit"._  Capture these as described below.
+&nbsp;
 
-Behave is designed for business user collaboration by making Features and Scenarios transparent.  Start using Behave by defining one or more `.feature` files.
+### JSON:API - Related Data, Filtering, Sorting, Pagination, Swagger
 
-For example, see the `place_order.feature`, as tested by the `Bad Order: Custom Service` Scenario, below.
+Your API is instantly ready to support ui and integration
+development, available in swagger, as shown below.  JSON:APIs are interesting because they
+are client configurable to **reduce network traffic** and **minimize organizational dependencies.**
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/scenario.png?raw=true"></figure>
+The creation process builds not only the API, but also swagger so you can explore it.  The Admin App Home page provides a link to the swagger.  In the browser:
 
-&nbsp;&nbsp;
+1. Click __Home__ to open the Home Page
+2. Click "2. API with __oas/Swagger__" to see the swagger
+3. (Leave the swagger and server running)
 
-##### Add Custom Service
+<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/ui-admin/swagger.png?raw=true"></figure>
+&nbsp;&nbsp;&nbsp;
 
-While the automatically-created API is a great start, you may uncover a need for a custom service.  This is easy to add - it's only about 10 lines of Python (`api/customize_api.py`), since the logic (discussed below) is enforced in the underlying data access.  For details, [see here](https://github.com/valhuber/ApiLogicServer/blob/main/README.md#api-customization).
+  > **Key Take-away:** instant *rich* APIs, with filtering, sorting, pagination and swagger.  **Custom App Dev is unblocked.**
 
 &nbsp;&nbsp;
 
-#### 2c. Logic Design
+---
 
-We now choose a scenario (e.g, `Bad Order`), and engage business users for a clear understanding of _check credit_.  This follows a ___familiar step-wise definition of terms:___
+## Customize and Debug
 
-| Analyst Question         | Business User Answer               |
-|:-------------------------|:-----------------------------------|
-| What do you mean by _Check Credit_?                      | The balance must be less than the credit limit
-| What is the _Balance_?  | The sum of the unshipped order amount totals
-| What is the Order _AmountTotal_? | The sum of the Order Detail Amounts           |
-| What is the _Amount_?     | Price * Quantity |
-| What is the _Price_?                 | It's copied from the Product (unaffected by subsequent changes)          |
+That's quite a good start on a project.  But we've all seen generators that get close, but fail because the results cannot be extended, debugged, or managed with tools such as git and diff.
 
-We capture in text as shown below.
+Let's examine how API Logic Server projects can be customized for both APIs and logic.  We'll first have a quick look at the created project structure, then some typical customizations.
 
-Note this "cocktail napkin spec" is short, yet clear.  That's because instead of diving unto unnecessary technical detail of _how_ (such as pseudocode), it focuses on ___what___.
+To run the customized app:
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/logic-spec.png?raw=true"></figure>
-  
+1. Stop the server
+2. Restart the server with **Run and Debug >> *3. API Logic Project: Logic***, and then
+3. Start the Browser at localhost:5656 by **clicking the url shown in the console log.**
+4. Re-access the swagger, and authorize (see below):
+   * Click "2. API with __oas/Swagger__" to see the swagger (as you did above)
+   * Get an **access_token** and **authorize** (see Show me how, below)
 
-&nbsp;&nbsp;
+<details markdown>
 
-## 3a. Declare Logic (from design)
+<summary> Show me how </summary>
 
-Business Logic is the heart of the system, enforcing our business policies.  Logic consists of multi-table constraints and derivations, and actions such as sending email and messages.  A core Behave objective is to define and test such behavior.
+&nbsp;
 
-It's generally accepted that such domain-specific logic _must_ require domain-specific code.  The problem is that this is:
-* **slow** (it's often nearly half the system).
-* **opaque** to business users.
-* **painful to maintain** - it's no secret that developers hate maintenance, since it's less coding than _"archaeology"._  A painful amount of time is spent reading the existing code, to understand where to insert the new logic.
+**Get `access_token`:**
 
-Ideally, our ___logic design is executable.___  
+* Click the `auth/Post` endpoint (at the end of the swagger)
+* Click **Try it out**
+* Click **Execute** (you'll need to scroll down a bit)
+* Copy the `access_token` to your clipboard
 
-So, API Logic Server provides Logic Automation, where logic is implemented as:
+<figure><img src="https://github.com/ApiLogicServer/Docs/blob/main/docs/images/security/token-get.png?raw=true"></figure>
 
-* [Spreadsheet-like ***rules***](https://github.com/valhuber/LogicBank/wiki/Examples) for multi-table derivations and constraints, and
+&nbsp;
+**Authenticate with your `access_token`**
 
-* Python, to implement logic not addressed in rules such as sending email or messages
+* Scroll up to the top of the swagger, and click **Authorize**
+* Enter **Bearer**, add a space, **paste** your `access_token`, click **Authorize**, and **Close** the dialog 
 
-So, [instead of several hundred lines of code](https://github.com/valhuber/LogicBank/wiki/by-code), we declare 5 rules [(more details here)](https://github.com/valhuber/ApiLogicServer/blob/main/README.md#logic).  
+<figure><img src="https://github.com/ApiLogicServer/Docs/blob/main/docs/images/security/token-auth.png?raw=true"></figure>
 
-Rules are entered in Python, with code completion, as shown below.  Observe how they exactly correspond to our design, and are executable by the API Logic Server rules engine:
+</details>
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/declare-logic.png?raw=true"></figure>
+&nbsp;
 
-Unlike manual code, logic is ***declarative:***
+### Project Structure
+Use VS Code's **Project Explorer** to see the project structure under *3. ApiLogicProject_Logic*:
 
-* **automatically reused** - re-use is usually achieved by careful design; rules make re-use automatic:
-  * Since rules are about the data (not a specific transaction), they automate all the transactions that touch the data (add order, delete order, change order shipped date, etc).  Even ones you might have overlooked (move order to different customer).
-  * Since rules are enforced as part of the API, they are automatically shared across *all* screens and services.
-* **automatically ordered** - maintenance is simply altering the rules; the system computes their execution order by automatically discovering their dependencies.  No more archaeology.
-* **transparent** - business users can read the spreadsheet-like rules.  We'll exploit this in the Behave Logic Report, described below.
+| Directory | Usage                         | Key Customization File             | Typical Customization                                                                 |
+|:-------------- |:------------------------------|:-----------------------------------|:--------------------------------------------------------------------------------------|
+| ```api``` | JSON:API                      | ```api/customize_api.py```         | Add new end points / services                                                         |
+| ```database``` | SQLAlchemy Data Model Classes | ```database/customize_models.py``` | Add derived attributes, and relationships missing in the schema                       |
+| ```logic``` | Transactional Logic           | ```logic/declare_logic.py```       | Declare multi-table derivations, constraints, and events such as send mail / messages |
+| ```security``` | Admin App                     | ```security/declare_security.py```          | Control role-based access to data rows                                                 |
+| ```ui``` | Admin App                     | ```ui/admin/admin.yaml```          | Control field display, ordering, etc.                                                 |
 
+<figure><img src="https://raw.githubusercontent.com/valhuber/ApiLogicServer/main/images/generated-project.png"></figure>
 
-&nbsp;&nbsp;
+Let's now explore some examples.
 
->  **Key Takeaway:** spreadsheet-like rules can dramatically reduce the effort for backend logic, and make it transparent
+### Admin App Customization
+There is no code for the Admin app - it's behavior is declared in the `admin.yaml` model file.  Alter this file to control labels, hide fields, change display order, etc:
 
-&nbsp;&nbsp;
+1. In your IDE, open **Explorer > 3. ApiLogicProject_Logic/ui/admin/admin.yaml**
+   * Find and alter the string `- label: 'Placed Order List'` (e.g, make it plural)
+   * Click Save
+3. Load the updated configuration: in the running Admin App, click __Configuration > Reset__ and __Apply__
+4. Revisit **Customer > Order** to observe the new label
 
->  **Key Takeaway:** keep your Logic Design high level (_what_ not _how_ -- think spreadsheet), and your design will often map directly to executable rules. 
+&nbsp;&nbsp;&nbsp;
 
-&nbsp;&nbsp;
+  > **Key Take-away:** you can alter labels, which fields are displayed and their order, etc -- via a simple model.  No need to learn a new framework, or deal with low-level code or html.
 
-## 3b. Code/Run Behave Scenarios
 
-Implement the actual scenarios (tests) in Python (`place_order.py`), using annotations (`@when`) to match scenarios and implementations.  In this project, the implementation is basically calling APIs to get old data, run transactions, and check results.
+&nbsp;&nbsp;&nbsp;
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/TDD-ide.png?raw=true"></figure>
+### API Customization
 
-Execute the tests using the pre-supplied Launch Configurations:
+While a standards-based API is a great start, sometimes you need custom endpoints tailored exactly to your business requirement.  You can create these as shown below, where we create an additional endpoint for `add_order`.
 
-1. Run Launch Configuration `API Logic Server` 
-1. Run Launch Configuration `Run Behave Logic` 
+To review the implementation: 
 
-The rules fire as transactions are run, and produce Logic Log files later used in Report Behave Logic (described below): 
+1. In your IDE, open **Explorer > 3. ApiLogicProject_Logic/api/customize_api.py**:
+3. Set the breakpoint as shown in `add_order`
+4. Use the swagger to access the `ServicesEndPoint > add_order`, and
+   1. **Try it out**, then 
+   2. **execute**
+5. Your breakpoint will be hit
+   1. You can examine the variables, step, etc.
+6. Click **Continue** on the floating debug menu (upper right in screen shot below)
 
-1. `test/api_logic_server_behave/behave.log` - summarizes test success / failure
-2. `api_logic_server_behave/scenario_logic_logs/Bad_Order_Custom_Service.log` - [Logic Log output](../Logic:-Rules-plus-Python#debugging).
-   * The code on line 161 signals the name of Logic Log
-   * Note the Logic Log actually consists of 2 sections:
-      * The first shows each rule firing, including complete old/new row values, with indentation for `multi-table chaining`
-      * The "Rules Fired" summarizes which rules actually fired, representing a _confirmation of our Logic Design_
+<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/tutorial/customize-api.png?raw=true"></figure>
 
->  You can use the debugger to stop in a test and verify results
+&nbsp;
 
-&nbsp;&nbsp;
+### Logic
+API and UI automation are impressive answers to _familiar_ challenges.  Logic automation is a _unique_ answer to a significant and unaddressed problem:
 
-## 4. **Create Behave Logic Report**
+> For transaction systems, backend constraint and derivation logic is often nearly *half* the system.  This is not addressed by conventional approaches of "your code goes here".
+ 
+The *logic* portion of API *Logic* server is a declarative approach - you declare spreadsheet-like rules for multi-table constraints and derivations.  The 5 rules shown below represent the same logic as 200 lines of Python - a remarkable **40X.**
 
-The log files are pretty interesting: a record of all our Features and Scenarios, including transparent underlying logic.  The problem is that it's buried in some text files inside our project.
+> Since they automate all the re-use and dependency management, rules are [40X more concise](https://github.com/valhuber/LogicBank/wiki/by-code) than code.  Like a spreadsheet, rules __watch__ for changes, __react__ by automatically executing relevant rules, which can __chain__ to activate other rules; you can [visualize the process here](https://valhuber.github.io/ApiLogicServer/Logic-Operation/#watch-react-chain).
 
-Ideally, publishing this in a transparent manner (e.g., a wiki accessible via the Browser) would be a great asset to the team.
+[Logic](https://valhuber.github.io/ApiLogicServer/Logic-Why/) consists of rules **and** conventional Python code.  Explore it like this:
 
-So, API Logic Server provides `report_behave_logic.py` to create a Behave Logic Report - _including logic_ - as a wiki file.
+1. Open **Explorer > 3. ApiLogicProject_Logic/logic/declare_logic.py**:
+   * Observe the 5 rules highlighted in the diagram below.  These are built with code completion.
+2. Set a breakpoint as shown in `congratulate_sales_rep`
+   * This event illustrates that logic is mainly _rules,_ customizable with standard _Python code_
+3. Using swagger, re-execute the `add_order` endpoint
+4. When you hit the breakpoint, expand `row` VARIABLES list (top left)
 
-To run it, use Launch Configuration `Behave Logic Report`:
+<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/tutorial/debug-logic.png?raw=true"></figure>
 
-1. Reads your current `readme.md` file (text like you are reading now), and
-2. Appends the [Behave Logic Report:](#behave-logic-report) by processing the files created in step 3b
-   1. Reading the `behave.log`, and
-   2. Injecting the `scenario_logic_logs` files
-3. Creates the output report as a wiki file named `report_behave_logic.md`
+Internally, rules execute by listening to SQLAlchemy `before_flush` events, as [described here](https://valhuber.github.io/ApiLogicServer/Logic-Operation/#how-usage-and-operation-overview).
 
-&nbsp;&nbsp;
+> This rule architecture ensures that rules are always re-used across all client applications and integrations.  This avoids common "fat client" approaches that embed logic in user interface controllers, which leads to replication and inconsistency.
 
->  **Key Takeaway:** Behave makes *requirements and tests* transparent; rules make your *logic* transparent; combine them both into the [**Behave Logic Report.**](#behave-logic-report)
+&nbsp;
 
-&nbsp;&nbsp;
+### Security Logic
+The declarative approach addresses not only multi-table derivation and constraint logic, it addresses security.  This controls who can login, and what data they see.  
+
+The overview Tutorial noted how grants on the `Category` table controlled what rows users like _u1_ and _u2_ were able to see.  The grant logic is in `security/declare_security.py`.  For more on security, [see here](https://apilogicserver.github.io/Docs/Security-Overview/).
 
-# Process Summary: Automation + Collaboration
+&nbsp;&nbsp;
 
-We've seen these key points:
+---
 
-1. API Logic Server kick-starts projects with **automated creation of Admin Apps**.
+## Test
 
-2. Working software promotes **business user collaboration** using Behave, to iterate the data model and create Logic Designs.
+You can test using standard api and ui test tools.  We recommend exploring the [Behave framework](https://valhuber.github.io/ApiLogicServer/Behave/).  This can be used as part of an overall agile approach as described in the [Logic Tutorial](https://valhuber.github.io/ApiLogicServer/Logic-Tutorial/).
 
-3. Logic Designs are automated with **spreadsheet-like rules**.
+TL;DR - features and test scripts are predefined in the sample; to run them (with the server running):
 
-4. Behave creates an **executable Test Suite**.
+1. Run Launch Configuration `Behave Run Behave` 
+2. Run Launch Configuration ``Behave Logic Report`` 
+3. Open `test/api_logic_server_behave/reports/Behave Logic Report.md`
 
-5. Test Suite execution creates a **Behave Logic Report:** your Features, Scenarios, Test Results, _and_ the underlying rules-based logic.
+&nbsp;&nbsp;
 
-Automation enables you to **deliver projects faster**; the Agile/Behave encourages collaboration to **reduce requirements risk**.
+   > The sample Scenarios below were chosen to illustrate the basic patterns of using rules. Open the disclosure box ("Tests - and their logic...") to see the implementation and notes.   
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/behave/introduction.png?raw=true"></figure>
-  
+For more information, see [Testing with Behave](https://valhuber.github.io/ApiLogicServer/Behave/).
 
 &nbsp;&nbsp;
 
-# Appendix: Executing Basic Tests
+---
 
-In addition to Behave, you can use manual approaches for testing:
+## Wrap up
+Let's recap what you've seen:
 
-<details markdown>
-<summary>Click to see how to run Basic tests</summary>
+* **ApiLogicProject Creation and Execution** - a database API and an Admin App - created automatically from a database, in moments instead of weeks or months
 
-<figure><img src="https://github.com/valhuber/apilogicserver/wiki/images/logic/run-server-test.png" title="run instructions"></figure>
 
-After you've [created the sample project](../Quick-Start), you can execute pre-defined tests as shown above:
+* **Customizable** - the UI, API and Logic - using Visual Studio code, for both editing and debugging
 
-1. Start the Server (e.g., under VS Code, Launch Configuration *ApiLogicServer*)
-2. Open a terminal window, and `cd test/basic; python server_test.py go`
-3. Examine the log in the *Debug Console*
 
->  You can build similar tests for your systems as you would in any project, either in Python (as shown here), in shell scripts (see the supplied example), etc.
-</details>
+### Next Steps
+
+After the Tutorial, these are excellent next steps:
+
+* Try other databases - here are [some installed samples](https://valhuber.github.io/ApiLogicServer/Data-Model-Examples/), and try your own
+* Explore the [Logic Tutorial](https://valhuber.github.io/ApiLogicServer/Logic-Tutorial/).
+
+
+### Docker cleanup
+VS Code leaves the container and image definitions intact, so you can quickly resume your session.  You may wish to delete this. It will look something like `vsc-ApiLogicProject...`.
+
+&nbsp;&nbsp;&nbsp;
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/extended_builder.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/extended_builder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/Todo_modelsZZ.py.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/fragments/Todo_modelsZZ.py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/configZZ.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/fragments/configZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/modelsZZ.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/fragments/modelsZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/nw_virtual_attrs.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/fragments/nw_virtual_attrs.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/fragments/ui_basic_web_app_runZZ.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/logging.yml` & `ApiLogicServer-8.4.0/api_logic_server_cli/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/ApiLogicServer.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Report_Behave_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/Windows_Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run___No_Security.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.idea/runConfigurations/run_docker.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/.vscode/launch.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/customize_api.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/customize_api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/json_encoder.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api/readme_customize_api.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api/readme_customize_api.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/api_logic_server_run.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/api_logic_server_run.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/config.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/env.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic/readme.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/alembic.ini` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/alembic.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/database/bind_databases.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/database/bind_databases.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.Dockerfile`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/authdb_mysql.sql`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/docker/build_image.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/docker/build_image.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/git_push_new_project.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logging.yml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/declare_logic.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/logic/readme_declare_logic.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/mypy.ini` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/mypy.ini`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/python_anywhere_wsgi.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/devops/python-anywhere/python_anywhere_wsgi.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.ps1` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/run.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/run.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/run.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/abstract_authentication_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/mem_auth_row.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/abstract_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/memory/auth_provider_no_swagger.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/auth_provider.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/authentication_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/__pycache__/db_auth.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/authentication_provider/sql/sqlite/auth_provider.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/declare_security.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze-th.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/notes_temp/pip-freeze.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/notes_temp/token.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/notes_temp/token.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/__pycache__/security_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authentication.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/authentication.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/authorization.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/authorization.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/security/system/custom_swagger.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/security/system/custom_swagger.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/templates/index.html` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_logic_report.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/behave_run.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/api_logic_server_behave/features/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/test/basic/server_test.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/admin/admin_loader.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/admin/home.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/andrew.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/anne.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/janet.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/laura.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/margaret.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/michael.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/nancy.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/robert.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Employee/steven.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/ui/images/Product/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/util.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/py.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/py.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/readme_venv.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/requirements-no-cli.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/venv-linux.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.ps1` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/venv.ps1`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype/venv_setup/venv.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype/venv_setup/venv.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/db.png` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/images/allocation/db.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/images/logic-diagram.png` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/images/allocation/logic-diagram.png`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/logic/declare_logic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/readme-allocation.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/Logic-Allocation.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Allocate Payment to Outstanding Orders
 
-This project is to illustrate the use of [Allocation](https://github.com/valhuber/LogicBank/wiki/Sample-Project---Allocation).
+This project is to illustrate the use of Allcation.
 
 Allocation is a pattern where:
 
 > A ```Provider``` allocates to a list of ```Recipients```,
 >creating ```Allocation``` rows.
 
 
@@ -12,15 +12,15 @@
 ```Orders```, and pays all/several off with a single ```Payment```.
 
 
 &nbsp;&nbsp;
 
 ## Data Model
 
-![Background](/images/db.png?raw=true "Optional Title")
+![Background](images/allocation/db.png "Overview")
 
 ## Requirements
 When the ```Payment``` is inserted, our system must:
 1. Allocate the ```Payment``` to ```Orders``` that have ```AmountOwed```, oldest first
 1. Keep track of how the ```Payment``` is allocated, by creating 
 a ```PaymentAllocation```
 1. As the ```Payment``` is allocated,
@@ -29,37 +29,32 @@
 
 
 &nbsp;&nbsp;
 
 
 # Setup
 
-The usual:
+Create the project:
+
 ```
-python -m venv venv
-source venv/bin/activate
-pip install -r requirements.txt
+ApiLogicServer create --project_name=allocation --db_url=allocation
 ```
-
-This should enable you to run launch configuration `ApiLogicServer`.
+After you establish the venv in the usual manner, you canopen the project in your IDE and run launch configuration `ApiLogicServer`.
 
 
 # Test
-Use Admin app, or
-
-cURL:
-```
-curl -X POST "http://localhost:5656/api/Payment/" -H  "accept: application/vnd.api+json" -H  "Content-Type: application/json" -d "{  \"data\": {    \"attributes\": {      \"Amount\": 100,      \"AmountUnAllocated\": 0,      \"CustomerId\": \"ALFKI\"    },    \"type\": \"Payment\"  }}"
-```
 
+Use `sh test/test.sh`
 
 &nbsp;&nbsp;
 
 # Walkthrough
 
+![Walkthrough](images/allocation/logic-diagram.png "Overview")
+
 The test illustrates allocation logic for our inserted payment,
 which operates as follows:
 1. The triggering event is the insertion of a ```Payment```, which triggers:
 1. The ```allocate``` rule.  It performs the allocation:
    1. Obtains the list of recipient orders by calling the function```unpaid_orders```
    1. For each recipient (```Order```), the system...
       1. Creates a ```PaymentAllocation```, links it to the ```Order``` and ```Payment```,
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_allocation/test/test.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_allocation/test/test.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -252,20 +252,20 @@
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 001e 0000 0003  ................
 00001010: 0061 0070 0069 6c67 3153 636f 6d70 0000  .a.p.ilg1Scomp..
-00001020: 0000 0000 13be 0000 0003 0061 0070 0069  ...........a.p.i
-00001030: 6d6f 4444 626c 6f62 0000 0008 83c6 8653  moDDblob.......S
-00001040: 596d c441 0000 0003 0061 0070 0069 6d6f  Ym.A.....a.p.imo
-00001050: 6444 626c 6f62 0000 0008 83c6 8653 596d  dDblob.......SYm
+00001020: 0000 0000 a9ed 0000 0003 0061 0070 0069  ...........a.p.i
+00001030: 6d6f 4444 626c 6f62 0000 0008 b7e5 90d0  moDDblob........
+00001040: ddfe c441 0000 0003 0061 0070 0069 6d6f  ...A.....a.p.imo
+00001050: 6444 626c 6f62 0000 0008 b7e5 90d0 ddfe  dDblob..........
 00001060: c441 0000 0003 0061 0070 0069 7068 3153  .A.....a.p.iph1S
-00001070: 636f 6d70 0000 0000 0000 2000 0000 0008  comp...... .....
+00001070: 636f 6d70 0000 0000 0000 d000 0000 0008  comp............
 00001080: 0064 0061 0074 0061 0062 0061 0073 0065  .d.a.t.a.b.a.s.e
 00001090: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
 000010a0: 7374 3030 d601 0203 0405 0607 0709 070b  st00............
 000010b0: 075d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000010c0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
 000010d0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
 000010e0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
@@ -273,15 +273,15 @@
 00001100: 5369 6465 6261 7209 0908 095f 1018 7b7b  Sidebar...._..{{
 00001110: 3235 342c 2032 387d 2c20 7b31 3039 312c  254, 28}, {1091,
 00001120: 2034 3932 7d7d 0908 1523 2f3b 525f 6b6c   492}}...#/;R_kl
 00001130: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
 00001140: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00001150: 0000 008b 0000 0008 0064 0061 0074 0061  .........d.a.t.a
 00001160: 0062 0061 0073 0065 6c67 3153 636f 6d70  .b.a.s.elg1Scomp
-00001170: 0000 0000 0000 06a1 0000 0008 0064 0061  .............d.a
+00001170: 0000 0000 0000 0bbd 0000 0008 0064 0061  .............d.a
 00001180: 0074 0061 0062 0061 0073 0065 6c73 7643  .t.a.b.a.s.elsvC
 00001190: 626c 6f62 0000 0316 6270 6c69 7374 3030  blob....bplist00
 000011a0: d801 0203 0405 0607 0809 0a0b 1b56 5758  .............VWX
 000011b0: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
 000011c0: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 000011d0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 000011e0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -376,53 +376,53 @@
 00001770: 7400 6100 6200 6100 7300 656d 6f64 4462  t.a.b.a.s.emodDb
 00001780: 6c6f 6200 0000 0889 6b44 36b8 92c4 4100  lob.....kD6...A.
 00001790: 0000 0800 6400 6100 7400 6100 6200 6100  ....d.a.t.a.b.a.
 000017a0: 7300 6570 6831 5363 6f6d 7000 0000 0000  s.eph1Scomp.....
 000017b0: 0030 0000 0000 0800 6400 6100 7400 6100  .0......d.a.t.a.
 000017c0: 6200 6100 7300 6576 5372 6e6c 6f6e 6700  b.a.s.evSrnlong.
 000017d0: 0000 0100 0000 0500 6c00 6f00 6700 6900  ........l.o.g.i.
-000017e0: 636c 6731 5363 6f6d 7000 0000 0000 0027  clg1Scomp......'
-000017f0: 9600 0000 0500 6c00 6f00 6700 6900 636d  ......l.o.g.i.cm
+000017e0: 636c 6731 5363 6f6d 7000 0000 0000 0029  clg1Scomp......)
+000017f0: b600 0000 0500 6c00 6f00 6700 6900 636d  ......l.o.g.i.cm
 00001800: 6f44 4462 6c6f 6200 0000 0835 8486 3d6a  oDDblob....5..=j
 00001810: 55c4 4100 0000 0500 6c00 6f00 6700 6900  U.A.....l.o.g.i.
 00001820: 636d 6f64 4462 6c6f 6200 0000 0835 8486  cmodDblob....5..
 00001830: 3d6a 55c4 4100 0000 0500 6c00 6f00 6700  =jU.A.....l.o.g.
 00001840: 6900 6370 6831 5363 6f6d 7000 0000 0000  i.cph1Scomp.....
 00001850: 0030 0000 0000 0800 7300 6500 6300 7500  .0......s.e.c.u.
 00001860: 7200 6900 7400 796c 6731 5363 6f6d 7000  r.i.t.ylg1Scomp.
-00001870: 0000 0000 0003 9600 0000 0800 7300 6500  ............s.e.
+00001870: 0000 0000 0004 8600 0000 0800 7300 6500  ............s.e.
 00001880: 6300 7500 7200 6900 7400 796d 6f44 4462  c.u.r.i.t.ymoDDb
 00001890: 6c6f 6200 0000 0842 2c22 cd60 aac4 4100  lob....B,".`..A.
 000018a0: 0000 0800 7300 6500 6300 7500 7200 6900  ....s.e.c.u.r.i.
 000018b0: 7400 796d 6f64 4462 6c6f 6200 0000 0842  t.ymodDblob....B
 000018c0: 2c22 cd60 aac4 4100 0000 0800 7300 6500  ,".`..A.....s.e.
 000018d0: 6300 7500 7200 6900 7400 7970 6831 5363  c.u.r.i.t.yph1Sc
 000018e0: 6f6d 7000 0000 0000 0010 0000 0000 0400  omp.............
 000018f0: 7400 6500 7300 746c 6731 5363 6f6d 7000  t.e.s.tlg1Scomp.
-00001900: 0000 0000 0235 fe00 0000 0400 7400 6500  .....5......t.e.
+00001900: 0000 0000 023a 1800 0000 0400 7400 6500  .....:......t.e.
 00001910: 7300 746d 6f44 4462 6c6f 6200 0000 0892  s.tmoDDblob.....
 00001920: b586 3d6a 55c4 4100 0000 0400 7400 6500  ..=jU.A.....t.e.
 00001930: 7300 746d 6f64 4462 6c6f 6200 0000 0892  s.tmodDblob.....
 00001940: b586 3d6a 55c4 4100 0000 0400 7400 6500  ..=jU.A.....t.e.
 00001950: 7300 7470 6831 5363 6f6d 7000 0000 0000  s.tph1Scomp.....
-00001960: 0380 0000 0000 0200 7500 6962 7773 7062  ........u.ibwspb
+00001960: 0390 0000 0000 0200 7500 6962 7773 7062  ........u.ibwspb
 00001970: 6c6f 6200 0000 b762 706c 6973 7430 30d6  lob....bplist00.
 00001980: 0102 0304 0506 0707 0907 0b07 5d53 686f  ............]Sho
 00001990: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
 000019a0: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
 000019b0: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
 000019c0: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
 000019d0: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
 000019e0: 6172 0909 0809 5f10 177b 7b35 342c 2033  ar...._..{{54, 3
 000019f0: 3038 7d2c 207b 3932 302c 2034 3932 7d7d  08}, {920, 492}}
 00001a00: 0908 1523 2f3b 525f 6b6c 6d6e 6f89 0000  ...#/;R_klmno...
 00001a10: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 00001a20: 0000 0000 0000 0000 0000 0000 008a 0000  ................
 00001a30: 0002 0075 0069 6c67 3153 636f 6d70 0000  ...u.ilg1Scomp..
-00001a40: 0000 0002 1957 0000 0002 0075 0069 6d6f  .....W.....u.imo
+00001a40: 0000 0002 1c1a 0000 0002 0075 0069 6d6f  ...........u.imo
 00001a50: 4444 626c 6f62 0000 0008 5586 4226 888f  DDblob....U.B&..
 00001a60: c441 0000 0002 0075 0069 6d6f 6444 626c  .A.....u.imodDbl
 00001a70: 6f62 0000 0008 5586 4226 888f c441 0000  ob....U.B&...A..
 00001a80: 0002 0075 0069 7068 3153 636f 6d70 0000  ...u.iph1Scomp..
 00001a90: 0000 0002 b000 0000 0002 0075 0069 7653  ...........u.ivS
 00001aa0: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -632,10 +632,10 @@
 00002770: 7400 6100 6200 6100 7300 656d 6f64 4462  t.a.b.a.s.emodDb
 00002780: 6c6f 6200 0000 0889 6b44 36b8 92c4 4100  lob.....kD6...A.
 00002790: 0000 0800 6400 6100 7400 6100 6200 6100  ....d.a.t.a.b.a.
 000027a0: 7300 6570 6831 5363 6f6d 7000 0000 0000  s.eph1Scomp.....
 000027b0: 0030 0000 0000 0800 6400 6100 7400 6100  .0......d.a.t.a.
 000027c0: 6200 6100 7300 6576 5372 6e6c 6f6e 6700  b.a.s.evSrnlong.
 000027d0: 0000 0100 0000 0500 6c00 6f00 6700 6900  ........l.o.g.i.
-000027e0: 636c 6731 5363 6f6d 7000 0000 0000 0027  clg1Scomp......'
-000027f0: 9600 0000 0500 6c00 6f00 6700 6900 636d  ......l.o.g.i.cm
+000027e0: 636c 6731 5363 6f6d 7000 0000 0000 0029  clg1Scomp......)
+000027f0: b600 0000 0500 6c00 6f00 6700 6900 636d  ......l.o.g.i.cm
 00002800: 6f44 4462                                oDDb
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/customize_api.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/customize_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from safrs import jsonapi_rpc, SAFRSAPI
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.orm import object_mapper
 from database import models
 from logic_bank.rule_bank.rule_bank import RuleBank
 
 # Called by api_logic_server_run.py, to customize api (new end points, services -- see add_order).
-# Separate from expose_api_models.py, to simplify merge if project recreated
+# Separate from expose_api_models.py, to simplify merge if project rebuilt
 
 
 def expose_services(app, api, project_dir, swagger_host: str, PORT: str):
     """ Customize API - new end points for services
 
     This sample illustrates
     * classic hello world,
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/api/multi-table-example/multi-table.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/database/customize_models.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/database/customize_models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/logic/declare_logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """
         Demonstrate that logic == Rules + Python (for extensibility)
     """
     def congratulate_sales_rep(row: models.Order, old_row: models.Order, logic_row: LogicRow):
         """ use events for sending email, messages, etc. """
         if logic_row.ins_upd_dlt == "ins":  # logic engine fills parents for insert
             sales_rep = row.Employee        # parent accessor
-            if sales_rep is None:
+            if sales_rep is None:           # breakpoint here
                 logic_row.log("no salesrep for this order")
             elif sales_rep.Manager is None:
                 logic_row.log("no manager for this order's salesrep")
             else:
                 logic_row.log(f'Hi, {sales_rep.Manager.FirstName} - '
                               f'Congratulate {sales_rep.FirstName} on their new order')
             category_1 = logic_row.session.query(models.Category).filter(models.Category.Id == 1).one()
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/security/declare_security.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/security/declare_security.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/place_order.feature`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/place_order.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/features/steps/salary_change.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/behave.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Item_Qty_to_exceed_.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Alter_Required_Date_-_adj.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Audit_Salary_Change.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Bad_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Good_Order_Custom_Service.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Raise_Must_be_Meaningful.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Reset_Shipped_-_adjust_lo.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Set_Shipped_-_adjust_logi.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/api_logic_server_behave/logs/scenario_logic_logs/Transaction_Processing.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/ADJUST_test_-_OrderDetail.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/AUDIT_test_-_Emp_Sal.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CASCADE_UPDATE_-_ShippedD.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/CUSTOM_SERVICE_Bad_Order.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/DELETE_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PATCH_-_low_credit.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/POST_test_-_Cust.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/results/PRUNE_test_-_ReqdDate.log`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/server_startup_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/test/basic/server_test.sh`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/admin/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/home.js` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/admin/home.js`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/admin/multi_app_project.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/beverages.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/cereals.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/condiments.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/confections.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/diary.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/meat.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/produce.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Category/seafood.gif`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/buchanan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/callahan.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/davolio.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/dodsworth.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/fuller.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/king.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/leverling.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/peacock.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw/ui/images/Employee/suyama.jpg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_prototype_nw_no_cust/readme.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_prototype_nw_no_cust/readme.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/1__Basic_App.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/2__ApiLogicProject.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/3__ApiLogicProject_Logic.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_chinook.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_classicmodels.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Execute_todo.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.idea/runConfigurations/Run_Behave_Logic_Report.xml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/.vscode/launch.json` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/.vscode/launch.json`

 * *Files 16% similar despite different names*

```diff
@@ -74,14 +74,51 @@
             "redirectOutput": true,
             "justMyCode": false,
             "args": ["--flask_host=localhost", "--port=5656", "--swagger_host=localhost", "--verbose=False"],
             "console": "internalConsole",
             "internalConsoleOptions": "openOnSessionStart"
         },
         {
+            "name": "Execute nw",
+            "type": "python",
+            "request": "launch",
+            "cwd": "${workspaceFolder}/nw",
+            "program": "api_logic_server_run.py",
+            "redirectOutput": true,
+            "justMyCode": false,
+            "args": ["--flask_host=localhost", "--port=5656", "--swagger_host=localhost", "--verbose=False"],
+            "console": "internalConsole",
+            "internalConsoleOptions": "openOnSessionStart"
+        },
+        {
+            "name": "Execute nw - No Security",
+            "type": "python",
+            "request": "launch",
+            "cwd": "${workspaceFolder}/nw",
+            "program": "api_logic_server_run.py",
+            "redirectOutput": true,
+            "justMyCode": false,
+            "env": {"SECURITY_ENABLED": "False"},
+            "args": ["--flask_host=localhost", "--port=5656", "--swagger_host=localhost", "--verbose=False"],
+            "console": "internalConsole",
+            "internalConsoleOptions": "openOnSessionStart"
+        },
+        {
+            "name": "Execute nw-",
+            "type": "python",
+            "request": "launch",
+            "cwd": "${workspaceFolder}/chinnw-ook",
+            "program": "api_logic_server_run.py",
+            "redirectOutput": true,
+            "justMyCode": false,
+            "args": ["--flask_host=localhost", "--port=5656", "--swagger_host=localhost", "--verbose=False"],
+            "console": "internalConsole",
+            "internalConsoleOptions": "openOnSessionStart"
+        },
+        {
             "name": "Execute Classic Models",
             "type": "python",
             "request": "launch",
             "cwd": "${workspaceFolder}/classicmodels",
             "program": "api_logic_server_run.py",
             "redirectOutput": true,
             "justMyCode": false,
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/flask_basic.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/raw_flask.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/api/end_points.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/config.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/database/models.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/flask_basic.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/logging.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/0. App_Fiddle/util.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/readme.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 To execute (see *Show me how*, below, for details): **start the server** with **Run and Debug >> *1. Instant Creation***, and then start the Browser at localhost:5656 **(url in the console log)**
 
 <details markdown>
 
 <summary>&nbsp;&nbsp;&nbsp;Show me how </summary>
 
-![](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/tutorial/2-apilogicproject.png?raw=true)
+![](https://github.com/ApiLogicServer/Docs/blob/main/docs/images/tutorial/2-apilogicproject-tutorial.png?raw=true)
 
 &nbsp;
 
 </details>
 
 &nbsp;
 
@@ -429,14 +429,51 @@
 
 &nbsp;
 
 **Project Structure**
 
 This tutorial is actually 3 independent projects.  When you create a project using `ApiLogicServer create --project_name=my_project`, the system will create a free-standing project.  The project will include your container settings, IDE settings etc, so you can just open it your IDE to run and debug.
 
+&nbsp;
+
+**Guided Demo**
+
+Demonstrations of API Logic Server often follow this script, provided as take-away notes.
+
+<details markdown>
+
+<summary> Guided Demo Summary </summary>
+
+&nbsp;
+
+1. Run the automatic **Admin App, and Swagger**<br><br>
+
+2. Explore the Admin App (no html, js): `ui/admin/admin.yaml`<br><br>
+
+3. Explore the API
+    * **Automatic API:** `api/expose_api_models.py`
+      * `database/models.py` - from schema
+    * **Custom Endpoint:** `api/customize_api.py` - see `add_order()`<br><br>
+
+4. Explore `logic/declare_logic.py`
+    * **Executable Design** - declarative
+    * **Breakpoint here**<br><br>
+
+5. Run **Custom APIs and Logic Execution / Debugging**
+    * In swagger: **POST ServicesEndPoint/add_order > Try it out**
+    * At the breakpoint, observe the 
+        * **Debugger State** -- row attributes, etc
+        * **Logic Log** -- line for each rule fire, showing row, with indents for chaining
+
+</details markdown>
+
+&nbsp;
+
+</details markdown>
+
 </details>
 
 &nbsp;
 
 
 <details markdown>
```

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/project_tutorial/sample_db.sqlite` & `ApiLogicServer-8.4.0/api_logic_server_cli/project_tutorial/sample_db.sqlite`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/.DS_Store`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/expose_existing_callable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/sqlacodegen_wrapper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/__pycache__/uri_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/console_log.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/.travis.yml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/README.rst`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/setup.cfg`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/__pycache__/codegen.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/sqlacodegen/main.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py` & `ApiLogicServer-8.4.0/api_logic_server_cli/sqlacodegen_wrapper/sqlacodegen_wrapper.py`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/templates/admin.yaml` & `ApiLogicServer-8.4.0/api_logic_server_cli/templates/admin.yaml`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.md` & `ApiLogicServer-8.4.0/api_logic_server_cli/templates/app_fiddle.md`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/templates/app_fiddle.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/templates/app_fiddle.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/templates/index.html` & `ApiLogicServer-8.4.0/api_logic_server_cli/templates/index.html`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/api_logic_server_cli/templates/login_endpoint.txt` & `ApiLogicServer-8.4.0/api_logic_server_cli/templates/login_endpoint.txt`

 * *Files identical despite different names*

### Comparing `ApiLogicServer-8.3.6/setup.py` & `ApiLogicServer-8.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         "SQLAlchemy-Utils==0.38.2",
         "Werkzeug==2.2.3",
         "logicbankutils==0.6.0",
         "inflect==5.0.2",
         "itsdangerous==2.1.2",
         "Jinja2==3.1.2",
         "MarkupSafe==2.1.1",
-        "safrs>=3.0.2",
+        "safrs>=3.0.4",
         "Flask-Admin==1.5.7",
         "Flask-Cors==3.0.0",
         "Flask==2.2.2",
         "Flask-JWT-Extended==4.4.4",
         "Flask-Login==0.6.2",
         "Flask-OpenID==1.3.0",
         "python-dotenv==0.15.0",
```

