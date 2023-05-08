# Comparing `tmp/croydon-0.9.0.tar.gz` & `tmp/croydon-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croydon-0.9.0.tar", last modified: Mon Apr 10 10:23:41 2023, max compression
+gzip compressed data, was "croydon-0.9.1.tar", last modified: Mon Apr 10 10:41:45 2023, max compression
```

## Comparing `croydon-0.9.0.tar` & `croydon-0.9.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.316404 croydon-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-10 10:23:34.000000 croydon-0.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-04-10 10:23:34.000000 croydon-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-10 10:23:41.316404 croydon-0.9.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.293403 croydon-0.9.0/croydon/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/baseapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.297403 croydon-0.9.0/croydon/cache/
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/cache/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/cache/abc.py
--rw-rw-rw-   0 root         (0) root         (0)     3227 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/cache/memcached.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/cache/no_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/cache/simple.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.298403 croydon-0.9.0/croydon/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/commands/init.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/config.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/context.py
--rw-rw-rw-   0 root         (0) root         (0)    10824 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/db.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.301403 croydon-0.9.0/croydon/models/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8871 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/counter.py
--rw-rw-rw-   0 root         (0) root         (0)    11546 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/index.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/meta_model.py
--rw-rw-rw-   0 root         (0) root         (0)     8869 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/storable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/models/submodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.303403 croydon-0.9.0/croydon/taskq/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/taskq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/taskq/base_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     3130 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/taskq/mongo_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/taskq/task.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/taskq/types.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/taskq/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.305404 croydon-0.9.0/croydon/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.306404 croydon-0.9.0/croydon/templates/app/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.308404 croydon-0.9.0/croydon/templates/app/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/commands/dev.py
--rw-rw-rw-   0 root         (0) root         (0)     1240 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/commands/index.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/commands/prod.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/commands/shell.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/commands/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.309404 croydon-0.9.0/croydon/templates/app/controllers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.309404 croydon-0.9.0/croydon/templates/app/controllers/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/controllers/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.310404 croydon-0.9.0/croydon/templates/app/controllers/api/v1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/controllers/api/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/controllers/api/v1/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.311404 croydon-0.9.0/croydon/templates/app/controllers/api/v1/response_types/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/controllers/api/v1/response_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/controllers/api/v1/response_types/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/extractors.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.312404 croydon-0.9.0/croydon/templates/app/models/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/models/session.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/models/token.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.313404 croydon-0.9.0/croydon/templates/app/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/tasks/ping_task.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/app/tasks/worker.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/crcmd.py
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/development.toml
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/production.toml
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/staging.toml
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/templates/testing.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.316404 croydon-0.9.0/croydon/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/tests/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/tests/mongo_mock_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/tests/test_base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/tests/test_storable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5546 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/tests/test_submodel.py
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/tests/test_validators.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/types.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-10 10:23:34.000000 croydon-0.9.0/croydon/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:23:41.295403 croydon-0.9.0/croydon.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-10 10:23:41.000000 croydon-0.9.0/croydon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2282 2023-04-10 10:23:41.000000 croydon-0.9.0/croydon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 10:23:41.000000 croydon-0.9.0/croydon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-10 10:23:41.000000 croydon-0.9.0/croydon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-10 10:23:41.000000 croydon-0.9.0/croydon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-10 10:23:41.000000 croydon-0.9.0/croydon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 10:23:41.317404 croydon-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-10 10:23:34.000000 croydon-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.597551 croydon-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-10 10:41:38.000000 croydon-0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-04-10 10:41:38.000000 croydon-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-10 10:41:45.596551 croydon-0.9.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.577550 croydon-0.9.1/croydon/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/baseapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.580550 croydon-0.9.1/croydon/cache/
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/cache/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/cache/abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/cache/memcached.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/cache/no_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/cache/simple.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.581550 croydon-0.9.1/croydon/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/commands/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10824 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     2745 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.584550 croydon-0.9.1/croydon/models/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8871 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/counter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11546 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/meta_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8869 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/storable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/models/submodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.586550 croydon-0.9.1/croydon/taskq/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/taskq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/taskq/base_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/taskq/mongo_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/taskq/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/taskq/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/taskq/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.587550 croydon-0.9.1/croydon/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.588550 croydon-0.9.1/croydon/templates/app/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.590551 croydon-0.9.1/croydon/templates/app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/commands/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/commands/index.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/commands/prod.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/commands/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/commands/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.590551 croydon-0.9.1/croydon/templates/app/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.590551 croydon-0.9.1/croydon/templates/app/controllers/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/controllers/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.591550 croydon-0.9.1/croydon/templates/app/controllers/api/v1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/controllers/api/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/controllers/api/v1/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.592551 croydon-0.9.1/croydon/templates/app/controllers/api/v1/response_types/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/controllers/api/v1/response_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/controllers/api/v1/response_types/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/extractors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.593551 croydon-0.9.1/croydon/templates/app/models/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      693 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/models/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/models/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.594551 croydon-0.9.1/croydon/templates/app/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/tasks/ping_task.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/app/tasks/worker.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/crcmd.py
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/development.toml
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/production.toml
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/staging.toml
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/templates/testing.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.596551 croydon-0.9.1/croydon/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/tests/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/tests/mongo_mock_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/tests/test_base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/tests/test_storable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5546 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/tests/test_submodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/tests/test_validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-10 10:41:38.000000 croydon-0.9.1/croydon/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:41:45.579550 croydon-0.9.1/croydon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-10 10:41:45.000000 croydon-0.9.1/croydon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2282 2023-04-10 10:41:45.000000 croydon-0.9.1/croydon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 10:41:45.000000 croydon-0.9.1/croydon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-10 10:41:45.000000 croydon-0.9.1/croydon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-10 10:41:45.000000 croydon-0.9.1/croydon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-10 10:41:45.000000 croydon-0.9.1/croydon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 10:41:45.597551 croydon-0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-10 10:41:38.000000 croydon-0.9.1/setup.py
```

### Comparing `croydon-0.9.0/LICENSE` & `croydon-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/baseapp.py` & `croydon-0.9.1/croydon/baseapp.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/cache/memcached.py` & `croydon-0.9.1/croydon/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/cache/simple.py` & `croydon-0.9.1/croydon/cache/simple.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/command.py` & `croydon-0.9.1/croydon/command.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/commands/init.py` & `croydon-0.9.1/croydon/commands/init.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/config.py` & `croydon-0.9.1/croydon/config.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/context.py` & `croydon-0.9.1/croydon/context.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/db.py` & `croydon-0.9.1/croydon/db.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/decorators.py` & `croydon-0.9.1/croydon/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         cache_key = f"{self.__class__.__name__}.{self.id}.{func.__name__}"
 
         t1 = time()
         value = await ctx.cache_l1.get(cache_key)
         if value:
             td = time() - t1
             ctx.log.debug(
-                "%s L2 hit %s %.3f secs", ctx.cache_l2.NAME, cache_key, td
+                "%s L1 hit %s %.3f secs", ctx.cache_l1.NAME, cache_key, td
             )
             return value
 
         t1 = time()
         value = await ctx.cache_l2.get(cache_key)
         if value:
             td = time() - t1
