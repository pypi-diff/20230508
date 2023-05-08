# Comparing `tmp/django_celery_results-2.5.0.tar.gz` & `tmp/django_celery_results-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_celery_results-2.5.0.tar", last modified: Mon Mar 13 11:44:37 2023, max compression
+gzip compressed data, was "django_celery_results-2.5.1.tar", last modified: Mon May  8 14:21:10 2023, max compression
```

## Comparing `django_celery_results-2.5.0.tar` & `django_celery_results-2.5.1.tar`

### file list

```diff
@@ -1,120 +1,119 @@
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.611520 django_celery_results-2.5.0/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3190 2023-03-13 11:20:36.000000 django_celery_results-2.5.0/AUTHORS
--rw-rw-r--   0 asif      (1000) asif      (1000)     4906 2023-03-13 11:36:29.000000 django_celery_results-2.5.0/Changelog
--rw-rw-r--   0 asif      (1000) asif      (1000)     2695 2023-03-13 11:20:36.000000 django_celery_results-2.5.0/LICENSE
--rw-rw-r--   0 asif      (1000) asif      (1000)      413 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/MANIFEST.in
--rw-rw-r--   0 asif      (1000) asif      (1000)     5804 2023-03-13 11:44:37.615521 django_celery_results-2.5.0/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)     4401 2023-03-13 11:41:26.000000 django_celery_results-2.5.0/README.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.591520 django_celery_results-2.5.0/django_celery_results/
--rw-rw-r--   0 asif      (1000) asif      (1000)      983 2023-03-13 11:39:24.000000 django_celery_results-2.5.0/django_celery_results/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2362 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/django_celery_results/admin.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      428 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/apps.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.591520 django_celery_results-2.5.0/django_celery_results/backends/
--rw-rw-r--   0 asif      (1000) asif      (1000)      117 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/backends/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1129 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/backends/cache.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11181 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/django_celery_results/backends/database.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.587520 django_celery_results-2.5.0/django_celery_results/locale/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.587520 django_celery_results-2.5.0/django_celery_results/locale/es/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.591520 django_celery_results-2.5.0/django_celery_results/locale/es/LC_MESSAGES/
--rw-rw-r--   0 asif      (1000) asif      (1000)     4381 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.587520 django_celery_results-2.5.0/django_celery_results/locale/pt_BR/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.595520 django_celery_results-2.5.0/django_celery_results/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5177 2022-03-01 07:09:38.000000 django_celery_results-2.5.0/django_celery_results/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.587520 django_celery_results-2.5.0/django_celery_results/locale/ru/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.595520 django_celery_results-2.5.0/django_celery_results/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 asif      (1000) asif      (1000)     6714 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.587520 django_celery_results-2.5.0/django_celery_results/locale/zh_Hans/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.599520 django_celery_results-2.5.0/django_celery_results/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5308 2022-04-17 06:42:40.000000 django_celery_results-2.5.0/django_celery_results/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-r--   0 asif      (1000) asif      (1000)     7822 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/django_celery_results/managers.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.603520 django_celery_results-2.5.0/django_celery_results/migrations/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2585 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0001_initial.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      872 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0002_add_task_name_args_kwargs.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      506 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0003_auto_20181106_1101.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4254 2022-03-01 07:09:38.000000 django_celery_results-2.5.0/django_celery_results/migrations/0004_auto_20190516_0412.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      688 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0005_taskresult_worker.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1399 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0006_taskresult_date_created.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      423 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0007_remove_taskresult_hidden.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1403 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0008_chordcounter.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8003 2022-03-01 07:09:38.000000 django_celery_results-2.5.0/django_celery_results/migrations/0009_groupresult.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1378 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0010_remove_duplicate_indices.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      585 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/0011_taskresult_periodic_task_name.py
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/migrations/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8100 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/django_celery_results/models.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2141 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/urls.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      587 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/utils.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1789 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/django_celery_results/views.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.591520 django_celery_results-2.5.0/django_celery_results.egg-info/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5804 2023-03-13 11:44:37.000000 django_celery_results-2.5.0/django_celery_results.egg-info/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)     3031 2023-03-13 11:44:37.000000 django_celery_results-2.5.0/django_celery_results.egg-info/SOURCES.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-03-13 11:44:37.000000 django_celery_results-2.5.0/django_celery_results.egg-info/dependency_links.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      144 2023-03-13 11:44:37.000000 django_celery_results-2.5.0/django_celery_results.egg-info/entry_points.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2022-03-01 07:48:58.000000 django_celery_results-2.5.0/django_celery_results.egg-info/not-zip-safe
--rw-rw-r--   0 asif      (1000) asif      (1000)       34 2023-03-13 11:44:37.000000 django_celery_results-2.5.0/django_celery_results.egg-info/requires.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       22 2023-03-13 11:44:37.000000 django_celery_results-2.5.0/django_celery_results.egg-info/top_level.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.603520 django_celery_results-2.5.0/docs/
--rw-rw-r--   0 asif      (1000) asif      (1000)     8405 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/Makefile
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.603520 django_celery_results-2.5.0/docs/_static/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/_static/.keep
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.603520 django_celery_results-2.5.0/docs/_templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/_templates/.keep
--rw-rw-r--   0 asif      (1000) asif      (1000)       26 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/changelog.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      868 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/conf.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      969 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/docs/copyright.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1627 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/docs/getting_started.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)       99 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/glossary.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.603520 django_celery_results-2.5.0/docs/images/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3364 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/images/favicon.ico
--rw-rw-r--   0 asif      (1000) asif      (1000)    26250 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/images/logo.png
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.607520 django_celery_results-2.5.0/docs/includes/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1034 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/includes/installation.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      953 2023-03-13 11:40:39.000000 django_celery_results-2.5.0/docs/includes/introduction.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      555 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/docs/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2020 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/docs/injecting_metadata.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7248 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/make.bat
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.607520 django_celery_results-2.5.0/docs/reference/
--rw-rw-r--   0 asif      (1000) asif      (1000)      321 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/reference/django_celery_results.backends.cache.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      330 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/reference/django_celery_results.backends.database.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/reference/django_celery_results.backends.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/reference/django_celery_results.managers.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/reference/django_celery_results.models.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/reference/django_celery_results.utils.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      348 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/reference/index.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.607520 django_celery_results-2.5.0/docs/templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1476 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/docs/templates/readme.txt
--rwxrwxr-x   0 asif      (1000) asif      (1000)      250 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/manage.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.611520 django_celery_results-2.5.0/requirements/
--rw-rw-r--   0 asif      (1000) asif      (1000)       34 2023-03-13 09:37:08.000000 django_celery_results-2.5.0/requirements/default.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       53 2023-03-13 09:37:08.000000 django_celery_results-2.5.0/requirements/docs.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       97 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/requirements/pkgutils.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       64 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/requirements/test-ci.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       17 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/requirements/test-django.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2023-03-13 09:37:08.000000 django_celery_results-2.5.0/requirements/test-django32.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2023-03-13 09:37:08.000000 django_celery_results-2.5.0/requirements/test-django40.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2023-03-13 09:37:08.000000 django_celery_results-2.5.0/requirements/test-django41.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2023-03-13 09:37:08.000000 django_celery_results-2.5.0/requirements/test-django42.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       82 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/requirements/test.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      378 2023-03-13 11:44:37.615521 django_celery_results-2.5.0/setup.cfg
--rw-rw-r--   0 asif      (1000) asif      (1000)     4216 2023-03-13 10:57:35.000000 django_celery_results-2.5.0/setup.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.611520 django_celery_results-2.5.0/t/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1322 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/conftest.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.611520 django_celery_results-2.5.0/t/integration/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/integration/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2256 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/integration/benchmark_models.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.611520 django_celery_results-2.5.0/t/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)       46 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      314 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/proj/celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4262 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/proj/settings.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      118 2023-03-13 11:20:36.000000 django_celery_results-2.5.0/t/proj/urls.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      387 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/proj/wsgi.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.611520 django_celery_results-2.5.0/t/unit/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/unit/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-03-13 11:44:37.611520 django_celery_results-2.5.0/t/unit/backends/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/unit/backends/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3350 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/unit/backends/test_cache.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    32299 2023-03-13 07:35:55.000000 django_celery_results-2.5.0/t/unit/backends/test_database.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1427 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/unit/test_migrations.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8977 2022-06-29 10:16:08.000000 django_celery_results-2.5.0/t/unit/test_models.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1469 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/unit/test_utils.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3995 2021-12-23 10:43:17.000000 django_celery_results-2.5.0/t/unit/test_views.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.176626 django_celery_results-2.5.1/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3190 2023-03-13 11:20:36.000000 django_celery_results-2.5.1/AUTHORS
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5096 2023-05-08 14:12:39.000000 django_celery_results-2.5.1/Changelog
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2693 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/LICENSE
+-rw-rw-r--   0 asif      (1000) asif      (1000)      413 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/MANIFEST.in
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6037 2023-05-08 14:21:10.176626 django_celery_results-2.5.1/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4405 2023-05-08 14:18:18.000000 django_celery_results-2.5.1/README.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.156626 django_celery_results-2.5.1/django_celery_results/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1007 2023-05-08 14:16:45.000000 django_celery_results-2.5.1/django_celery_results/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2362 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/django_celery_results/admin.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      428 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/apps.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.156626 django_celery_results-2.5.1/django_celery_results/backends/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      117 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/backends/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1129 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/backends/cache.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11181 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/django_celery_results/backends/database.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.152625 django_celery_results-2.5.1/django_celery_results/locale/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.152625 django_celery_results-2.5.1/django_celery_results/locale/es/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.156626 django_celery_results-2.5.1/django_celery_results/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4381 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.152625 django_celery_results-2.5.1/django_celery_results/locale/pt_BR/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.160626 django_celery_results-2.5.1/django_celery_results/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5177 2022-03-01 07:09:38.000000 django_celery_results-2.5.1/django_celery_results/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.152625 django_celery_results-2.5.1/django_celery_results/locale/ru/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.160626 django_celery_results-2.5.1/django_celery_results/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6714 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.152625 django_celery_results-2.5.1/django_celery_results/locale/zh_Hans/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.160626 django_celery_results-2.5.1/django_celery_results/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5308 2022-04-17 06:42:40.000000 django_celery_results-2.5.1/django_celery_results/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7798 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/django_celery_results/managers.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.164626 django_celery_results-2.5.1/django_celery_results/migrations/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2585 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0001_initial.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      872 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0002_add_task_name_args_kwargs.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      506 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0003_auto_20181106_1101.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4254 2022-03-01 07:09:38.000000 django_celery_results-2.5.1/django_celery_results/migrations/0004_auto_20190516_0412.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      688 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0005_taskresult_worker.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1399 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0006_taskresult_date_created.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      423 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0007_remove_taskresult_hidden.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1403 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0008_chordcounter.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8003 2022-03-01 07:09:38.000000 django_celery_results-2.5.1/django_celery_results/migrations/0009_groupresult.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1378 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0010_remove_duplicate_indices.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      585 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/0011_taskresult_periodic_task_name.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/migrations/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8100 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/django_celery_results/models.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2141 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/urls.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      477 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/django_celery_results/utils.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1789 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/django_celery_results/views.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.156626 django_celery_results-2.5.1/django_celery_results.egg-info/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6037 2023-05-08 14:21:09.000000 django_celery_results-2.5.1/django_celery_results.egg-info/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3010 2023-05-08 14:21:09.000000 django_celery_results-2.5.1/django_celery_results.egg-info/SOURCES.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-05-08 14:21:09.000000 django_celery_results-2.5.1/django_celery_results.egg-info/dependency_links.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      144 2023-05-08 14:21:09.000000 django_celery_results-2.5.1/django_celery_results.egg-info/entry_points.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        1 2022-03-01 07:48:58.000000 django_celery_results-2.5.1/django_celery_results.egg-info/not-zip-safe
+-rw-rw-r--   0 asif      (1000) asif      (1000)       34 2023-05-08 14:21:09.000000 django_celery_results-2.5.1/django_celery_results.egg-info/requires.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       22 2023-05-08 14:21:09.000000 django_celery_results-2.5.1/django_celery_results.egg-info/top_level.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.164626 django_celery_results-2.5.1/docs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8410 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/docs/Makefile
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.164626 django_celery_results-2.5.1/docs/_static/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/_static/.keep
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.164626 django_celery_results-2.5.1/docs/_templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/_templates/.keep
+-rw-rw-r--   0 asif      (1000) asif      (1000)       26 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/changelog.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      869 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/docs/conf.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      967 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/docs/copyright.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1870 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/docs/getting_started.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)       99 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/glossary.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.168626 django_celery_results-2.5.1/docs/images/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3364 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/images/favicon.ico
+-rw-rw-r--   0 asif      (1000) asif      (1000)    26250 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/images/logo.png
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.168626 django_celery_results-2.5.1/docs/includes/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1035 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/docs/includes/installation.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      956 2023-05-08 14:17:24.000000 django_celery_results-2.5.1/docs/includes/introduction.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      555 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/docs/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2020 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/docs/injecting_metadata.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7253 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/docs/make.bat
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.168626 django_celery_results-2.5.1/docs/reference/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      321 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/reference/django_celery_results.backends.cache.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      330 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/reference/django_celery_results.backends.database.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/reference/django_celery_results.backends.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/reference/django_celery_results.managers.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/reference/django_celery_results.models.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/reference/django_celery_results.utils.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      348 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/docs/reference/index.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.168626 django_celery_results-2.5.1/docs/templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1479 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/docs/templates/readme.txt
+-rwxrwxr-x   0 asif      (1000) asif      (1000)      250 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/manage.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.172626 django_celery_results-2.5.1/requirements/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       34 2023-03-13 09:37:08.000000 django_celery_results-2.5.1/requirements/default.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       53 2023-03-13 09:37:08.000000 django_celery_results-2.5.1/requirements/docs.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       97 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/requirements/pkgutils.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       64 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/requirements/test-ci.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       32 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/requirements/test-django.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2023-03-13 09:37:08.000000 django_celery_results-2.5.1/requirements/test-django32.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2023-03-13 09:37:08.000000 django_celery_results-2.5.1/requirements/test-django40.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2023-03-13 09:37:08.000000 django_celery_results-2.5.1/requirements/test-django41.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      121 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/requirements/test-django42.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       82 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/requirements/test.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      378 2023-05-08 14:21:10.180626 django_celery_results-2.5.1/setup.cfg
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4557 2023-05-08 13:51:53.000000 django_celery_results-2.5.1/setup.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.172626 django_celery_results-2.5.1/t/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1322 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/conftest.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.172626 django_celery_results-2.5.1/t/integration/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/integration/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2256 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/integration/benchmark_models.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.176626 django_celery_results-2.5.1/t/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       46 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      314 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/proj/celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4262 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/proj/settings.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      118 2023-03-13 11:20:36.000000 django_celery_results-2.5.1/t/proj/urls.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      387 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/proj/wsgi.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.176626 django_celery_results-2.5.1/t/unit/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/unit/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-08 14:21:10.176626 django_celery_results-2.5.1/t/unit/backends/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/unit/backends/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3350 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/unit/backends/test_cache.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32299 2023-03-13 07:35:55.000000 django_celery_results-2.5.1/t/unit/backends/test_database.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1427 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/unit/test_migrations.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8977 2022-06-29 10:16:08.000000 django_celery_results-2.5.1/t/unit/test_models.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3995 2021-12-23 10:43:17.000000 django_celery_results-2.5.1/t/unit/test_views.py
```

### Comparing `django_celery_results-2.5.0/AUTHORS` & `django_celery_results-2.5.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/Changelog` & `django_celery_results-2.5.1/Changelog`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 .. _changelog:
 
 ================
  Change history
 ================
 
+.. _version-2.5.1:
+
+2.5.1
+=====
+:release-date: 2023-05-08 8:15 P.M. UTC+6:00
+:release-by: Asif Saif Uddin
+
+- Revert "feat: raw delete expired instead of Queryset.delete (#235)" partially.
+
+
 .. _version-2.5.0:
 
 2.5.0
 =====
 :release-date: 2023-03-13 5:45 P.M. UTC+6:00
 :release-by: Asif Saif Uddin
```

