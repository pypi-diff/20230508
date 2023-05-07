# Comparing `tmp/faker-file-0.9.2.tar.gz` & `tmp/faker-file-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker-file-0.9.2.tar", last modified: Fri Dec 23 00:11:34 2022, max compression
+gzip compressed data, was "faker-file-0.9.3.tar", last modified: Tue Jan  3 21:34:18 2023, max compression
```

## Comparing `faker-file-0.9.2.tar` & `faker-file-0.9.3.tar`

### file list

```diff
@@ -1,206 +1,207 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.088732 faker-file-0.9.2/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      302 2022-12-18 20:21:28.000000 faker-file-0.9.2/.coveragerc
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-17 15:38:13.000000 faker-file-0.9.2/.coveralls.yml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      108 2022-12-17 15:38:13.000000 faker-file-0.9.2/.dockerignore
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 faker-file-0.9.2/.env
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.072731 faker-file-0.9.2/.github/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/.github/workflows/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1743 2022-12-22 23:26:40.000000 faker-file-0.9.2/.github/workflows/test.yml
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      468 2022-12-22 19:52:01.000000 faker-file-0.9.2/.gitignore
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      375 2022-12-17 15:38:13.000000 faker-file-0.9.2/.matyan.ini
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3687 2022-12-22 23:58:13.000000 faker-file-0.9.2/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      478 2022-12-17 15:38:13.000000 faker-file-0.9.2/Dockerfile
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2022-12-17 15:38:13.000000 faker-file-0.9.2/LICENSE.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2022-12-17 15:38:13.000000 faker-file-0.9.2/MANIFEST.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     9849 2022-12-23 00:11:34.088732 faker-file-0.9.2/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     8668 2022-12-22 20:58:22.000000 faker-file-0.9.2/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/docs/
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      634 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/Makefile
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/changelog.rst
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10555 2022-12-22 20:42:26.000000 faker-file-0.9.2/docs/conf.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10548 2022-12-22 20:40:51.000000 faker-file-0.9.2/docs/conf.py.distrib
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      179 2022-12-18 20:57:05.000000 faker-file-0.9.2/docs/documentation.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      675 2022-12-18 20:21:28.000000 faker-file-0.9.2/docs/faker_file.providers.mixins.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3051 2022-12-18 20:21:28.000000 faker-file-0.9.2/docs/faker_file.providers.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      734 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/faker_file.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1313 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/faker_file.storages.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      780 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/faker_file.tests.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/index.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/index.rst.distrib
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      800 2022-12-17 15:38:13.000000 faker-file-0.9.2/docs/make.bat
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      155 2022-12-18 20:57:10.000000 faker-file-0.9.2/docs/package.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6622 2022-12-22 21:02:12.000000 faker-file-0.9.2/docs/quick_start.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    14589 2022-12-22 19:52:01.000000 faker-file-0.9.2/docs/recipes.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/examples/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/__init__.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/examples/django_example/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      146 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/README.rst
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/__init__.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/examples/django_example/factories/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/factories/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3604 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/django_example/factories/upload_upload.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      250 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/manage.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/examples/django_example/project/
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/__init__.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/examples/django_example/project/settings/
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       19 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/settings/__init__.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4563 2022-12-22 20:38:43.000000 faker-file-0.9.2/examples/django_example/project/settings/base.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      293 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/settings/core.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       20 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/settings/dev.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       19 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/settings/docs.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/settings/local_settings.example
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       20 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/settings/testing.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      496 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/urls.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      390 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/project/wsgi.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/examples/django_example/upload/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/upload/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      259 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/upload/admin.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.076731 faker-file-0.9.2/examples/django_example/upload/migrations/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      932 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/upload/migrations/0001_initial.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/upload/migrations/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      414 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/django_example/upload/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.080731 faker-file-0.9.2/examples/requirements/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       71 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/requirements/common.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3476 2022-12-22 23:21:21.000000 faker-file-0.9.2/examples/requirements/common.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/requirements/debug.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1156 2022-12-22 23:21:23.000000 faker-file-0.9.2/examples/requirements/debug.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        6 2022-12-20 19:55:33.000000 faker-file-0.9.2/examples/requirements/deployment.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1328 2022-12-22 23:21:26.000000 faker-file-0.9.2/examples/requirements/deployment.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/requirements/dev.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5784 2022-12-22 23:21:35.000000 faker-file-0.9.2/examples/requirements/dev.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-20 19:55:33.000000 faker-file-0.9.2/examples/requirements/django_2_2.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4880 2022-12-22 23:21:57.000000 faker-file-0.9.2/examples/requirements/django_2_2.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:03.000000 faker-file-0.9.2/examples/requirements/django_2_2_and_flask.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6116 2022-12-22 23:22:56.000000 faker-file-0.9.2/examples/requirements/django_2_2_and_flask.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-20 19:55:33.000000 faker-file-0.9.2/examples/requirements/django_3_0.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4914 2022-12-22 23:22:06.000000 faker-file-0.9.2/examples/requirements/django_3_0.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:21.000000 faker-file-0.9.2/examples/requirements/django_3_0_and_flask.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6150 2022-12-22 23:23:08.000000 faker-file-0.9.2/examples/requirements/django_3_0_and_flask.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-20 19:55:33.000000 faker-file-0.9.2/examples/requirements/django_3_1.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4914 2022-12-22 23:22:15.000000 faker-file-0.9.2/examples/requirements/django_3_1.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:38.000000 faker-file-0.9.2/examples/requirements/django_3_1_and_flask.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6150 2022-12-22 23:23:21.000000 faker-file-0.9.2/examples/requirements/django_3_1_and_flask.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2022-12-20 19:55:33.000000 faker-file-0.9.2/examples/requirements/django_3_2.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4914 2022-12-22 23:22:24.000000 faker-file-0.9.2/examples/requirements/django_3_2.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:50.000000 faker-file-0.9.2/examples/requirements/django_3_2_and_flask.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6150 2022-12-22 23:23:32.000000 faker-file-0.9.2/examples/requirements/django_3_2_and_flask.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2022-12-20 19:55:33.000000 faker-file-0.9.2/examples/requirements/django_4_0.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4883 2022-12-22 23:22:36.000000 faker-file-0.9.2/examples/requirements/django_4_0.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:14:04.000000 faker-file-0.9.2/examples/requirements/django_4_0_and_flask.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6126 2022-12-22 23:23:44.000000 faker-file-0.9.2/examples/requirements/django_4_0_and_flask.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2022-12-20 19:55:33.000000 faker-file-0.9.2/examples/requirements/django_4_1.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4883 2022-12-22 23:22:45.000000 faker-file-0.9.2/examples/requirements/django_4_1.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:14:16.000000 faker-file-0.9.2/examples/requirements/django_4_1_and_flask.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6126 2022-12-22 23:23:58.000000 faker-file-0.9.2/examples/requirements/django_4_1_and_flask.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       63 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/requirements/docs.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6079 2022-12-22 23:24:10.000000 faker-file-0.9.2/examples/requirements/docs.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      412 2022-12-22 23:17:12.000000 faker-file-0.9.2/examples/requirements/flask.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5735 2022-12-22 23:21:46.000000 faker-file-0.9.2/examples/requirements/flask.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       77 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/requirements/style_checkers.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1822 2022-12-22 23:24:18.000000 faker-file-0.9.2/examples/requirements/style_checkers.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      112 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/requirements/test.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1577 2022-12-22 23:24:22.000000 faker-file-0.9.2/examples/requirements/test.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/requirements/testing.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4911 2022-12-22 23:24:33.000000 faker-file-0.9.2/examples/requirements/testing.txt
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.080731 faker-file-0.9.2/examples/sqlalchemy_example/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      470 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.080731 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1020 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/__init__.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.080731 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       38 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/README
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2016 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/env.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      494 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/script.py.mako
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.080731 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/versions/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      621 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/versions/2695cb77cdf2_create_product_table.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2173 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic.ini
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      386 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/config.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      362 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/config_test.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      156 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/data.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1305 2022-12-22 20:37:06.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/main.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      423 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.080731 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/static/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1150 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/static/favicon.ico
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.080731 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/templates/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.084731 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/templates/admin/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      766 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/templates/admin/index.html
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      539 2022-12-17 15:38:13.000000 faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/templates/tree_list.html
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      101 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/sqlalchemy_example/run_server.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.084731 faker-file-0.9.2/examples/sqlalchemy_example/sqlalchemy_factories/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       39 2022-12-22 19:52:01.000000 faker-file-0.9.2/examples/sqlalchemy_example/sqlalchemy_factories/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3062 2022-12-22 20:20:39.000000 faker-file-0.9.2/examples/sqlalchemy_example/sqlalchemy_factories/faker_file_admin_upload.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      191 2022-12-17 15:38:13.000000 faker-file-0.9.2/mypy.ini
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1776 2022-12-17 15:38:13.000000 faker-file-0.9.2/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      484 2022-12-17 15:38:13.000000 faker-file-0.9.2/pytest.ini
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.084731 faker-file-0.9.2/scripts/
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       90 2022-12-22 19:52:01.000000 faker-file-0.9.2/scripts/alembic_migrate.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/black.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      121 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/build_docs.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      109 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/check_release.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      382 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/clean_up.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1677 2022-12-22 21:16:31.000000 faker-file-0.9.2/scripts/compile_requirements.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       66 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/doc8.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       69 2022-12-22 19:52:01.000000 faker-file-0.9.2/scripts/flask_runserver.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      314 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/install.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       49 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/isort.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      253 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/make_migrations.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      110 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/make_release.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       73 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/migrate.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      286 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/rebuild_docs.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      105 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/runserver.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       88 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/shell.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       60 2022-12-22 19:58:36.000000 faker-file-0.9.2/scripts/sqlalchemy_shell.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/test_tests.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      139 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/uninstall.sh
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      487 2022-12-17 15:38:13.000000 faker-file-0.9.2/scripts/upgrade_requirements.sh
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      198 2022-12-23 00:11:34.088732 faker-file-0.9.2/setup.cfg
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2600 2022-12-22 20:57:36.000000 faker-file-0.9.2/setup.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.072731 faker-file-0.9.2/src/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.084731 faker-file-0.9.2/src/faker_file/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      168 2022-12-22 20:57:24.000000 faker-file-0.9.2/src/faker_file/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1454 2022-12-17 18:36:47.000000 faker-file-0.9.2/src/faker_file/base.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      418 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/constants.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      417 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/helpers.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.084731 faker-file-0.9.2/src/faker_file/providers/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2687 2022-12-17 17:06:01.000000 faker-file-0.9.2/src/faker_file/providers/bin_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3879 2022-12-17 17:06:01.000000 faker-file-0.9.2/src/faker_file/providers/csv_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3032 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/docx_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2455 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/ico_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2462 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/jpeg_file.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.084731 faker-file-0.9.2/src/faker_file/providers/mixins/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/mixins/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2197 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/mixins/image_mixin.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2790 2022-12-17 17:06:01.000000 faker-file-0.9.2/src/faker_file/providers/mixins/tablular_data_mixin.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3146 2022-12-17 17:06:01.000000 faker-file-0.9.2/src/faker_file/providers/ods_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3217 2022-12-17 18:02:49.000000 faker-file-0.9.2/src/faker_file/providers/pdf_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2454 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/png_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3265 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/pptx_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2558 2022-12-18 20:30:31.000000 faker-file-0.9.2/src/faker_file/providers/random_file_from_dir.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2839 2022-12-22 20:55:49.000000 faker-file-0.9.2/src/faker_file/providers/rtf_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2455 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/svg_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2839 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/txt_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2465 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/providers/webp_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3162 2022-12-17 17:06:01.000000 faker-file-0.9.2/src/faker_file/providers/xlsx_file.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    15404 2022-12-22 20:50:01.000000 faker-file-0.9.2/src/faker_file/providers/zip_file.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.088732 faker-file-0.9.2/src/faker_file/storages/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/storages/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      904 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/storages/aws_s3.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      966 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/storages/azure_cloud_storage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1456 2022-12-18 20:21:28.000000 faker-file-0.9.2/src/faker_file/storages/base.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3681 2022-12-20 19:55:33.000000 faker-file-0.9.2/src/faker_file/storages/cloud.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2914 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/storages/filesystem.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1097 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/storages/google_cloud_storage.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.088732 faker-file-0.9.2/src/faker_file/tests/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.2/src/faker_file/tests/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1902 2022-12-22 19:52:01.000000 faker-file-0.9.2/src/faker_file/tests/test_django_integration.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    16972 2022-12-22 23:50:22.000000 faker-file-0.9.2/src/faker_file/tests/test_providers.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1735 2022-12-22 23:43:45.000000 faker-file-0.9.2/src/faker_file/tests/test_sqlalchemy_integration.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6308 2022-12-20 19:55:33.000000 faker-file-0.9.2/src/faker_file/tests/test_storages.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-23 00:11:34.084731 faker-file-0.9.2/src/faker_file.egg-info/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     9849 2022-12-23 00:11:34.000000 faker-file-0.9.2/src/faker_file.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6230 2022-12-23 00:11:34.000000 faker-file-0.9.2/src/faker_file.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2022-12-23 00:11:34.000000 faker-file-0.9.2/src/faker_file.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        6 2022-12-23 00:11:34.000000 faker-file-0.9.2/src/faker_file.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2022-12-23 00:11:34.000000 faker-file-0.9.2/src/faker_file.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       76 2022-12-17 15:38:13.000000 faker-file-0.9.2/tests.coveragerc
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      837 2022-12-22 23:37:12.000000 faker-file-0.9.2/tox.ini
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.121863 faker-file-0.9.3/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      302 2022-12-18 20:21:28.000000 faker-file-0.9.3/.coveragerc
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-17 15:38:13.000000 faker-file-0.9.3/.coveralls.yml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      108 2022-12-17 15:38:13.000000 faker-file-0.9.3/.dockerignore
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 faker-file-0.9.3/.env
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.097862 faker-file-0.9.3/.github/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.101862 faker-file-0.9.3/.github/workflows/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4425 2022-12-27 21:29:13.000000 faker-file-0.9.3/.github/workflows/test.yml
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      475 2022-12-27 21:29:13.000000 faker-file-0.9.3/.gitignore
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      375 2022-12-17 15:38:13.000000 faker-file-0.9.3/.matyan.ini
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3749 2023-01-03 01:28:04.000000 faker-file-0.9.3/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      478 2022-12-17 15:38:13.000000 faker-file-0.9.3/Dockerfile
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2022-12-17 15:38:13.000000 faker-file-0.9.3/LICENSE.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2022-12-17 15:38:13.000000 faker-file-0.9.3/MANIFEST.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10084 2023-01-03 21:34:18.121863 faker-file-0.9.3/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     8900 2023-01-03 21:07:46.000000 faker-file-0.9.3/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/docs/
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      634 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/Makefile
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/changelog.rst
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10555 2022-12-22 20:42:26.000000 faker-file-0.9.3/docs/conf.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10548 2022-12-22 20:40:51.000000 faker-file-0.9.3/docs/conf.py.distrib
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      179 2022-12-18 20:57:05.000000 faker-file-0.9.3/docs/documentation.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      675 2022-12-18 20:21:28.000000 faker-file-0.9.3/docs/faker_file.providers.mixins.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3051 2022-12-18 20:21:28.000000 faker-file-0.9.3/docs/faker_file.providers.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      734 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/faker_file.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1313 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/faker_file.storages.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      780 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/faker_file.tests.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/index.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/index.rst.distrib
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      800 2022-12-17 15:38:13.000000 faker-file-0.9.3/docs/make.bat
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      155 2022-12-18 20:57:10.000000 faker-file-0.9.3/docs/package.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6866 2023-01-03 21:07:05.000000 faker-file-0.9.3/docs/quick_start.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    14589 2022-12-22 19:52:01.000000 faker-file-0.9.3/docs/recipes.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/examples/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/__init__.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/examples/django_example/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      146 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/README.rst
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/__init__.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/examples/django_example/factories/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       37 2022-12-23 21:13:23.000000 faker-file-0.9.3/examples/django_example/factories/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3604 2022-12-22 19:52:01.000000 faker-file-0.9.3/examples/django_example/factories/upload_upload.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      250 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/manage.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/examples/django_example/project/
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/project/__init__.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/examples/django_example/project/settings/
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       27 2022-12-23 21:13:38.000000 faker-file-0.9.3/examples/django_example/project/settings/__init__.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4571 2022-12-23 21:13:56.000000 faker-file-0.9.3/examples/django_example/project/settings/base.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      293 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/project/settings/core.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-23 21:14:08.000000 faker-file-0.9.3/examples/django_example/project/settings/dev.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       27 2022-12-23 21:14:17.000000 faker-file-0.9.3/examples/django_example/project/settings/docs.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/project/settings/local_settings.example
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-23 21:14:24.000000 faker-file-0.9.3/examples/django_example/project/settings/testing.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      496 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/project/urls.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      390 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/project/wsgi.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/examples/django_example/upload/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/upload/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      259 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/upload/admin.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.105862 faker-file-0.9.3/examples/django_example/upload/migrations/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      932 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/upload/migrations/0001_initial.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/upload/migrations/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      414 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/django_example/upload/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.109862 faker-file-0.9.3/examples/requirements/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       80 2023-01-03 01:15:34.000000 faker-file-0.9.3/examples/requirements/common.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3705 2023-01-03 01:15:43.000000 faker-file-0.9.3/examples/requirements/common.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/requirements/debug.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1132 2023-01-03 01:15:44.000000 faker-file-0.9.3/examples/requirements/debug.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        6 2022-12-20 19:55:33.000000 faker-file-0.9.3/examples/requirements/deployment.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1304 2023-01-03 01:15:45.000000 faker-file-0.9.3/examples/requirements/deployment.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/requirements/dev.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6038 2023-01-03 01:15:46.000000 faker-file-0.9.3/examples/requirements/dev.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-20 19:55:33.000000 faker-file-0.9.3/examples/requirements/django_2_2.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5134 2023-01-03 01:15:49.000000 faker-file-0.9.3/examples/requirements/django_2_2.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:03.000000 faker-file-0.9.3/examples/requirements/django_2_2_and_flask.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6319 2023-01-03 01:15:58.000000 faker-file-0.9.3/examples/requirements/django_2_2_and_flask.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-20 19:55:33.000000 faker-file-0.9.3/examples/requirements/django_3_0.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5168 2023-01-03 01:15:51.000000 faker-file-0.9.3/examples/requirements/django_3_0.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:21.000000 faker-file-0.9.3/examples/requirements/django_3_0_and_flask.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6353 2023-01-03 01:16:00.000000 faker-file-0.9.3/examples/requirements/django_3_0_and_flask.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2022-12-20 19:55:33.000000 faker-file-0.9.3/examples/requirements/django_3_1.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5168 2023-01-03 01:15:52.000000 faker-file-0.9.3/examples/requirements/django_3_1.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:38.000000 faker-file-0.9.3/examples/requirements/django_3_1_and_flask.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6353 2023-01-03 01:16:01.000000 faker-file-0.9.3/examples/requirements/django_3_1_and_flask.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2022-12-20 19:55:33.000000 faker-file-0.9.3/examples/requirements/django_3_2.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5168 2023-01-03 01:15:54.000000 faker-file-0.9.3/examples/requirements/django_3_2.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:13:50.000000 faker-file-0.9.3/examples/requirements/django_3_2_and_flask.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6353 2023-01-03 01:16:03.000000 faker-file-0.9.3/examples/requirements/django_3_2_and_flask.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2022-12-20 19:55:33.000000 faker-file-0.9.3/examples/requirements/django_4_0.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5137 2023-01-03 01:15:55.000000 faker-file-0.9.3/examples/requirements/django_4_0.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:14:04.000000 faker-file-0.9.3/examples/requirements/django_4_0_and_flask.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6329 2023-01-03 01:16:04.000000 faker-file-0.9.3/examples/requirements/django_4_0_and_flask.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2022-12-20 19:55:33.000000 faker-file-0.9.3/examples/requirements/django_4_1.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5137 2023-01-03 01:15:57.000000 faker-file-0.9.3/examples/requirements/django_4_1.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-22 21:14:16.000000 faker-file-0.9.3/examples/requirements/django_4_1_and_flask.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6329 2023-01-03 01:16:05.000000 faker-file-0.9.3/examples/requirements/django_4_1_and_flask.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       63 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/requirements/docs.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6274 2023-01-03 01:16:08.000000 faker-file-0.9.3/examples/requirements/docs.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      412 2022-12-22 23:17:12.000000 faker-file-0.9.3/examples/requirements/flask.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5938 2023-01-03 01:15:48.000000 faker-file-0.9.3/examples/requirements/flask.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       77 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/requirements/style_checkers.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1798 2023-01-03 01:16:09.000000 faker-file-0.9.3/examples/requirements/style_checkers.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      112 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/requirements/test.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1553 2023-01-03 01:16:10.000000 faker-file-0.9.3/examples/requirements/test.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/requirements/testing.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5165 2023-01-03 01:16:11.000000 faker-file-0.9.3/examples/requirements/testing.txt
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      470 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/sqlalchemy_example/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1028 2022-12-23 21:15:45.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/__init__.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       39 2022-12-23 21:23:25.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/README
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2016 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/env.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      494 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/script.py.mako
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/versions/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      620 2022-12-23 21:22:15.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/versions/2695cb77cdf2_create_product_table.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2173 2022-12-22 19:52:01.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic.ini
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      386 2022-12-22 19:52:01.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/config.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      362 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/config_test.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      156 2022-12-22 19:52:01.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/data.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1305 2022-12-22 20:37:06.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/main.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      423 2022-12-22 19:52:01.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/static/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1150 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/static/favicon.ico
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/templates/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/templates/admin/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      766 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/templates/admin/index.html
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      539 2022-12-17 15:38:13.000000 faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/templates/tree_list.html
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      101 2022-12-22 19:52:01.000000 faker-file-0.9.3/examples/sqlalchemy_example/run_server.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.113862 faker-file-0.9.3/examples/sqlalchemy_example/sqlalchemy_factories/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       47 2022-12-23 21:16:09.000000 faker-file-0.9.3/examples/sqlalchemy_example/sqlalchemy_factories/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3062 2022-12-22 20:20:39.000000 faker-file-0.9.3/examples/sqlalchemy_example/sqlalchemy_factories/faker_file_admin_upload.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      191 2022-12-17 15:38:13.000000 faker-file-0.9.3/mypy.ini
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1729 2022-12-23 21:15:09.000000 faker-file-0.9.3/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      535 2022-12-23 20:40:25.000000 faker-file-0.9.3/pytest.ini
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.117862 faker-file-0.9.3/scripts/
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       90 2022-12-22 19:52:01.000000 faker-file-0.9.3/scripts/alembic_migrate.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       28 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/black.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      121 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/build_docs.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      109 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/check_release.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      382 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/clean_up.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1677 2022-12-22 21:16:31.000000 faker-file-0.9.3/scripts/compile_requirements.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       25 2022-12-27 21:29:13.000000 faker-file-0.9.3/scripts/doc8.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       69 2022-12-22 19:52:01.000000 faker-file-0.9.3/scripts/flask_runserver.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      314 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/install.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       49 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/isort.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      253 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/make_migrations.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      110 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/make_release.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       73 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/migrate.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      286 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/rebuild_docs.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      105 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/runserver.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       88 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/shell.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       60 2022-12-22 19:58:36.000000 faker-file-0.9.3/scripts/sqlalchemy_shell.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/test_tests.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      139 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/uninstall.sh
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      487 2022-12-17 15:38:13.000000 faker-file-0.9.3/scripts/upgrade_requirements.sh
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      329 2023-01-03 21:34:18.121863 faker-file-0.9.3/setup.cfg
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2683 2023-01-03 01:14:29.000000 faker-file-0.9.3/setup.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.101862 faker-file-0.9.3/src/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.117862 faker-file-0.9.3/src/faker_file/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      168 2023-01-03 01:27:44.000000 faker-file-0.9.3/src/faker_file/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1454 2022-12-17 18:36:47.000000 faker-file-0.9.3/src/faker_file/base.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      418 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/constants.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      417 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/helpers.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.121863 faker-file-0.9.3/src/faker_file/providers/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2687 2022-12-17 17:06:01.000000 faker-file-0.9.3/src/faker_file/providers/bin_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3879 2022-12-17 17:06:01.000000 faker-file-0.9.3/src/faker_file/providers/csv_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3032 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/docx_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3960 2023-01-03 21:29:17.000000 faker-file-0.9.3/src/faker_file/providers/epub_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2455 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/ico_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2462 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/jpeg_file.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.121863 faker-file-0.9.3/src/faker_file/providers/mixins/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/mixins/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2197 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/mixins/image_mixin.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2790 2022-12-17 17:06:01.000000 faker-file-0.9.3/src/faker_file/providers/mixins/tablular_data_mixin.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3146 2022-12-17 17:06:01.000000 faker-file-0.9.3/src/faker_file/providers/ods_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3217 2022-12-17 18:02:49.000000 faker-file-0.9.3/src/faker_file/providers/pdf_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2454 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/png_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3265 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/pptx_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2558 2022-12-18 20:30:31.000000 faker-file-0.9.3/src/faker_file/providers/random_file_from_dir.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2839 2022-12-22 20:55:49.000000 faker-file-0.9.3/src/faker_file/providers/rtf_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2455 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/svg_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2839 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/txt_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2465 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/providers/webp_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3162 2022-12-17 17:06:01.000000 faker-file-0.9.3/src/faker_file/providers/xlsx_file.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    16237 2023-01-03 21:12:06.000000 faker-file-0.9.3/src/faker_file/providers/zip_file.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.121863 faker-file-0.9.3/src/faker_file/storages/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/storages/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      904 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/storages/aws_s3.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      966 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/storages/azure_cloud_storage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1456 2022-12-18 20:21:28.000000 faker-file-0.9.3/src/faker_file/storages/base.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3681 2022-12-20 19:55:33.000000 faker-file-0.9.3/src/faker_file/storages/cloud.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2914 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/storages/filesystem.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1097 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/storages/google_cloud_storage.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.121863 faker-file-0.9.3/src/faker_file/tests/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2022-12-17 15:38:13.000000 faker-file-0.9.3/src/faker_file/tests/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1902 2022-12-22 19:52:01.000000 faker-file-0.9.3/src/faker_file/tests/test_django_integration.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    17907 2023-01-03 21:28:25.000000 faker-file-0.9.3/src/faker_file/tests/test_providers.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1657 2022-12-23 22:24:07.000000 faker-file-0.9.3/src/faker_file/tests/test_sqlalchemy_integration.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     7890 2022-12-27 21:29:13.000000 faker-file-0.9.3/src/faker_file/tests/test_storages.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-01-03 21:34:18.117862 faker-file-0.9.3/src/faker_file.egg-info/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10084 2023-01-03 21:34:18.000000 faker-file-0.9.3/src/faker_file.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6268 2023-01-03 21:34:18.000000 faker-file-0.9.3/src/faker_file.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-01-03 21:34:18.000000 faker-file-0.9.3/src/faker_file.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        6 2023-01-03 21:34:18.000000 faker-file-0.9.3/src/faker_file.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-01-03 21:34:18.000000 faker-file-0.9.3/src/faker_file.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       76 2022-12-17 15:38:13.000000 faker-file-0.9.3/tests.coveragerc
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      937 2022-12-23 22:20:50.000000 faker-file-0.9.3/tox.ini
```

### Comparing `faker-file-0.9.2/CHANGELOG.rst` & `faker-file-0.9.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.9.3
+-----
+2023-01-03
+
+- Add ``EpubFileProvider`` provider.
+
 0.9.2
 -----
 2022-12-23
 
 - Add ``RrfFileProvider``.
 - Added ``SQLAlchemy`` factory example.
