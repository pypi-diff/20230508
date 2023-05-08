# Comparing `tmp/blueapps-4.7.0rc0.tar.gz` & `tmp/blueapps-4.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blueapps-4.7.0rc0.tar", last modified: Wed Apr 26 07:49:57 2023, max compression
+gzip compressed data, was "dist/blueapps-4.7.0rc1.tar", last modified: Mon May  8 11:22:04 2023, max compression
```

## Comparing `blueapps-4.7.0rc0.tar` & `blueapps-4.7.0rc1.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/middleware/
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/request_provider.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/middleware/bkui/
--rw-r--r--   0 root         (0) root         (0)     1296 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/bkui/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/bkui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/
--rw-r--r--   0 root         (0) root         (0)     2516 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/decorators.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7918 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/pxfilter.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/middleware/xss/utils.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/
--rw-r--r--   0 root         (0) root         (0)     1873 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/base.py
--rw-r--r--   0 root         (0) root         (0)     3778 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/lock.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/request_provider.py
--rw-r--r--   0 root         (0) root         (0)      884 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2887 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/jwt_client.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/time.py
--rw-r--r--   0 root         (0) root         (0)     8333 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/esbclient.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/fancy_dict.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/json.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/unique.py
--rw-r--r--   0 root         (0) root         (0)     3694 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/db.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/local.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)     1432 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/open/
--rw-r--r--   0 root         (0) root         (0)     1337 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/utils/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)     1427 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/utils/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/
--rw-r--r--   0 root         (0) root         (0)     1420 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/metric.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/assets/
--rw-r--r--   0 root         (0) root         (0)   169851 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/assets/local_jaeger.png
--rw-r--r--   0 root         (0) root         (0)     3491 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/docs/trace.md
--rw-r--r--   0 root         (0) root         (0)     1859 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/export.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/
--rw-r--r--   0 root         (0) root         (0)     2658 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/instrumentor.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/server.py
--rw-r--r--   0 root         (0) root         (0)     1109 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/celery.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrumentor.py
--rw-r--r--   0 root         (0) root         (0)     4919 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/setup.py
--rw-r--r--   0 root         (0) root         (0)      671 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/README.md
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/apps.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/celery.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/opentelemetry/utils.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/metrics.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/
--rw-r--r--   0 root         (0) root         (0)     1409 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/
--rw-r--r--   0 root         (0) root         (0)     5628 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/base.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/exceptions/middleware.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/handler/
--rw-r--r--   0 root         (0) root         (0)     1593 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/handler/wsgi.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/handler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/celery/
--rw-r--r--   0 root         (0) root         (0)      835 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/celery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/celery/celery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/core/sites/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/sites/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/core/sites/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/
--rw-r--r--   0 root         (0) root         (0)     5600 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/log.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/database.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/environ.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/validators.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/default_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      942 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/conf/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      986 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/conf/sites/tencent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/
--rw-r--r--   0 root         (0) root         (0)     5954 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/base.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/app.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/
--rw-r--r--   0 root         (0) root         (0)     6356 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/
--rw-r--r--   0 root         (0) root         (0)     2489 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celerybeat.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celery.py
--rw-r--r--   0 root         (0) root         (0)     7158 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/templates.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      833 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/bk_commands/test.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/test/
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/test/override_middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/dummy/
--rw-r--r--   0 root         (0) root         (0)     1005 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/dummy/dummy_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/dummy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4323 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/serializer_fields.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/filters.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/authentication.py
--rw-r--r--   0 root         (0) root         (0)     2039 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/pagination.py
--rw-r--r--   0 root         (0) root         (0)     5453 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/serializers.py
--rw-r--r--   0 root         (0) root         (0)     3234 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/utils/viewset_mixin.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/viewsets.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/README.md
--rw-r--r--   0 root         (0) root         (0)     2763 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/renderers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/swagger/
--rw-r--r--   0 root         (0) root         (0)     7127 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/swagger/schemas.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/contrib/drf/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/patch/
--rw-r--r--   0 root         (0) root         (0)     3773 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/log.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/settings_paas_services.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/patch/settings_open_saas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/
--rw-r--r--   0 root         (0) root         (0)     1046 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/decorators.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/management/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/management/commands/
--rw-r--r--   0 root         (0) root         (0)     1079 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/management/commands/apigw_clean_cache.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/apps.py
--rw-r--r--   0 root         (0) root         (0)     1287 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/utils/
--rw-r--r--   0 root         (0) root         (0)      940 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/utils/sms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/handlers/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6562 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/handlers/response.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/views.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/static/account/
--rw-r--r--   0 root         (0) root         (0)     2049 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/static/account/login.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/
--rw-r--r--   0 root         (0) root         (0)     3176 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7830 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/models.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_token/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/null/
--rw-r--r--   0 root         (0) root         (0)      941 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/null/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/
--rw-r--r--   0 root         (0) root         (0)     3634 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/models.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/forms.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/
--rw-r--r--   0 root         (0) root         (0)     4669 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/backends.py
--rw-r--r--   0 root         (0) root         (0)      907 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/weixin/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/
--rw-r--r--   0 root         (0) root         (0)     3337 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/backends.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/rio/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/
--rw-r--r--   0 root         (0) root         (0)     2307 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/
--rw-r--r--   0 root         (0) root         (0)     3668 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/middlewares.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/backends.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/models.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/components/ptlogin/forms.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/templates/account/
--rw-r--r--   0 root         (0) root         (0)     1905 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/templates/account/login_page.html
--rw-r--r--   0 root         (0) root         (0)     1355 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/templates/account/login_success.html
--rw-r--r--   0 root         (0) root         (0)     1946 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/readme.md
--rw-r--r--   0 root         (0) root         (0)     1249 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/backends.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/conf.py
--rw-r--r--   0 root         (0) root         (0)     8875 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/models.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/migrations/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0003_verifyinfo.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0002_init_superuser.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0004_create_cache_table.py
--rw-r--r--   0 root         (0) root         (0)     7369 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/migrations/0001_initial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/ieod/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/ieod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/ieod/conf.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/open/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/open/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/open/conf.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/account/sites/tencent/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/tencent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/account/sites/tencent/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/template/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps/template/backends/
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4226 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/backends/mako.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/blueapps/template/context_processors.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     4156 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/blueapps.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      833 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/test.py
--rw-r--r--   0 root         (0) root         (0)     4038 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/setup.py
--rw-r--r--   0 root         (0) root         (0)     3383 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/README.md
--rw-r--r--   0 root         (0) root         (0)     4156 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-26 07:49:57.000000 blueapps-4.7.0rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7810 2023-04-26 07:46:53.000000 blueapps-4.7.0rc0/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/middleware/
+-rw-r--r--   0 root         (0) root         (0)      842 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/request_provider.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/middleware/bkui/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/bkui/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/bkui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7918 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/pxfilter.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/middleware/xss/utils.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/base.py
+-rw-r--r--   0 root         (0) root         (0)     3778 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/lock.py
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/request_provider.py
+-rw-r--r--   0 root         (0) root         (0)      884 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/jwt_client.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/time.py
+-rw-r--r--   0 root         (0) root         (0)     8333 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/esbclient.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/fancy_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/json.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/unique.py
+-rw-r--r--   0 root         (0) root         (0)     3694 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/db.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/local.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/open/
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/open/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/utils/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/utils/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/metric.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/assets/
+-rw-r--r--   0 root         (0) root         (0)   169851 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/assets/local_jaeger.png
+-rw-r--r--   0 root         (0) root         (0)     3491 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/docs/trace.md
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/export.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/instrumentor.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/server.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/celery.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrumentor.py
+-rw-r--r--   0 root         (0) root         (0)     4919 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/setup.py
+-rw-r--r--   0 root         (0) root         (0)      671 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/README.md
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/apps.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/celery.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/opentelemetry/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/
+-rw-r--r--   0 root         (0) root         (0)     5628 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/base.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/exceptions/middleware.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/handler/
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/handler/wsgi.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/handler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/celery/
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/celery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/celery/celery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/core/sites/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/sites/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/core/sites/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/
+-rw-r--r--   0 root         (0) root         (0)     5600 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/log.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/database.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/environ.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/validators.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      942 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/open/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/conf/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      986 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/conf/sites/tencent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/
+-rw-r--r--   0 root         (0) root         (0)     5954 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/base.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/app.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/
+-rw-r--r--   0 root         (0) root         (0)     6356 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celerybeat.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celery.py
+-rw-r--r--   0 root         (0) root         (0)     7158 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/templates.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      833 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/bk_commands/test.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/test/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/test/override_middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/dummy/
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/dummy/dummy_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/dummy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/serializer_fields.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/filters.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/pagination.py
+-rw-r--r--   0 root         (0) root         (0)     5453 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/serializers.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/utils/viewset_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/viewsets.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/README.md
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/renderers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/swagger/
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/swagger/schemas.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/contrib/drf/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/patch/
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/log.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/settings_paas_services.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/patch/settings_open_saas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/management/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/management/commands/apigw_clean_cache.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/utils/
+-rw-r--r--   0 root         (0) root         (0)      940 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/utils/sms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/handlers/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6562 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/handlers/response.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/views.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/static/account/
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/static/account/login.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7830 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/models.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_token/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/null/
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/null/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/models.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/forms.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/backends.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/weixin/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/rio/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/
+-rw-r--r--   0 root         (0) root         (0)     3668 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/backends.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/models.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/components/ptlogin/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/templates/account/
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/templates/account/login_page.html
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/templates/account/login_success.html
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/readme.md
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/backends.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/conf.py
+-rw-r--r--   0 root         (0) root         (0)     8875 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/models.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0003_verifyinfo.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0002_init_superuser.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0004_create_cache_table.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/migrations/0001_initial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/ieod/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/ieod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/ieod/conf.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/open/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/open/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/open/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/account/sites/tencent/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/tencent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/account/sites/tencent/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/template/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps/template/backends/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/backends/mako.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/blueapps/template/context_processors.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/blueapps.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      833 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/test.py
+-rw-r--r--   0 root         (0) root         (0)     4038 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/README.md
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-08 11:22:04.000000 blueapps-4.7.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     7810 2023-05-08 11:19:09.000000 blueapps-4.7.0rc1/LICENSE.txt
```

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/request_provider.py` & `blueapps-4.7.0rc1/blueapps/middleware/request_provider.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/__init__.py` & `blueapps-4.7.0rc1/blueapps/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/bkui/middlewares.py` & `blueapps-4.7.0rc1/blueapps/middleware/bkui/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/bkui/__init__.py` & `blueapps-4.7.0rc1/blueapps/middleware/bkui/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/xss/decorators.py` & `blueapps-4.7.0rc1/blueapps/middleware/xss/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/xss/middlewares.py` & `blueapps-4.7.0rc1/blueapps/middleware/xss/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/xss/__init__.py` & `blueapps-4.7.0rc1/blueapps/middleware/xss/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/xss/pxfilter.py` & `blueapps-4.7.0rc1/blueapps/middleware/xss/pxfilter.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/middleware/xss/utils.py` & `blueapps-4.7.0rc1/blueapps/middleware/xss/utils.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/__init__.py` & `blueapps-4.7.0rc1/blueapps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-VERSION = "4.7.0rc0"
+VERSION = "4.7.0rc1"
 __version__ = VERSION
 
 
 RUN_VER = ""
 
 
 def get_run_ver():
```