### Comparing `django_celery_results-2.5.0/LICENSE` & `django_celery_results-2.5.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Copyright (c) 2009-2012 Ask Solem.  All Rights Reserved.
 
 django-celery-results is licensed under The BSD License (3 Clause, also known as
 the new BSD license).  The license is an OSI approved Open Source
 license and is GPL-compatible(1).
 
 The license text can also be found here:
-http://www.opensource.org/licenses/BSD-3-Clause
+https://opensource.org/license/bsd-3-clause/
 
 License
 =======
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
     * Redistributions of source code must retain the above copyright
@@ -39,15 +39,15 @@
 Documentation License
 =====================
 
 The documentation portion of django-celery-results (the rendered contents of the
 "docs" directory of a software distribution or checkout) is supplied
 under the "Creative Commons Attribution-ShareAlike 4.0
 International" (CC BY-SA 4.0) License as described by
-http://creativecommons.org/licenses/by-sa/4.0/
+https://creativecommons.org/licenses/by-sa/4.0/
 
 Footnotes
 =========
 (1) A GPL-compatible license makes it possible to
     combine django-celery-results with other software that is released
     under the GPL, it does not mean that we're distributing
     django-celery-results under the GPL license.  The BSD license, unlike the GPL,
```

### Comparing `django_celery_results-2.5.0/PKG-INFO` & `django_celery_results-2.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: django_celery_results
-Version: 2.5.0
+Version: 2.5.1
 Summary: Celery result backends for Django.
 Home-page: https://github.com/celery/django-celery-results
 Author: Asif Saif Uddin, Ask Solem