```

### Comparing `faker-file-0.9.2/LICENSE.rst` & `faker-file-0.9.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/PKG-INFO` & `faker-file-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: faker-file
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generate fake files.
 Home-page: https://github.com/barseghyanartur/faker-file/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file/issues
 Project-URL: Documentation, https://faker-file.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/faker-file
 Project-URL: Changelog, https://faker-file.readthedocs.io/en/latest/changelog.html
 Keywords: faker,faker-file,files,testing,factories
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 ==========
 faker-file
 ==========
-**Generate fake files**
+**Generate files with fake data**
 
 .. image:: https://img.shields.io/pypi/v/faker-file.svg
    :target: https://pypi.python.org/pypi/faker-file
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/pyversions/faker-file.svg
     :target: https://pypi.python.org/pypi/faker-file/
@@ -58,18 +58,20 @@
 Prerequisites
 =============
 All of core dependencies of this package are `MIT` licensed.
 Most of optional dependencies of this package are `MIT` licensed, while
 a few are `BSD`- or `Apache 2` licensed. All licenses are mentioned
 below between the brackets.
 
-- Core package requires Python 3.7, 3.8, 3.9, 3.10 and 3.11.
+- Core package requires Python 3.7, 3.8, 3.9, 3.10 or 3.11.
+- ``Faker`` (`MIT`) is the only required dependency.
 - ``Django`` (`BSD`) integration with ``factory_boy`` (`MIT`) has
   been tested with ``Django`` 2.2, 3.0, 3.1, 3.2, 4.0 and 4.1.
 - ``DOCX`` file support requires ``python-docx`` (`MIT`).