### Comparing `blueapps-4.7.0rc0/blueapps/utils/base.py` & `blueapps-4.7.0rc1/blueapps/utils/base.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/lock.py` & `blueapps-4.7.0rc1/blueapps/utils/lock.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/request_provider.py` & `blueapps-4.7.0rc1/blueapps/utils/request_provider.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/logger.py` & `blueapps-4.7.0rc1/blueapps/utils/logger.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/__init__.py` & `blueapps-4.7.0rc1/blueapps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/jwt_client.py` & `blueapps-4.7.0rc1/blueapps/utils/jwt_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/constants.py` & `blueapps-4.7.0rc1/blueapps/utils/constants.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/tools.py` & `blueapps-4.7.0rc1/blueapps/utils/tools.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/time.py` & `blueapps-4.7.0rc1/blueapps/utils/time.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/esbclient.py` & `blueapps-4.7.0rc1/blueapps/utils/esbclient.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/fancy_dict.py` & `blueapps-4.7.0rc1/blueapps/utils/fancy_dict.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/json.py` & `blueapps-4.7.0rc1/blueapps/utils/json.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/unique.py` & `blueapps-4.7.0rc1/blueapps/utils/unique.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/db.py` & `blueapps-4.7.0rc1/blueapps/utils/db.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/local.py` & `blueapps-4.7.0rc1/blueapps/utils/local.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/cache.py` & `blueapps-4.7.0rc1/blueapps/utils/cache.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/sites/ieod/__init__.py` & `blueapps-4.7.0rc1/blueapps/utils/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/sites/__init__.py` & `blueapps-4.7.0rc1/blueapps/utils/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/sites/open/__init__.py` & `blueapps-4.7.0rc1/blueapps/utils/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/utils/sites/tencent/__init__.py` & `blueapps-4.7.0rc1/blueapps/utils/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/docs/metric.md` & `blueapps-4.7.0rc1/blueapps/opentelemetry/docs/metric.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/docs/assets/local_jaeger.png` & `blueapps-4.7.0rc1/blueapps/opentelemetry/docs/assets/local_jaeger.png`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/docs/trace.md` & `blueapps-4.7.0rc1/blueapps/opentelemetry/docs/trace.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/export.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/export.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/middlewares.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/__init__.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/instrumentor.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/instrumentor.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/server.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/server.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/metrics/celery.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/metrics/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/__init__.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/instrumentor.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/instrumentor.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/setup.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/setup.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/README.md` & `blueapps-4.7.0rc1/blueapps/opentelemetry/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/constants.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/constants.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/apps.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/apps.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/__init__.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/instrument_app/celery.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/instrument_app/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/opentelemetry/utils.py` & `blueapps-4.7.0rc1/blueapps/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/metrics.py` & `blueapps-4.7.0rc1/blueapps/metrics.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/settings.py` & `blueapps-4.7.0rc1/blueapps/settings.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/wsgi.py` & `blueapps-4.7.0rc1/blueapps/core/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/exceptions/base.py` & `blueapps-4.7.0rc1/blueapps/core/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/exceptions/__init__.py` & `blueapps-4.7.0rc1/blueapps/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/exceptions/middleware.py` & `blueapps-4.7.0rc1/blueapps/core/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/__init__.py` & `blueapps-4.7.0rc1/blueapps/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/handler/wsgi.py` & `blueapps-4.7.0rc1/blueapps/core/handler/wsgi.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/handler/__init__.py` & `blueapps-4.7.0rc1/blueapps/core/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/celery/__init__.py` & `blueapps-4.7.0rc1/blueapps/core/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/celery/celery.py` & `blueapps-4.7.0rc1/blueapps/core/celery/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/sites/__init__.py` & `blueapps-4.7.0rc1/blueapps/core/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/core/sites/middleware.py` & `blueapps-4.7.0rc1/blueapps/core/sites/middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/log.py` & `blueapps-4.7.0rc1/blueapps/conf/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/__init__.py` & `blueapps-4.7.0rc1/blueapps/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/database.py` & `blueapps-4.7.0rc1/blueapps/conf/database.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/environ.py` & `blueapps-4.7.0rc1/blueapps/conf/environ.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/validators.py` & `blueapps-4.7.0rc1/blueapps/conf/validators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/default_settings.py` & `blueapps-4.7.0rc1/blueapps/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/sites/ieod/__init__.py` & `blueapps-4.7.0rc1/blueapps/conf/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/sites/__init__.py` & `blueapps-4.7.0rc1/blueapps/conf/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/sites/open/__init__.py` & `blueapps-4.7.0rc1/blueapps/conf/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/conf/sites/tencent/__init__.py` & `blueapps-4.7.0rc1/blueapps/conf/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/base.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/base.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/app.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/app.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/__init__.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/migrate_from_djcelery_handler.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/handlers/__init__.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/migrate_from_djcelery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/__init__.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celerybeat.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celerybeat.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/commands/celery.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/management/templates.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/management/templates.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/__init__.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/bk_commands/test.py` & `blueapps-4.7.0rc1/blueapps/contrib/bk_commands/test.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/__init__.py` & `blueapps-4.7.0rc1/blueapps/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/test/override_middleware.py` & `blueapps-4.7.0rc1/blueapps/contrib/test/override_middleware.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/dummy/dummy_client.py` & `blueapps-4.7.0rc1/blueapps/contrib/dummy/dummy_client.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/__init__.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/serializer.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/serializer.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/serializer_fields.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/serializer_fields.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/filters.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/filters.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/__init__.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/authentication.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/pagination.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/serializers.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/utils/viewset_mixin.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/utils/viewset_mixin.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/viewsets.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/README.md` & `blueapps-4.7.0rc1/blueapps/contrib/drf/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/renderers.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/renderers.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/swagger/schemas.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/swagger/schemas.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/contrib/drf/exception.py` & `blueapps-4.7.0rc1/blueapps/contrib/drf/exception.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/patch/log.py` & `blueapps-4.7.0rc1/blueapps/patch/log.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/patch/__init__.py` & `blueapps-4.7.0rc1/blueapps/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/patch/settings_paas_services.py` & `blueapps-4.7.0rc1/blueapps/patch/settings_paas_services.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/patch/settings_open_saas.py` & `blueapps-4.7.0rc1/blueapps/patch/settings_open_saas.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/decorators.py` & `blueapps-4.7.0rc1/blueapps/account/decorators.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/middlewares.py` & `blueapps-4.7.0rc1/blueapps/account/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/management/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/management/commands/apigw_clean_cache.py` & `blueapps-4.7.0rc1/blueapps/account/management/commands/apigw_clean_cache.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/management/commands/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/apps.py` & `blueapps-4.7.0rc1/blueapps/account/apps.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/utils/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/utils/http.py` & `blueapps-4.7.0rc1/blueapps/account/utils/http.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/utils/sms.py` & `blueapps-4.7.0rc1/blueapps/account/utils/sms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/handlers/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/handlers/response.py` & `blueapps-4.7.0rc1/blueapps/account/handlers/response.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/views.py` & `blueapps-4.7.0rc1/blueapps/account/views.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/urls.py` & `blueapps-4.7.0rc1/blueapps/account/urls.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/static/account/login.js` & `blueapps-4.7.0rc1/blueapps/account/static/account/login.js`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_token/middlewares.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_token/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_token/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_token/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_token/backends.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_token/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_token/models.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_token/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_token/forms.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_token/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/null/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/null/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/middlewares.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/backends.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/models.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_ticket/forms.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_ticket/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/weixin/middlewares.py` & `blueapps-4.7.0rc1/blueapps/account/components/weixin/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/weixin/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/weixin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/weixin/backends.py` & `blueapps-4.7.0rc1/blueapps/account/components/weixin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/weixin/forms.py` & `blueapps-4.7.0rc1/blueapps/account/components/weixin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/rio/middlewares.py` & `blueapps-4.7.0rc1/blueapps/account/components/rio/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/rio/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/rio/backends.py` & `blueapps-4.7.0rc1/blueapps/account/components/rio/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/rio/forms.py` & `blueapps-4.7.0rc1/blueapps/account/components/rio/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/middlewares.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/bk_jwt/backends.py` & `blueapps-4.7.0rc1/blueapps/account/components/bk_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/middlewares.py` & `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/middlewares.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/backends.py` & `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/models.py` & `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/components/ptlogin/forms.py` & `blueapps-4.7.0rc1/blueapps/account/components/ptlogin/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/admin.py` & `blueapps-4.7.0rc1/blueapps/account/admin.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/templates/account/login_page.html` & `blueapps-4.7.0rc1/blueapps/account/templates/account/login_page.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/templates/account/login_success.html` & `blueapps-4.7.0rc1/blueapps/account/templates/account/login_success.html`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/readme.md` & `blueapps-4.7.0rc1/blueapps/account/readme.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/backends.py` & `blueapps-4.7.0rc1/blueapps/account/backends.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/conf.py` & `blueapps-4.7.0rc1/blueapps/account/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/models.py` & `blueapps-4.7.0rc1/blueapps/account/models.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/forms.py` & `blueapps-4.7.0rc1/blueapps/account/forms.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/migrations/0003_verifyinfo.py` & `blueapps-4.7.0rc1/blueapps/account/migrations/0003_verifyinfo.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/migrations/0002_init_superuser.py` & `blueapps-4.7.0rc1/blueapps/account/migrations/0002_init_superuser.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/migrations/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/migrations/0004_create_cache_table.py` & `blueapps-4.7.0rc1/blueapps/account/migrations/0004_create_cache_table.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/migrations/0001_initial.py` & `blueapps-4.7.0rc1/blueapps/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/ieod/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/sites/ieod/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/ieod/conf.py` & `blueapps-4.7.0rc1/blueapps/account/sites/ieod/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/open/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/sites/open/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/open/conf.py` & `blueapps-4.7.0rc1/blueapps/account/sites/open/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/default.py` & `blueapps-4.7.0rc1/blueapps/account/sites/default.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/tencent/__init__.py` & `blueapps-4.7.0rc1/blueapps/account/sites/tencent/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/account/sites/tencent/conf.py` & `blueapps-4.7.0rc1/blueapps/account/sites/tencent/conf.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/template/__init__.py` & `blueapps-4.7.0rc1/blueapps/template/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/template/backends/__init__.py` & `blueapps-4.7.0rc1/blueapps/template/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/template/backends/mako.py` & `blueapps-4.7.0rc1/blueapps/template/backends/mako.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps/template/context_processors.py` & `blueapps-4.7.0rc1/blueapps/template/context_processors.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps.egg-info/SOURCES.txt` & `blueapps-4.7.0rc1/blueapps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/blueapps.egg-info/PKG-INFO` & `blueapps-4.7.0rc1/blueapps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.7.0rc0
+Version: 4.7.0rc1
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
```

### Comparing `blueapps-4.7.0rc0/blueapps.egg-info/requires.txt` & `blueapps-4.7.0rc1/blueapps.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Django<4.0.0,>=2.2.6
-mysqlclient<=2.0.3,>=1.4.4
+mysqlclient<=2.1.1,>=1.4.4
 bkoauth>=0.0.12
 MarkupSafe<2.0.0,>=1.1.1
 Mako<2.0,>=1.0.6
 requests<3.0.0,>=2.22.0
 python-json-logger>=0.1.7
 whitenoise<=5.2.0,>=3.3.0
 Werkzeug<2.0.0,>=1.0.0
