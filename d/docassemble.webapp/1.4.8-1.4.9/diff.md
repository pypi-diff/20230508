# Comparing `tmp/docassemble.webapp-1.4.8.tar.gz` & `tmp/docassemble.webapp-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.webapp-1.4.8.tar", last modified: Thu Aug 25 13:37:32 2022, max compression
+gzip compressed data, was "docassemble.webapp-1.4.9.tar", last modified: Sat Sep 10 18:16:06 2022, max compression
```

## Comparing `docassemble.webapp-1.4.8.tar` & `docassemble.webapp-1.4.9.tar`

### file list

```diff
@@ -1,751 +1,752 @@
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.173663 docassemble.webapp-1.4.8/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:58.000000 docassemble.webapp-1.4.8/MANIFEST.in
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      683 2022-08-25 13:37:32.173663 docassemble.webapp-1.4.8/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2021-12-05 22:33:51.000000 docassemble.webapp-1.4.8/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.101663 docassemble.webapp-1.4.8/docassemble/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      154 2015-04-18 00:46:05.000000 docassemble.webapp-1.4.8/docassemble/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.109663 docassemble.webapp-1.4.8/docassemble/webapp/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       22 2022-08-25 13:37:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.109663 docassemble.webapp-1.4.8/docassemble/webapp/alembic/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       38 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/README
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2181 2021-12-05 22:33:51.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/env.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      548 2018-05-13 01:00:37.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/script.py.mako
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.109663 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      537 2017-12-02 01:46:58.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4573 2019-02-06 01:19:15.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      557 2018-05-13 01:02:46.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      630 2022-04-07 22:05:03.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      510 2017-08-21 11:36:02.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/77e8971ffcbf_first_alembic_revision.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3895 2020-02-26 12:40:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4182 2022-04-07 22:10:51.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      525 2020-02-23 18:38:41.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/c2ef4831ef76_user_last_login.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1226 2018-05-16 02:31:37.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      728 2019-06-27 21:40:29.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1647 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.8/docassemble/webapp/alembic.ini
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1093 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/api_key.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2070 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/app_object.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2558 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/app_socket.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58619 2022-08-06 02:18:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/backend.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      460 2021-12-26 22:02:10.000000 docassemble.webapp-1.4.8/docassemble/webapp/cleanup_sessions.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2820 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/clicksend.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      719 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/cloud.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      958 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/cloud_deregister.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1111 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/cloud_register.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2022-01-05 03:31:15.000000 docassemble.webapp-1.4.8/docassemble/webapp/config_worker.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.109663 docassemble.webapp-1.4.8/docassemble/webapp/core/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      167 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/core/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6408 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/core/models.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15884 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/create_tables.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      386 2021-12-26 15:43:32.000000 docassemble.webapp-1.4.8/docassemble/webapp/createminio.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17429 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/cron.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      603 2022-03-14 02:29:44.000000 docassemble.webapp-1.4.8/docassemble/webapp/daredis.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.109663 docassemble.webapp-1.4.8/docassemble/webapp/data/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        6 2022-08-25 13:37:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/VERSION.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6875 2022-08-25 12:31:02.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/db-schema.txt
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.109663 docassemble.webapp-1.4.8/docassemble/webapp/data/questions/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18794 2021-12-05 22:33:51.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/questions/wizard-template.yml
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.109663 docassemble.webapp-1.4.8/docassemble/webapp/data/static/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.113663 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    10351 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/android-chrome-192x192.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29787 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/android-chrome-512x512.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3030 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/apple-touch-icon.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      246 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/browserconfig.xml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      632 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/favicon-16x16.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1400 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/favicon-32x32.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    15086 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/favicon.ico
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3752 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/mstile-150x150.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3485 2017-04-02 22:18:46.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      426 2022-03-19 15:08:38.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/site.webmanifest
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       26 2017-04-02 20:26:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/robots.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4638 2017-05-16 01:19:25.000000 docassemble.webapp-1.4.8/docassemble/webapp/data/static/test-document.docx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2568 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/database.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2018 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/db_object.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      811 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/deregister.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9400 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/develop.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14881 2022-08-06 15:54:16.000000 docassemble.webapp-1.4.8/docassemble/webapp/file_access.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      335 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/file_number.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36027 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/files.py
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     4882 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/fix_postgresql_tables.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2492 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/fixpickle.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1907 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/google_api.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5027 2022-08-20 00:56:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/info.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3861 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/install_certs.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3465 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/jsonstore.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1829 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/list-cloud.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1921 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/listlog.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      273 2021-12-26 19:04:49.000000 docassemble.webapp-1.4.8/docassemble/webapp/logserver.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    35285 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/machinelearning.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4165 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/mailgun_mail.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.113663 docassemble.webapp-1.4.8/docassemble/webapp/packages/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-04-15 09:56:46.000000 docassemble.webapp-1.4.8/docassemble/webapp/packages/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2008 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/packages/models.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26047 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/playground.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7671 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/process_email.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/register.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2311 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/restart.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      120 2019-09-02 21:06:35.000000 docassemble.webapp-1.4.8/docassemble/webapp/run.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/screenreader.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5039 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/sendgrid_mail.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1524964 2022-08-25 13:07:40.000000 docassemble.webapp-1.4.8/docassemble/webapp/server.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8601 2022-08-25 13:37:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/setup.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    52178 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/socketserver.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       98 2021-12-26 20:50:16.000000 docassemble.webapp-1.4.8/docassemble/webapp/socketstop.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      212 2021-12-26 20:50:31.000000 docassemble.webapp-1.4.8/docassemble/webapp/sockettest.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      309 2021-12-26 22:12:02.000000 docassemble.webapp-1.4.8/docassemble/webapp/sqlalchemy_url.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      139 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/starthook.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.113663 docassemble.webapp-1.4.8/docassemble/webapp/static/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.117663 docassemble.webapp-1.4.8/docassemble/webapp/static/app/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   143258 2018-02-28 23:06:39.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.eot
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   128180 2018-02-28 23:05:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.ttf
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    57620 2018-02-28 23:05:25.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.woff
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    44300 2018-02-28 23:05:32.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.woff2
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22174 2022-08-13 15:47:22.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/additional-methods.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   169245 2022-08-25 03:18:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/adminbundle.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    30376 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18176 2022-05-29 15:01:36.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23094 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12021 2022-05-29 15:03:35.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.min.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      482 2018-06-05 11:33:56.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/auth0-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1229 2017-03-18 01:24:28.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/azure-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      147 2018-09-13 21:10:37.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/blank.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    44242 2022-08-25 03:18:08.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundle.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   557372 2022-08-25 03:18:10.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundle.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   467870 2022-08-25 03:18:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundlenojquery.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   469252 2022-08-25 03:18:10.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundlewrapjquery.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1150 2017-04-02 21:01:48.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/chat.ico
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1257 2015-04-04 15:28:40.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/facebook-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1387 2015-10-05 03:38:54.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/google-logo.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    89501 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24601 2022-08-13 15:45:36.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.validate.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3407 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.visible.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2050 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.visible.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1685 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/js.cookie.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1264 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/keycloak-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      351 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/option-vertical.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2685 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/option-vertical.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      430 2017-06-15 10:37:03.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/phone-logo.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21548 2022-08-25 03:18:09.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/playgroundbundle.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   705804 2022-08-25 03:18:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/playgroundbundle.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3584 2017-04-02 15:19:56.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/pygments.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1527 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/pygments.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    64273 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/socket.io.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   160264 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/socket.io.min.js.map
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2015-04-04 16:31:24.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/twitter-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2717 2018-09-18 02:49:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/upload.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2109 2016-09-25 16:03:42.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/webrtc.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2365 2016-10-18 04:15:55.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/webrtc.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3020 2020-01-09 14:49:13.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/app/wrap.svg
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.117663 docassemble.webapp-1.4.8/docassemble/webapp/static/areyousure/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5559 2019-07-18 00:51:35.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/areyousure/jquery.are-you-sure.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.097663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   193529 2022-05-28 11:30:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   521648 2022-05-28 11:30:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    79742 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   328436 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60055 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   214177 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.097663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.117663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      775 2022-06-18 20:07:15.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      672 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.117663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/js/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    17033 2022-08-25 00:03:57.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10339 2022-08-25 03:17:09.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.117663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1555 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    11990 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.117663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2042 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1728 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    12262 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     9020 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.121663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/img/
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     2670 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      847 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.121663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   251889 2022-07-07 01:41:01.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   162834 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5592 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6812 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6175 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6582 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5996 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5884 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6129 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5836 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6071 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8175 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6111 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5483 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7063 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5227 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6253 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6087 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6093 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6241 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5819 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6024 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7319 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8967 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6230 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6110 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5887 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5916 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5526 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5835 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6137 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6118 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5971 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7694 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6126 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5574 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5801 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5676 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7300 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6129 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7360 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6413 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6012 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5562 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5587 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    75990 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29919 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   120577 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    42997 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.097663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fa/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2177 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1773 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fas/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2065 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1818 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.097663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    84330 2022-05-28 12:14:36.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51588 2022-05-28 12:14:47.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/css/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    11286 2022-05-28 12:22:31.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9935 2022-05-28 12:25:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.101663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.101663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/dialog/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      507 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/dialog/dialog.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5250 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/dialog/dialog.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.125663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1544 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/autorefresh.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      116 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/fullscreen.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1495 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/fullscreen.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4659 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/panel.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2829 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/placeholder.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1916 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/rulers.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7121 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8542 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/closetag.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3987 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/continuelist.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6816 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2356 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/matchtags.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1004 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1681 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2578 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/css-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11456 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/html-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6853 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      623 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/show-hint.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19979 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/show-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9604 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5703 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4628 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1582 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1347 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5463 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2141 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6214 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      188 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3856 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11712 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/search.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12232 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/searchcursor.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/keymap/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16334 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/keymap/emacs.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26692 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/keymap/sublime.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   224465 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/keymap/vim.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/lib/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8720 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/lib/codemirror.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   400195 2022-02-21 08:06:39.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/lib/codemirror.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.101663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    40846 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/css.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2837 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/gss.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      461 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/gss_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2219 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4072 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/less.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1908 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/less_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2808 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/scss.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3180 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/scss_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7521 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/htmlmixed/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5686 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3427 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.129663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4665 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38890 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/javascript.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2135 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20326 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1607 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/typescript.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.133663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28731 2022-03-06 21:30:57.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12779 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31323 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/markdown.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38878 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.133663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/python/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6267 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/python/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14924 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/python/python.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2848 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/python/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.133663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/xml/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2163 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/xml/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1759 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/xml/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13351 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/xml/xml.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.133663 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/yaml/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2106 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/yaml/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3733 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/yaml/yaml.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.153663 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17615 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/actions-parameters.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12998 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/actions.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11717 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/age_in_years.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56854 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/alignment.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21418 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/all-true.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    50677 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/allow-emailing-false.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4389 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/as-datetime.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   135261 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/attachment-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13634 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/audio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19808 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/auto-terms.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_flash.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_javascript.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_refresh.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_with_response_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_response_action_flash.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10740 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21691 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons-icons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12060 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons-labels.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13126 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6047 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/capitalize.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4394 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/chat-partners-available.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12402 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/check-in.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    11099 2022-03-26 01:52:28.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-combobox.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12690 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-dropdown.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21433 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-icons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18570 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-with-default.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18714 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7383 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/comment.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10803 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/continue-button-label.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12974 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/continue.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11638 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/country.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26548 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/cron.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    43642 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/css.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5623 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/currency.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5285 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/current-datetime.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16116 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dadict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3851 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dafile.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11418 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/database_storage.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11803 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-difference.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12966 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4232 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-interval.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9474 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-parts.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5541 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dead-end.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13778 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/decoration.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9069 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/def.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11281 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/defined.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/del.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4006 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/device.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10517 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dialog-box.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    56019 2022-01-15 19:48:01.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-docx.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58370 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-file.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60880 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-language.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67827 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-variable-name.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56752 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34388 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/docx-template-table.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34388 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/docx-template.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14361 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/doors.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10627 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/email-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/email-to-case-simple.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/email-to-case.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18351 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/emoji-inline.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11709 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exists.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7103 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit-buttons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9702 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit-choices.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12116 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit-url.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9401 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8708 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/external_files.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25174 2022-01-15 19:48:01.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-checkboxes.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    12060 2022-03-26 01:52:28.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-choices-combobox.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11548 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-choices.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15535 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-mc-exclude.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15535 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-mc.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23017 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-noyesmaybe.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24617 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesno.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22588 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesnomaybe.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24388 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesnoradio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19913 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesnowide.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20509 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fix-punctuation.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4717 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/for_fruit.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/force-ask.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7776 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/force-gather.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32606 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/formatting.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8533 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-dict-object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17024 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-dict-value.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13811 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-dict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7789 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit-at-least-two.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11776 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit-gather.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10334 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit-number.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14113 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14906 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-set-object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10364 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-set.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8716 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/generic-object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4433 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/get-default-timezone.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16575 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/help-damages-audio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24021 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/help.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20465 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/hideif-boolean.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29068 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/html.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15386 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/image-sets.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14948 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/images.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8182 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/imports.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/include.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15384 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/indefinite-article.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14115 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/initial.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3633 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interface.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17183 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interview-help.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21760 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interview-url.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21938 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interview_url_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2159 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/js_action_call.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11157 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/js_url_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2337 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/js_variables.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15459 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/label.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14517 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/language.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8437 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/language_from_browser.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4335 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/language_from_browser_restricted.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3704 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/lists.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25876 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/loading-legal.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23906 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/loading-util.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7724 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/madlibs.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3546 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-01.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3118 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-02.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-03.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-04.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3292 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-05.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9163 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-06.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2462 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-07.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6832 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-09.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mandatory.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67776 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/markdown.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10310 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/menu-item.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10655 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/message.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15962 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/metadata.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16028 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/min.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11344 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/minlength.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9444 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-classify.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9181 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-datatype.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18348 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-export-yaml.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      354 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-export.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-predict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-save-and-predict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9658 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mlarea-datatype.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11104 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/modules.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11064 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/money-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9787 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/need.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13309 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/nested-loop.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12230 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/nice-number.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10407 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/no-label-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    27436 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/note.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12595 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/noun-plural.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/noyes.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14737 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/number-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15620 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-checkboxes.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14699 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-disable-others.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12845 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-radio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10235 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-selections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10453 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17062 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/objects.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22843 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ocr-chord.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    20326 2022-03-16 21:01:39.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ocr.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23012 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/optional-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8274 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ordinal-number.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12679 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/other.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58333 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/page-numbers.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16253 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/password-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9496 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/past-tense.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51015 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-a.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19862 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-fill-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12171 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-fill-signature.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24929 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-fill.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12918 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/periodic-amount.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11325 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/periodic-value.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18236 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/prevent-back.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18236 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/prevent-going-back.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9509 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/progress-features.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9795 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/progress.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18786 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pull-down-with-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15669 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pull-down.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20531 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/qr-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/quantity-noun.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13533 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/quote_paragraphs.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26949 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/radio-list.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21419 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/range.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/reconsider.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22042 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/redis.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8298 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/refresh.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10247 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/reload.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7496 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/required-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/reset.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10248 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/response-json.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7484 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/response-svg.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      825 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/response.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22273 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/resume-button-label.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    45696 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/review.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23005 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/salutation.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24041 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/save-url-to-file.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9746 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/script.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20969 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29156 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-get-sections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22084 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-review.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21920 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-set-sections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22565 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29498 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9226 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/send-email.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14517 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/set-language.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15637 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/showif-boolean.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16875 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/showif.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34661 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/shuffle.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31270 2022-05-29 15:13:33.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/signature.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5202 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/signin.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58915 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/single-spacing.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5901 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/space-underscore.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10375 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/state.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18965 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/static_image.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10109 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/subdivision-type.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7275 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/table-mako.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6771 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/table-markdown.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7143 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/table.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    12382 2022-03-16 21:01:39.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/target-template.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31740 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/template-file.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    35991 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/template-subject.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31740 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/template.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19527 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/terms.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10990 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-box-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20969 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-default.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18283 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-field.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    25422 2022-01-15 19:48:04.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-help.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23948 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-hint.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13398 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/timezone-list.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5432 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/title-case.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4107 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/today.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26745 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/under.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25496 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/upload-multiple.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24708 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/upload.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17380 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/url-of.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41705 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/valid-formats.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11304 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/value.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/variables_as_json.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   245391 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/video.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8585 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/yesno-custom.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/yesno.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11557 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/examples/yesnomaybe.png
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.101663 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.161663 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1821541 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/all.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1731502 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/all.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   469693 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/brands.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   460931 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/brands.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36844 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/conflict-detection.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15225 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   111921 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/fontawesome.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    54607 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/fontawesome.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   151400 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/regular.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   146079 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/regular.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1089184 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/solid.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1070545 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/solid.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    30832 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/v4-shims.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26281 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/v4-shims.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.161663 docassemble.webapp-1.4.8/docassemble/webapp/static/img/
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     2670 2019-07-16 21:18:49.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/img/loading-sm.gif
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      847 2019-07-16 21:18:49.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/img/loading.gif
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3431 2021-02-15 17:42:19.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.101663 docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.161663 docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2101 2019-01-15 13:27:33.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12680 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1516 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6499 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.161663 docassemble.webapp-1.4.8/docassemble/webapp/static/office/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1464 2018-09-14 00:24:57.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/office/cat-in-circle-32.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2799 2018-09-14 00:24:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/office/cat-in-circle-80.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      100 2018-09-15 12:39:38.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/office/office.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4280 2019-09-28 01:21:47.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/office/officeinner.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   248871 2018-09-15 03:21:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/office/polyfill.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20178 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/office/word.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.161663 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1753 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/README.md
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13080 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-off.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8341 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-off.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13392 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-on.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8322 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-on.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7572 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8049 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    16801 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-snap.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9961 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-snap.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13231 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-stapler.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9920 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-stapler.ogg
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.161663 docassemble.webapp-1.4.8/docassemble/webapp/static/yamlmixed/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6478 2020-02-22 15:17:40.000000 docassemble.webapp-1.4.8/docassemble/webapp/static/yamlmixed/yamlmixed.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1410 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/telnyx.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.161663 docassemble.webapp-1.4.8/docassemble/webapp/templates/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:13.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.165663 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:25.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13895 2022-08-24 00:53:05.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-12-23 00:30:43.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/blank.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      406 2018-06-28 11:35:30.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/flask_extra_wide_base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      602 2020-01-03 14:53:32.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/flask_two_col_base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      490 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/flask_user_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      406 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/flask_wide_base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      487 2017-06-07 12:01:03.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/flask_wide_twocol_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5727 2021-12-16 14:09:24.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/form_macros.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       41 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/page_base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      213 2018-06-07 11:37:36.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/page_base_half.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      283 2018-06-07 11:37:54.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/page_base_half_pgfiles.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/page_base_half_wider.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.165663 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:30.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1814 2021-12-16 14:09:30.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/_macros.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1505 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/change_password.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.169663 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       63 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/base_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       54 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/base_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       50 2015-03-30 03:22:41.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/base_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      468 2018-05-16 10:28:37.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/confirm_email_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      369 2018-05-16 10:29:16.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/confirm_email_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      118 2018-05-16 10:29:27.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/confirm_email_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      442 2018-05-16 10:30:11.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/forgot_password_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      350 2018-05-16 10:30:33.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/forgot_password_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      114 2018-05-16 10:30:45.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/forgot_password_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      260 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/invite_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      249 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/invite_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-05-16 10:31:29.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/invite_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      371 2018-05-16 10:33:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/password_changed_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      347 2018-05-16 10:33:28.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/password_changed_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:33:41.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/password_changed_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      568 2018-05-16 10:34:39.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/registered_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      464 2018-05-16 10:35:16.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/registered_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      220 2018-05-16 10:35:57.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/registered_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      511 2019-12-04 12:31:59.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/reregistered_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      424 2019-12-04 12:32:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/reregistered_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      120 2019-12-04 13:14:45.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/reregistered_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      362 2018-05-16 10:37:44.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/username_changed_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      312 2018-05-16 10:38:00.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/username_changed_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:38:13.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/username_changed_subject.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1077 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/forgot_password.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1387 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/google_login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2021-12-16 14:11:26.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/invite.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10016 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1898 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/login_or_register.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1285 2020-07-28 01:34:57.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/manage_emails.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/member_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      742 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_choose.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_reconfigure.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      538 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_setup.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      440 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_sms_setup.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_verify_sms_setup.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      414 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/phone_login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      503 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/phone_login_verify.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/public_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8993 2022-08-24 01:43:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/register.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      432 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/resend_confirm_email.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1203 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/reset_password.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      961 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/user_profile.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.173663 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      760 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/404.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      772 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/501.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      877 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/admin_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1670 2022-03-06 21:20:12.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/config.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      371 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/create_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1023 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/create_playground_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      642 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/gd_sync_wait.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1284 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/github.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      404 2020-07-28 01:29:18.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/google_sync.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      966 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/googledrive.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      163 2016-11-26 18:11:31.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/health_check.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1050 2020-07-28 01:28:13.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/home_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4605 2022-05-16 12:54:38.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/interviews.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3130 2022-02-23 03:19:47.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/logs.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      667 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_account.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3299 2022-02-19 19:30:54.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_api.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2217 2022-06-11 12:37:06.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_playgrounds.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4957 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_projects.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      882 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/member_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1737 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/monitor.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      640 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/od_sync_wait.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2019-09-28 01:16:26.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officeaddin.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      545 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officefunctionfile.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5637 2019-05-21 21:50:45.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officemanifest.xml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4932 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officeouter.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      967 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/onedrive.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      726 2018-02-25 11:28:04.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/packages.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9997 2022-06-11 13:13:03.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/playground.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      198 2018-11-23 20:30:43.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/playground_poll.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9591 2022-06-11 13:12:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/playgroundfiles.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11491 2021-12-17 02:07:03.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/playgroundpackages.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      900 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/pull_playground_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1428 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/rename_project.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      294 2017-10-05 03:05:06.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/restart.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      457 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/socketserver.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      416 2017-11-04 17:12:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/start-embedded.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1106 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/start.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      579 2020-04-12 15:32:42.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/test_embed.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      244 2017-05-30 00:47:01.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/testgoogledrive.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      354 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/testpost.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14703 2022-03-15 17:45:23.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/train.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2558 2022-05-11 13:43:23.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/update_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/update_package_wait.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3122 2022-03-19 16:00:09.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/utilities.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      125 2017-01-19 12:40:42.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/view_source.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      939 2019-05-21 21:49:14.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/webrtc.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.173663 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:37.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      669 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/add_user_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2661 2022-03-05 15:41:47.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/edit_user_profile_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      474 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/new_role_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      703 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/request_developer.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      593 2022-02-21 16:31:46.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/rolelist.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5644 2022-08-24 16:46:18.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/user_profile_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4071 2022-08-09 20:39:49.000000 docassemble.webapp-1.4.8/docassemble/webapp/templates/users/userlist.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      182 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/testrun.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      946 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/translations.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41528 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/update.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      486 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/update_config.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2592 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/user_database.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.173663 docassemble.webapp-1.4.8/docassemble/webapp/users/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.8/docassemble/webapp/users/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17310 2022-08-23 11:40:07.000000 docassemble.webapp-1.4.8/docassemble/webapp/users/forms.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8037 2022-08-17 03:06:02.000000 docassemble.webapp-1.4.8/docassemble/webapp/users/models.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23856 2022-08-24 02:14:51.000000 docassemble.webapp-1.4.8/docassemble/webapp/users/views.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      975 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/watchdog.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    90584 2022-08-05 21:23:53.000000 docassemble.webapp-1.4.8/docassemble/webapp/worker.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      581 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.8/docassemble/webapp/wsgi_restart.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:32.101663 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      683 2022-08-25 13:37:31.000000 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36448 2022-08-25 13:37:31.000000 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/SOURCES.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-08-25 13:37:31.000000 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/dependency_links.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-08-25 13:37:31.000000 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/namespace_packages.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-08-25 13:37:31.000000 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/not-zip-safe
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4658 2022-08-25 13:37:31.000000 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/requires.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-08-25 13:37:31.000000 docassemble.webapp-1.4.8/docassemble.webapp.egg-info/top_level.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       79 2022-08-25 13:37:32.173663 docassemble.webapp-1.4.8/setup.cfg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10471 2022-08-25 13:37:07.000000 docassemble.webapp-1.4.8/setup.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.946496 docassemble.webapp-1.4.9/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:58.000000 docassemble.webapp-1.4.9/MANIFEST.in
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      683 2022-09-10 18:16:06.946496 docassemble.webapp-1.4.9/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2021-12-05 22:33:51.000000 docassemble.webapp-1.4.9/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      154 2015-04-18 00:46:05.000000 docassemble.webapp-1.4.9/docassemble/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.882496 docassemble.webapp-1.4.9/docassemble/webapp/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       22 2022-09-10 18:15:31.000000 docassemble.webapp-1.4.9/docassemble/webapp/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.882496 docassemble.webapp-1.4.9/docassemble/webapp/alembic/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       38 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/README
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2181 2021-12-05 22:33:51.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/env.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      548 2018-05-13 01:00:37.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/script.py.mako
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.882496 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      538 2022-08-30 13:14:42.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4550 2022-08-30 13:16:09.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      557 2018-05-13 01:02:46.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      606 2022-08-30 13:16:25.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      511 2022-08-30 13:16:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/77e8971ffcbf_first_alembic_revision.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3897 2022-08-30 13:17:16.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4158 2022-08-30 13:17:36.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      527 2022-08-30 13:15:29.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/c2ef4831ef76_user_last_login.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1226 2018-05-16 02:31:37.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      729 2022-08-30 13:15:42.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      548 2022-08-30 13:13:41.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/fd1547c94c46_add_a_column_for_the_voicerss_voice.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1647 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.9/docassemble/webapp/alembic.ini
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1093 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/api_key.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2070 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/app_object.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2558 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/app_socket.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58754 2022-09-06 15:34:07.000000 docassemble.webapp-1.4.9/docassemble/webapp/backend.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      460 2021-12-26 22:02:10.000000 docassemble.webapp-1.4.9/docassemble/webapp/cleanup_sessions.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2820 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/clicksend.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      719 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/cloud.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      958 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/cloud_deregister.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1111 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/cloud_register.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2022-01-05 03:31:15.000000 docassemble.webapp-1.4.9/docassemble/webapp/config_worker.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.882496 docassemble.webapp-1.4.9/docassemble/webapp/core/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      167 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/core/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6445 2022-08-30 13:13:31.000000 docassemble.webapp-1.4.9/docassemble/webapp/core/models.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15884 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/create_tables.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      386 2021-12-26 15:43:32.000000 docassemble.webapp-1.4.9/docassemble/webapp/createminio.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17429 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/cron.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      603 2022-03-14 02:29:44.000000 docassemble.webapp-1.4.9/docassemble/webapp/daredis.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.882496 docassemble.webapp-1.4.9/docassemble/webapp/data/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        6 2022-09-10 18:15:31.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/VERSION.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6913 2022-09-10 18:05:46.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/db-schema.txt
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.882496 docassemble.webapp-1.4.9/docassemble/webapp/data/questions/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18794 2021-12-05 22:33:51.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/questions/wizard-template.yml
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.882496 docassemble.webapp-1.4.9/docassemble/webapp/data/static/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.886496 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    10351 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/android-chrome-192x192.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29787 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/android-chrome-512x512.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3030 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/apple-touch-icon.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      246 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/browserconfig.xml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      632 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/favicon-16x16.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1400 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/favicon-32x32.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    15086 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/favicon.ico
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3752 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/mstile-150x150.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3485 2017-04-02 22:18:46.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      426 2022-03-19 15:08:38.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/site.webmanifest
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       26 2017-04-02 20:26:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/robots.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4638 2017-05-16 01:19:25.000000 docassemble.webapp-1.4.9/docassemble/webapp/data/static/test-document.docx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2568 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/database.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2018 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/db_object.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      811 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/deregister.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9400 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/develop.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14881 2022-08-06 15:54:16.000000 docassemble.webapp-1.4.9/docassemble/webapp/file_access.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      335 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/file_number.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36027 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/files.py
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     4882 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/fix_postgresql_tables.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2492 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/fixpickle.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1907 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/google_api.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5027 2022-08-20 00:56:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/info.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3861 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/install_certs.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3465 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/jsonstore.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1829 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/list-cloud.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1921 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/listlog.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      273 2021-12-26 19:04:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/logserver.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    35285 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/machinelearning.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4165 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/mailgun_mail.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.886496 docassemble.webapp-1.4.9/docassemble/webapp/packages/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-04-15 09:56:46.000000 docassemble.webapp-1.4.9/docassemble/webapp/packages/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2008 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/packages/models.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26047 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/playground.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7671 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/process_email.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/register.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2311 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/restart.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      120 2019-09-02 21:06:35.000000 docassemble.webapp-1.4.9/docassemble/webapp/run.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/screenreader.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5039 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/sendgrid_mail.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1528361 2022-09-08 01:39:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/server.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8601 2022-09-10 18:15:31.000000 docassemble.webapp-1.4.9/docassemble/webapp/setup.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    52178 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/socketserver.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       98 2021-12-26 20:50:16.000000 docassemble.webapp-1.4.9/docassemble/webapp/socketstop.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      212 2021-12-26 20:50:31.000000 docassemble.webapp-1.4.9/docassemble/webapp/sockettest.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      309 2021-12-26 22:12:02.000000 docassemble.webapp-1.4.9/docassemble/webapp/sqlalchemy_url.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      139 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/starthook.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.886496 docassemble.webapp-1.4.9/docassemble/webapp/static/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/app/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   143258 2018-02-28 23:06:39.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.eot
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   128180 2018-02-28 23:05:07.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.ttf
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    57620 2018-02-28 23:05:25.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.woff
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    44300 2018-02-28 23:05:32.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.woff2
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22174 2022-08-13 15:47:22.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/additional-methods.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   169245 2022-08-25 03:18:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/adminbundle.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    30376 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18176 2022-05-29 15:01:36.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23094 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12021 2022-05-29 15:03:35.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.min.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      482 2018-06-05 11:33:56.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/auth0-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1229 2017-03-18 01:24:28.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/azure-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      147 2018-09-13 21:10:37.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/blank.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    44242 2022-08-25 03:18:08.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundle.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   557372 2022-08-25 03:18:10.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundle.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   467870 2022-08-25 03:18:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundlenojquery.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   469252 2022-08-25 03:18:10.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundlewrapjquery.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1150 2017-04-02 21:01:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/chat.ico
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1257 2015-04-04 15:28:40.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/facebook-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1387 2015-10-05 03:38:54.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/google-logo.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    89501 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24601 2022-08-13 15:45:36.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.validate.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3407 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.visible.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2050 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.visible.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1685 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/js.cookie.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1264 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/keycloak-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      351 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/option-vertical.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2685 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/option-vertical.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      430 2017-06-15 10:37:03.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/phone-logo.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21548 2022-08-25 03:18:09.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/playgroundbundle.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   705804 2022-08-25 03:18:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/playgroundbundle.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3584 2017-04-02 15:19:56.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/pygments.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1527 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/pygments.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    64273 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/socket.io.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   160264 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/socket.io.min.js.map
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2015-04-04 16:31:24.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/twitter-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2717 2018-09-18 02:49:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/upload.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2109 2016-09-25 16:03:42.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/webrtc.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2365 2016-10-18 04:15:55.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/webrtc.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3020 2020-01-09 14:49:13.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/app/wrap.svg
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/areyousure/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5559 2019-07-18 00:51:35.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/areyousure/jquery.are-you-sure.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   193529 2022-05-28 11:30:07.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   521648 2022-05-28 11:30:07.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    79742 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   328436 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60055 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   214177 2022-05-28 11:30:45.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      775 2022-06-18 20:07:15.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      672 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/js/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    17033 2022-08-25 00:03:57.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10339 2022-08-25 03:17:09.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1555 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    11990 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2042 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1728 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    12262 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     9020 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/img/
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     2670 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      847 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.890496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   251889 2022-07-07 01:41:01.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   162834 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.894496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5592 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6812 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6175 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6582 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5996 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5884 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6129 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5836 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6071 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8175 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6111 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5483 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7063 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5227 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6253 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6087 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6093 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6241 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5819 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6024 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7319 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8967 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6230 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6110 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5887 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5916 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5526 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5835 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6137 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6118 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5971 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7694 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6126 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5574 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5801 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5676 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7300 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6129 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7360 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6413 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6012 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5562 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5587 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    75990 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29919 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   120577 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    42997 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fa/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2177 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1773 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fas/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2065 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1818 2022-06-18 21:05:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    84330 2022-05-28 12:14:36.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51588 2022-05-28 12:14:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/css/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    11286 2022-05-28 12:22:31.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9935 2022-05-28 12:25:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/dialog/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      507 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/dialog/dialog.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5250 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/dialog/dialog.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1544 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/autorefresh.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      116 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/fullscreen.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1495 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/fullscreen.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4659 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/panel.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2829 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/placeholder.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1916 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/rulers.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.898496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7121 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8542 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/closetag.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3987 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/continuelist.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6816 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2356 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/matchtags.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1004 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1681 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2578 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/css-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11456 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/html-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6853 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      623 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/show-hint.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19979 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/show-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9604 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5703 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4628 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1582 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1347 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5463 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2141 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6214 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      188 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3856 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11712 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/search.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12232 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/searchcursor.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/keymap/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16334 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/keymap/emacs.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26692 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/keymap/sublime.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   224465 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/keymap/vim.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/lib/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8720 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/lib/codemirror.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   400195 2022-02-21 08:06:39.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/lib/codemirror.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    40846 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/css.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2837 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/gss.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      461 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/gss_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2219 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4072 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/less.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1908 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/less_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2808 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/scss.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3180 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/scss_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7521 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/htmlmixed/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5686 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3427 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4665 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38890 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/javascript.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2135 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20326 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1607 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/typescript.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.902496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28731 2022-03-06 21:30:57.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12779 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31323 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/markdown.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38878 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.906496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/python/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6267 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/python/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14924 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/python/python.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2848 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/python/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.906496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/xml/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2163 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/xml/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1759 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/xml/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13351 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/xml/xml.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.906496 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/yaml/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2106 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/yaml/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3733 2022-02-21 08:06:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/yaml/yaml.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.926496 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17615 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/actions-parameters.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12998 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/actions.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11717 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/age_in_years.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56854 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/alignment.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21418 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/all-true.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    50677 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/allow-emailing-false.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4389 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/as-datetime.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   135261 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/attachment-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13634 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/audio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19808 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/auto-terms.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_flash.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_javascript.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_refresh.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_with_response_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_response_action_flash.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10740 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21691 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons-icons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12060 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons-labels.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13126 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6047 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/capitalize.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4394 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/chat-partners-available.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12402 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/check-in.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11099 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-combobox.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12690 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-dropdown.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21433 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-icons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18570 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-with-default.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18714 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7383 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/comment.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10803 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/continue-button-label.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12974 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/continue.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11638 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/country.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26548 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/cron.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    43642 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/css.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5623 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/currency.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5285 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/current-datetime.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16116 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dadict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3851 2022-09-09 11:27:40.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dafile.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11418 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/database_storage.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11803 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-difference.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12966 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4232 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-interval.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9474 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-parts.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5541 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dead-end.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13778 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/decoration.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9069 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/def.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11281 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/defined.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/del.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4006 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/device.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10517 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dialog-box.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56019 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-docx.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58370 2022-07-08 19:20:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-file.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60880 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-language.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67827 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-variable-name.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56752 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34388 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/docx-template-table.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34388 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/docx-template.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14361 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/doors.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10627 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/email-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/email-to-case-simple.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/email-to-case.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18351 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/emoji-inline.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11709 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exists.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7103 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit-buttons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9702 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit-choices.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12116 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit-url.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9401 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8708 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/external_files.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25174 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-checkboxes.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12060 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-choices-combobox.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11548 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-choices.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15535 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-mc-exclude.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15535 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-mc.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23017 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-noyesmaybe.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24617 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesno.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22588 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesnomaybe.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24388 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesnoradio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19913 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesnowide.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20509 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fix-punctuation.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4717 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/for_fruit.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/force-ask.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7776 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/force-gather.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32606 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/formatting.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8533 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-dict-object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17024 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-dict-value.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13811 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-dict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7789 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit-at-least-two.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11776 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit-gather.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10334 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit-number.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14113 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14906 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-set-object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10364 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-set.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8716 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/generic-object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4433 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/get-default-timezone.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16575 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/help-damages-audio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24021 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/help.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20465 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/hideif-boolean.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29068 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/html.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15386 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/image-sets.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14948 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/images.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8182 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/imports.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/include.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15384 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/indefinite-article.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14115 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/initial.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3633 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interface.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17183 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interview-help.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21760 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interview-url.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21938 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interview_url_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2159 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/js_action_call.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11157 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/js_url_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2337 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/js_variables.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15459 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/label.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14517 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/language.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8437 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/language_from_browser.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4335 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/language_from_browser_restricted.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3704 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/lists.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25876 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/loading-legal.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23906 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/loading-util.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7724 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/madlibs.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3546 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-01.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3118 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-02.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-03.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-04.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3292 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-05.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9163 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-06.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2462 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-07.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6832 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-09.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mandatory.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67776 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/markdown.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10310 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/menu-item.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10655 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/message.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15962 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/metadata.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16028 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/min.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11344 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/minlength.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9444 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-classify.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9181 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-datatype.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18348 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-export-yaml.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      354 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-export.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-predict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-save-and-predict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9658 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mlarea-datatype.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11104 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/modules.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11064 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/money-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9787 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/need.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13309 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/nested-loop.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12230 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/nice-number.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10407 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/no-label-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    27436 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/note.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12595 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/noun-plural.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/noyes.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14737 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/number-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15620 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-checkboxes.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14699 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-disable-others.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12845 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-radio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10235 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-selections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10453 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17062 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/objects.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22843 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ocr-chord.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20326 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ocr.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23012 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/optional-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8274 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ordinal-number.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12679 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/other.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58333 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/page-numbers.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16253 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/password-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9496 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/past-tense.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51015 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-a.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19862 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-fill-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12171 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-fill-signature.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24929 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-fill.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12918 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/periodic-amount.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11325 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/periodic-value.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18236 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/prevent-back.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18236 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/prevent-going-back.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9509 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/progress-features.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9795 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/progress.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18786 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pull-down-with-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15669 2022-07-08 19:20:48.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pull-down.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20531 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/qr-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/quantity-noun.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13533 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/quote_paragraphs.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26949 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/radio-list.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21419 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/range.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/reconsider.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22042 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/redis.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8298 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/refresh.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10247 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/reload.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7496 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/required-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/reset.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10248 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/response-json.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7484 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/response-svg.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      825 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/response.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22273 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/resume-button-label.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    45696 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/review.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23005 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/salutation.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24041 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/save-url-to-file.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9746 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/script.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20969 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29156 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-get-sections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22084 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-review.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21920 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-set-sections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22565 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29498 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9226 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/send-email.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14517 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/set-language.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15637 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/showif-boolean.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16875 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/showif.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34661 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/shuffle.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31270 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/signature.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5202 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/signin.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58915 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/single-spacing.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5901 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/space-underscore.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10375 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/state.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18965 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/static_image.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10109 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/subdivision-type.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7275 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/table-mako.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6771 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/table-markdown.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7143 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/table.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12382 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/target-template.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31740 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/template-file.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    35991 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/template-subject.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31740 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/template.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19527 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/terms.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10990 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-box-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20969 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-default.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18283 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25422 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-help.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23948 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-hint.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13398 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/timezone-list.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5432 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/title-case.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4107 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/today.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26745 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/under.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25496 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/upload-multiple.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24708 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/upload.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17380 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/url-of.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41705 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/valid-formats.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11304 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/value.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/variables_as_json.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   245391 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/video.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8585 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/yesno-custom.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/yesno.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11557 2022-07-08 19:20:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/examples/yesnomaybe.png
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.934496 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1821541 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/all.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1731502 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/all.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   469693 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/brands.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   460931 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/brands.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36844 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/conflict-detection.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15225 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   111921 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/fontawesome.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    54607 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/fontawesome.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   151400 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/regular.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   146079 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/regular.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1089184 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/solid.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1070545 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/solid.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    30832 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/v4-shims.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26281 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/v4-shims.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.934496 docassemble.webapp-1.4.9/docassemble/webapp/static/img/
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     2670 2019-07-16 21:18:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/img/loading-sm.gif
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      847 2019-07-16 21:18:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/img/loading.gif
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3431 2021-02-15 17:42:19.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.934496 docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2101 2019-01-15 13:27:33.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12680 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1516 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6499 2022-07-28 22:47:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.934496 docassemble.webapp-1.4.9/docassemble/webapp/static/office/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1464 2018-09-14 00:24:57.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/office/cat-in-circle-32.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2799 2018-09-14 00:24:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/office/cat-in-circle-80.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      100 2018-09-15 12:39:38.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/office/office.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4280 2019-09-28 01:21:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/office/officeinner.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   248871 2018-09-15 03:21:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/office/polyfill.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20178 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/office/word.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.934496 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1753 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/README.md
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13080 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-off.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8341 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-off.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13392 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-on.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8322 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-on.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7572 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8049 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    16801 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-snap.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9961 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-snap.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13231 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-stapler.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9920 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-stapler.ogg
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.934496 docassemble.webapp-1.4.9/docassemble/webapp/static/yamlmixed/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6478 2020-02-22 15:17:40.000000 docassemble.webapp-1.4.9/docassemble/webapp/static/yamlmixed/yamlmixed.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1410 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/telnyx.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.934496 docassemble.webapp-1.4.9/docassemble/webapp/templates/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:13.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.938496 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:25.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13895 2022-08-30 14:45:21.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-12-23 00:30:43.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/blank.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      406 2018-06-28 11:35:30.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/flask_extra_wide_base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      602 2020-01-03 14:53:32.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/flask_two_col_base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      490 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/flask_user_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      406 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/flask_wide_base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      487 2017-06-07 12:01:03.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/flask_wide_twocol_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5727 2021-12-16 14:09:24.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/form_macros.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       41 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/page_base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      213 2018-06-07 11:37:36.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/page_base_half.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      283 2018-06-07 11:37:54.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/page_base_half_pgfiles.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/page_base_half_wider.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.938496 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:30.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1814 2021-12-16 14:09:30.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/_macros.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1505 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/change_password.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.942496 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       63 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/base_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       54 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/base_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       50 2015-03-30 03:22:41.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/base_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      468 2018-05-16 10:28:37.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/confirm_email_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      369 2018-05-16 10:29:16.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/confirm_email_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      118 2018-05-16 10:29:27.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/confirm_email_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      442 2018-05-16 10:30:11.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/forgot_password_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      350 2018-05-16 10:30:33.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/forgot_password_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      114 2018-05-16 10:30:45.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/forgot_password_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      260 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/invite_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      249 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/invite_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-05-16 10:31:29.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/invite_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      371 2018-05-16 10:33:07.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/password_changed_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      347 2018-05-16 10:33:28.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/password_changed_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:33:41.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/password_changed_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      568 2018-05-16 10:34:39.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/registered_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      464 2018-05-16 10:35:16.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/registered_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      220 2018-05-16 10:35:57.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/registered_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      511 2019-12-04 12:31:59.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/reregistered_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      424 2019-12-04 12:32:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/reregistered_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      120 2019-12-04 13:14:45.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/reregistered_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      362 2018-05-16 10:37:44.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/username_changed_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      312 2018-05-16 10:38:00.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/username_changed_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:38:13.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/username_changed_subject.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1077 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/forgot_password.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1387 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/google_login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2021-12-16 14:11:26.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/invite.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10016 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1898 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/login_or_register.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1285 2020-07-28 01:34:57.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/manage_emails.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/member_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      742 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_choose.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_reconfigure.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      538 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_setup.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      440 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_sms_setup.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_verify_sms_setup.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      414 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/phone_login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      503 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/phone_login_verify.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/public_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8993 2022-08-24 01:43:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/register.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      432 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/resend_confirm_email.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1203 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/reset_password.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      961 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/user_profile.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.942496 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      760 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/404.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      772 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/501.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      877 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/admin_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1670 2022-03-06 21:20:12.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/config.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      371 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/create_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1023 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/create_playground_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      642 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/gd_sync_wait.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1284 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/github.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      404 2020-07-28 01:29:18.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/google_sync.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      966 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/googledrive.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      163 2016-11-26 18:11:31.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/health_check.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1050 2020-07-28 01:28:13.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/home_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4605 2022-05-16 12:54:38.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/interviews.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3130 2022-02-23 03:19:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/logs.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      667 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_account.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3299 2022-02-19 19:30:54.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_api.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2217 2022-06-11 12:37:06.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_playgrounds.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4957 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_projects.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      882 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/member_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1737 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/monitor.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      640 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/od_sync_wait.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2019-09-28 01:16:26.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officeaddin.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      545 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officefunctionfile.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5637 2019-05-21 21:50:45.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officemanifest.xml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4932 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officeouter.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      967 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/onedrive.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      726 2018-02-25 11:28:04.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/packages.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9997 2022-06-11 13:13:03.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/playground.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      198 2018-11-23 20:30:43.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/playground_poll.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9591 2022-06-11 13:12:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/playgroundfiles.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11491 2021-12-17 02:07:03.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/playgroundpackages.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      900 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/pull_playground_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1428 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/rename_project.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      294 2017-10-05 03:05:06.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/restart.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      457 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/socketserver.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      416 2017-11-04 17:12:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/start-embedded.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1106 2021-05-05 12:56:34.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/start.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      579 2020-04-12 15:32:42.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/test_embed.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      244 2017-05-30 00:47:01.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/testgoogledrive.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      354 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/testpost.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14703 2022-03-15 17:45:23.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/train.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2558 2022-05-11 13:43:23.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/update_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/update_package_wait.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3122 2022-03-19 16:00:09.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/utilities.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      125 2017-01-19 12:40:42.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/view_source.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      939 2019-05-21 21:49:14.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/webrtc.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.946496 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:37.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      669 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/add_user_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2661 2022-03-05 15:41:47.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/edit_user_profile_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      474 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/new_role_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      703 2021-12-05 22:33:52.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/request_developer.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      593 2022-02-21 16:31:46.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/rolelist.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5644 2022-08-24 16:46:18.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/user_profile_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4071 2022-08-09 20:39:49.000000 docassemble.webapp-1.4.9/docassemble/webapp/templates/users/userlist.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      182 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/testrun.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      946 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/translations.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41528 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/update.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      486 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/update_config.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2592 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/user_database.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.946496 docassemble.webapp-1.4.9/docassemble/webapp/users/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.9/docassemble/webapp/users/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17310 2022-08-23 11:40:07.000000 docassemble.webapp-1.4.9/docassemble/webapp/users/forms.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8037 2022-08-17 03:06:02.000000 docassemble.webapp-1.4.9/docassemble/webapp/users/models.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23856 2022-08-24 02:14:51.000000 docassemble.webapp-1.4.9/docassemble/webapp/users/views.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      975 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/watchdog.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    90584 2022-08-05 21:23:53.000000 docassemble.webapp-1.4.9/docassemble/webapp/worker.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      581 2022-08-05 21:01:20.000000 docassemble.webapp-1.4.9/docassemble/webapp/wsgi_restart.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:16:06.874496 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      683 2022-09-10 18:16:06.000000 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36536 2022-09-10 18:16:06.000000 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/SOURCES.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-09-10 18:16:06.000000 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/dependency_links.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-09-10 18:16:06.000000 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/namespace_packages.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-09-10 18:16:06.000000 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/not-zip-safe
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4658 2022-09-10 18:16:06.000000 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/requires.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-09-10 18:16:06.000000 docassemble.webapp-1.4.9/docassemble.webapp.egg-info/top_level.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       79 2022-09-10 18:16:06.946496 docassemble.webapp-1.4.9/setup.cfg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10471 2022-09-10 18:15:31.000000 docassemble.webapp-1.4.9/setup.py
```

### Comparing `docassemble.webapp-1.4.8/PKG-INFO` & `docassemble.webapp-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.webapp
-Version: 1.4.8
+Version: 1.4.9
 Summary: The web application components of the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Description: See the [docassemble web site] for a description of **docassemble**
         and installation instructions.
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/env.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/env.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/script.py.mako` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     op.add_column(dbtableprefix + 'package', sa.Column('gitbranch', sa.String(255)))
 
+
 def downgrade():
     op.drop_column(dbtableprefix + 'package', 'gitbranch')
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 Revision ID: 4328f2c08f05
 Revises: eb61567ea005
 Create Date: 2019-02-05 19:23:02.744161
 
 """
 from alembic import op
-import sqlalchemy as sa
 from docassemble.webapp.database import dbtableprefix
 
 
 # revision identifiers, used by Alembic.
 revision = '4328f2c08f05'
 down_revision = 'eb61567ea005'
 branch_labels = None
@@ -40,14 +39,15 @@
     op.create_index(dbtableprefix + 'ix_userdictkeys_filename', 'userdictkeys', ['filename'])
     op.create_index(dbtableprefix + 'ix_userdictkeys_key', 'userdictkeys', ['key'])
     op.create_index(dbtableprefix + 'ix_userdictkeys_temp_user_id', 'userdictkeys', ['temp_user_id'])
     op.create_index(dbtableprefix + 'ix_userdictkeys_user_id', 'userdictkeys', ['user_id'])
     op.create_index(dbtableprefix + 'ix_userdict_key_filename', 'userdict', ['key', 'filename'])
     op.create_index(dbtableprefix + 'ix_userdictkeys_key_filename', 'userdictkeys', ['key', 'filename'])
 
+
 def downgrade():
     op.drop_index(dbtableprefix + 'ix_attachments_filename', table_name='attachments')
     op.drop_index(dbtableprefix + 'ix_attachments_key', table_name='attachments')
     op.drop_index(dbtableprefix + 'ix_chatlog_filename', table_name='chatlog')
     op.drop_index(dbtableprefix + 'ix_chatlog_key', table_name='chatlog')
     op.drop_index(dbtableprefix + 'ix_machinelearning_key', table_name='machinelearning')
     op.drop_index(dbtableprefix + 'ix_objectstorage_key', table_name='objectstorage')
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 Revision ID: 693d02299f38
 Revises: c2ef4831ef76
 Create Date: 2021-05-08 07:49:59.180288
 
 """
 from alembic import op
-import sqlalchemy as sa
 from docassemble.webapp.database import dbtableprefix
 
 
 # revision identifiers, used by Alembic.
 revision = '693d02299f38'
 down_revision = 'c2ef4831ef76'
 branch_labels = None
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """alter database for mysql compatibility
 
 Revision ID: 9be372ec38bc
 Revises: 4328f2c08f05
 Create Date: 2020-02-16 15:43:35.276655
 
 """
+import sys
 from alembic import op
 import sqlalchemy as sa
 from docassemble.webapp.database import dbtableprefix, dbprefix, daconfig
-import sys
 
 # revision identifiers, used by Alembic.
 revision = '9be372ec38bc'
 down_revision = '4328f2c08f05'
 branch_labels = None
 depends_on = None
 
+
 def upgrade():
     if dbprefix.startswith('postgresql') and not daconfig.get('force text to varchar upgrade', False):
         sys.stderr.write("Not changing text type to varchar type because underlying database is PostgreSQL\n")
     else:
         op.alter_column(
             table_name='userdict',
             column_name='filename',
@@ -78,14 +79,15 @@
         op.alter_column(
             table_name='globalobjectstorage',
             column_name='key',
             type_=sa.String(1024)
         )
     op.create_index(dbtableprefix + 'ix_uploads_yamlfile', 'uploads', ['yamlfile'])
 
+
 def downgrade():
     op.alter_column(
         table_name='userdict',
         column_name='filename',
         type_=sa.Text()
     )
     op.alter_column(
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 Revision ID: a8746ddab8cb
 Revises: 693d02299f38
 Create Date: 2022-04-07 17:49:47.832279
 
 """
 from alembic import op
-import sqlalchemy as sa
 from docassemble.webapp.database import dbtableprefix
 
 
 # revision identifiers, used by Alembic.
 revision = 'a8746ddab8cb'
 down_revision = '693d02299f38'
 branch_labels = None
@@ -34,14 +33,15 @@
     op.create_unique_constraint(dbtableprefix + 'uploadsroleauth_id_key', dbtableprefix + 'uploadsroleauth', ['id'])
     op.create_unique_constraint(dbtableprefix + 'uploadsuserauth_id_key', dbtableprefix + 'uploadsuserauth', ['id'])
     op.create_unique_constraint(dbtableprefix + 'user_id_key', dbtableprefix + 'user', ['id'])
     op.create_unique_constraint(dbtableprefix + 'user_auth_id_key', dbtableprefix + 'user_auth', ['id'])
     op.create_unique_constraint(dbtableprefix + 'user_invite_id_key', dbtableprefix + 'user_invite', ['id'])
     op.create_unique_constraint(dbtableprefix + 'user_roles_id_key', dbtableprefix + 'user_roles', ['id'])
 
+
 def downgrade():
     op.drop_constraint(dbtableprefix + 'chatlog_id_key', dbtableprefix + 'chatlog')
     op.drop_constraint(dbtableprefix + 'email_id_key', dbtableprefix + 'email')
     op.drop_constraint(dbtableprefix + 'emailattachment_id_key', dbtableprefix + 'emailattachment')
     op.drop_constraint(dbtableprefix + 'globalobjectstorage_id_key', dbtableprefix + 'globalobjectstorage')
     op.drop_constraint(dbtableprefix + 'jsonstorage_id_key', dbtableprefix + 'jsonstorage')
     op.drop_constraint(dbtableprefix + 'machinelearning_id_key', dbtableprefix + 'machinelearning')
@@ -54,8 +54,7 @@
     op.drop_constraint(dbtableprefix + 'uploads_indexno_key', dbtableprefix + 'uploads')
     op.drop_constraint(dbtableprefix + 'uploadsroleauth_id_key', dbtableprefix + 'uploadsroleauth')
     op.drop_constraint(dbtableprefix + 'uploadsuserauth_id_key', dbtableprefix + 'uploadsuserauth')
     op.drop_constraint(dbtableprefix + 'user_id_key', dbtableprefix + 'user')
     op.drop_constraint(dbtableprefix + 'user_auth_id_key', dbtableprefix + 'user_auth')
     op.drop_constraint(dbtableprefix + 'user_invite_id_key', dbtableprefix + 'user_invite')
     op.drop_constraint(dbtableprefix + 'user_roles_id_key', dbtableprefix + 'user_roles')
-
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 depends_on = None
 
 
 def upgrade():
     op.add_column(dbtableprefix + 'uploads', sa.Column('private', sa.Boolean, server_default=sa.true()))
     op.add_column(dbtableprefix + 'uploads', sa.Column('persistent', sa.Boolean, server_default=sa.false()))
 
+
 def downgrade():
     op.drop_column(dbtableprefix + 'uploads', 'private')
     op.drop_column(dbtableprefix + 'uploads', 'persistent')
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/alembic.ini` & `docassemble.webapp-1.4.9/docassemble/webapp/alembic.ini`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/api_key.py` & `docassemble.webapp-1.4.9/docassemble/webapp/api_key.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/app_object.py` & `docassemble.webapp-1.4.9/docassemble/webapp/app_object.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/app_socket.py` & `docassemble.webapp-1.4.9/docassemble/webapp/app_socket.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/backend.py` & `docassemble.webapp-1.4.9/docassemble/webapp/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,15 @@
 
 def da_send_mail(the_message):
     mail.send(the_message)
 
 DEFAULT_LANGUAGE = daconfig.get('language', 'en')
 DEFAULT_LOCALE = daconfig.get('locale', 'en_US.utf8')
 DEFAULT_DIALECT = daconfig.get('dialect', 'us')