+- ``EPUB`` file support requires ``xml2epub`` (`MIT`) and ``jinja2`` (`BSD`).
 - ``ICO``, ``JPEG``, ``PNG``, ``SVG`` and ``WEBP`` files support
   requires ``imgkit`` (`MIT`).
 - ``PDF`` file support requires ``pdfkit`` (`MIT`).
 - ``PPTX`` file support requires ``python-pptx`` (`MIT`).
 - ``ODS`` file support requires ``tablib`` (`MIT`) and ``odfpy`` (`Apache 2`).
 - ``XLSX`` file support requires ``tablib`` (`MIT`) and ``openpyxl`` (`MIT`).
 - ``PathyFileSystemStorage`` storage support requires ``pathy`` (`Apache 2`).
@@ -103,14 +105,20 @@
 
 **With DOCX support**
 
 .. code-block:: sh
 
     pip install faker-file[docx]
 
+**With EPUB support**
+
+.. code-block:: sh
+
+    pip install faker-file[epub]
+
 **With images support**
 
 .. code-block:: sh
 
     pip install faker-file[images]
 
 **With XLSX support**
@@ -136,14 +144,15 @@
 ========
 
 Supported file types
 --------------------
 - ``BIN``
 - ``CSV``
 - ``DOCX``
+- ``EPUB``
 - ``ICO``
 - ``JPEG``
 - ``ODS``
 - ``PDF``
 - ``PNG``
 - ``RTF``
 - ``PPTX``
@@ -200,16 +209,16 @@
     from django.db import models
 
     class Upload(models.Model):
 
         # ...
         file = models.FileField()
 
-upload/factory.py
-~~~~~~~~~~~~~~~~~
+upload/factories.py
+~~~~~~~~~~~~~~~~~~~
 Note, that when using ``faker-file`` with ``Django`` and native file system
 storages, you need to pass your ``MEDIA_ROOT`` setting as ``root_path`` value
 to the chosen file storage as show below.
 
 .. code-block:: python
 
     import factory
@@ -386,9 +395,7 @@
 For any security issues contact me at the e-mail given in the `Author`_ section.
 
 For overall issues, go to `GitHub <https://github.com/barseghyanartur/faker-file/issues>`_.
 
 Author
 ======
 Artur Barseghyan <artur.barseghyan@gmail.com>
-
-
```

### Comparing `faker-file-0.9.2/README.rst` & `faker-file-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ==========
 faker-file
 ==========
-**Generate fake files**
+**Generate files with fake data**
 
 .. image:: https://img.shields.io/pypi/v/faker-file.svg
    :target: https://pypi.python.org/pypi/faker-file
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/pyversions/faker-file.svg
     :target: https://pypi.python.org/pypi/faker-file/
@@ -30,18 +30,20 @@
 Prerequisites
 =============
 All of core dependencies of this package are `MIT` licensed.
 Most of optional dependencies of this package are `MIT` licensed, while
 a few are `BSD`- or `Apache 2` licensed. All licenses are mentioned
 below between the brackets.
 
