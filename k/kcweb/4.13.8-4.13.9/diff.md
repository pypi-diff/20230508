# Comparing `tmp/kcweb-4.13.8.tar.gz` & `tmp/kcweb-4.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kcweb-4.13.8.tar", last modified: Sat Sep  4 15:57:52 2021, max compression
+gzip compressed data, was "dist/kcweb-4.13.9.tar", last modified: Sun Sep  5 11:10:54 2021, max compression
```

## Comparing `kcweb-4.13.8.tar` & `kcweb-4.13.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/
--rw-r--r--   0 root         (0) root         (0)       59 2021-09-04 15:57:52.000000 kcweb-4.13.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/
--rw-r--r--   0 root         (0) root         (0)       44 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/common/
--rw-r--r--   0 root         (0) root         (0)     2084 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/common/session.py
--rw-r--r--   0 root         (0) root         (0)      115 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3995 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/common/request.py
--rw-r--r--   0 root         (0) root         (0)    57879 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/common/autoload.py
--rw-r--r--   0 root         (0) root         (0)      142 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/common/globals.py
--rw-r--r--   0 root         (0) root         (0)    43137 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/tpl/
--rw-r--r--   0 root         (0) root         (0)      789 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/tpl/error.html
--rw-r--r--   0 root         (0) root         (0)     2069 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/tpl/err.html
--rw-r--r--   0 root         (0) root         (0)     2335 2021-09-04 15:46:18.000000 kcweb-4.13.8/kcweb/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/config/
--rw-r--r--   0 root         (0) root         (0)     5815 2021-09-04 15:46:18.000000 kcweb-4.13.8/kcweb/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/filetype/
--rw-r--r--   0 root         (0) root         (0)      223 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/filetype/types/
--rw-r--r--   0 root         (0) root         (0)     1448 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2312 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/font.py
--rw-r--r--   0 root         (0) root         (0)     3832 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/audio.py
--rw-r--r--   0 root         (0) root         (0)      928 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/isobmff.py
--rw-r--r--   0 root         (0) root         (0)      675 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/base.py
--rw-r--r--   0 root         (0) root         (0)     6337 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/image.py
--rw-r--r--   0 root         (0) root         (0)    12601 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/archive.py
--rw-r--r--   0 root         (0) root         (0)     5354 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/types/video.py
--rw-r--r--   0 root         (0) root         (0)     2521 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2122 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/filetype.py
--rw-r--r--   0 root         (0) root         (0)     1670 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/utils.py
--rw-r--r--   0 root         (0) root         (0)     2449 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/filetype/match.py
--rw-r--r--   0 root         (0) root         (0)     8807 2021-09-04 15:46:18.000000 kcweb-4.13.8/kcweb/utill/queues.py
--rw-r--r--   0 root         (0) root         (0)     1043 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/cache/
--rw-r--r--   0 root         (0) root         (0)    10147 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/cache/cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/rediss/
--rw-r--r--   0 root         (0) root         (0)    11358 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/sentinel.py
--rw-r--r--   0 root         (0) root         (0)      992 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      666 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/utils.py
--rw-r--r--   0 root         (0) root         (0)    47617 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/connection.py
--rw-r--r--   0 root         (0) root         (0)     4012 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/_compat.py
--rw-r--r--   0 root         (0) root         (0)    10835 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/lock.py
--rw-r--r--   0 root         (0) root         (0)   146593 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/client.py
--rw-r--r--   0 root         (0) root         (0)      992 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/rediss/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7868 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/redis.py
--rw-r--r--   0 root         (0) root         (0)     3564 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/dateutil/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/dateutil/tz/
--rw-r--r--   0 root         (0) root         (0)      551 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/tz/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2301 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/tz/_factories.py
--rw-r--r--   0 root         (0) root         (0)    12975 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/tz/_common.py
--rw-r--r--   0 root         (0) root         (0)    12935 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/tz/win.py
--rw-r--r--   0 root         (0) root         (0)    62446 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/tz/tz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/dateutil/parser/
--rw-r--r--   0 root         (0) root         (0)     1727 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13106 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/parser/isoparser.py
--rw-r--r--   0 root         (0) root         (0)    57682 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/parser/_parser.py
--rw-r--r--   0 root         (0) root         (0)       59 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/tzwin.py
--rw-r--r--   0 root         (0) root         (0)      222 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      116 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/dateutil/zoneinfo/
--rw-r--r--   0 root         (0) root         (0)     5889 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/zoneinfo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1719 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/zoneinfo/rebuild.py
--rw-r--r--   0 root         (0) root         (0)    24903 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/relativedelta.py
--rw-r--r--   0 root         (0) root         (0)      932 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/_common.py
--rw-r--r--   0 root         (0) root         (0)     1963 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/utils.py
--rw-r--r--   0 root         (0) root         (0)    66546 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/rrule.py
--rw-r--r--   0 root         (0) root         (0)     2684 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/dateutil/easter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/db/
--rw-r--r--   0 root         (0) root         (0)    57862 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/mysql.py
--rw-r--r--   0 root         (0) root         (0)    21291 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/sqlite.py
--rw-r--r--   0 root         (0) root         (0)    11665 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/
--rw-r--r--   0 root         (0) root         (0)    12024 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/protocol.py
--rw-r--r--   0 root         (0) root         (0)     4732 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)      658 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/optionfile.py
--rw-r--r--   0 root         (0) root         (0)    49041 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/connections.py
--rw-r--r--   0 root         (0) root         (0)      180 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/util.py
--rw-r--r--   0 root         (0) root         (0)     3716 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/err.py
--rw-r--r--   0 root         (0) root         (0)      360 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/times.py
--rw-r--r--   0 root         (0) root         (0)    10330 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/charset.py
--rw-r--r--   0 root         (0) root         (0)     7720 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/COMMAND.py
--rw-r--r--   0 root         (0) root         (0)      214 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/FLAG.py
--rw-r--r--   0 root         (0) root         (0)     2228 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/CR.py
--rw-r--r--   0 root         (0) root         (0)      372 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/FIELD_TYPE.py
--rw-r--r--   0 root         (0) root         (0)      334 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/SERVER_STATUS.py
--rw-r--r--   0 root         (0) root         (0)      853 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/CLIENT.py
--rw-r--r--   0 root         (0) root         (0)    12297 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/constants/ER.py
--rw-r--r--   0 root         (0) root         (0)     4049 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/_socketio.py
--rw-r--r--   0 root         (0) root         (0)    12235 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/converters.py
--rw-r--r--   0 root         (0) root         (0)      481 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/_compat.py
--rw-r--r--   0 root         (0) root         (0)    17238 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/pymysql/cursors.py
--rw-r--r--   0 root         (0) root         (0)    22385 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/sqlite copy.py
--rw-r--r--   0 root         (0) root         (0)     6357 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/utill/db/model.py
--rw-r--r--   0 root         (0) root         (0)     1970 2021-09-04 08:18:39.000000 kcweb-4.13.8/kcweb/Events.py
--rw-r--r--   0 root         (0) root         (0)     2335 2021-09-04 15:57:50.000000 kcweb-4.13.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      339 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2755 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       89 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      237 2021-09-04 15:57:52.000000 kcweb-4.13.8/kcweb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      237 2021-09-04 15:57:52.000000 kcweb-4.13.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/
+-rw-r--r--   0 root         (0) root         (0)       59 2021-09-05 11:10:54.000000 kcweb-4.13.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/
+-rw-r--r--   0 root         (0) root         (0)       44 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/common/
+-rw-r--r--   0 root         (0) root         (0)     2084 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/common/session.py
+-rw-r--r--   0 root         (0) root         (0)      115 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/common/request.py
+-rw-r--r--   0 root         (0) root         (0)    57879 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/common/autoload.py
+-rw-r--r--   0 root         (0) root         (0)      142 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/common/globals.py
+-rw-r--r--   0 root         (0) root         (0)    43137 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/tpl/
+-rw-r--r--   0 root         (0) root         (0)      789 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/tpl/error.html
+-rw-r--r--   0 root         (0) root         (0)     2069 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/tpl/err.html
+-rw-r--r--   0 root         (0) root         (0)     2335 2021-09-05 11:10:20.000000 kcweb-4.13.9/kcweb/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/config/
+-rw-r--r--   0 root         (0) root         (0)     5815 2021-09-05 11:10:20.000000 kcweb-4.13.9/kcweb/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/filetype/
+-rw-r--r--   0 root         (0) root         (0)      223 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/filetype/types/
+-rw-r--r--   0 root         (0) root         (0)     1448 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/font.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/audio.py
+-rw-r--r--   0 root         (0) root         (0)      928 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/isobmff.py
+-rw-r--r--   0 root         (0) root         (0)      675 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/base.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/image.py
+-rw-r--r--   0 root         (0) root         (0)    12601 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/archive.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/types/video.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/filetype.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/filetype/match.py
+-rw-r--r--   0 root         (0) root         (0)     8950 2021-09-05 11:10:20.000000 kcweb-4.13.9/kcweb/utill/queues.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/cache/
+-rw-r--r--   0 root         (0) root         (0)    10147 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/cache/cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/rediss/
+-rw-r--r--   0 root         (0) root         (0)    11358 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/sentinel.py
+-rw-r--r--   0 root         (0) root         (0)      992 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      666 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/utils.py
+-rw-r--r--   0 root         (0) root         (0)    47617 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/connection.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/_compat.py
+-rw-r--r--   0 root         (0) root         (0)    10835 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/lock.py
+-rw-r--r--   0 root         (0) root         (0)   146593 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/client.py
+-rw-r--r--   0 root         (0) root         (0)      992 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/rediss/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7868 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/redis.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/dateutil/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/dateutil/tz/
+-rw-r--r--   0 root         (0) root         (0)      551 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/tz/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/tz/_factories.py
+-rw-r--r--   0 root         (0) root         (0)    12975 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/tz/_common.py
+-rw-r--r--   0 root         (0) root         (0)    12935 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/tz/win.py
+-rw-r--r--   0 root         (0) root         (0)    62446 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/tz/tz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/dateutil/parser/
+-rw-r--r--   0 root         (0) root         (0)     1727 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13106 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/parser/isoparser.py
+-rw-r--r--   0 root         (0) root         (0)    57682 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/parser/_parser.py
+-rw-r--r--   0 root         (0) root         (0)       59 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/tzwin.py
+-rw-r--r--   0 root         (0) root         (0)      222 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      116 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/dateutil/zoneinfo/
+-rw-r--r--   0 root         (0) root         (0)     5889 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/zoneinfo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/zoneinfo/rebuild.py
+-rw-r--r--   0 root         (0) root         (0)    24903 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/relativedelta.py
+-rw-r--r--   0 root         (0) root         (0)      932 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/_common.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/utils.py
+-rw-r--r--   0 root         (0) root         (0)    66546 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/rrule.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/dateutil/easter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/db/
+-rw-r--r--   0 root         (0) root         (0)    57862 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/mysql.py
+-rw-r--r--   0 root         (0) root         (0)    21291 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)    11665 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/
+-rw-r--r--   0 root         (0) root         (0)    12024 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      658 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/optionfile.py
+-rw-r--r--   0 root         (0) root         (0)    49041 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/connections.py
+-rw-r--r--   0 root         (0) root         (0)      180 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/util.py
+-rw-r--r--   0 root         (0) root         (0)     3716 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/err.py
+-rw-r--r--   0 root         (0) root         (0)      360 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/times.py
+-rw-r--r--   0 root         (0) root         (0)    10330 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/charset.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/COMMAND.py
+-rw-r--r--   0 root         (0) root         (0)      214 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/FLAG.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/CR.py
+-rw-r--r--   0 root         (0) root         (0)      372 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 root         (0) root         (0)      334 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 root         (0) root         (0)      853 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/CLIENT.py
+-rw-r--r--   0 root         (0) root         (0)    12297 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/constants/ER.py
+-rw-r--r--   0 root         (0) root         (0)     4049 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/_socketio.py
+-rw-r--r--   0 root         (0) root         (0)    12235 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/converters.py
+-rw-r--r--   0 root         (0) root         (0)      481 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/_compat.py
+-rw-r--r--   0 root         (0) root         (0)    17238 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/pymysql/cursors.py
+-rw-r--r--   0 root         (0) root         (0)    22385 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/sqlite copy.py
+-rw-r--r--   0 root         (0) root         (0)     6357 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/utill/db/model.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2021-09-04 08:18:39.000000 kcweb-4.13.9/kcweb/Events.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2021-09-05 11:10:40.000000 kcweb-4.13.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      339 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2755 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2021-09-05 11:10:54.000000 kcweb-4.13.9/kcweb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      237 2021-09-05 11:10:54.000000 kcweb-4.13.9/PKG-INFO
```

### Comparing `kcweb-4.13.8/kcweb/common/session.py` & `kcweb-4.13.9/kcweb/common/session.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/common/request.py` & `kcweb-4.13.9/kcweb/common/request.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/common/autoload.py` & `kcweb-4.13.9/kcweb/common/autoload.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/app.py` & `kcweb-4.13.9/kcweb/app.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/tpl/error.html` & `kcweb-4.13.9/kcweb/tpl/error.html`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/tpl/err.html` & `kcweb-4.13.9/kcweb/tpl/err.html`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/setup.py` & `kcweb-4.13.9/kcweb/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         con=f.read()
         f.close()
     else:
         con=''
     return con
 confkcw={}
 confkcw['name']='kcweb'                             #项目的名称 