+DEFAULT_VOICE = daconfig.get('voice', None)
 if 'timezone' in daconfig and daconfig['timezone'] is not None:
     DEFAULT_TIMEZONE = daconfig['timezone']
 else:
     try:
         DEFAULT_TIMEZONE = tzlocal.get_localzone_name()
     except:
         DEFAULT_TIMEZONE = 'America/New_York'
@@ -304,14 +305,15 @@
 
 DEFAULT_COUNTRY = daconfig.get('country', None) or re.sub(r'^.*_', '', re.sub(r'\..*', r'', DEFAULT_LOCALE))
 
 
 docassemble.base.functions.update_server(default_language=DEFAULT_LANGUAGE,
                                          default_locale=DEFAULT_LOCALE,
                                          default_dialect=DEFAULT_DIALECT,
+                                         default_voice=DEFAULT_VOICE,
                                          default_timezone=DEFAULT_TIMEZONE,
                                          default_country=DEFAULT_COUNTRY,
                                          daconfig=daconfig,
                                          hostname=hostname,
                                          debug_status=DEBUG,
                                          save_numbered_file=save_numbered_file,
                                          send_mail=da_send_mail,
@@ -331,15 +333,15 @@
                                          server_sql_delete=sql_delete,
                                          server_sql_keys=sql_keys,
                                          alchemy_url=docassemble.webapp.user_database.alchemy_url,
                                          connect_args=docassemble.webapp.user_database.connect_args,
                                          default_table_class=DEFAULT_TABLE_CLASS,
                                          default_thead_class=DEFAULT_THEAD_CLASS,
                                          to_text=to_text)