-- Core package requires Python 3.7, 3.8, 3.9, 3.10 and 3.11.
+- Core package requires Python 3.7, 3.8, 3.9, 3.10 or 3.11.
+- ``Faker`` (`MIT`) is the only required dependency.
 - ``Django`` (`BSD`) integration with ``factory_boy`` (`MIT`) has
   been tested with ``Django`` 2.2, 3.0, 3.1, 3.2, 4.0 and 4.1.
 - ``DOCX`` file support requires ``python-docx`` (`MIT`).
+- ``EPUB`` file support requires ``xml2epub`` (`MIT`) and ``jinja2`` (`BSD`).
 - ``ICO``, ``JPEG``, ``PNG``, ``SVG`` and ``WEBP`` files support
   requires ``imgkit`` (`MIT`).
 - ``PDF`` file support requires ``pdfkit`` (`MIT`).
 - ``PPTX`` file support requires ``python-pptx`` (`MIT`).
 - ``ODS`` file support requires ``tablib`` (`MIT`) and ``odfpy`` (`Apache 2`).
 - ``XLSX`` file support requires ``tablib`` (`MIT`) and ``openpyxl`` (`MIT`).
 - ``PathyFileSystemStorage`` storage support requires ``pathy`` (`Apache 2`).
@@ -75,14 +77,20 @@
 
 **With DOCX support**
 
 .. code-block:: sh
 
     pip install faker-file[docx]
 
+**With EPUB support**
+
+.. code-block:: sh
+
+    pip install faker-file[epub]
+
 **With images support**
 
 .. code-block:: sh
 
     pip install faker-file[images]
 
 **With XLSX support**
@@ -108,14 +116,15 @@
 ========
 
 Supported file types
 --------------------
 - ``BIN``
 - ``CSV``
 - ``DOCX``
+- ``EPUB``
 - ``ICO``
 - ``JPEG``
 - ``ODS``
 - ``PDF``
 - ``PNG``
 - ``RTF``
 - ``PPTX``
@@ -172,16 +181,16 @@
     from django.db import models
 
     class Upload(models.Model):
 
         # ...
         file = models.FileField()
 
-upload/factory.py
-~~~~~~~~~~~~~~~~~
+upload/factories.py
+~~~~~~~~~~~~~~~~~~~
 Note, that when using ``faker-file`` with ``Django`` and native file system
 storages, you need to pass your ``MEDIA_ROOT`` setting as ``root_path`` value
 to the chosen file storage as show below.
 
 .. code-block:: python
 
     import factory
```

### Comparing `faker-file-0.9.2/docs/Makefile` & `faker-file-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/conf.py` & `faker-file-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/conf.py.distrib` & `faker-file-0.9.3/docs/conf.py.distrib`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/faker_file.providers.mixins.rst` & `faker-file-0.9.3/docs/faker_file.providers.mixins.rst`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/faker_file.providers.rst` & `faker-file-0.9.3/docs/faker_file.providers.rst`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/faker_file.rst` & `faker-file-0.9.3/docs/faker_file.rst`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/faker_file.storages.rst` & `faker-file-0.9.3/docs/faker_file.storages.rst`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/faker_file.tests.rst` & `faker-file-0.9.3/docs/faker_file.tests.rst`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/make.bat` & `faker-file-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/docs/quick_start.rst` & `faker-file-0.9.3/docs/quick_start.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 .. code-block:: python
 
     from faker import Faker
     from faker_file.providers.bin_file import BinFileProvider
     from faker_file.providers.csv_file import CsvFileProvider
     from faker_file.providers.docx_file import DocxFileProvider
+    from faker_file.providers.epub_file import EpubFileProvider
     from faker_file.providers.ico_file import IcoFileProvider
     from faker_file.providers.jpeg_file import JpegFileProvider
     from faker_file.providers.ods_file import OdsFileProvider
     from faker_file.providers.pdf_file import PdfFileProvider
     from faker_file.providers.png_file import PngFileProvider
     from faker_file.providers.pptx_file import PptxFileProvider
     from faker_file.providers.random_file_from_dir import RandomFileFromDirProvider
@@ -33,14 +34,15 @@
     from faker_file.providers.xlsx_file import XlsxFileProvider
     from faker_file.providers.zip_file import ZipFileProvider
 
     FAKER = Faker()
     FAKER.add_provider(BinFileProvider)
     FAKER.add_provider(CsvFileProvider)
     FAKER.add_provider(DocxFileProvider)
+    FAKER.add_provider(EpubFileProvider)
     FAKER.add_provider(IcoFileProvider)
     FAKER.add_provider(JpegFileProvider)
     FAKER.add_provider(OdsFileProvider)
     FAKER.add_provider(PdfFileProvider)
     FAKER.add_provider(PngFileProvider)
     FAKER.add_provider(PptxFileProvider)
     FAKER.add_provider(RandomFileFromDirProvider)
@@ -54,14 +56,15 @@
 **Usage examples**
 
 .. code-block:: python
 
     bin_file = FAKER.bin_file()
     csv_file = FAKER.csv_file()
     docx_file = FAKER.docx_file()
+    epub_file = FAKER.epub_file()
     ico_file = FAKER.ico_file()
     jpeg_file = FAKER.jpeg_file()
     ods_file = FAKER.ods_file()
     pdf_file = FAKER.pdf_file()
     png_file = FAKER.png_file()
     pptx_file = FAKER.pptx_file()
     rtf_file = FAKER.rtf_file()
@@ -77,14 +80,15 @@
 
 .. code-block:: python
 
     from factory import Faker
     from faker_file.providers.bin_file import BinFileProvider
     from faker_file.providers.csv_file import CsvFileProvider
     from faker_file.providers.docx_file import DocxFileProvider
+    from faker_file.providers.epub_file import EpubFileProvider
     from faker_file.providers.ico_file import IcoFileProvider
     from faker_file.providers.jpeg_file import JpegFileProvider
     from faker_file.providers.ods_file import OdsFileProvider
     from faker_file.providers.pdf_file import PdfFileProvider
     from faker_file.providers.png_file import PngFileProvider
     from faker_file.providers.pptx_file import PptxFileProvider
     from faker_file.providers.random_file_from_dir import RandomFileFromDirProvider
@@ -94,14 +98,15 @@
     from faker_file.providers.webp_file import WebpFileProvider
     from faker_file.providers.xlsx_file import XlsxFileProvider
     from faker_file.providers.zip_file import ZipFileProvider
 
     Faker.add_provider(BinFileProvider)
     Faker.add_provider(CsvFileProvider)
     Faker.add_provider(DocxFileProvider)
+    Faker.add_provider(EpubFileProvider)
     Faker.add_provider(IcoFileProvider)
     Faker.add_provider(JpegFileProvider)
     Faker.add_provider(OdsFileProvider)
     Faker.add_provider(PdfFileProvider)
     Faker.add_provider(PngFileProvider)
     Faker.add_provider(PptxFileProvider)
     Faker.add_provider(RandomFileFromDirProvider)
```

### Comparing `faker-file-0.9.2/docs/recipes.rst` & `faker-file-0.9.3/docs/recipes.rst`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/django_example/factories/upload_upload.py` & `faker-file-0.9.3/examples/django_example/factories/upload_upload.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/django_example/project/settings/base.py` & `faker-file-0.9.3/examples/django_example/project/settings/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,10 +168,10 @@
             "propagate": False,
         },
     },
 }
 
 # Do not put any settings below this line
 try:
-    from .local_settings import *
+    from .local_settings import *  # noqa
 except ImportError:
     pass
```

### Comparing `faker-file-0.9.2/examples/django_example/upload/migrations/0001_initial.py` & `faker-file-0.9.3/examples/django_example/upload/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/requirements/common.txt` & `faker-file-0.9.3/examples/requirements/common.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/common.in
+#    pip-compile examples/requirements/common.in
 #
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -65,22 +67,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -90,15 +97,17 @@
 packaging==22.0
     # via pytest
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 pluggy==1.0.0
     # via pytest
 protobuf==4.21.11
     # via
     #   google-api-core
     #   google-cloud-storage
     #   googleapis-common-protos
@@ -129,14 +138,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -147,27 +157,29 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 tablib==3.2.1
     # via -r examples/requirements/common.in
 tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
+    # via pytest
 typer==0.3.2
     # via
     #   pathy
     #   typer-cli
 typer-cli==0.0.12
     # via pathy
 typing-extensions==4.4.0
     # via azure-core
 urllib3==1.26.13
     # via
     #   botocore
     #   requests
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/requirements/debug.txt` & `faker-file-0.9.3/examples/requirements/debug.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/debug.in
+#    pip-compile examples/requirements/debug.in
 #
 asttokens==2.2.0
     # via stack-data
 backcall==0.2.0
     # via ipython
 decorator==5.1.1
     # via
```

### Comparing `faker-file-0.9.2/examples/requirements/deployment.txt` & `faker-file-0.9.3/examples/requirements/deployment.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/deployment.in
+#    pip-compile examples/requirements/deployment.in
 #
 bleach==5.0.1
     # via readme-renderer
 certifi==2022.9.24
     # via requests
 cffi==1.15.1
     # via cryptography
```

### Comparing `faker-file-0.9.2/examples/requirements/dev.txt` & `faker-file-0.9.3/examples/requirements/dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/dev.in
+#    pip-compile examples/requirements/dev.in
 #
 asgiref==3.5.2
     # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 bleach==5.0.1
     # via readme-renderer
 boto3==1.26.33
     # via pathy
 botocore==1.29.33
     # via
     #   boto3
@@ -106,24 +108,29 @@
     # via msrest
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 keyring==23.11.0
     # via twine
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 more-itertools==9.0.0
     # via jaraco-classes
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
@@ -139,15 +146,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 pkginfo==1.9.2
     # via twine
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -215,14 +224,15 @@
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
     #   requests-toolbelt
     #   twine
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==12.6.0
@@ -243,14 +253,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -278,9 +290,11 @@
     #   twine
 virtualenv==20.17.0
     # via tox
 webencodings==0.5.1
     # via bleach
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/django_2_2.txt` & `faker-file-0.9.3/examples/requirements/django_3_0.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_2_2.in
+#    pip-compile examples/requirements/django_3_0.in
 #
+asgiref==3.5.2
+    # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -38,23 +42,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==2.2.28
+django==3.0.14
     # via
-    #   -r examples/requirements/django_2_2.in
+    #   -r examples/requirements/django_3_0.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==3.0
-    # via -r examples/requirements/django_2_2.in
+django-debug-toolbar==2.2.1
+    # via -r examples/requirements/django_3_0.in
 django-storages==1.12.3