-Author-email: auvipy@gmai.com, ask@celeryproject.org
+Author-email: auvipy@gmail.com
 License: BSD
+Project-URL: Documentation, https://django-celery-results.readthedocs.io/en/latest/
+Project-URL: Changelog, https://django-celery-results.readthedocs.io/en/latest/changelog.html
+Project-URL: Repository, https://github.com/celery/django-celery-results
 Keywords: celery django database result backend
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -34,18 +37,18 @@
 
 =====================================================================
  Celery Result Backends using the Django ORM/Cache framework.
 =====================================================================
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp|
 
-:Version: 2.5.0
-:Web: http://django-celery-results.readthedocs.io/
-:Download: http://pypi.python.org/pypi/django-celery-results
-:Source: http://github.com/celery/django-celery-results
+:Version: 2.5.1
+:Web: https://django-celery-results.readthedocs.io/
+:Download: https://pypi.python.org/pypi/django-celery-results
+:Source: https://github.com/celery/django-celery-results
 :Keywords: django, celery, database, results
 
 About
 =====
 
 This extension enables you to store Celery task results using the Django ORM.
 
@@ -56,15 +59,15 @@
 Installing
 ==========
 
 The installation instructions for this extension is available
 from the `Celery documentation`_
 
 .. _`Celery documentation`:
-    http://docs.celeryproject.org/en/latest/django/first-steps-with-django.html#django-celery-results-using-the-django-orm-cache-as-a-result-backend
+    https://docs.celeryproject.org/en/latest/django/first-steps-with-django.html#django-celery-results-using-the-django-orm-cache-as-a-result-backend
 
 .. _installation:
 
 Installation
 ============
 
 You can install django-celery-results either via the Python Package Index (PyPI)
@@ -76,15 +79,15 @@
 
 .. _installing-from-source:
 
 Downloading and installing from source
 --------------------------------------
 
 Download the latest version of django-celery-results from
-http://pypi.python.org/pypi/django-celery-results
+https://pypi.python.org/pypi/django-celery-results
 
 You can install it by doing the following,::
 
     $ tar xvfz django-celery-results-0.0.0.tar.gz
     $ cd django-celery-results-0.0.0
     $ python setup.py build
     # python setup.py install
@@ -133,24 +136,24 @@
 
 .. |license| image:: https://img.shields.io/pypi/l/django-celery-results.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/django-celery-results.svg
     :alt: django-celery-results can be installed via wheel
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyversion| image:: https://img.shields.io/pypi/pyversions/django-celery-results.svg
     :alt: Supported Python versions.
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyimp| image:: https://img.shields.io/pypi/implementation/django-celery-results.svg
     :alt: Support Python implementations.