-docassemble.base.functions.set_language(DEFAULT_LANGUAGE, dialect=DEFAULT_DIALECT)
+docassemble.base.functions.set_language(DEFAULT_LANGUAGE, dialect=DEFAULT_DIALECT, voice=DEFAULT_VOICE)
 docassemble.base.functions.set_locale(DEFAULT_LOCALE)
 docassemble.base.functions.update_locale()
 
 
 def fix_words():
     word_file_list = daconfig.get('words', [])
     if not isinstance(word_file_list, list):
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/clicksend.py` & `docassemble.webapp-1.4.9/docassemble/webapp/clicksend.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/cloud.py` & `docassemble.webapp-1.4.9/docassemble/webapp/cloud.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/cloud_deregister.py` & `docassemble.webapp-1.4.9/docassemble/webapp/cloud_deregister.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/cloud_register.py` & `docassemble.webapp-1.4.9/docassemble/webapp/cloud_register.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/core/models.py` & `docassemble.webapp-1.4.9/docassemble/webapp/core/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     filename = db.Column(db.String(255), index=True)
     key = db.Column(db.String(250), index=True)
     phrase = db.Column(db.Text())
     question = db.Column(db.Integer())
     type = db.Column(db.String(20))
     language = db.Column(db.String(10))
     dialect = db.Column(db.String(10))