-    # via -r examples/requirements/django_2_2.in
+    # via -r examples/requirements/django_3_0.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -86,22 +90,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -115,15 +124,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -181,14 +192,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -200,14 +212,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -230,7 +244,9 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/requirements/django_2_2_and_flask.txt` & `faker-file-0.9.3/examples/requirements/django_3_2_and_flask.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_2_2_and_flask.in
+#    pip-compile examples/requirements/django_3_2_and_flask.in
 #
 alembic==1.9.0
     # via -r examples/requirements/flask.in
+asgiref==3.6.0
+    # via django
 attrs==22.2.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via flask-babelex
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.36
     # via pathy
 botocore==1.29.36
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -48,23 +52,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==2.2.28
+django==3.2.16
     # via
-    #   -r examples/requirements/django_2_2.in
+    #   -r examples/requirements/django_3_2.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==3.0
-    # via -r examples/requirements/django_2_2.in
-django-storages==1.12.3
-    # via -r examples/requirements/django_2_2.in
+django-debug-toolbar==3.8.1
+    # via -r examples/requirements/django_3_2.in
+django-storages==1.13.1
+    # via -r examples/requirements/django_3_2.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -121,22 +125,24 @@
     # via msrest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
     #   flask
     #   flask-babelex
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.2
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 mako==1.2.4
     # via alembic
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mako
     #   werkzeug
@@ -159,15 +165,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.6.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -228,14 +236,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
@@ -244,14 +253,16 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 speaklater==1.3
     # via flask-babelex
 sqlalchemy==1.4.45
     # via
     #   -r examples/requirements/flask.in
     #   alembic
     #   flask-sqlalchemy
@@ -287,9 +298,11 @@
     # via tox
 werkzeug==2.2.2
     # via flask
 wtforms==3.0.1
     # via flask-admin
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/django_3_0.txt` & `faker-file-0.9.3/examples/requirements/django_3_1.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_3_0.in
+#    pip-compile examples/requirements/django_3_1.in
 #
 asgiref==3.5.2
     # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -40,23 +42,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==3.0.14
+django==3.1.14
     # via
-    #   -r examples/requirements/django_3_0.in
+    #   -r examples/requirements/django_3_1.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==2.2.1
-    # via -r examples/requirements/django_3_0.in
+django-debug-toolbar==3.1.1
+    # via -r examples/requirements/django_3_1.in
 django-storages==1.12.3
-    # via -r examples/requirements/django_3_0.in
+    # via -r examples/requirements/django_3_1.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -88,22 +90,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -117,15 +124,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -183,14 +192,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -202,14 +212,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -232,7 +244,9 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/requirements/django_3_0_and_flask.txt` & `faker-file-0.9.3/examples/requirements/django_3_1_and_flask.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_3_0_and_flask.in
+#    pip-compile examples/requirements/django_3_1_and_flask.in
 #
 alembic==1.9.0
     # via -r examples/requirements/flask.in
 asgiref==3.6.0
     # via django
 attrs==22.2.0
     # via pytest
@@ -14,14 +14,16 @@
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via flask-babelex
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.36
     # via pathy
 botocore==1.29.36
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -50,23 +52,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==3.0.14
+django==3.1.14
     # via
-    #   -r examples/requirements/django_3_0.in
+    #   -r examples/requirements/django_3_1.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==2.2.1
-    # via -r examples/requirements/django_3_0.in
+django-debug-toolbar==3.1.1
+    # via -r examples/requirements/django_3_1.in
 django-storages==1.12.3
-    # via -r examples/requirements/django_3_0.in
+    # via -r examples/requirements/django_3_1.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -123,22 +125,24 @@
     # via msrest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
     #   flask
     #   flask-babelex
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.2
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 mako==1.2.4
     # via alembic
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mako
     #   werkzeug
@@ -161,15 +165,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.6.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -230,14 +236,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
@@ -246,14 +253,16 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 speaklater==1.3
     # via flask-babelex
 sqlalchemy==1.4.45
     # via
     #   -r examples/requirements/flask.in
     #   alembic
     #   flask-sqlalchemy
@@ -289,9 +298,11 @@
     # via tox
 werkzeug==2.2.2
     # via flask
 wtforms==3.0.1
     # via flask-admin
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/django_3_1.txt` & `faker-file-0.9.3/examples/requirements/django_3_2.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_3_1.in
+#    pip-compile examples/requirements/django_3_2.in
 #
 asgiref==3.5.2
     # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -40,23 +42,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==3.1.14
+django==3.2.16
     # via
-    #   -r examples/requirements/django_3_1.in
+    #   -r examples/requirements/django_3_2.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==3.1.1
-    # via -r examples/requirements/django_3_1.in
-django-storages==1.12.3
-    # via -r examples/requirements/django_3_1.in
+django-debug-toolbar==3.8.1
+    # via -r examples/requirements/django_3_2.in
+django-storages==1.13.1
+    # via -r examples/requirements/django_3_2.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -88,22 +90,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -117,15 +124,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -183,14 +192,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -202,14 +212,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -232,7 +244,9 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/requirements/django_3_1_and_flask.txt` & `faker-file-0.9.3/examples/requirements/django_2_2_and_flask.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_3_1_and_flask.in
+#    pip-compile examples/requirements/django_2_2_and_flask.in
 #
 alembic==1.9.0
     # via -r examples/requirements/flask.in
-asgiref==3.6.0
-    # via django
 attrs==22.2.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via flask-babelex
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.36
     # via pathy
 botocore==1.29.36
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -50,23 +50,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==3.1.14
+django==2.2.28
     # via
-    #   -r examples/requirements/django_3_1.in
+    #   -r examples/requirements/django_2_2.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==3.1.1
-    # via -r examples/requirements/django_3_1.in
+django-debug-toolbar==3.0
+    # via -r examples/requirements/django_2_2.in
 django-storages==1.12.3
-    # via -r examples/requirements/django_3_1.in
+    # via -r examples/requirements/django_2_2.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -123,22 +123,24 @@
     # via msrest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
     #   flask
     #   flask-babelex
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.2
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 mako==1.2.4
     # via alembic
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mako
     #   werkzeug
@@ -161,15 +163,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.6.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -230,14 +234,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
@@ -246,14 +251,16 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 speaklater==1.3
     # via flask-babelex
 sqlalchemy==1.4.45
     # via
     #   -r examples/requirements/flask.in
     #   alembic
     #   flask-sqlalchemy
@@ -289,9 +296,11 @@
     # via tox
 werkzeug==2.2.2
     # via flask
 wtforms==3.0.1
     # via flask-admin
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/django_3_2.txt` & `faker-file-0.9.3/examples/requirements/django_4_0.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_3_2.in
+#    pip-compile examples/requirements/django_4_0.in
 #
 asgiref==3.5.2
     # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -40,23 +42,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==3.2.16
+django==4.0.8
     # via
-    #   -r examples/requirements/django_3_2.in
+    #   -r examples/requirements/django_4_0.in
     #   django-debug-toolbar
     #   django-storages
 django-debug-toolbar==3.8.1
-    # via -r examples/requirements/django_3_2.in
+    # via -r examples/requirements/django_4_0.in
 django-storages==1.13.1
-    # via -r examples/requirements/django_3_2.in
+    # via -r examples/requirements/django_4_0.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -88,22 +90,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -117,15 +124,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -174,23 +183,22 @@
     # via
     #   botocore
     #   faker
 python-docx==0.8.11
     # via -r examples/requirements/common.in
 python-pptx==0.6.21
     # via -r examples/requirements/common.in
-pytz==2022.6
-    # via django
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -202,14 +210,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -232,7 +242,9 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/requirements/django_3_2_and_flask.txt` & `faker-file-0.9.3/examples/requirements/django_3_0_and_flask.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_3_2_and_flask.in
+#    pip-compile examples/requirements/django_3_0_and_flask.in
 #
 alembic==1.9.0
     # via -r examples/requirements/flask.in
 asgiref==3.6.0
     # via django
 attrs==22.2.0
     # via pytest
@@ -14,14 +14,16 @@
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via flask-babelex
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.36
     # via pathy
 botocore==1.29.36
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -50,23 +52,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==3.2.16
+django==3.0.14
     # via
-    #   -r examples/requirements/django_3_2.in
+    #   -r examples/requirements/django_3_0.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==3.8.1
-    # via -r examples/requirements/django_3_2.in
-django-storages==1.13.1
-    # via -r examples/requirements/django_3_2.in
+django-debug-toolbar==2.2.1
+    # via -r examples/requirements/django_3_0.in
+django-storages==1.12.3
+    # via -r examples/requirements/django_3_0.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -123,22 +125,24 @@
     # via msrest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
     #   flask
     #   flask-babelex
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.2
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 mako==1.2.4
     # via alembic
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mako
     #   werkzeug
@@ -161,15 +165,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.6.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -230,14 +236,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
@@ -246,14 +253,16 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 speaklater==1.3
     # via flask-babelex
 sqlalchemy==1.4.45
     # via
     #   -r examples/requirements/flask.in
     #   alembic
     #   flask-sqlalchemy
@@ -289,9 +298,11 @@
     # via tox
 werkzeug==2.2.2
     # via flask
 wtforms==3.0.1
     # via flask-admin
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/django_4_0.txt` & `faker-file-0.9.3/examples/requirements/django_4_1.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_4_0.in
+#    pip-compile examples/requirements/django_4_1.in
 #
 asgiref==3.5.2
     # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -40,23 +42,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==4.0.8
+django==4.1.3
     # via
-    #   -r examples/requirements/django_4_0.in
+    #   -r examples/requirements/django_4_1.in
     #   django-debug-toolbar
     #   django-storages
 django-debug-toolbar==3.8.1
-    # via -r examples/requirements/django_4_0.in
+    # via -r examples/requirements/django_4_1.in
 django-storages==1.13.1
-    # via -r examples/requirements/django_4_0.in
+    # via -r examples/requirements/django_4_1.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -88,22 +90,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -117,15 +124,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -181,14 +190,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -200,14 +210,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -230,7 +242,9 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/requirements/django_4_0_and_flask.txt` & `faker-file-0.9.3/examples/requirements/django_4_0_and_flask.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_4_0_and_flask.in
+#    pip-compile examples/requirements/django_4_0_and_flask.in
 #
 alembic==1.9.0
     # via -r examples/requirements/flask.in
 asgiref==3.6.0
     # via django
 attrs==22.2.0
     # via pytest
@@ -14,14 +14,16 @@
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via flask-babelex
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.36
     # via pathy
 botocore==1.29.36
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -123,22 +125,24 @@
     # via msrest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
     #   flask
     #   flask-babelex
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.2
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 mako==1.2.4
     # via alembic
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mako
     #   werkzeug
@@ -161,15 +165,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.6.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -228,14 +234,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
@@ -244,14 +251,16 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 speaklater==1.3
     # via flask-babelex
 sqlalchemy==1.4.45
     # via
     #   -r examples/requirements/flask.in
     #   alembic
     #   flask-sqlalchemy