-confkcw['version']='4.13.8'							#项目版本
+confkcw['version']='4.13.9'							#项目版本
 confkcw['description']=''       #项目的简单描述
 confkcw['long_description']="增加任务队列进度条"     #项目详细描述
 confkcw['license']='MIT License'                    #开源协议   mit开源
 confkcw['url']=''
 confkcw['author']='禄可集团-坤坤'  					 #名字
 confkcw['author_email']='fk1402936534@qq.com' 	     #邮件地址
 confkcw['maintainer']='坤坤' 						 #维护人员的名字
```

### Comparing `kcweb-4.13.8/kcweb/config/__init__.py` & `kcweb-4.13.9/kcweb/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 email['pwd']='' #发件人邮箱密码(如申请的smtp给的口令)
 email['sendNick']='' #发件人昵称
 email['theme']='' #默认主题
 email['recNick']='' #默认收件人昵称
 
 kcweb={}
 kcweb['name']='kcweb'                             #项目的名称
-kcweb['version']='4.13.8'							#项目版本
+kcweb['version']='4.13.9'							#项目版本
 kcweb['description']=''       #项目的简单描述
 kcweb['long_description']=''     #项目详细描述
 kcweb['license']='MIT'                    #开源协议   mit开源
 kcweb['url']=''
 kcweb['author']='禄可集团-坤坤'  					 #名字
 kcweb['author_email']='fk1402936534@qq.com' 	     #邮件地址
 kcweb['maintainer']='坤坤' 						 #维护人员的名字