+    voice = db.Column(db.String(20))
     upload = db.Column(db.Integer(), db.ForeignKey(dbtableprefix + 'uploads.indexno', ondelete='CASCADE'))
     encrypted = db.Column(db.Boolean(), nullable=False, server_default=true())
     digest = db.Column(db.Text())
 
 
 class Supervisors(db.Model):
     __tablename__ = dbtableprefix + "supervisors"
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/create_tables.py` & `docassemble.webapp-1.4.9/docassemble/webapp/create_tables.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/cron.py` & `docassemble.webapp-1.4.9/docassemble/webapp/cron.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/daredis.py` & `docassemble.webapp-1.4.9/docassemble/webapp/daredis.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/db-schema.txt` & `docassemble.webapp-1.4.9/docassemble/webapp/data/db-schema.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 speaklist|upload|integer||
 speaklist|encrypted|boolean||true
 package|active|boolean||true
+machinelearning|modtime|timestamp without time zone||
 package_auth|id|integer||nextval('package_auth_id_seq'::regclass)
 package_auth|package_id|integer||
 package_auth|user_id|integer||
-machinelearning|modtime|timestamp without time zone||
-shortener|id|integer||nextval('shortener_id_seq'::regclass)
 install|id|integer||nextval('install_id_seq'::regclass)