```

### Comparing `blueapps-4.7.0rc0/test.py` & `blueapps-4.7.0rc1/test.py`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/setup.py` & `blueapps-4.7.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     #   py_modules=["my_module"],
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
         "Django>=2.2.6,<4.0.0",
-        "mysqlclient>=1.4.4,<=2.0.3",
+        "mysqlclient>=1.4.4,<=2.1.1",
         "bkoauth>=0.0.12",
         "MarkupSafe>=1.1.1,<2.0.0",
         "Mako>=1.0.6,<2.0",
         "requests>=2.22.0,<3.0.0",
         "python-json-logger>=0.1.7",
         "whitenoise>=3.3.0,<=5.2.0",
         "Werkzeug>=1.0.0,<2.0.0",
```

### Comparing `blueapps-4.7.0rc0/README.md` & `blueapps-4.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `blueapps-4.7.0rc0/PKG-INFO` & `blueapps-4.7.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapps
-Version: 4.7.0rc0
+Version: 4.7.0rc1
 Summary: development framework for blueking
 Home-page: https://github.com/TencentBlueKing/blueapps
 Author: blueking
 Author-email: blueking@tencent.com
 License: UNKNOWN
 Description: # 蓝鲸Python开发框架Blueapps
```

### Comparing `blueapps-4.7.0rc0/LICENSE.txt` & `blueapps-4.7.0rc1/LICENSE.txt`

 * *Files identical despite different names*