@@ -287,9 +296,11 @@
     # via tox
 werkzeug==2.2.2
     # via flask
 wtforms==3.0.1
     # via flask-admin
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/django_4_1.txt` & `faker-file-0.9.3/examples/requirements/testing.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_4_1.in
+#    pip-compile examples/requirements/testing.in
 #
 asgiref==3.5.2
     # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -40,23 +42,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==4.1.3
+django==3.2.16
     # via
-    #   -r examples/requirements/django_4_1.in
+    #   -r examples/requirements/django_3_2.in
     #   django-debug-toolbar
     #   django-storages
 django-debug-toolbar==3.8.1
-    # via -r examples/requirements/django_4_1.in
+    # via -r examples/requirements/django_3_2.in
 django-storages==1.13.1
-    # via -r examples/requirements/django_4_1.in
+    # via -r examples/requirements/django_3_2.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -88,22 +90,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -117,15 +124,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -174,21 +183,24 @@
     # via
     #   botocore
     #   faker
 python-docx==0.8.11
     # via -r examples/requirements/common.in
 python-pptx==0.6.21
     # via -r examples/requirements/common.in
+pytz==2022.6
+    # via django
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -200,14 +212,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -230,7 +244,9 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/requirements/django_4_1_and_flask.txt` & `faker-file-0.9.3/examples/requirements/django_4_1_and_flask.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/django_4_1_and_flask.in
+#    pip-compile examples/requirements/django_4_1_and_flask.in
 #
 alembic==1.9.0
     # via -r examples/requirements/flask.in
 asgiref==3.6.0
     # via django
 attrs==22.2.0
     # via pytest
@@ -14,14 +14,16 @@
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via flask-babelex
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.36
     # via pathy
 botocore==1.29.36
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -123,22 +125,24 @@
     # via msrest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
     #   flask
     #   flask-babelex
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.2
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 mako==1.2.4
     # via alembic
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mako
     #   werkzeug
@@ -161,15 +165,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.6.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -228,14 +234,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
@@ -244,14 +251,16 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 speaklater==1.3
     # via flask-babelex
 sqlalchemy==1.4.45
     # via
     #   -r examples/requirements/flask.in
     #   alembic
     #   flask-sqlalchemy
@@ -287,9 +296,11 @@
     # via tox
 werkzeug==2.2.2
     # via flask
 wtforms==3.0.1
     # via flask-admin
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/docs.txt` & `faker-file-0.9.3/examples/requirements/docs.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/docs.in
+#    pip-compile examples/requirements/docs.in
 #
 alabaster==0.7.12
     # via sphinx
 asgiref==3.5.2
     # via django
 attrs==22.1.0
     # via pytest
@@ -14,14 +14,16 @@
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via sphinx
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -104,22 +106,24 @@
     # via pytest
 isodate==0.6.1
     # via msrest
 jinja2==3.1.2
     # via
     #   rst2pdf
     #   sphinx
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 markupsafe==2.1.1
     # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
@@ -140,14 +144,15 @@
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
     # via
     #   python-pptx
     #   reportlab
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -218,14 +223,15 @@
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
     #   sphinx
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 rst2pdf==0.99
     # via -r examples/requirements/docs.in
 s3transfer==0.6.0
@@ -243,14 +249,16 @@
     #   tox
 smart-open==6.3.0
     # via pathy
 smartypants==2.0.1
     # via rst2pdf
 snowballstemmer==2.2.0
     # via sphinx
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sphinx==5.3.0
     # via -r examples/requirements/docs.in
 sphinxcontrib-applehelp==1.0.2
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.0
@@ -287,13 +295,15 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `faker-file-0.9.2/examples/requirements/flask.txt` & `faker-file-0.9.3/examples/requirements/flask.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/flask.in
+#    pip-compile examples/requirements/flask.in
 #
 alembic==1.9.0
     # via -r examples/requirements/flask.in
 attrs==22.2.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
 babel==2.11.0
     # via flask-babelex
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.36
     # via pathy
 botocore==1.29.36
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -112,22 +114,24 @@
     # via msrest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via
     #   flask
     #   flask-babelex
+    #   xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.2
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
 mako==1.2.4
     # via alembic
 markupsafe==2.1.1
     # via
     #   jinja2
     #   mako
     #   werkzeug
@@ -150,15 +154,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.6.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
@@ -217,14 +223,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
@@ -233,14 +240,16 @@
     #   google-auth
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 speaklater==1.3
     # via flask-babelex
 sqlalchemy==1.4.45
     # via
     #   -r examples/requirements/flask.in
     #   alembic
     #   flask-sqlalchemy
@@ -272,9 +281,11 @@
     # via tox
 werkzeug==2.2.2
     # via flask
 wtforms==3.0.1
     # via flask-admin
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
 zipp==3.11.0
     # via importlib-metadata
```

### Comparing `faker-file-0.9.2/examples/requirements/style_checkers.txt` & `faker-file-0.9.3/examples/requirements/style_checkers.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/style_checkers.in
+#    pip-compile examples/requirements/style_checkers.in
 #
 astroid==2.12.13
     # via pylint
 black==22.10.0
     # via -r examples/requirements/style_checkers.in
 cfgv==3.3.1
     # via pre-commit
```

### Comparing `faker-file-0.9.2/examples/requirements/test.txt` & `faker-file-0.9.3/examples/requirements/test.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/test.in
+#    pip-compile examples/requirements/test.in
 #
 attrs==22.1.0
     # via pytest
 coverage[toml]==6.5.0
     # via
     #   -r examples/requirements/test.in
     #   pytest-cov
```

### Comparing `faker-file-0.9.2/examples/requirements/testing.txt` & `faker-file-0.9.3/examples/requirements/django_2_2.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --resolver=backtracking examples/requirements/testing.in
+#    pip-compile examples/requirements/django_2_2.in
 #
-asgiref==3.5.2
-    # via django
 attrs==22.1.0
     # via pytest
 azure-core==1.26.1
     # via
     #   azure-storage-blob
     #   msrest
 azure-storage-blob==12.14.1
     # via pathy
+beautifulsoup4==4.11.1
+    # via xml2epub
 boto3==1.26.29
     # via pathy
 botocore==1.29.29
     # via
     #   boto3
     #   s3transfer
 cachetools==5.2.0
@@ -40,23 +40,23 @@
     #   pytest-cov
 cryptography==38.0.4
     # via azure-storage-blob
 defusedxml==0.7.1
     # via odfpy
 distlib==0.3.6
     # via virtualenv
-django==3.2.16
+django==2.2.28
     # via
-    #   -r examples/requirements/django_3_2.in
+    #   -r examples/requirements/django_2_2.in
     #   django-debug-toolbar
     #   django-storages
-django-debug-toolbar==3.8.1
-    # via -r examples/requirements/django_3_2.in
-django-storages==1.13.1
-    # via -r examples/requirements/django_3_2.in
+django-debug-toolbar==3.0
+    # via -r examples/requirements/django_2_2.in
+django-storages==1.12.3
+    # via -r examples/requirements/django_2_2.in
 et-xmlfile==1.1.0
     # via openpyxl
 factory-boy==3.2.1
     # via -r examples/requirements/test.in
 faker==15.3.4
     # via
     #   -r examples/requirements/test.in
@@ -88,22 +88,27 @@
     # via requests
 imgkit==1.2.2
     # via -r examples/requirements/common.in
 iniconfig==1.1.1
     # via pytest
 isodate==0.6.1
     # via msrest
+jinja2==3.1.2
+    # via xml2epub
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 lxml==4.9.1
     # via
     #   python-docx
     #   python-pptx
+    #   xml2epub
+markupsafe==2.1.1
+    # via jinja2
 mock==4.0.3
     # via pathy
 msrest==0.7.1
     # via azure-storage-blob
 oauthlib==3.2.2
     # via requests-oauthlib
 odfpy==1.4.1
@@ -117,15 +122,17 @@
 parametrize==0.1.1
     # via -r examples/requirements/test.in
 pathy[all]==0.10.1
     # via -r examples/requirements/common.in
 pdfkit==1.0.0
     # via -r examples/requirements/common.in
 pillow==9.3.0
-    # via python-pptx
+    # via
+    #   python-pptx
+    #   xml2epub
 platformdirs==2.5.4
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 protobuf==4.21.11
@@ -183,14 +190,15 @@
 requests==2.28.1
     # via
     #   azure-core
     #   google-api-core
     #   google-cloud-storage
     #   msrest
     #   requests-oauthlib
+    #   xml2epub
 requests-oauthlib==1.3.1
     # via msrest
 rsa==4.9
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 shellingham==1.5.0
@@ -202,14 +210,16 @@
     #   google-cloud-storage
     #   imgkit
     #   isodate
     #   python-dateutil
     #   tox
 smart-open==6.3.0
     # via pathy
+soupsieve==2.3.2.post1
+    # via beautifulsoup4
 sqlparse==0.4.3
     # via
     #   django
     #   django-debug-toolbar
 tablib==3.2.1
     # via -r examples/requirements/common.in
 toml==0.10.2
@@ -232,7 +242,9 @@
     # via
     #   botocore
     #   requests
 virtualenv==20.17.0
     # via tox
 xlsxwriter==3.0.3
     # via python-pptx
+xml2epub==2.6.2
+    # via -r examples/requirements/common.in
```

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/__init__.py` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 
     if override:
         session["lang"] = override
 
     return session.get("lang", "en")
 
 
-import faker_file_admin.main
+import faker_file_admin.main  # noqa
```

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/env.py` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/env.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic/versions/2695cb77cdf2_create_product_table.py` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic/versions/2695cb77cdf2_create_product_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """create upload table
 
 Revision ID: 2695cb77cdf2
-Revises: 
+Revises:
 Create Date: 2022-12-06 23:46:09.000000
 
 """
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
```

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/alembic.ini` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/alembic.ini`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/main.py` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/main.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/static/favicon.ico` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/templates/admin/index.html` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/faker_file_admin/templates/tree_list.html` & `faker-file-0.9.3/examples/sqlalchemy_example/faker_file_admin/templates/tree_list.html`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/examples/sqlalchemy_example/sqlalchemy_factories/faker_file_admin_upload.py` & `faker-file-0.9.3/examples/sqlalchemy_example/sqlalchemy_factories/faker_file_admin_upload.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/pyproject.toml` & `faker-file-0.9.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -61,19 +61,16 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "examples/django_example/project/wsgi.py",
 ]
 per-file-ignores = {}
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 # Assume Python 3.10.
 target-version = "py310"