-    :target: http://pypi.python.org/pypi/django-celery-results/
-    
+    :target: https://pypi.python.org/pypi/django-celery-results/
+
 django-celery-results for enterprise
 ------------------------------------
 
 Available as part of the Tidelift Subscription.
 
 The maintainer of django-celery-results and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source packages you use to build your applications. Save time, reduce risk, and improve code health, while paying the maintainer of the exact packages you use. `Learn more. <https://tidelift.com/subscription/pkg/pypi-django-celery-results?utm_source=pypi-django-celery-results&utm_medium=referral&utm_campaign=readme>`_
```

### Comparing `django_celery_results-2.5.0/README.rst` & `django_celery_results-2.5.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 =====================================================================
  Celery Result Backends using the Django ORM/Cache framework.
 =====================================================================
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp|
 
-:Version: 2.5.0
-:Web: http://django-celery-results.readthedocs.io/
-:Download: http://pypi.python.org/pypi/django-celery-results
-:Source: http://github.com/celery/django-celery-results
+:Version: 2.5.1
+:Web: https://django-celery-results.readthedocs.io/
+:Download: https://pypi.python.org/pypi/django-celery-results
+:Source: https://github.com/celery/django-celery-results
 :Keywords: django, celery, database, results
 
 About
 =====
 
 This extension enables you to store Celery task results using the Django ORM.
 
@@ -22,15 +22,15 @@
 Installing
 ==========
 
 The installation instructions for this extension is available
 from the `Celery documentation`_
 
 .. _`Celery documentation`:
-    http://docs.celeryproject.org/en/latest/django/first-steps-with-django.html#django-celery-results-using-the-django-orm-cache-as-a-result-backend
+    https://docs.celeryproject.org/en/latest/django/first-steps-with-django.html#django-celery-results-using-the-django-orm-cache-as-a-result-backend
 
 .. _installation:
 
 Installation
 ============
 
 You can install django-celery-results either via the Python Package Index (PyPI)
@@ -42,15 +42,15 @@
 
 .. _installing-from-source:
 
 Downloading and installing from source
 --------------------------------------
 
 Download the latest version of django-celery-results from
-http://pypi.python.org/pypi/django-celery-results
+https://pypi.python.org/pypi/django-celery-results
 
 You can install it by doing the following,::
 
     $ tar xvfz django-celery-results-0.0.0.tar.gz
     $ cd django-celery-results-0.0.0
     $ python setup.py build
     # python setup.py install
@@ -99,24 +99,24 @@
 
 .. |license| image:: https://img.shields.io/pypi/l/django-celery-results.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/django-celery-results.svg
     :alt: django-celery-results can be installed via wheel
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyversion| image:: https://img.shields.io/pypi/pyversions/django-celery-results.svg
     :alt: Supported Python versions.
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyimp| image:: https://img.shields.io/pypi/implementation/django-celery-results.svg
     :alt: Support Python implementations.
-    :target: http://pypi.python.org/pypi/django-celery-results/
-    
+    :target: https://pypi.python.org/pypi/django-celery-results/
+
 django-celery-results for enterprise
 ------------------------------------
 
 Available as part of the Tidelift Subscription.
 
 The maintainer of django-celery-results and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source packages you use to build your applications. Save time, reduce risk, and improve code health, while paying the maintainer of the exact packages you use. `Learn more. <https://tidelift.com/subscription/pkg/pypi-django-celery-results?utm_source=pypi-django-celery-results&utm_medium=referral&utm_campaign=readme>`_