+shortener|id|integer||nextval('shortener_id_seq'::regclass)
 machinelearning|active|boolean||false
 install|version|integer||
+globalobjectstorage|id|integer||nextval('globalobjectstorage_id_seq'::regclass)
 shortener|user_id|integer||
 shortener|temp_user_id|integer||
-globalobjectstorage|id|integer||nextval('globalobjectstorage_id_seq'::regclass)
+install|package_id|integer||
 shortener|index|integer||
 shortener|modtime|timestamp without time zone||now()
 role|id|integer||nextval('role_id_seq'::regclass)
-install|package_id|integer||
 jsonstorage|id|integer||nextval('jsonstorage_id_seq'::regclass)
-supervisors|id|integer||nextval('supervisors_id_seq'::regclass)
 email|datetime_received|timestamp without time zone||
+supervisors|id|integer||nextval('supervisors_id_seq'::regclass)
 machinelearning|id|integer||nextval('machinelearning_id_seq'::regclass)
-supervisors|start_time|timestamp without time zone||now()
 jsonstorage|data|jsonb||
-uploads|indexno|integer||nextval('uploads_indexno_seq'::regclass)
+supervisors|start_time|timestamp without time zone||now()
 globalobjectstorage|encrypted|boolean||true
+uploads|indexno|integer||nextval('uploads_indexno_seq'::regclass)
 jsonstorage|modtime|timestamp without time zone||now()
 jsonstorage|persistent|boolean||false
+objectstorage|id|integer||nextval('objectstorage_id_seq'::regclass)
 uploads|private|boolean||true
 uploads|persistent|boolean||false
 uploadsroleauth|id|integer||nextval('uploadsroleauth_id_seq'::regclass)
 uploadsroleauth|uploads_indexno|integer||
 uploadsroleauth|role_id|integer||
 uploadsuserauth|id|integer||nextval('uploadsuserauth_id_seq'::regclass)
 uploadsuserauth|uploads_indexno|integer||
 uploadsuserauth|user_id|integer||
 uploadsuserauth|temp_user_id|integer||
 tempuser|id|integer||nextval('tempuser_id_seq'::regclass)
 user_auth|id|integer||nextval('user_auth_id_seq'::regclass)
 user_auth|user_id|integer||
-objectstorage|id|integer||nextval('objectstorage_id_seq'::regclass)
 globalobjectstorage|user_id|integer||
-user_invite|id|integer||nextval('user_invite_id_seq'::regclass)
 globalobjectstorage|temp_user_id|integer||
+user_invite|id|integer||nextval('user_invite_id_seq'::regclass)
+chatlog|id|integer||nextval('chatlog_id_seq'::regclass)
 user_invite|role_id|integer||
 user_invite|invited_by_user_id|integer||
-chatlog|id|integer||nextval('chatlog_id_seq'::regclass)
+package|id|integer||nextval('package_id_seq'::regclass)
 user_roles|id|integer||nextval('user_roles_id_seq'::regclass)
 user_roles|user_id|integer||
 user_roles|role_id|integer||
 userdict|indexno|integer||nextval('userdict_indexno_seq'::regclass)
-package|id|integer||nextval('package_id_seq'::regclass)
 attachments|question|integer||
 attachments|id|integer||nextval('attachments_id_seq'::regclass)
+chatlog|user_id|integer||
 userdict|user_id|integer||
 userdict|encrypted|boolean||true
 userdict|modtime|timestamp without time zone||
 userdictkeys|indexno|integer||nextval('userdictkeys_indexno_seq'::regclass)
-chatlog|user_id|integer||
 chatlog|temp_user_id|integer||
+chatlog|owner_id|integer||
 userdictkeys|user_id|integer||
 userdictkeys|temp_user_id|integer||
 user|id|integer||nextval('user_id_seq'::regclass)
-chatlog|owner_id|integer||
 chatlog|temp_owner_id|integer||
 chatlog|open_to_peer|boolean||false
+chatlog|encrypted|boolean||true
 user|confirmed_at|timestamp without time zone||
 user|active|boolean||false
-chatlog|encrypted|boolean||true
 chatlog|modtime|timestamp without time zone||
 emailattachment|id|integer||nextval('emailattachment_id_seq'::regclass)
 emailattachment|email_id|integer||
 emailattachment|index|integer||
 attachments|encrypted|boolean||true
 email|id|integer||nextval('email_id_seq'::regclass)
 emailattachment|upload|integer||
 speaklist|id|integer||nextval('speaklist_id_seq'::regclass)
 package|upload|integer||
 package|version|integer||1
 email|datetime_message|timestamp without time zone||
 speaklist|question|integer||
+machinelearning|create_time|timestamp without time zone||
 user|modified_at|timestamp without time zone||
 user|last_login|timestamp without time zone||
-machinelearning|create_time|timestamp without time zone||
 package|dependency|boolean||false
 package|core|boolean||false
-speaklist|language|character varying|10|
+speaklist|dialect|character varying|10|
 attachments|key|character varying|250|
 attachments|dictionary|text||
 attachments|filename|text||
 email|short|character varying|250|
 email|all_addr|text||
 email|to_addr|text||
 email|cc_addr|text||
@@ -122,17 +122,18 @@
 chatlog|message|text||
 emailattachment|content_type|text||
 emailattachment|extension|text||
 speaklist|filename|character varying|255|
 speaklist|key|character varying|250|
 speaklist|phrase|text||
 speaklist|type|character varying|20|
+speaklist|language|character varying|10|
 alembic_version|version_num|character varying|32|
-speaklist|dialect|character varying|10|
 speaklist|digest|text||