-
-[tool.ruff.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
```

### Comparing `faker-file-0.9.2/scripts/compile_requirements.sh` & `faker-file-0.9.3/scripts/compile_requirements.sh`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/setup.py` & `faker-file-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import find_packages, setup
 
-version = "0.9.2"
+version = "0.9.3"
 
 try:
     readme = open(os.path.join(os.path.dirname(__file__), "README.rst")).read()
 except OSError:
     readme = ""
 
 dependency_links = []
@@ -35,20 +35,22 @@
             "odfpy",
             "openpyxl",
             "pathy[all]",
             "pdfkit",
             "python-docx",
             "python-pptx",
             "tablib",
+            "xml2epub",
         ],
         "django": ["Django>=2.2"],
         "docx": ["python-docx"],
         "images": ["imgkit"],
         "pdf": ["pdfkit"],
         "pptx": ["python-pptx"],
+        "epub": ["xml2epub"],
         "sqlalchemy": ["SQLAlchemy>=1.0", "SQLAlchemy-Utils>=0.37.0"],
         "xlsx": ["tablib", "openpyxl"],
         "ods": ["tablib", "odfpy"],
         "s3": ["pathy[s3]"],
         "gcs": ["pathy[gcs]"],
         "azure": ["pathy[azure]"],
     },
@@ -83,12 +85,13 @@
     keywords="faker, faker-file, files, testing, factories",
     author="Artur Barseghyan",
     author_email="artur.barseghyan@gmail.com",
     url="https://github.com/barseghyanartur/faker-file/",
     package_dir={"": "src"},
     packages=find_packages(where="./src"),
     license="MIT",
+    python_requires=">=3.7",
     install_requires=install_requires,
     tests_require=tests_require,
     dependency_links=dependency_links,
     include_package_data=True,
 )
```

### Comparing `faker-file-0.9.2/src/faker_file/base.py` & `faker-file-0.9.3/src/faker_file/base.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/bin_file.py` & `faker-file-0.9.3/src/faker_file/providers/bin_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/csv_file.py` & `faker-file-0.9.3/src/faker_file/providers/csv_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/docx_file.py` & `faker-file-0.9.3/src/faker_file/providers/docx_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/ico_file.py` & `faker-file-0.9.3/src/faker_file/providers/ico_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/jpeg_file.py` & `faker-file-0.9.3/src/faker_file/providers/jpeg_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/mixins/image_mixin.py` & `faker-file-0.9.3/src/faker_file/providers/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/mixins/tablular_data_mixin.py` & `faker-file-0.9.3/src/faker_file/providers/mixins/tablular_data_mixin.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/ods_file.py` & `faker-file-0.9.3/src/faker_file/providers/ods_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/pdf_file.py` & `faker-file-0.9.3/src/faker_file/providers/pdf_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/png_file.py` & `faker-file-0.9.3/src/faker_file/providers/png_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/pptx_file.py` & `faker-file-0.9.3/src/faker_file/providers/pptx_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/random_file_from_dir.py` & `faker-file-0.9.3/src/faker_file/providers/random_file_from_dir.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/rtf_file.py` & `faker-file-0.9.3/src/faker_file/providers/rtf_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/svg_file.py` & `faker-file-0.9.3/src/faker_file/providers/svg_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/txt_file.py` & `faker-file-0.9.3/src/faker_file/providers/txt_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/webp_file.py` & `faker-file-0.9.3/src/faker_file/providers/webp_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/xlsx_file.py` & `faker-file-0.9.3/src/faker_file/providers/xlsx_file.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/providers/zip_file.py` & `faker-file-0.9.3/src/faker_file/providers/zip_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 __copyright__ = "2022 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "ZipFileProvider",
     "create_inner_bin_file",
     "create_inner_csv_file",
     "create_inner_docx_file",
+    "create_inner_epub_file",
     "create_inner_ico_file",
     "create_inner_jpeg_file",
     "create_inner_ods_file",
     "create_inner_pdf_file",
     "create_inner_png_file",
     "create_inner_pptx_file",
     "create_inner_rtf_file",
@@ -109,14 +110,43 @@
         max_nb_chars=max_nb_chars,
         wrap_chars_after=wrap_chars_after,
         content=content,
         **kwargs,
     )
 
 