```

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/__init__.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/font.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/font.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/audio.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/audio.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/isobmff.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/isobmff.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/base.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/base.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/image.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/image.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/archive.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/archive.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/types/video.py` & `kcweb-4.13.9/kcweb/utill/filetype/types/video.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/helpers.py` & `kcweb-4.13.9/kcweb/utill/filetype/helpers.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/filetype.py` & `kcweb-4.13.9/kcweb/utill/filetype/filetype.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/utils.py` & `kcweb-4.13.9/kcweb/utill/filetype/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/filetype/match.py` & `kcweb-4.13.9/kcweb/utill/filetype/match.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/queues.py` & `kcweb-4.13.9/kcweb/utill/queues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from queue import Queue
 from .db import model
 from .db import sqlite as kcwsqlite
-import threading,time,os,hashlib,random
+import threading,time,os,hashlib,random,traceback
 queuesdbpath=os.path.split(os.path.realpath(__file__))[0]+"/Queues"
 class model_kcweb_task(model.model):
     "任务"
     config={'type':'sqlite','db':queuesdbpath}
     model.dbtype.conf=config
     table="model_kcweb_queues" 
     fields={
@@ -48,36 +48,38 @@
             if not Queues.__globalqueue.empty():
                 value=Queues.__globalqueue.get()
                 kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid = '"+value['task']['taskid']+"' and code!=4").update({"code":3,"msg":"正在执行","error":""})
                 if value['args']:
                     try:
                         value['target'](*value['args'])
                     except Exception as e:
-                        # import traceback
-                        # print(traceback.print_exc())
-                        kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid = '"+value['task']['taskid']+"' and code!=4").update({"code":1,'endtime':int(time.time()),'updtime':int(time.time()),"msg":"失败","error":str(e)})
+                        kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid = '"+value['task']['taskid']+"' and code!=4").update({"code":1,'endtime':int(time.time()),'updtime':int(time.time()),"msg":"失败:"+str(e),"error":str(traceback.format_exc())})
                     else:
                         kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid = '"+value['task']['taskid']+"' and code!=4").update({"code":4,"start":100,'endtime':int(time.time()),'updtime':int(time.time()),"msg":"执行完成"})
                 else:
                     try:
                         value['target']()
                     except Exception as e:
-                        # import traceback
-                        # print(traceback.print_exc())
-                        kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid = '"+value['task']['taskid']+"' and code!=4").update({"code":1,'endtime':int(time.time()),'updtime':int(time.time()),"msg":"失败","error":str(e)})
+                        kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid = '"+value['task']['taskid']+"' and code!=4").update({"code":1,'endtime':int(time.time()),'updtime':int(time.time()),"msg":"失败:"+str(e),"error":str(traceback.format_exc())})
                     else:
                         kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid = '"+value['task']['taskid']+"' and code!=4").update({"code":4,"start":100,'endtime':int(time.time()),'updtime':int(time.time()),"msg":"执行完成"})
             else:
                 time.sleep(1)
     def delhist():
         """清除任务历史记录(包括 成功的 失败的 已完成的)"""
         return kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("code","in",0,1,4).delete()
     def delwhere(where):
         "通过where条件删除 (不推荐使用)"
         return kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where(where).delete()
+    def setfield(taskid,key,value):
+        """设置指定字段(不建议使用)"""
+        try:
+            return kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid",taskid).update({key:value})
+        except:
+            return False
     def setstart(taskid,start=0.001,describes=None):
         """增加进度条起始位置
         
         start 支持0.001到10
         """
         if start>=0.001 and start<=10:
             arr=kcwsqlite.sqlite().connect(queuesdbpath).table("model_kcweb_queues").where("taskid",taskid).find()
```