+speaklist|voice|character varying|20|
 package_auth|authtype|character varying|255|'owner'::character varying
 shortener|short|character varying|250|
 shortener|filename|character varying|255|
 shortener|uid|character varying|250|
 shortener|key|character varying|255|
 role|name|character varying|50|
 role|description|character varying|255|
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/questions/wizard-template.yml` & `docassemble.webapp-1.4.9/docassemble/webapp/data/questions/wizard-template.yml`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/android-chrome-192x192.png` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/android-chrome-512x512.png` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/apple-touch-icon.png` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/favicon-16x16.png` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/favicon-32x32.png` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/favicon.ico` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/mstile-150x150.png` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/data/static/test-document.docx` & `docassemble.webapp-1.4.9/docassemble/webapp/data/static/test-document.docx`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/database.py` & `docassemble.webapp-1.4.9/docassemble/webapp/database.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/db_object.py` & `docassemble.webapp-1.4.9/docassemble/webapp/db_object.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/deregister.py` & `docassemble.webapp-1.4.9/docassemble/webapp/deregister.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/develop.py` & `docassemble.webapp-1.4.9/docassemble/webapp/develop.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/file_access.py` & `docassemble.webapp-1.4.9/docassemble/webapp/file_access.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/files.py` & `docassemble.webapp-1.4.9/docassemble/webapp/files.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/fix_postgresql_tables.py` & `docassemble.webapp-1.4.9/docassemble/webapp/fix_postgresql_tables.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/fixpickle.py` & `docassemble.webapp-1.4.9/docassemble/webapp/fixpickle.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/google_api.py` & `docassemble.webapp-1.4.9/docassemble/webapp/google_api.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/info.py` & `docassemble.webapp-1.4.9/docassemble/webapp/info.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/install_certs.py` & `docassemble.webapp-1.4.9/docassemble/webapp/install_certs.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/jsonstore.py` & `docassemble.webapp-1.4.9/docassemble/webapp/jsonstore.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/list-cloud.py` & `docassemble.webapp-1.4.9/docassemble/webapp/list-cloud.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/listlog.py` & `docassemble.webapp-1.4.9/docassemble/webapp/listlog.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/machinelearning.py` & `docassemble.webapp-1.4.9/docassemble/webapp/machinelearning.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/mailgun_mail.py` & `docassemble.webapp-1.4.9/docassemble/webapp/mailgun_mail.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/packages/models.py` & `docassemble.webapp-1.4.9/docassemble/webapp/packages/models.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/playground.py` & `docassemble.webapp-1.4.9/docassemble/webapp/playground.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/process_email.py` & `docassemble.webapp-1.4.9/docassemble/webapp/process_email.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/register.py` & `docassemble.webapp-1.4.9/docassemble/webapp/register.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/restart.py` & `docassemble.webapp-1.4.9/docassemble/webapp/restart.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/screenreader.py` & `docassemble.webapp-1.4.9/docassemble/webapp/screenreader.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/sendgrid_mail.py` & `docassemble.webapp-1.4.9/docassemble/webapp/sendgrid_mail.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/server.py` & `docassemble.webapp-1.4.9/docassemble/webapp/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,43 +518,61 @@
 os.environ['PYTHON_EGG_CACHE'] = tempfile.gettempdir()
 PNG_RESOLUTION = daconfig.get('png resolution', 300)
 PNG_SCREEN_RESOLUTION = daconfig.get('png screen resolution', 72)
 PDFTOPPM_COMMAND = daconfig.get('pdftoppm', 'pdftoppm')
 DEFAULT_LANGUAGE = daconfig.get('language', 'en')
 DEFAULT_LOCALE = daconfig.get('locale', 'en_US.utf8')
 DEFAULT_DIALECT = daconfig.get('dialect', 'us')
+DEFAULT_VOICE = daconfig.get('voice', None)
 LOGSERVER = daconfig.get('log server', None)
 CHECKIN_INTERVAL = int(daconfig.get('checkin interval', 6000))
 # message_sequence = dbtableprefix + 'message_id_seq'
 NOTIFICATION_CONTAINER = '<div class="datopcenter col-sm-7 col-md-6 col-lg-5" id="daflash">%s</div>'
 NOTIFICATION_MESSAGE = '<div class="da-alert alert alert-%s alert-dismissible fade show" role="alert">%s<button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button></div>'
 
 USING_SUPERVISOR = bool(os.environ.get('SUPERVISOR_SERVER_URL', None))
 SINGLE_SERVER = USING_SUPERVISOR and bool(':all:' in ':' + os.environ.get('CONTAINERROLE', 'all') + ':')
 
 audio_mimetype_table = {'mp3': 'audio/mpeg', 'ogg': 'audio/ogg'}
 
 valid_voicerss_dialects = {
+    'ar': ['eg', 'sa'],
+    'bg': ['bg'],
     'ca': ['es'],
-    'zh': ['cn', 'hk', 'tw'],
+    'cs': ['cz'],
     'da': ['dk'],
-    'nl': ['nl'],
-    'en': ['au', 'ca', 'gb', 'in', 'us'],
+    'de': ['de', 'at', 'ch'],
+    'el': ['gr'],
+    'en': ['au', 'ca', 'gb', 'in', 'ie', 'us'],
+    'es': ['mx', 'es'],
     'fi': ['fi'],
-    'fr': ['ca, fr'],
-    'de': ['de'],
+    'fr': ['ca', 'fr', 'ch'],
+    'he': ['il'],
+    'hi': ['in'],
+    'hr': ['hr'],
+    'hu': ['hu'],
+    'id': ['id'],
     'it': ['it'],
     'ja': ['jp'],
     'ko': ['kr'],
+    'ms': ['my'],
     'nb': ['no'],
+    'nl': ['be', 'nl'],
     'pl': ['pl'],
     'pt': ['br', 'pt'],
+    'ro': ['ro'],
     'ru': ['ru'],
-    'es': ['mx', 'es'],
-    'sv': ['se']
+    'sk': ['sk'],
+    'sl': ['si'],
+    'sv': ['se'],
+    'ta': ['in'],
+    'th': ['th'],
+    'tr': ['tr'],
+    'vi': ['vn'],
+    'zh': ['cn', 'hk', 'tw']
     }
 
 voicerss_config = daconfig.get('voicerss', None)
 VOICERSS_ENABLED = not bool(not voicerss_config or ('enable' in voicerss_config and not voicerss_config['enable']) or not ('key' in voicerss_config and voicerss_config['key']))
 ROOT = daconfig.get('root', '/')
 # app.logger.warning("default sender is " + current_app.config['MAIL_DEFAULT_SENDER'] + "\n")
 exit_page = daconfig.get('exitpage', 'https://docassemble.org')
@@ -986,14 +1004,32 @@
     #     return render_template(user_manager.login_template,
     #                            form=login_form,
     #                            login_form=login_form,
     #                            register_form=register_form,
     #                            extra_css=Markup(extra_css),
     #                            extra_js=Markup(extra_js))
     # else:
+    if app.config['AUTO_LOGIN'] and not (app.config['USE_PASSWORD_LOGIN'] or ('admin' in request.args and request.args['admin'] == '1') or ('from_logout' in request.args and request.args['from_logout'] == '1')):
+        if app.config['AUTO_LOGIN'] is True:
+            number_of_methods = 0
+            the_method = None
+            for login_method in ('USE_PHONE_LOGIN', 'USE_GOOGLE_LOGIN', 'USE_FACEBOOK_LOGIN', 'USE_TWITTER_LOGIN', 'USE_AUTH0_LOGIN', 'USE_KEYCLOAK_LOGIN', 'USE_AZURE_LOGIN'):
+                if app.config[login_method]:
+                    number_of_methods += 1
+                    the_method = re.sub(r'USE_(.*)_LOGIN', r'\1', login_method).lower()
+            if number_of_methods > 1:
+                the_method = None
+        else:
+            the_method = app.config['AUTO_LOGIN']
+        if the_method == 'phone':
+            return redirect(url_for('phone_login'))
+        if the_method == 'google':
+            return redirect(url_for('google_page', next=request.args.get('next', '')))
+        if the_method in ('facebook', 'twitter', 'auth0', 'keycloak', 'azure'):
+            return redirect(url_for('oauth_authorize', provider=the_method, next=request.args.get('next', '')))
     response = make_response(user_manager.render_function(user_manager.login_template,
                                                           form=login_form,
                                                           login_form=login_form,
                                                           register_form=register_form), 200)
     response.headers['Cache-Control'] = 'no-store, no-cache, must-revalidate, post-check=0, pre-check=0, max-age=0'
     return response
 
@@ -1024,17 +1060,17 @@
             next_url = decrypt_phrase(repad(bytearray(request.args['next'], encoding='utf-8')).decode(), app.secret_key)
         except:
             pass
     if next_url is None:
         next_url = daconfig.get('logoutpage', None)
     if next_url is None:
         if session.get('language', None) and session['language'] != DEFAULT_LANGUAGE:
-            next_url = _endpoint_url(user_manager.after_logout_endpoint, lang=session['language'])
+            next_url = _endpoint_url(user_manager.after_logout_endpoint, lang=session['language'], from_logout='1')
         else:
-            next_url = _endpoint_url(user_manager.after_logout_endpoint)
+            next_url = _endpoint_url(user_manager.after_logout_endpoint, from_logout='1')
     if current_user.is_authenticated:
         if current_user.social_id.startswith('auth0$') and 'oauth' in daconfig and 'auth0' in daconfig['oauth'] and 'domain' in daconfig['oauth']['auth0']:
             if next_url.startswith('/'):
                 next_url = get_base_url() + next_url
             next_url = 'https://' + daconfig['oauth']['auth0']['domain'] + '/v2/logout?' + urlencode(dict(returnTo=next_url, client_id=daconfig['oauth']['auth0']['id']))
         if current_user.social_id.startswith('keycloak$') and 'oauth' in daconfig and 'keycloak' in daconfig['oauth'] and 'domain' in daconfig['oauth']['keycloak']:
             if next_url.startswith('/'):
@@ -1417,14 +1453,15 @@
 app.config['USE_KEYCLOAK_LOGIN'] = False
 app.config['USE_AZURE_LOGIN'] = False
 app.config['USE_GOOGLE_DRIVE'] = False
 app.config['USE_ONEDRIVE'] = False
 app.config['USE_PHONE_LOGIN'] = False
 app.config['USE_GITHUB'] = False
 app.config['USE_PASSWORD_LOGIN'] = not bool(daconfig.get('password login', True) is False)
+app.config['AUTO_LOGIN'] = daconfig.get('auto login', False)
 if twilio_config is not None and daconfig.get('phone login', False) is True:
     app.config['USE_PHONE_LOGIN'] = True
 if 'oauth' in daconfig:
     app.config['OAUTH_CREDENTIALS'] = daconfig['oauth']
     app.config['USE_GOOGLE_LOGIN'] = bool('google' in daconfig['oauth'] and not ('enable' in daconfig['oauth']['google'] and daconfig['oauth']['google']['enable'] is False))
     app.config['USE_FACEBOOK_LOGIN'] = bool('facebook' in daconfig['oauth'] and not ('enable' in daconfig['oauth']['facebook'] and daconfig['oauth']['facebook']['enable'] is False))
     app.config['USE_TWITTER_LOGIN'] = bool('twitter' in daconfig['oauth'] and not ('enable' in daconfig['oauth']['twitter'] and daconfig['oauth']['twitter']['enable'] is False))
@@ -8386,14 +8423,15 @@
       else {
         daIframeEmbed = false;
       }
       var daJsEmbed = """ + (json.dumps(js_target) if is_js else 'false') + """;
       var daAllowGoingBack = """ + ('true' if allow_going_back else 'false') + """;
       var daSteps = """ + str(steps) + """;
       var daIsUser = """ + is_user + """;
+      var daUserId = """ + ('null' if current_user.is_anonymous else str(current_user.id)) + """;
       var daChatStatus = """ + json.dumps(chat_status) + """;
       var daChatAvailable = """ + json.dumps(chat_available) + """;
       var daChatPartnersAvailable = 0;
       var daPhoneAvailable = false;
       var daChatMode = """ + json.dumps(chat_mode) + """;
       var daSendChanges = """ + send_changes + """;
       var daInitialized = false;
@@ -11871,14 +11909,15 @@
         bodyclass += ' da-pad-for-footer'
     if debug_mode:
         interview_status.screen_reader_text = {}
     if 'speak_text' in interview_status.extras and interview_status.extras['speak_text']:
         interview_status.initialize_screen_reader()
         util_language = docassemble.base.functions.get_language()
         util_dialect = docassemble.base.functions.get_dialect()
+        util_voice = docassemble.base.functions.get_voice()
         question_language = interview_status.question.language
         if len(interview.translations) > 0:
             the_language = util_language
         elif question_language != '*':
             the_language = question_language
         else:
             the_language = util_language
@@ -11890,17 +11929,27 @@
             the_dialect = voicerss_config['dialects'][the_language]
         elif the_language in valid_voicerss_dialects:
             the_dialect = valid_voicerss_dialects[the_language][0]
         else:
             logmessage("index: unable to determine dialect; reverting to default")
             the_language = DEFAULT_LANGUAGE
             the_dialect = DEFAULT_DIALECT
+        if the_language == util_language and the_dialect == util_dialect and util_voice is not None:
+            the_voice = util_voice
+        elif voicerss_config and 'voices' in voicerss_config and isinstance(voicerss_config['voices'], dict) and the_language in voicerss_config['voices'] and isinstance(voicerss_config['voices'][the_language], dict) and the_dialect in voicerss_config['voices'][the_language]:
+            the_voice = voicerss_config['voices'][the_language][the_dialect]
+        elif voicerss_config and 'voices' in voicerss_config and isinstance(voicerss_config['voices'], dict) and the_language in voicerss_config['voices'] and isinstance(voicerss_config['voices'][the_language], str):
+            the_voice = voicerss_config['voices'][the_language]
+        elif the_language == DEFAULT_LANGUAGE and the_dialect == DEFAULT_DIALECT:
+            the_voice = DEFAULT_VOICE
+        else:
+            the_voice = None
         for question_type in ('question', 'help'):
             for audio_format in ('mp3', 'ogg'):
-                interview_status.screen_reader_links[question_type].append([url_for('speak_file', i=yaml_filename, question=interview_status.question.number, digest='XXXTHEXXX' + question_type + 'XXXHASHXXX', type=question_type, format=audio_format, language=the_language, dialect=the_dialect), audio_mimetype_table[audio_format]])
+                interview_status.screen_reader_links[question_type].append([url_for('speak_file', i=yaml_filename, question=interview_status.question.number, digest='XXXTHEXXX' + question_type + 'XXXHASHXXX', type=question_type, format=audio_format, language=the_language, dialect=the_dialect, voice=the_voice or ''), audio_mimetype_table[audio_format]])
     if (not validated) and the_question.name == interview_status.question.name:
         for def_key, def_val in new_values.items():
             safe_def_key = safeid(def_key)
             if isinstance(def_val, list):
                 def_val = '[' + ','.join(def_val) + ']'
             if safe_def_key in all_field_numbers:
                 for number in all_field_numbers[safe_def_key]:
@@ -12015,27 +12064,30 @@
             phrase = to_text(interview_status.screen_reader_text[question_type])
             if encrypted:
                 the_phrase = encrypt_phrase(phrase, secret)
             else:
                 the_phrase = pack_phrase(phrase)
             the_hash = MD5Hash(data=phrase).hexdigest()
             content = re.sub(r'XXXTHEXXX' + question_type + 'XXXHASHXXX', the_hash, content)
-            existing_entry = db.session.execute(select(SpeakList).filter_by(filename=yaml_filename, key=user_code, question=interview_status.question.number, digest=the_hash, type=question_type, language=the_language, dialect=the_dialect).with_for_update()).scalar()
+            params = {'filename': yaml_filename, 'key': user_code, 'question': interview_status.question.number, 'digest': the_hash, 'type': question_type, 'language': the_language, 'dialect': the_dialect}
+            if the_voice:
+                params['voice'] = the_voice
+            existing_entry = db.session.execute(select(SpeakList).filter_by(**params).with_for_update()).scalar()
             if existing_entry:
                 if existing_entry.encrypted:
                     existing_phrase = decrypt_phrase(existing_entry.phrase, secret)
                 else:
                     existing_phrase = unpack_phrase(existing_entry.phrase)
                 if phrase != existing_phrase:
                     logmessage("index: the phrase changed; updating it")
                     existing_entry.phrase = the_phrase
                     existing_entry.upload = None
                     existing_entry.encrypted = encrypted
             else:
-                new_entry = SpeakList(filename=yaml_filename, key=user_code, phrase=the_phrase, question=interview_status.question.number, digest=the_hash, type=question_type, language=the_language, dialect=the_dialect, encrypted=encrypted)
+                new_entry = SpeakList(filename=yaml_filename, key=user_code, phrase=the_phrase, question=interview_status.question.number, digest=the_hash, type=question_type, language=the_language, dialect=the_dialect, encrypted=encrypted, voice=the_voice)
                 db.session.add(new_entry)
             db.session.commit()
     append_css_urls = []
     if not is_ajax:
         start_output = standard_header_start
         if 'css' in interview.external_files:
             for packageref, fileref in interview.external_files['css']:
@@ -12414,27 +12466,33 @@
     key = session_info['uid']
     # encrypted = session_info['encrypted']
     question = request.args.get('question', None)
     question_type = request.args.get('type', None)
     file_format = request.args.get('format', None)
     the_language = request.args.get('language', None)
     the_dialect = request.args.get('dialect', None)
+    the_voice = request.args.get('voice', '')
+    if the_voice == '':
+        the_voice = None
     the_hash = request.args.get('digest', None)
     secret = request.cookies.get('secret', None)
     if secret is not None:
         secret = str(secret)
     if file_format not in ('mp3', 'ogg') or not (filename and key and question and question_type and file_format and the_language and the_dialect):
         logmessage("speak_file: could not serve speak file because invalid or missing data was provided: filename " + str(filename) + " and key " + str(key) + " and question number " + str(question) + " and question type " + str(question_type) + " and language " + str(the_language) + " and dialect " + str(the_dialect))
         return ('File not found', 404)
-    entry = db.session.execute(select(SpeakList).filter_by(filename=filename, key=key, question=question, digest=the_hash, type=question_type, language=the_language, dialect=the_dialect)).scalar()
+    params = {'filename': filename, 'key': key, 'question': question, 'digest': the_hash, 'type': question_type, 'language': the_language, 'dialect': the_dialect}
+    if the_voice:
+        params['voice'] = the_voice
+    entry = db.session.execute(select(SpeakList).filter_by(**params)).scalar()
     if not entry:
-        logmessage("speak_file: could not serve speak file because no entry could be found in speaklist for filename " + str(filename) + " and key " + str(key) + " and question number " + str(question) + " and question type " + str(question_type) + " and language " + str(the_language) + " and dialect " + str(the_dialect))
+        logmessage("speak_file: could not serve speak file because no entry could be found in speaklist for filename " + str(filename) + " and key " + str(key) + " and question number " + str(question) + " and question type " + str(question_type) + " and language " + str(the_language) + " and dialect " + str(the_dialect) + " and voice " + str(the_voice))
         return ('File not found', 404)
     if not entry.upload:
-        existing_entry = db.session.execute(select(SpeakList).where(and_(SpeakList.phrase == entry.phrase, SpeakList.language == entry.language, SpeakList.dialect == entry.dialect, SpeakList.upload != None, SpeakList.encrypted == entry.encrypted))).scalar()  # noqa: E711 # pylint: disable=singleton-comparison
+        existing_entry = db.session.execute(select(SpeakList).where(and_(SpeakList.phrase == entry.phrase, SpeakList.language == entry.language, SpeakList.dialect == entry.dialect, SpeakList.voice == entry.voice, SpeakList.upload != None, SpeakList.encrypted == entry.encrypted))).scalar()  # noqa: E711 # pylint: disable=singleton-comparison
         if existing_entry:
             logmessage("speak_file: found existing entry: " + str(existing_entry.id) + ".  Setting to " + str(existing_entry.upload))
             entry.upload = existing_entry.upload
         else:
             if not VOICERSS_ENABLED:
                 logmessage("speak_file: could not serve speak file because voicerss not enabled")
                 return ('File not found', 404)
@@ -12443,15 +12501,18 @@
             if entry.encrypted:
                 phrase = decrypt_phrase(entry.phrase, secret)
             else:
                 phrase = unpack_phrase(entry.phrase)
             url = voicerss_config.get('url', "https://api.voicerss.org/")
             # logmessage("Retrieving " + url)
             audio_file = SavedFile(new_file_number, extension='mp3', fix=True, should_not_exist=True)
-            audio_file.fetch_url_post(url, dict(f=voicerss_config.get('format', '16khz_16bit_stereo'), key=voicerss_config['key'], src=phrase, hl=str(entry.language) + '-' + str(entry.dialect)))
+            voicerss_parameters = {'f': voicerss_config.get('format', '16khz_16bit_stereo'), 'key': voicerss_config['key'], 'src': phrase, 'hl': str(entry.language) + '-' + str(entry.dialect)}
+            if the_voice is not None:
+                voicerss_parameters['v'] = the_voice
+            audio_file.fetch_url_post(url, voicerss_parameters)
             if audio_file.size_in_bytes() > 100:
                 call_array = [daconfig.get('pacpl', 'pacpl'), '-t', 'ogg', audio_file.path + '.mp3']
                 logmessage("speak_file: calling " + " ".join(call_array))
                 result = subprocess.run(call_array, check=False).returncode
                 if result != 0:
                     logmessage("speak_file: failed to convert downloaded mp3 (" + audio_file.path + '.mp3' + ") to ogg")
                     return ('File not found', 404)
@@ -28614,15 +28675,15 @@
                 if len(r.keys('da:apikey:userid:*:key:' + new_api_key + ':info')) == 0:
                     r.set('da:apikey:userid:' + str(current_user.id) + ':key:' + new_api_key + ':info', json.dumps(info))
                     success = True
                     break
             if not success:
                 flash(word("Could not create new key"), 'error')
                 return render_template('pages/manage_api.html', **argu)
-            argu['description'] = Markup(word("Your new API key, known internally as %s, is %s") % (form.name.data, "<code>" + api_key + "</code>") + '.  ' + word("This is the only time you will be able to see your API key, so make sure to make a note of it and keep it in a secure place."))
+            argu['description'] = Markup(word("Your new API key, known internally as <strong>%s</strong>, is:<br />%s<br />") % (form.name.data, "<code>" + api_key + "</code>") + word("<strong>This is the only time you will be able to see your API key</strong>, so make sure to make a note of it and keep it in a secure place."))
         elif action == 'edit':
             argu['title'] = word("Edit API Key")
             argu['tab_title'] = argu['title']
             argu['page_title'] = argu['title']
             api_key = form.key.data
             argu['api_key'] = api_key
             rkey = 'da:apikey:userid:' + str(current_user.id) + ':key:' + str(form.key.data) + ':info'
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/setup.py` & `docassemble.webapp-1.4.9/docassemble/webapp/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import timedelta
 import re
 import importlib
 from docassemble.webapp.app_object import app
 from docassemble.base.config import daconfig
 import docassemble.webapp.database
-da_version = '1.4.8'
+da_version = '1.4.9'
 app.config['DA_VERSION'] = da_version
 app.config['APP_NAME'] = daconfig.get('appname', 'docassemble')
 app.config['BRAND_NAME'] = daconfig.get('brandname', daconfig.get('appname', 'docassemble'))
 app.config['SHOW_PROFILE'] = bool(daconfig.get('show profile link', True))
 app.config['SHOW_MY_INTERVIEWS'] = bool(daconfig.get('show interviews link', True))
 app.config['SHOW_DISPATCH'] = bool(len(daconfig['dispatch']) and daconfig.get('show dispatch link', False) > 0)
 app.config['MAIL_USERNAME'] = daconfig['mail'].get('username', None)
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/socketserver.py` & `docassemble.webapp-1.4.9/docassemble/webapp/socketserver.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.eot` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.eot`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.ttf` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.woff` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/MaterialIcons-Regular.woff2` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/additional-methods.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/additional-methods.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/adminbundle.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/adminbundle.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/app.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/app.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/azure-logo.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/azure-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundle.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundle.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundle.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundle.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundlenojquery.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundlenojquery.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/bundlewrapjquery.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/bundlewrapjquery.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/chat.ico` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/chat.ico`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/facebook-logo.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/facebook-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/google-logo.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/google-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.validate.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.validate.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.visible.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.visible.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/jquery.visible.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/jquery.visible.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/js.cookie.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/keycloak-logo.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/keycloak-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/option-vertical.svg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/option-vertical.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/playgroundbundle.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/playgroundbundle.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/playgroundbundle.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/playgroundbundle.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/pygments.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/pygments.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/pygments.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/pygments.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/socket.io.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/socket.io.min.js.map` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/socket.io.min.js.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/twitter-logo.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/twitter-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/upload.svg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/upload.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/webrtc.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/webrtc.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/webrtc.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/webrtc.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/app/wrap.svg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/app/wrap.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/areyousure/jquery.are-you-sure.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/areyousure/jquery.are-you-sure.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/css/bootstrap.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/README.md` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/dialog/dialog.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/dialog/dialog.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/autorefresh.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/autorefresh.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/fullscreen.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/fullscreen.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/panel.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/panel.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/placeholder.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/placeholder.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/display/rulers.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/display/rulers.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/closetag.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/closetag.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/continuelist.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/continuelist.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/matchtags.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/matchtags.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/css-hint.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/css-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/html-hint.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/html-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/show-hint.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/show-hint.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/show-hint.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/show-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/search.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/search.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/addon/search/searchcursor.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/addon/search/searchcursor.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/keymap/emacs.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/keymap/emacs.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/keymap/sublime.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/keymap/sublime.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/keymap/vim.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/keymap/vim.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/lib/codemirror.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/lib/codemirror.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/lib/codemirror.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/lib/codemirror.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/css.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/css.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/gss.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/gss.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/less.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/less.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/less_test.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/less_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/scss.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/scss.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/scss_test.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/scss_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/css/test.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/css/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/javascript.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/test.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/javascript/typescript.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/javascript/typescript.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/markdown.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/markdown/test.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/markdown/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/python/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/python/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/python/python.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/python/test.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/python/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/xml/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/xml/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/xml/test.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/xml/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/xml/xml.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/xml/xml.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/yaml/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/yaml/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/codemirror/mode/yaml/yaml.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/codemirror/mode/yaml/yaml.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/actions-parameters.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/actions-parameters.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/actions.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/actions.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/age_in_years.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/age_in_years.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/alignment.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/alignment.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/all-true.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/all-true.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/allow-emailing-false.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/allow-emailing-false.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/as-datetime.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/as-datetime.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/attachment-code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/attachment-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/audio.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/audio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/auto-terms.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/auto-terms.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_flash.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_flash.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_javascript.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_javascript.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_refresh.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_refresh.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_action_with_response_action.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_action_with_response_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/background_response_action_flash.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/background_response_action_flash.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons-code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons-icons.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons-icons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons-labels.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons-labels.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/buttons.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/buttons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/capitalize.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/capitalize.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/chat-partners-available.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/chat-partners-available.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/check-in.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/check-in.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-combobox.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-combobox.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-dropdown.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-dropdown.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-icons.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-icons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices-with-default.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices-with-default.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/choices.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/choices.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/comment.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/comment.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/continue-button-label.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/continue-button-label.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/continue.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/continue.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/country.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/country.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/cron.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/cron.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/css.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/css.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/currency.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/currency.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/current-datetime.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/current-datetime.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dadict.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dadict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dafile.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dafile.png`

 * *Files 4% similar despite different names*

#### sng

```diff
@@ -233,29 +233,29 @@
     (216,217,218)     # rgb = (0xd8,0xd9,0xda)
     (238,238,238)     # rgb = (0xee,0xee,0xee)
     (  0,128,  1)     # rgb = (0x00,0x80,0x01)
     (  0,  0,  0)     # rgb = (0x00,0x00,0x00) grey0
 }
 bKGD {index: 222}
 tIME {
-    # 11 Nov 2021 21:20:10 GMT
-    year:   2021
-    month:  11
-    day:    11
-    hour:   21
-    minute: 20
-    second: 10
+    #  9 Sep 2022 11:27:40 GMT
+    year:   2022
+    month:  9
+    day:    9
+    hour:   11
+    minute: 27
+    second: 40
 }
 tEXt {
     keyword: "date:create";
-    text: "2021-11-11T20:58:53+00:00";
+    text: "2022-09-09T11:27:34+00:00";
 }
 tEXt {
     keyword: "date:modify";
-    text: "2021-11-11T20:58:53+00:00";
+    text: "2022-09-09T11:27:34+00:00";
 }
 IMAGE {
     pixels hex
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
```

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/database_storage.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/database_storage.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-difference.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-difference.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-interval.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-interval.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/date-parts.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/date-parts.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dead-end.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dead-end.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/decoration.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/decoration.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/def.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/def.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/defined.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/defined.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/del.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/del.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/device.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/device.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/dialog-box.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/dialog-box.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-docx.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-docx.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-file.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-file.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-language.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-language.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document-variable-name.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document-variable-name.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/document.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/document.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/docx-template-table.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/docx-template-table.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/docx-template.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/docx-template.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/doors.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/doors.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/email-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/email-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/email-to-case-simple.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/email-to-case-simple.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/email-to-case.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/email-to-case.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/emoji-inline.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/emoji-inline.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exists.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exists.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit-buttons.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit-buttons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit-choices.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit-choices.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit-url.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit-url.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/exit.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/exit.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/external_files.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/external_files.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-checkboxes.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-checkboxes.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-choices-combobox.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-choices-combobox.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-choices.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-choices.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-mc-exclude.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-mc-exclude.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-mc.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-mc.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-noyesmaybe.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-noyesmaybe.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesno.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesno.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesnomaybe.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesnomaybe.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesnoradio.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesnoradio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fields-yesnowide.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fields-yesnowide.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/fix-punctuation.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/fix-punctuation.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/for_fruit.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/for_fruit.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/force-ask.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/force-ask.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/force-gather.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/force-gather.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/formatting.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/formatting.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-dict-object.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-dict-object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-dict-value.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-dict-value.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-dict.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-dict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit-at-least-two.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit-at-least-two.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit-gather.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit-gather.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit-number.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit-number.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-fruit.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-fruit.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-set-object.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-set-object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/gather-set.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/gather-set.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/generic-object.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/generic-object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/get-default-timezone.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/get-default-timezone.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/help-damages-audio.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/help-damages-audio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/help.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/help.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/hideif-boolean.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/hideif-boolean.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/html.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/html.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/image-sets.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/image-sets.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/images.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/images.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/imports.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/imports.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/include.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/include.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/indefinite-article.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/indefinite-article.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/initial.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/initial.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interface.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interface.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interview-help.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interview-help.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interview-url.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interview-url.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/interview_url_action.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/interview_url_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/js_action_call.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/js_action_call.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/js_url_action.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/js_url_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/js_variables.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/js_variables.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/label.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/label.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/language.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/language.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/language_from_browser.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/language_from_browser.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/language_from_browser_restricted.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/language_from_browser_restricted.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/lists.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/lists.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/loading-legal.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/loading-legal.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/loading-util.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/loading-util.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/madlibs.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/madlibs.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-01.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-01.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-02.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-02.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-03.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-03.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-04.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-04.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-05.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-05.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-06.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-06.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-07.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-07.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mako-09.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mako-09.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mandatory.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mandatory.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/markdown.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/markdown.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/menu-item.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/menu-item.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/message.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/message.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/metadata.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/metadata.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/min.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/min.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/minlength.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/minlength.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-classify.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-classify.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-datatype.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-datatype.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-export-yaml.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-export-yaml.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-predict.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-predict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ml-save-and-predict.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ml-save-and-predict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/mlarea-datatype.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/mlarea-datatype.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/modules.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/modules.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/money-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/money-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/need.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/need.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/nested-loop.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/nested-loop.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/nice-number.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/nice-number.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/no-label-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/no-label-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/note.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/note.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/noun-plural.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/noun-plural.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/noyes.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/noyes.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/number-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/number-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-checkboxes.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-checkboxes.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-disable-others.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-disable-others.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-radio.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-radio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object-selections.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object-selections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/object.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/objects.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/objects.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ocr-chord.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ocr-chord.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ocr.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ocr.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/optional-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/optional-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/ordinal-number.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/ordinal-number.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/other.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/other.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/page-numbers.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/page-numbers.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/password-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/password-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/past-tense.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/past-tense.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-a.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-a.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-fill-code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-fill-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-fill-signature.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-fill-signature.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pdf-fill.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pdf-fill.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/periodic-amount.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/periodic-amount.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/periodic-value.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/periodic-value.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/prevent-back.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/prevent-back.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/prevent-going-back.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/prevent-going-back.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/progress-features.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/progress-features.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/progress.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/progress.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pull-down-with-code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pull-down-with-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/pull-down.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/pull-down.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/qr-code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/qr-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/quantity-noun.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/quantity-noun.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/quote_paragraphs.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/quote_paragraphs.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/radio-list.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/radio-list.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/range.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/range.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/reconsider.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/reconsider.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/redis.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/redis.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/refresh.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/refresh.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/reload.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/reload.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/required-code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/required-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/reset.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/reset.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/response-json.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/response-json.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/response-svg.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/response-svg.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/response.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/response.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/resume-button-label.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/resume-button-label.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/review.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/review.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/salutation.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/salutation.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/save-url-to-file.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/save-url-to-file.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/script.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/script.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-code.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-get-sections.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-get-sections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-review.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-review.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords-set-sections.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords-set-sections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections-keywords.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections-keywords.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/sections.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/sections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/send-email.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/send-email.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/set-language.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/set-language.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/showif-boolean.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/showif-boolean.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/showif.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/showif.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/shuffle.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/shuffle.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/signature.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/signature.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/signin.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/signin.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/single-spacing.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/single-spacing.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/space-underscore.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/space-underscore.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/state.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/state.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/static_image.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/static_image.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/subdivision-type.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/subdivision-type.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/table-mako.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/table-mako.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/table-markdown.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/table-markdown.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/table.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/table.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/target-template.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/target-template.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/template-file.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/template-file.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/template-subject.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/template-subject.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/template.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/template.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/terms.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/terms.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-box-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-box-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-default.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-default.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-field.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-help.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-help.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/text-hint.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/text-hint.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/timezone-list.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/timezone-list.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/title-case.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/title-case.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/today.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/today.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/under.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/under.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/upload-multiple.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/upload-multiple.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/upload.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/upload.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/url-of.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/url-of.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/valid-formats.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/valid-formats.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/value.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/value.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/variables_as_json.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/variables_as_json.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/video.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/video.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/yesno-custom.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/yesno-custom.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/yesno.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/yesno.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/examples/yesnomaybe.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/examples/yesnomaybe.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/all.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/all.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/all.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/all.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/brands.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/brands.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/brands.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/brands.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/conflict-detection.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/conflict-detection.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/fontawesome.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/fontawesome.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/regular.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/regular.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/regular.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/regular.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/solid.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/solid.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/solid.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/v4-shims.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/v4-shims.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/fontawesome/js/v4-shims.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/fontawesome/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/img/loading-sm.gif` & `docassemble.webapp-1.4.9/docassemble/webapp/static/img/loading-sm.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/img/loading.gif` & `docassemble.webapp-1.4.9/docassemble/webapp/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/index.html` & `docassemble.webapp-1.4.9/docassemble/webapp/static/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css` & `docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/office/cat-in-circle-32.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/office/cat-in-circle-32.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/office/cat-in-circle-80.png` & `docassemble.webapp-1.4.9/docassemble/webapp/static/office/cat-in-circle-80.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/office/officeinner.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/office/officeinner.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/office/polyfill.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/office/polyfill.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/office/word.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/office/word.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/README.md` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-off.mp3` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-off.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-off.ogg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-off.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-on.mp3` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-on.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click-on.ogg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click-on.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click.mp3` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-click.ogg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-click.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-snap.mp3` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-snap.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-snap.ogg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-snap.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-stapler.mp3` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-stapler.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/sounds/notification-stapler.ogg` & `docassemble.webapp-1.4.9/docassemble/webapp/static/sounds/notification-stapler.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/static/yamlmixed/yamlmixed.js` & `docassemble.webapp-1.4.9/docassemble/webapp/static/yamlmixed/yamlmixed.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/telnyx.py` & `docassemble.webapp-1.4.9/docassemble/webapp/telnyx.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/base.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/flask_two_col_base.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/flask_two_col_base.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/base_templates/form_macros.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/base_templates/form_macros.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/_macros.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/_macros.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/change_password.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/change_password.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/emails/registered_message.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/emails/registered_message.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/forgot_password.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/forgot_password.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/google_login.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/google_login.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/invite.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/invite.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/login.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/login.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/login_or_register.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/login_or_register.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/manage_emails.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/manage_emails.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_choose.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_choose.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_reconfigure.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_reconfigure.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/mfa_setup.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/mfa_setup.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/register.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/register.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/reset_password.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/reset_password.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/flask_user/user_profile.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/flask_user/user_profile.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/404.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/404.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/501.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/501.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/admin_page.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/admin_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/config.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/config.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/create_playground_package.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/create_playground_package.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/gd_sync_wait.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/gd_sync_wait.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/github.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/github.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/googledrive.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/googledrive.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/home_page.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/home_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/interviews.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/interviews.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/logs.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/logs.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_account.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_account.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_api.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_api.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_playgrounds.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_playgrounds.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/manage_projects.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/manage_projects.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/member_page.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/member_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/monitor.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/monitor.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/od_sync_wait.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/od_sync_wait.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officeaddin.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officeaddin.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officefunctionfile.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officefunctionfile.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officemanifest.xml` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officemanifest.xml`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/officeouter.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/officeouter.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/onedrive.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/onedrive.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/packages.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/packages.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/playground.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/playground.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/playgroundfiles.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/playgroundfiles.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/playgroundpackages.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/playgroundpackages.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/pull_playground_package.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/pull_playground_package.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/rename_project.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/rename_project.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/start.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/start.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/test_embed.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/test_embed.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/train.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/train.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/update_package.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/update_package.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/update_package_wait.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/update_package_wait.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/utilities.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/utilities.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/pages/webrtc.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/pages/webrtc.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/users/add_user_page.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/users/add_user_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/users/edit_user_profile_page.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/users/edit_user_profile_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/users/request_developer.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/users/request_developer.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/users/rolelist.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/users/rolelist.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/users/user_profile_page.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/users/user_profile_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/templates/users/userlist.html` & `docassemble.webapp-1.4.9/docassemble/webapp/templates/users/userlist.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/translations.py` & `docassemble.webapp-1.4.9/docassemble/webapp/translations.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/update.py` & `docassemble.webapp-1.4.9/docassemble/webapp/update.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/user_database.py` & `docassemble.webapp-1.4.9/docassemble/webapp/user_database.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/users/forms.py` & `docassemble.webapp-1.4.9/docassemble/webapp/users/forms.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/users/models.py` & `docassemble.webapp-1.4.9/docassemble/webapp/users/models.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/users/views.py` & `docassemble.webapp-1.4.9/docassemble/webapp/users/views.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/watchdog.py` & `docassemble.webapp-1.4.9/docassemble/webapp/watchdog.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/worker.py` & `docassemble.webapp-1.4.9/docassemble/webapp/worker.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble/webapp/wsgi_restart.py` & `docassemble.webapp-1.4.9/docassemble/webapp/wsgi_restart.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.8/docassemble.webapp.egg-info/PKG-INFO` & `docassemble.webapp-1.4.9/docassemble.webapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.webapp
-Version: 1.4.8
+Version: 1.4.9
 Summary: The web application components of the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Description: See the [docassemble web site] for a description of **docassemble**
         and installation instructions.
```

### Comparing `docassemble.webapp-1.4.8/docassemble.webapp.egg-info/SOURCES.txt` & `docassemble.webapp-1.4.9/docassemble.webapp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py
 docassemble/webapp/alembic/versions/77e8971ffcbf_first_alembic_revision.py
 docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py
 docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py
 docassemble/webapp/alembic/versions/c2ef4831ef76_user_last_login.py
 docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py
 docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py
+docassemble/webapp/alembic/versions/fd1547c94c46_add_a_column_for_the_voicerss_voice.py
 docassemble/webapp/core/__init__.py
 docassemble/webapp/core/models.py
 docassemble/webapp/data/VERSION.txt
 docassemble/webapp/data/db-schema.txt
 docassemble/webapp/data/questions/wizard-template.yml
 docassemble/webapp/data/static/robots.txt
 docassemble/webapp/data/static/test-document.docx
```

### Comparing `docassemble.webapp-1.4.8/docassemble.webapp.egg-info/requires.txt` & `docassemble.webapp-1.4.9/docassemble.webapp.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -76,17 +76,17 @@
 cryptography==36.0.2
 cssselect2==0.5.0
 da-pkg-resources==0.0.1
 defusedxml==0.7.1
 dnspython==2.2.1
 docassemble-backports==1.0
 docassemble-textstat==0.7.2
-docassemble.base==1.4.8
-docassemble.demo==1.4.8
-docassemble==1.4.8
+docassemble.base==1.4.9
+docassemble.demo==1.4.9
+docassemble==1.4.9
 docassemblekvsession==0.7
 docopt==0.6.2
 docutils==0.18.1
 docxcompose==1.3.4
 docxtpl==0.16.3
 email-validator==1.1.3
 et-xmlfile==1.1.0
```

### Comparing `docassemble.webapp-1.4.8/setup.py` & `docassemble.webapp-1.4.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
 
 setup_requires = [
     'enum34==1.1.10'
     ]
 install_requires = [
-    'docassemble==1.4.8',
-    'docassemble.base==1.4.8',
-    'docassemble.demo==1.4.8',
+    'docassemble==1.4.9',
+    'docassemble.base==1.4.9',
+    'docassemble.demo==1.4.9',
     "3to2==1.1.1",
     "airtable-python-wrapper==0.15.3",
     "alembic==1.7.7",
     "amqp==5.1.0",
     "asn1crypto==1.5.1",
     "astunparse==1.6.3",
     "async-generator==1.10",
@@ -270,15 +270,15 @@
 
 if sys.version_info < (3, 9):
     install_requires.append("backports.zoneinfo==0.2.1")
 else:
     install_requires.append("docassemble-backports==1.0")
 
 setup(name='docassemble.webapp',
-      version='1.4.8',
+      version='1.4.9',
       python_requires='>=3.8',
       description=('The web application components of the docassemble system.'),
       long_description=read("README.md"),
       long_description_content_type='text/markdown',
       author='Jonathan Pyle',
       author_email='jhpyle@gmail.com',
       license='MIT',
```