+def create_inner_epub_file(
+    storage: BaseStorage = None,
+    prefix: Optional[str] = None,
+    generator: Union[Provider, Faker] = None,
+    max_nb_chars: int = DEFAULT_TEXT_MAX_NB_CHARS,
+    wrap_chars_after: Optional[int] = None,
+    content: Optional[str] = None,
+    title: Optional[str] = None,
+    chapter_title: Optional[str] = None,
+    **kwargs,
+) -> StringValue:
+    """Create inner EPUB file."""
+    try:
+        from .epub_file import EpubFileProvider
+    except ImportError as err:
+        raise err
+
+    return EpubFileProvider(generator).epub_file(
+        storage=storage,
+        prefix=prefix,
+        max_nb_chars=max_nb_chars,
+        wrap_chars_after=wrap_chars_after,
+        content=content,
+        title=title,
+        chapter_title=chapter_title,
+        **kwargs,
+    )
+
+
 def create_inner_ico_file(
     storage: BaseStorage = None,
     prefix: Optional[str] = None,
     generator: Union[Provider, Faker] = None,
     max_nb_chars: int = DEFAULT_IMAGE_MAX_NB_CHARS,
     wrap_chars_after: Optional[int] = None,
     content: Optional[str] = None,
```

### Comparing `faker-file-0.9.2/src/faker_file/storages/aws_s3.py` & `faker-file-0.9.3/src/faker_file/storages/aws_s3.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/storages/azure_cloud_storage.py` & `faker-file-0.9.3/src/faker_file/storages/azure_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/storages/base.py` & `faker-file-0.9.3/src/faker_file/storages/base.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/storages/cloud.py` & `faker-file-0.9.3/src/faker_file/storages/cloud.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/storages/filesystem.py` & `faker-file-0.9.3/src/faker_file/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/storages/google_cloud_storage.py` & `faker-file-0.9.3/src/faker_file/storages/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/tests/test_django_integration.py` & `faker-file-0.9.3/src/faker_file/tests/test_django_integration.py`

 * *Files identical despite different names*

### Comparing `faker-file-0.9.2/src/faker_file/tests/test_providers.py` & `faker-file-0.9.3/src/faker_file/tests/test_providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pathy import use_fs
 
 from ..base import DEFAULT_REL_PATH
 from ..constants import DEFAULT_TEXT_CONTENT_TEMPLATE
 from ..providers.bin_file import BinFileProvider
 from ..providers.csv_file import CsvFileProvider
 from ..providers.docx_file import DocxFileProvider
+from ..providers.epub_file import EpubFileProvider
 from ..providers.ico_file import IcoFileProvider
 from ..providers.jpeg_file import JpegFileProvider
 from ..providers.ods_file import OdsFileProvider
 from ..providers.pdf_file import PdfFileProvider
 from ..providers.png_file import PngFileProvider
 from ..providers.pptx_file import PptxFileProvider
 from ..providers.random_file_from_dir import RandomFileFromDirProvider
@@ -27,14 +28,15 @@
 from ..providers.webp_file import WebpFileProvider
 from ..providers.xlsx_file import XlsxFileProvider
 from ..providers.zip_file import (
     ZipFileProvider,
     create_inner_bin_file,
     create_inner_csv_file,
     create_inner_docx_file,
+    create_inner_epub_file,
     create_inner_ico_file,
     create_inner_jpeg_file,
     create_inner_ods_file,
     create_inner_pdf_file,
     create_inner_png_file,
     create_inner_pptx_file,
     create_inner_rtf_file,
@@ -53,14 +55,15 @@
 __license__ = "MIT"
 __all__ = ("ProvidersTestCase",)
 
 
 FileProvider = Union[
     CsvFileProvider,
     DocxFileProvider,
+    EpubFileProvider,
     IcoFileProvider,
     JpegFileProvider,
     PdfFileProvider,
     PngFileProvider,
     PptxFileProvider,
     RtfFileProvider,
     SvgFileProvider,
@@ -111,14 +114,36 @@
             "docx_file",
             {
                 "wrap_chars_after": 40,
                 "content": _FAKER.text(),
             },
             None,
         ),
+        # EPUB
+        (EpubFileProvider, "epub_file", {}, None),
+        (EpubFileProvider, "epub_file", {}, False),
+        (EpubFileProvider, "epub_file", {}, PATHY_FS_STORAGE),
+        (
+            EpubFileProvider,
+            "epub_file",
+            {
+                "wrap_chars_after": 40,
+                "content": DEFAULT_TEXT_CONTENT_TEMPLATE,
+            },
+            None,
+        ),
+        (
+            EpubFileProvider,
+            "epub_file",
+            {
+                "wrap_chars_after": 40,
+                "content": _FAKER.text(),
+            },
+            None,
+        ),
         # ICO
         (IcoFileProvider, "ico_file", {}, None),
         (IcoFileProvider, "ico_file", {}, False),
         (IcoFileProvider, "ico_file", {}, PATHY_FS_STORAGE),
         (
             IcoFileProvider,
             "ico_file",
@@ -407,14 +432,15 @@
     @parametrize(
         "create_inner_file_func, content",
         [
             (None, None),
             (create_inner_bin_file, b"Lorem ipsum"),
             (create_inner_csv_file, "Lorem ipsum"),
             (create_inner_docx_file, "Lorem ipsum"),
+            (create_inner_epub_file, "Lorem ipsum"),
             (create_inner_ico_file, "Lorem ipsum"),
             (create_inner_jpeg_file, "Lorem ipsum"),
             (create_inner_ods_file, None),
             (create_inner_pdf_file, "Lorem ipsum"),
             (create_inner_png_file, "Lorem ipsum"),
             (create_inner_pptx_file, "Lorem ipsum"),
             (create_inner_rtf_file, "Lorem ipsum"),
@@ -475,14 +501,20 @@
             ),
             # DOCX
             (
                 "faker_file.providers.docx_file",
                 "DocxFileProvider",
                 create_inner_docx_file,
             ),
+            # EPUB
+            (
+                "faker_file.providers.epub_file",
+                "EpubFileProvider",
+                create_inner_epub_file,
+            ),
             # ICO
             (
                 "faker_file.providers.ico_file",
                 "IcoFileProvider",
                 create_inner_ico_file,
             ),
             # JPEG
```

### Comparing `faker-file-0.9.2/src/faker_file/tests/test_sqlalchemy_integration.py` & `faker-file-0.9.3/src/faker_file/tests/test_sqlalchemy_integration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,58 @@
-# from typing import Callable
-# from unittest import TestCase, skip
-#
-# import sqlalchemy_factories as factories
-# from faker import Faker
-# from faker_file_admin import app
-# from faker_file_admin.models import Upload
-# from parametrize import parametrize
-# from sqlalchemy import create_engine
-# from sqlalchemy.orm import sessionmaker
-#
-# from ..storages.filesystem import FileSystemStorage
-#
-# __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
-# __copyright__ = "2022 Artur Barseghyan"
-# __license__ = "MIT"
-# __all__ = ("SQLAlchemyIntegrationTestCase",)
-#
-#
-# STORAGE = FileSystemStorage(root_path="", rel_path="tmp")
-#
-#
-# class SQLAlchemyIntegrationTestCase(TestCase):
-#     """SQLAlchemy integration test case."""
-#
-#     engine = create_engine("sqlite:///:memory:")
-#     Session = sessionmaker(bind=engine)
-#     session = Session()
-#
-#     def setUp(self: "SQLAlchemyIntegrationTestCase"):
-#         Upload.metadata.create_all(self.engine)
-#         self.session.commit()
-#
-#     def tearDown(self: "SQLAlchemyIntegrationTestCase"):
-#         Upload.metadata.drop_all(self.engine)
-#
-#     FAKER: Faker
-#
-#     @parametrize(
-#         "factory",
-#         [
-#             (factories.DocxUploadFactory,),
-#             (factories.PdfUploadFactory,),
-#             (factories.PptxUploadFactory,),
-#             (factories.TxtUploadFactory,),
-#             (factories.ZipUploadFactory,),
-#         ],
-#     )
-#     @skip
-#     def test_file(
-#         self: "SQLAlchemyIntegrationTestCase", factory: Callable
-#     ) -> None:
-#         """Test file."""
-#         with app.app_context():
-#             _upload = factory()
-#             self.session.commit()
-#             self.assertTrue(STORAGE.exists(_upload.file))
+from typing import Callable
+from unittest import TestCase
+
+import pytest
+import sqlalchemy_factories as factories
+from faker import Faker
+from faker_file_admin import app
+from faker_file_admin.models import Upload
+from parametrize import parametrize
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
+
+from ..storages.filesystem import FileSystemStorage
+
+__author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
+__copyright__ = "2022 Artur Barseghyan"
+__license__ = "MIT"
+__all__ = ("SQLAlchemyIntegrationTestCase",)
+
+
+STORAGE = FileSystemStorage(root_path="", rel_path="tmp")
+
+
+class SQLAlchemyIntegrationTestCase(TestCase):
+    """SQLAlchemy integration test case."""
+
+    engine = create_engine("sqlite:///:memory:")
+    Session = sessionmaker(bind=engine)
+    session = Session()
+
+    def setUp(self: "SQLAlchemyIntegrationTestCase"):
+        Upload.metadata.create_all(self.engine)
+        self.session.commit()
+
+    def tearDown(self: "SQLAlchemyIntegrationTestCase"):
+        Upload.metadata.drop_all(self.engine)
+
+    FAKER: Faker
+
+    @parametrize(
+        "factory",
+        [
+            (factories.DocxUploadFactory,),
+            (factories.PdfUploadFactory,),
+            (factories.PptxUploadFactory,),
+            (factories.TxtUploadFactory,),
+            (factories.ZipUploadFactory,),
+        ],
+    )
+    @pytest.mark.optional
+    def test_file(
+        self: "SQLAlchemyIntegrationTestCase", factory: Callable
+    ) -> None:
+        """Test file."""
+        with app.app_context():
+            _upload = factory()
+            self.session.commit()
+            self.assertTrue(STORAGE.exists(_upload.file))
```

### Comparing `faker-file-0.9.2/src/faker_file/tests/test_storages.py` & `faker-file-0.9.3/src/faker_file/tests/test_storages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import tempfile
 import unittest
 from pathlib import Path
 from typing import Any, Dict, Type
 
+# import pytest
 from faker import Faker
 from parametrize import parametrize
 from pathy import use_fs, use_fs_cache
 
 from ..storages.aws_s3 import AWSS3Storage
 from ..storages.azure_cloud_storage import AzureCloudStorage
 from ..storages.base import BaseStorage
 from ..storages.cloud import CloudStorage, PathyFileSystemStorage
 from ..storages.filesystem import FileSystemStorage
 from ..storages.google_cloud_storage import GoogleCloudStorage
 
+# from unittest.mock import patch
+
+
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2022 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = ("TestStoragesTestCase",)
 
 FAKER = Faker()
 
 
+# class _GoogleCloudCredentials:
+#     token = "1234"
+#     project_id = "1234"
+
+
 class TestStoragesTestCase(unittest.TestCase):
     """Test storages."""
 
     @parametrize(
         "storage_cls, kwargs, prefix, extension",
         [
             # FileSystemStorage
@@ -204,7 +213,46 @@
         class TestCloudStorage(CloudStorage):
             schema: str = "file"
 
         test_storage = TestCloudStorage(bucket_name="testing")
         method = getattr(test_storage, method_name)
         with self.assertRaises(NotImplementedError):
             method(**method_kwargs)
+
+    def test_file_system_storage_abspath(self):
+        """Test `FileSystemStorage` `abspath`."""
+        storage = FileSystemStorage(
+            root_path=tempfile.gettempdir(),
+            rel_path="rel_tmp",
+        )
+        filename = storage.generate_filename(prefix="", extension="tmp")
+        self.assertTrue(storage.abspath(filename).startswith("/tmp/rel_tmp/"))
+
+    def test_pathy_file_system_storage_abspath(self):
+        """Test `PathyFileSystemStorage` `abspath`."""
+        storage = PathyFileSystemStorage(
+            bucket_name="faker-file-tmp",
+            root_path="root_tmp",
+            rel_path="rel_tmp",
+        )
+        filename = storage.generate_filename(prefix="", extension="tmp")
+        self.assertTrue(
+            storage.abspath(filename).startswith(
+                "file://faker-file-tmp/root_tmp/rel_tmp/"
+            )
+        )
+
+    # @patch(
+    #     "faker_file.storages.google_cloud_storage.service_account."
+    #     "Credentials.from_service_account_file",
+    #     new_callable=lambda: lambda __x: _GoogleCloudCredentials(),
+    # )
+    # @pytest.mark.xfail
+    # def test_google_cloud_storage_authentication(self, func):
+    #     """Test `GoogleCloudStorage` authentication."""
+    #     GoogleCloudStorage(
+    #         bucket_name="testing",
+    #         rel_path="tmp",
+    #         credentials={
+    #             "json_file_path": "/i/dont/exist.json",
+    #         },
+    #     )
```

### Comparing `faker-file-0.9.2/src/faker_file.egg-info/PKG-INFO` & `faker-file-0.9.3/src/faker_file.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: faker-file
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generate fake files.
 Home-page: https://github.com/barseghyanartur/faker-file/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file/issues
 Project-URL: Documentation, https://faker-file.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/faker-file
 Project-URL: Changelog, https://faker-file.readthedocs.io/en/latest/changelog.html
 Keywords: faker,faker-file,files,testing,factories
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 
 ==========
 faker-file
 ==========
-**Generate fake files**
+**Generate files with fake data**
 
 .. image:: https://img.shields.io/pypi/v/faker-file.svg
    :target: https://pypi.python.org/pypi/faker-file
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/pyversions/faker-file.svg
     :target: https://pypi.python.org/pypi/faker-file/
@@ -58,18 +58,20 @@
 Prerequisites
 =============
 All of core dependencies of this package are `MIT` licensed.
 Most of optional dependencies of this package are `MIT` licensed, while
 a few are `BSD`- or `Apache 2` licensed. All licenses are mentioned
 below between the brackets.
 
-- Core package requires Python 3.7, 3.8, 3.9, 3.10 and 3.11.
+- Core package requires Python 3.7, 3.8, 3.9, 3.10 or 3.11.
+- ``Faker`` (`MIT`) is the only required dependency.
 - ``Django`` (`BSD`) integration with ``factory_boy`` (`MIT`) has
   been tested with ``Django`` 2.2, 3.0, 3.1, 3.2, 4.0 and 4.1.
 - ``DOCX`` file support requires ``python-docx`` (`MIT`).
+- ``EPUB`` file support requires ``xml2epub`` (`MIT`) and ``jinja2`` (`BSD`).
 - ``ICO``, ``JPEG``, ``PNG``, ``SVG`` and ``WEBP`` files support
   requires ``imgkit`` (`MIT`).
 - ``PDF`` file support requires ``pdfkit`` (`MIT`).
 - ``PPTX`` file support requires ``python-pptx`` (`MIT`).
 - ``ODS`` file support requires ``tablib`` (`MIT`) and ``odfpy`` (`Apache 2`).
 - ``XLSX`` file support requires ``tablib`` (`MIT`) and ``openpyxl`` (`MIT`).
 - ``PathyFileSystemStorage`` storage support requires ``pathy`` (`Apache 2`).
@@ -103,14 +105,20 @@
 
 **With DOCX support**
 
 .. code-block:: sh
 
     pip install faker-file[docx]
 
+**With EPUB support**
+
+.. code-block:: sh
+
+    pip install faker-file[epub]
+
 **With images support**
 
 .. code-block:: sh
 
     pip install faker-file[images]
 
 **With XLSX support**
@@ -136,14 +144,15 @@
 ========
 
 Supported file types
 --------------------
 - ``BIN``
 - ``CSV``
 - ``DOCX``
+- ``EPUB``
 - ``ICO``
 - ``JPEG``
 - ``ODS``
 - ``PDF``
 - ``PNG``
 - ``RTF``
 - ``PPTX``
@@ -200,16 +209,16 @@
     from django.db import models
 
     class Upload(models.Model):
 
         # ...
         file = models.FileField()
 
-upload/factory.py
-~~~~~~~~~~~~~~~~~
+upload/factories.py
+~~~~~~~~~~~~~~~~~~~
 Note, that when using ``faker-file`` with ``Django`` and native file system
 storages, you need to pass your ``MEDIA_ROOT`` setting as ``root_path`` value
 to the chosen file storage as show below.
 
 .. code-block:: python
 
     import factory
@@ -386,9 +395,7 @@
 For any security issues contact me at the e-mail given in the `Author`_ section.
 
 For overall issues, go to `GitHub <https://github.com/barseghyanartur/faker-file/issues>`_.
 
 Author
 ======
 Artur Barseghyan <artur.barseghyan@gmail.com>
-
-
```

### Comparing `faker-file-0.9.2/src/faker_file.egg-info/SOURCES.txt` & `faker-file-0.9.3/src/faker_file.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 src/faker_file.egg-info/dependency_links.txt
 src/faker_file.egg-info/requires.txt
 src/faker_file.egg-info/top_level.txt
 src/faker_file/providers/__init__.py
 src/faker_file/providers/bin_file.py
 src/faker_file/providers/csv_file.py
 src/faker_file/providers/docx_file.py
+src/faker_file/providers/epub_file.py
 src/faker_file/providers/ico_file.py
 src/faker_file/providers/jpeg_file.py
 src/faker_file/providers/ods_file.py
 src/faker_file/providers/pdf_file.py
 src/faker_file/providers/png_file.py
 src/faker_file/providers/pptx_file.py
 src/faker_file/providers/random_file_from_dir.py
```