```

### Comparing `django_celery_results-2.5.0/django_celery_results/__init__.py` & `django_celery_results-2.5.1/django_celery_results/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Celery result backends for Django."""
 # :copyright: (c) 2016, Ask Solem.
+# :copyright: (c) 2017-2033, Asif Saif Uddin.
 #             All rights reserved.
 # :license:   BSD (3 Clause), see LICENSE for more details.
 
 import re
 from collections import namedtuple
 
 import django
 
-__version__ = '2.5.0'
+__version__ = '2.5.1'
 __author__ = 'Asif Saif Uddin, Ask Solem'
-__contact__ = 'auvipy@gmai.com, ask@celeryproject.org'
+__contact__ = 'auvipy@gmail.com'
 __homepage__ = 'https://github.com/celery/django-celery-results'
 __docformat__ = 'restructuredtext'
 
 # -eof meta-
 
 version_info_t = namedtuple('version_info_t', (
     'major', 'minor', 'micro', 'releaselevel', 'serial',
```

### Comparing `django_celery_results-2.5.0/django_celery_results/admin.py` & `django_celery_results-2.5.1/django_celery_results/admin.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/backends/cache.py` & `django_celery_results-2.5.1/django_celery_results/backends/cache.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/backends/database.py` & `django_celery_results-2.5.1/django_celery_results/backends/database.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/locale/es/LC_MESSAGES/django.po` & `django_celery_results-2.5.1/django_celery_results/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/locale/pt_BR/LC_MESSAGES/django.po` & `django_celery_results-2.5.1/django_celery_results/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/locale/ru/LC_MESSAGES/django.po` & `django_celery_results-2.5.1/django_celery_results/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/locale/zh_Hans/LC_MESSAGES/django.po` & `django_celery_results-2.5.1/django_celery_results/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/managers.py` & `django_celery_results-2.5.1/django_celery_results/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import wraps
 from itertools import count
 
 from celery.utils.time import maybe_timedelta
 from django.conf import settings
 from django.db import connections, models, router, transaction
 
-from .utils import now, raw_delete
+from .utils import now
 
 W_ISOLATION_REP = """
 Polling results with transaction isolation level 'repeatable-read'
 within the same transaction may give outdated results.
 
 Be sure to commit the transaction for each poll iteration.
 """
@@ -83,15 +83,15 @@
     def get_all_expired(self, expires):
         """Get all expired results."""
         return self.filter(date_done__lt=now() - maybe_timedelta(expires))
 
     def delete_expired(self, expires):
         """Delete all expired results."""
         with transaction.atomic(using=self.db):
-            raw_delete(queryset=self.get_all_expired(expires))
+            self.get_all_expired(expires).delete()
 
 
 class TaskResultManager(ResultManager):
     """Manager for :class:`~.models.TaskResult` models."""
 
     _last_id = None
```

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0001_initial.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0002_add_task_name_args_kwargs.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0002_add_task_name_args_kwargs.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0004_auto_20190516_0412.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0004_auto_20190516_0412.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0005_taskresult_worker.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0005_taskresult_worker.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0006_taskresult_date_created.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0006_taskresult_date_created.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0008_chordcounter.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0008_chordcounter.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0009_groupresult.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0009_groupresult.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0010_remove_duplicate_indices.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0010_remove_duplicate_indices.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/migrations/0011_taskresult_periodic_task_name.py` & `django_celery_results-2.5.1/django_celery_results/migrations/0011_taskresult_periodic_task_name.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/models.py` & `django_celery_results-2.5.1/django_celery_results/models.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/urls.py` & `django_celery_results-2.5.1/django_celery_results/urls.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results/views.py` & `django_celery_results-2.5.1/django_celery_results/views.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/django_celery_results.egg-info/PKG-INFO` & `django_celery_results-2.5.1/django_celery_results.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: django-celery-results
-Version: 2.5.0
+Version: 2.5.1
 Summary: Celery result backends for Django.
 Home-page: https://github.com/celery/django-celery-results
 Author: Asif Saif Uddin, Ask Solem
-Author-email: auvipy@gmai.com, ask@celeryproject.org
+Author-email: auvipy@gmail.com
 License: BSD
+Project-URL: Documentation, https://django-celery-results.readthedocs.io/en/latest/
+Project-URL: Changelog, https://django-celery-results.readthedocs.io/en/latest/changelog.html
+Project-URL: Repository, https://github.com/celery/django-celery-results
 Keywords: celery django database result backend
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -34,18 +37,18 @@
 
 =====================================================================
  Celery Result Backends using the Django ORM/Cache framework.
 =====================================================================
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp|
 
-:Version: 2.5.0
-:Web: http://django-celery-results.readthedocs.io/
-:Download: http://pypi.python.org/pypi/django-celery-results
-:Source: http://github.com/celery/django-celery-results
+:Version: 2.5.1
+:Web: https://django-celery-results.readthedocs.io/
+:Download: https://pypi.python.org/pypi/django-celery-results
+:Source: https://github.com/celery/django-celery-results
 :Keywords: django, celery, database, results
 
 About
 =====
 
 This extension enables you to store Celery task results using the Django ORM.
 
@@ -56,15 +59,15 @@
 Installing
 ==========
 
 The installation instructions for this extension is available
 from the `Celery documentation`_
 
 .. _`Celery documentation`:
-    http://docs.celeryproject.org/en/latest/django/first-steps-with-django.html#django-celery-results-using-the-django-orm-cache-as-a-result-backend
+    https://docs.celeryproject.org/en/latest/django/first-steps-with-django.html#django-celery-results-using-the-django-orm-cache-as-a-result-backend
 
 .. _installation:
 
 Installation
 ============
 
 You can install django-celery-results either via the Python Package Index (PyPI)
@@ -76,15 +79,15 @@
 
 .. _installing-from-source:
 
 Downloading and installing from source
 --------------------------------------
 
 Download the latest version of django-celery-results from
-http://pypi.python.org/pypi/django-celery-results
+https://pypi.python.org/pypi/django-celery-results
 
 You can install it by doing the following,::
 
     $ tar xvfz django-celery-results-0.0.0.tar.gz
     $ cd django-celery-results-0.0.0
     $ python setup.py build
     # python setup.py install
@@ -133,24 +136,24 @@
 
 .. |license| image:: https://img.shields.io/pypi/l/django-celery-results.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/django-celery-results.svg
     :alt: django-celery-results can be installed via wheel
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyversion| image:: https://img.shields.io/pypi/pyversions/django-celery-results.svg
     :alt: Supported Python versions.
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyimp| image:: https://img.shields.io/pypi/implementation/django-celery-results.svg
     :alt: Support Python implementations.
-    :target: http://pypi.python.org/pypi/django-celery-results/
-    
+    :target: https://pypi.python.org/pypi/django-celery-results/
+
 django-celery-results for enterprise
 ------------------------------------
 
 Available as part of the Tidelift Subscription.
 
 The maintainer of django-celery-results and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source packages you use to build your applications. Save time, reduce risk, and improve code health, while paying the maintainer of the exact packages you use. `Learn more. <https://tidelift.com/subscription/pkg/pypi-django-celery-results?utm_source=pypi-django-celery-results&utm_medium=referral&utm_campaign=readme>`_
```

### Comparing `django_celery_results-2.5.0/django_celery_results.egg-info/SOURCES.txt` & `django_celery_results-2.5.1/django_celery_results.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,12 +81,11 @@
 t/proj/celery.py
 t/proj/settings.py
 t/proj/urls.py
 t/proj/wsgi.py
 t/unit/__init__.py
 t/unit/test_migrations.py
 t/unit/test_models.py
-t/unit/test_utils.py
 t/unit/test_views.py
 t/unit/backends/__init__.py
 t/unit/backends/test_cache.py
 t/unit/backends/test_database.py
```

### Comparing `django_celery_results-2.5.0/docs/Makefile` & `django_celery_results-2.5.1/docs/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 PAPER         =
 BUILDDIR      = _build
 
 # User-friendly check for sphinx-build
 ifeq ($(shell which $(SPHINXBUILD) >/dev/null 2>&1; echo $$?), 1)
-	$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don\'t have Sphinx installed, grab it from http://sphinx-doc.org/)
+	$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don\'t have Sphinx installed, grab it from https://www.sphinx-doc.org/)
 endif
 
 # Internal variables.
 PAPEROPT_a4     = -D latex_paper_size=a4
 PAPEROPT_letter = -D latex_paper_size=letter
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) .
 # the i18n builder cannot share the environment and doctrees with the others
```

### Comparing `django_celery_results-2.5.0/docs/conf.py` & `django_celery_results-2.5.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sphinx_celery import conf
 
 globals().update(conf.build_config(
     'django_celery_results', __file__,
     project='django_celery_results',
     # version_dev='2.0',
     # version_stable='1.4',
-    canonical_url='http://django-celery-results.readthedocs.io',
+    canonical_url='https://django-celery-results.readthedocs.io',
     webdomain='',
     github_project='celery/django-celery-results',
     copyright='2009-2022',
     django_settings='proj.settings',
     include_intersphinx={'python', 'sphinx', 'django', 'celery'},
     path_additions=[os.path.join(os.pardir, 't')],
     extra_extensions=['sphinx.ext.napoleon'],
```

### Comparing `django_celery_results-2.5.0/docs/copyright.rst` & `django_celery_results-2.5.1/docs/copyright.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 .. |copy|   unicode:: U+000A9 .. COPYRIGHT SIGN
 
 Copyright |copy| 2016, Ask Solem
 
 All rights reserved.  This material may be copied or distributed only
 subject to the terms and conditions set forth in the `Creative Commons
 Attribution-ShareAlike 4.0 International
-<http://creativecommons.org/licenses/by-sa/4.0/legalcode>`_ license.
+<https://creativecommons.org/licenses/by-sa/4.0/legalcode>`_ license.
 
 You may share and adapt the material, even for commercial purposes, but
 you must give the original author credit.
 If you alter, transform, or build upon this
 work, you may distribute the resulting work only under the same license or
 a license compatible to this one.
 
 .. note::
 
    While the django-celery-results *documentation* is offered under the
    Creative Commons *Attribution-ShareAlike 4.0 International* license
    the django-celery-results *software* is offered under the
-   `BSD License (3 Clause) <http://www.opensource.org/licenses/BSD-3-Clause>`_
+   `BSD License (3 Clause) <https://opensource.org/license/bsd-3-clause/>`_
```

### Comparing `django_celery_results-2.5.0/docs/getting_started.rst` & `django_celery_results-2.5.1/docs/getting_started.rst`

 * *Files 11% similar despite different names*

```diff
@@ -56,7 +56,13 @@
         }
 
     If you want to include extended information about your tasks remember to enable the :setting:`result_extended` setting.
 
     .. code-block:: python
 
         CELERY_RESULT_EXTENDED = True
+
+    If you want to track the execution duration of your tasks (by comparing `date_created` and `date_done` in TaskResult), enable the :setting:`track_started` setting.
+    
+    .. code-block:: python
+
+        CELERY_TASK_TRACK_STARTED = True
```

### Comparing `django_celery_results-2.5.0/docs/images/favicon.ico` & `django_celery_results-2.5.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/docs/images/logo.png` & `django_celery_results-2.5.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/docs/includes/installation.txt` & `django_celery_results-2.5.1/docs/includes/installation.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 .. _installing-from-source:
 
 Downloading and installing from source
 --------------------------------------
 
 Download the latest version of django-celery-results from
-http://pypi.python.org/pypi/django-celery-results
+https://pypi.python.org/pypi/django-celery-results
 
 You can install it by doing the following,::
 
     $ tar xvfz django-celery-results-0.0.0.tar.gz
     $ cd django-celery-results-0.0.0
     $ python setup.py build
     # python setup.py install
```

### Comparing `django_celery_results-2.5.0/docs/includes/introduction.txt` & `django_celery_results-2.5.1/docs/includes/introduction.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-:Version: 2.5.0
-:Web: http://django-celery-results.readthedocs.io/
-:Download: http://pypi.python.org/pypi/django-celery-results
-:Source: http://github.com/celery/django-celery-results
+:Version: 2.5.1
+:Web: https://django-celery-results.readthedocs.io/
+:Download: https://pypi.python.org/pypi/django-celery-results
+:Source: https://github.com/celery/django-celery-results
 :Keywords: django, celery, database, results
 
 About
 =====
 
 This extension enables you to store Celery task and group results using the Django ORM.
```

### Comparing `django_celery_results-2.5.0/docs/index.rst` & `django_celery_results-2.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/docs/injecting_metadata.rst` & `django_celery_results-2.5.1/docs/injecting_metadata.rst`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/docs/make.bat` & `django_celery_results-2.5.1/docs/make.bat`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
 	echo.may add the Sphinx directory to PATH.
 	echo.
 	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
+	echo.https://www.sphinx-doc.org/
 	exit /b 1
 )
 
 :sphinx_ok
 
 
 if "%1" == "html" (
```

### Comparing `django_celery_results-2.5.0/docs/templates/readme.txt` & `django_celery_results-2.5.1/docs/templates/readme.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 .. |license| image:: https://img.shields.io/pypi/l/django-celery-results.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/django-celery-results.svg
     :alt: django-celery-results can be installed via wheel
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyversion| image:: https://img.shields.io/pypi/pyversions/django-celery-results.svg
     :alt: Supported Python versions.
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
 
 .. |pyimp| image:: https://img.shields.io/pypi/implementation/django-celery-results.svg
     :alt: Support Python implementations.
-    :target: http://pypi.python.org/pypi/django-celery-results/
+    :target: https://pypi.python.org/pypi/django-celery-results/
```

### Comparing `django_celery_results-2.5.0/setup.py` & `django_celery_results-2.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 # -*- Long Description -*-
 
 
 if os.path.exists('README.rst'):
     long_description = codecs.open('README.rst', 'r', 'utf-8').read()
 else:
-    long_description = f'See http://pypi.python.org/pypi/{NAME}'
+    long_description = f'See https://pypi.python.org/pypi/{NAME}'
 
 # -*- %%% -*-
 
 
 class pytest(setuptools.command.test.test):
     user_options = [('pytest-args=', 'a', 'Arguments to pass to pytest')]
 
@@ -137,14 +137,24 @@
     description=meta['doc'],
     long_description=long_description,
     long_description_content_type='text/x-rst',
     keywords='celery django database result backend',
     author=meta['author'],
     author_email=meta['contact'],
     url=meta['homepage'],
+    project_urls={
+        'Documentation': (
+            'https://django-celery-results.readthedocs.io/en/latest/'
+        ),
+        'Changelog': (
+            'https://django-celery-results.readthedocs.io/en/latest/'
+            'changelog.html'
+        ),
+        'Repository': 'https://github.com/celery/django-celery-results',
+    },
     platforms=['any'],
     license='BSD',
     classifiers=classifiers,
     install_requires=reqs('default.txt'),
     tests_require=reqs('test.txt') + reqs('test-django.txt'),
     cmdclass={'test': pytest},
     entry_points={
```

### Comparing `django_celery_results-2.5.0/t/conftest.py` & `django_celery_results-2.5.1/t/conftest.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/t/integration/benchmark_models.py` & `django_celery_results-2.5.1/t/integration/benchmark_models.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/t/proj/settings.py` & `django_celery_results-2.5.1/t/proj/settings.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/t/unit/backends/test_cache.py` & `django_celery_results-2.5.1/t/unit/backends/test_cache.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/t/unit/backends/test_database.py` & `django_celery_results-2.5.1/t/unit/backends/test_database.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/t/unit/test_migrations.py` & `django_celery_results-2.5.1/t/unit/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/t/unit/test_models.py` & `django_celery_results-2.5.1/t/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `django_celery_results-2.5.0/t/unit/test_views.py` & `django_celery_results-2.5.1/t/unit/test_views.py`

 * *Files identical despite different names*