```

### Comparing `croydon-0.9.0/croydon/errors.py` & `croydon-0.9.1/croydon/errors.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/models/base_model.py` & `croydon-0.9.1/croydon/models/base_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/models/counter.py` & `croydon-0.9.1/croydon/models/counter.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/models/fields.py` & `croydon-0.9.1/croydon/models/fields.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/models/index.py` & `croydon-0.9.1/croydon/models/index.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/models/meta_model.py` & `croydon-0.9.1/croydon/models/meta_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/models/storable_model.py` & `croydon-0.9.1/croydon/models/storable_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/models/submodel.py` & `croydon-0.9.1/croydon/models/submodel.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/taskq/base_queue.py` & `croydon-0.9.1/croydon/taskq/base_queue.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/taskq/mongo_queue.py` & `croydon-0.9.1/croydon/taskq/mongo_queue.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/taskq/task.py` & `croydon-0.9.1/croydon/taskq/task.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/taskq/types.py` & `croydon-0.9.1/croydon/taskq/types.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/commands/dev.py` & `croydon-0.9.1/croydon/templates/app/commands/dev.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/commands/index.py` & `croydon-0.9.1/croydon/templates/app/commands/index.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/commands/prod.py` & `croydon-0.9.1/croydon/templates/app/commands/prod.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/commands/shell.py` & `croydon-0.9.1/croydon/templates/app/commands/shell.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/controllers/api/v1/account.py` & `croydon-0.9.1/croydon/templates/app/controllers/api/v1/account.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/controllers/api/v1/response_types/account.py` & `croydon-0.9.1/croydon/templates/app/controllers/api/v1/response_types/account.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/extractors.py` & `croydon-0.9.1/croydon/templates/app/extractors.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/middleware.py` & `croydon-0.9.1/croydon/templates/app/middleware.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/models/session.py` & `croydon-0.9.1/croydon/templates/app/models/session.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/models/token.py` & `croydon-0.9.1/croydon/templates/app/models/token.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/app/models/user.py` & `croydon-0.9.1/croydon/templates/app/models/user.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/development.toml` & `croydon-0.9.1/croydon/templates/development.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/production.toml` & `croydon-0.9.1/croydon/templates/production.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/staging.toml` & `croydon-0.9.1/croydon/templates/staging.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/templates/testing.toml` & `croydon-0.9.1/croydon/templates/testing.toml`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/tests/mongo_mock_test.py` & `croydon-0.9.1/croydon/tests/mongo_mock_test.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/tests/test_base_model.py` & `croydon-0.9.1/croydon/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/tests/test_storable_model.py` & `croydon-0.9.1/croydon/tests/test_storable_model.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/tests/test_submodel.py` & `croydon-0.9.1/croydon/tests/test_submodel.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/tests/test_validators.py` & `croydon-0.9.1/croydon/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/types.py` & `croydon-0.9.1/croydon/types.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon/util.py` & `croydon-0.9.1/croydon/util.py`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/croydon.egg-info/SOURCES.txt` & `croydon-0.9.1/croydon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `croydon-0.9.0/setup.py` & `croydon-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="croydon",
-    version="0.9.0",
+    version="0.9.1",
     description="a micro webframework based on fastapi and motor",
     url="https://gitlab.com/viert/croydon",
     author="Pavel Vorobyov",
     author_email="aquavitale@yandex.ru",
     license="MIT",
     packages=[pkg for pkg in find_packages() if pkg.startswith("croydon")],
     include_package_data=True,
```