### Comparing `kcweb-4.13.8/kcweb/utill/app.py` & `kcweb-4.13.9/kcweb/utill/app.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/cache/cache.py` & `kcweb-4.13.9/kcweb/utill/cache/cache.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/sentinel.py` & `kcweb-4.13.9/kcweb/utill/rediss/sentinel.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/__init__.py` & `kcweb-4.13.9/kcweb/utill/rediss/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/utils.py` & `kcweb-4.13.9/kcweb/utill/rediss/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/connection.py` & `kcweb-4.13.9/kcweb/utill/rediss/connection.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/_compat.py` & `kcweb-4.13.9/kcweb/utill/rediss/_compat.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/lock.py` & `kcweb-4.13.9/kcweb/utill/rediss/lock.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/client.py` & `kcweb-4.13.9/kcweb/utill/rediss/client.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/rediss/exceptions.py` & `kcweb-4.13.9/kcweb/utill/rediss/exceptions.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/redis.py` & `kcweb-4.13.9/kcweb/utill/redis.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/http.py` & `kcweb-4.13.9/kcweb/utill/http.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/tz/__init__.py` & `kcweb-4.13.9/kcweb/utill/dateutil/tz/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/tz/_factories.py` & `kcweb-4.13.9/kcweb/utill/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/tz/_common.py` & `kcweb-4.13.9/kcweb/utill/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/tz/win.py` & `kcweb-4.13.9/kcweb/utill/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/tz/tz.py` & `kcweb-4.13.9/kcweb/utill/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/parser/__init__.py` & `kcweb-4.13.9/kcweb/utill/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/parser/isoparser.py` & `kcweb-4.13.9/kcweb/utill/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/parser/_parser.py` & `kcweb-4.13.9/kcweb/utill/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/zoneinfo/__init__.py` & `kcweb-4.13.9/kcweb/utill/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/zoneinfo/rebuild.py` & `kcweb-4.13.9/kcweb/utill/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/relativedelta.py` & `kcweb-4.13.9/kcweb/utill/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/_common.py` & `kcweb-4.13.9/kcweb/utill/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/utils.py` & `kcweb-4.13.9/kcweb/utill/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/rrule.py` & `kcweb-4.13.9/kcweb/utill/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/dateutil/easter.py` & `kcweb-4.13.9/kcweb/utill/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/mysql.py` & `kcweb-4.13.9/kcweb/utill/db/mysql.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/sqlite.py` & `kcweb-4.13.9/kcweb/utill/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/mongodb.py` & `kcweb-4.13.9/kcweb/utill/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/protocol.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/protocol.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/__init__.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/optionfile.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/connections.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/connections.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/err.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/err.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/charset.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/charset.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/_auth.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/_auth.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/constants/COMMAND.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/constants/CR.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/constants/CLIENT.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/constants/ER.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/_socketio.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/_socketio.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/converters.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/converters.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/pymysql/cursors.py` & `kcweb-4.13.9/kcweb/utill/db/pymysql/cursors.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/sqlite copy.py` & `kcweb-4.13.9/kcweb/utill/db/sqlite copy.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/utill/db/model.py` & `kcweb-4.13.9/kcweb/utill/db/model.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/kcweb/Events.py` & `kcweb-4.13.9/kcweb/Events.py`

 * *Files identical despite different names*

### Comparing `kcweb-4.13.8/setup.py` & `kcweb-4.13.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         con=f.read()
         f.close()
     else:
         con=''
     return con
 confkcw={}
 confkcw['name']='kcweb'                             #项目的名称 
-confkcw['version']='4.13.8'							#项目版本
+confkcw['version']='4.13.9'							#项目版本
 confkcw['description']=''       #项目的简单描述
 confkcw['long_description']="增加任务队列进度条"     #项目详细描述
 confkcw['license']='MIT License'                    #开源协议   mit开源
 confkcw['url']=''
 confkcw['author']='禄可集团-坤坤'  					 #名字
 confkcw['author_email']='fk1402936534@qq.com' 	     #邮件地址
 confkcw['maintainer']='坤坤' 						 #维护人员的名字
```

### Comparing `kcweb-4.13.8/kcweb.egg-info/SOURCES.txt` & `kcweb-4.13.9/kcweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

