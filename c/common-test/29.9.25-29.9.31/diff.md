# Comparing `tmp/common-test-29.9.25.tar.gz` & `tmp/common-test-29.9.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.25.tar", last modified: Thu May  4 06:22:01 2023, max compression
+gzip compressed data, was "common-test-29.9.31.tar", last modified: Mon May  8 02:04:26 2023, max compression
```

## Comparing `common-test-29.9.25.tar` & `common-test-29.9.31.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.683143 common-test-29.9.25/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-04 06:22:01.683347 common-test-29.9.25/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.651921 common-test-29.9.25/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.25/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.653728 common-test-29.9.25/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.25/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.25/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.25/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.25/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.655934 common-test-29.9.25/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.25/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.25/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3551 2023-05-04 02:54:16.000000 common-test-29.9.25/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.25/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.656784 common-test-29.9.25/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.25/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.25/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.658461 common-test-29.9.25/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.25/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17403 2023-05-04 01:35:15.000000 common-test-29.9.25/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.25/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.661200 common-test-29.9.25/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.25/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.25/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.25/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.669298 common-test-29.9.25/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.25/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11195 2023-05-04 01:28:37.000000 common-test-29.9.25/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.25/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.25/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.670060 common-test-29.9.25/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.25/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.25/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.673501 common-test-29.9.25/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.25/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.25/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-05-04 02:54:16.000000 common-test-29.9.25/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.679717 common-test-29.9.25/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.25/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.25/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.25/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7982 2023-05-04 02:29:22.000000 common-test-29.9.25/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6732 2023-05-04 05:54:33.000000 common-test-29.9.25/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.25/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    11215 2023-04-24 05:43:36.000000 common-test-29.9.25/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.25/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.25/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.25/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-04 06:22:01.682658 common-test-29.9.25/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-04 06:22:01.000000 common-test-29.9.25/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-04 06:22:01.684225 common-test-29.9.25/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1641 2023-04-27 05:55:54.000000 common-test-29.9.25/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.205552 common-test-29.9.31/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 02:04:26.205759 common-test-29.9.31/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.186705 common-test-29.9.31/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.31/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.188507 common-test-29.9.31/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.31/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7021 2023-05-06 02:44:55.000000 common-test-29.9.31/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.31/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.31/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.189864 common-test-29.9.31/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.31/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.31/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.31/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.31/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.190428 common-test-29.9.31/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.31/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.31/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.191433 common-test-29.9.31/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.31/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.31/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.31/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.193789 common-test-29.9.31/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.31/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.31/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.196299 common-test-29.9.31/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.31/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.31/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.31/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.196960 common-test-29.9.31/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.31/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.31/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.199109 common-test-29.9.31/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3594 2023-05-08 01:30:00.000000 common-test-29.9.31/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.31/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.31/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13609 2023-05-05 06:58:50.000000 common-test-29.9.31/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.31/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8671 2023-05-06 06:54:30.000000 common-test-29.9.31/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.202587 common-test-29.9.31/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.31/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.31/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.31/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7879 2023-05-05 07:35:27.000000 common-test-29.9.31/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6886 2023-05-08 02:03:18.000000 common-test-29.9.31/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.31/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.31/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.31/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.31/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    16627 2023-05-08 02:04:19.000000 common-test-29.9.31/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.205110 common-test-29.9.31/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-08 02:04:26.206675 common-test-29.9.31/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.31/setup.py
```

### Comparing `common-test-29.9.25/PKG-INFO` & `common-test-29.9.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.25
+Version: 29.9.31
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.25/common/autotest/base_requests.py` & `common-test-29.9.31/common/autotest/base_requests.py`

 * *Files 13% similar despite different names*

```diff
@@ -81,16 +81,14 @@
         """
         DataBus.save_init_data()
         schemal_data = get_yaml_ApiSchemal(schemal_key)
         url = DataProcess.handle_path(schemal_data['url'])
         if url.find("http") == -1:
             url = get_system_key(host) + DataProcess.handle_path(url)
         cls._convert_url(url)
-        if isinstance(data, str):
-            data = DataProcess.handle_data(data)
         header = DataProcess.handle_header(header)
         try:
             if datatype == 'json':
                 data = DataProcess.handle_data(data)
             else:
                 data = DataProcess.handle_data(data, False)
         except Exception as e:
@@ -104,14 +102,35 @@
             if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
                 MysqlPlatForm.insert_api_data(url, schemal_data['method'], header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         return res
 
     @classmethod
+    def api_request(self, url, method, parametric_key=None, header=None, data=None, file=None, cookie=None, datatype: str='json', desc: str= ""):
+        DataBus.save_init_data()
+        try:
+            if datatype == 'json':
+                data = DataProcess.handle_data(data)
+            else:
+                data = DataProcess.handle_data(data, False)
+        except Exception as e:
+            logger.info(f'测试数据：{data} 转换异常:' + repr(e))
+        res = cls.http_request(url=DataProcess.handle_path(url), method=method, parametric_key=parametric_key,
+                               header=DataProcess.setDictEncode(DataProcess.handle_header(header)), data=data,
+                               file=file, cookie=cookie,desc=desc)
+        try:
+            if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
+                MysqlPlatForm.insert_api_data(url, method, header, data, res.elapsed.total_seconds(),
+                                              res.status_code)
+        except:
+            logger.warning("保存请求数据异常")
+        return res
+
+    @classmethod
     def _convert_url(self,url):
         _url = url.replace("//", '####').split('/')
         _newurl = '';
         for i in range(len(_url)):
             if _url[i].find(Constant.DATA_NO_CONTENT) == -1:
                 _newurl = _newurl + _url[i] + '/'
         _newurl = _newurl.replace("//", "/").replace("####", "//")
```

### Comparing `common-test-29.9.25/common/autotest/handle_allure.py` & `common-test-29.9.31/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/autotest/handle_assert.py` & `common-test-29.9.31/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/common/api_driver.py` & `common-test-29.9.31/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/common/constant.py` & `common-test-29.9.31/common/common/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     TEST_SRTCYCLE_NAME = 'CycleName'
     TEST_SRTCYCLE_URL = 'CycleURL'
     TEST_CASE_NAME_LIST = 'TestCaseNameList'
     TEST_SUIT_NAME_LIST ='TestSuitNameList'
     GIT_PROJECTNAME = 'gitProjectName'
     ALLURE_PATH = 'AllurePath'
     RUN_TYPE = 'RuntType'
+    Data_init = 'DATAINIT'
     RUN_TYPE_JENKINS = 'jenkins'
     CASE_NAME_RUN_FIX = 'CASENAMERUNID'
     CASE_NAME_NO_FIX ='CASENAMEID'
 
 
 
     SEND_URSER_LIST = 'toUser'
```

### Comparing `common-test-29.9.25/common/common/test.py` & `common-test-29.9.31/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/config/config.py` & `common-test-29.9.31/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/data/data_process.py` & `common-test-29.9.31/common/data/data_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,14 +320,22 @@
                 return data
             if data is None:
                 return False
             if isinstance(data, str):
                 _data = data
             else:
                 _data = str(data)
+            if isinstance(data,list):
+                if data.__len__()==0:
+                    return False
+                else:
+                    for temp in data:
+                        if self.isNotNull(temp):
+                            return True
+                    return False
             if _data is None or _data.strip() == '':
                 return False
             else:
                 return True
         except Exception as e:
             logger.info('判断数据是否为空异常,数据：'+data)
             return True
@@ -344,19 +352,16 @@
     @classmethod
     def check_test_data(self, testdatas:list):
         _testDatas=[]
         try:
             for testdata in testdatas:
                 casename = format_caseName(testdata[Constant.CASE_TITLE])
                 if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-                    cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
-                    caserunid = ServicePlatForm.getCaseByCycle(cycleId, casename, Constant.STATUS_PRE, caseNo)[
+                    caserunid = ServicePlatForm.getCaseByCycle(casename, Constant.STATUS_PRE)[
                         'caserunid']
-                    logger.info(
-                        f'获取周期编号：{cycleId} 用例名称:{casename} 状态:{Constant.STATUS_PRE} 用例编号:{caseNo}  运行编号:{caserunid}')
                     if caserunid != '00000':
                         _testDatas.append(testdata)
                 else:
                     if Constant.CASE_STATUS in testdata:
                         if testdata[Constant.CASE_STATUS].strip() != '否':
                             _testDatas.append(testdata)
                     else:
```

### Comparing `common-test-29.9.25/common/data/handle_common.py` & `common-test-29.9.31/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/db/handle_db.py` & `common-test-29.9.31/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/db/handle_db_batch.py` & `common-test-29.9.31/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/db/handle_mysqldb.py` & `common-test-29.9.31/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/db/handle_oracle.py` & `common-test-29.9.31/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/db/handle_sqlserver.py` & `common-test-29.9.31/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/file/ReadFile.py` & `common-test-29.9.31/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/file/handle_excel.py` & `common-test-29.9.31/common/file/handle_excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,17 +246,16 @@
         casename = format_caseName(testdata[Constant.CASE_TITLE])
         caseNo = testdata[Constant.CASE_NO]
         if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
             return True
         if DataProcess.isNotNull(casename) == False or DataProcess.isNotNull(caseNo) == False:
             return False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
-            caserunid = ServicePlatForm.getCaseByCycle(cycleId, casename, Constant.STATUS_PRE, caseNo)['caserunid']
-            logger.info(f'获取周期编号：{cycleId} 用例名称:{casename} 状态:{Constant.STATUS_PRE} 用例编号:{caseNo}  运行编号:{caserunid}')
+            caserunid = ServicePlatForm.getCaseByCycle(casename, Constant.STATUS_PRE, caseNo)['caserunid']
+            logger.info(f'用例名称:{casename} 状态:{Constant.STATUS_PRE} 用例编号:{caseNo}  运行编号:{caserunid}')
             if caserunid == '00000':
                 return False
             else:
                 return True
         if testdata[Constant.CASE_STATUS].strip() == '否':
             return False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
```

### Comparing `common-test-29.9.25/common/file/handle_file.py` & `common-test-29.9.31/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/file/handle_reques.py` & `common-test-29.9.31/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/file/handle_system.py` & `common-test-29.9.31/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/file/handle_yaml.py` & `common-test-29.9.31/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/mq/handle_rabbit.py` & `common-test-29.9.31/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/plat/ATF_platform.py` & `common-test-29.9.31/common/plat/jira_platform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,302 +1,292 @@
-
-from loguru import logger
 import json
+import os
+import re
+from jsonpath import jsonpath
+
 from common.common.api_driver import APIDriver
+from common.data.handle_common import get_system_key, set_system_key
 from common.common.constant import Constant
-from common.data.handle_common import get_system_key,format_caseName,set_system_key
-from common.plat.mysql_platform import MysqlPlatForm
+from requests.auth import HTTPBasicAuth
 from common.data.data_process import DataProcess
+from loguru import logger
 
+class JiraPlatForm(object):
 
 
-class ATFPlatForm(object):
-
     @classmethod
-    def db_ops(self, _key, _sql, env: str = Constant.ENV):
+    def getJiraIssueInfo(self, jira_no):
         """
-        执行SQL操作
-        :param _key:
-        :param _sql:
-        :param env:
+        通过Jira号获取jira信息
+        :param jira_no:
         :return:
         """
-        _sqltemp=_sql.encode("utf-8").decode("latin1")
-        if get_system_key(env) is not None:
-            env = get_system_key(env)
-        sql_type = _sql.strip().split(" ")[0].lower()
-        if "select" == sql_type:
-            _tempdata = APIDriver.http_request(url=f"{Constant.ATF_URL_API}/querySetResult/{_key}/{env}",
-                                               method='post', parametric_key='data', data=_sqltemp
-                                               )
-            logger.info(f"执行sql成功:{_sql}")
-            return list(_tempdata.json())
-        if "insert" == sql_type or "delete":
-            _tempdata = APIDriver.http_request(url=f"{Constant.ATF_URL_API}/doExecute/{_key}/{env}",
-                                               method='post', parametric_key='data', data=_sqltemp)
-            logger.info(f"执行sql成功:{_sql}")
-            return _tempdata.text
-        else:
-            logger.error("不支持其他语句类型执行，请检查sql")
+
+        return APIDriver.http_request(url=f"{Constant.JIRA_URL}/rest/api/latest/issue/{jira_no}",method='get',
+                                        _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME),get_system_key(Constant.JIRA_PASSWORD))
+                                      )
+
+
 
 
     @classmethod
-    def runDeploy(self,jobName, _pramater):
+    def setJiraFlowStatus(self, flow_id):
         """
-        推送测试结果
-        :param jobName:
-        :param _pramater:
-        :return:
-        """
-        _tempdata = APIDriver.http_request(url=f"{Constant.ATF_URL}/jenkins/runDeploy/{jobName}",
-                                               method='get', parametric_key='params', data=_pramater)
-        return _tempdata
-
+                触发工作流程
+                :param jira_key: Jira_key
+                :param flow_id: 流程ID
+                :return:
+                """
+        if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)):
+            jira_key =get_system_key(Constant.ISSUE_KEY)
+            logger.info(f'更新{jira_key}工作流状态')
+            return APIDriver.http_request(url=f"{Constant.JIRA_URL}/rest/api/2/issue/{jira_key}/transitions?expand=transitions.fields",
+                                          method='post',
+                                          parametric_key='json',
+                                          data=json.loads('{"transition":{"id":"flow_id"}}'.replace('flow_id',flow_id)),
+                                          _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME),
+                                                              get_system_key(Constant.JIRA_PASSWORD))
+                                          )
+        else:
+            return "no issue key"
 
     @classmethod
-    def getProjectData(self, projectName, projectKey):
+    def setJiraComment(self, comment):
         """
-        获取项目数据
-        :param projectName: 项目别名
-        :param projectKey: 关键词
+        添加Jira的备注
+        :param jira_key:
+        :param comment:
         :return:
         """
+        if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)):
+            jira_key = get_system_key(Constant.ISSUE_KEY)
+            return APIDriver.http_request(url=f"{Constant.JIRA_URL}/rest/api/2/issue/{jira_key}/comment",
+                                          method='post',
+                                          parametric_key='json',
+                                          data=json.loads('{"body":"comment"}'.replace('comment',comment)),
+                                          _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME),
+                                                            get_system_key(Constant.JIRA_PASSWORD))
+                                         )
+        else:
+            return "no issue key"
+
+    @classmethod
+    def getJiraIssueSummer(self, case_name):
+        jira_no = get_system_key(Constant.CASE_NAME_NO_FIX+case_name)
+        _link = f'{Constant.JIRA_URL}/browse/{jira_no}'
+        return case_name, _link, jira_no
 
-        try:
-            content = APIDriver.http_request(url=f"{Constant.ATF_URL}/api/getProjectData/{projectName}/{projectKey}",
-            method='get')
-            return (json.loads(content.content)["data"]["projectValue"])
-        except Exception as e:
-            logger.info(f"{Constant.ATF_URL}/api/getProjectData/{projectName}/{projectKey}" + "获取不到value")
-            return None
 
     @classmethod
-    def setProjectData(self, projectKey, value, type = 1):
+    def getJiraTestCaseKey(self, case_name, jira_key):
         """
-        设置项目数据
-        :param projectName: 项目别名
-        :param projectKey: 关键词
-        :param value: 值
-        :param type: 数据类型[0可以重复使用，1不可以重复使用]
-        :return:
+        通过项目id和测试用例名，获取测试用例的链接：
+        例如：
         """
-        if get_system_key('ProjectAlice') is not None and get_system_key('ProjectAlice').strip() != '':
-            projectName = get_system_key('ProjectAlice')
-            return APIDriver.http_request(
-                url=f"{Constant.ATF_URL}/api/setProjectData/{projectName}/{projectKey}/{value}/{type}",
-                method='get'
-                )
-
-    @classmethod
-    def getCycleByCaseName(self, CaseName:str):
-        _list = []
         try:
-            _listCase = CaseName.split(";")
-            if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)) and DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-                for _temp in _listCase:
-                    _dict =MysqlPlatForm.get_test_case_info(get_system_key(Constant.ISSUE_KEY), get_system_key(Constant.TEST_SRTCYCLE_ID), format_caseName(_temp))
-                    if len(_dict) > 0:
-                        _list.append(_dict[0])
+            project_id = get_system_key(Constant.PROJECT_NAME).split("（")[-1].split("）")[0]
+            jql = "summary ~  %s AND project in (%s) AND issuetype = 测试用例 AND 用例执行方式 = 自动化" % (str(case_name), str(project_id))
+            fields = ["id", "key", "summary"]
+            content = JiraPlatForm.getDataByJql(jql, fields)
+            for item in content["issues"]:
+                if item["fields"]["summary"].strip() == str(case_name).strip():
+                    jira_key = item['key']
+                    set_system_key(Constant.CASE_NAME_NO_FIX+case_name, jira_key)
         except Exception as e:
-            logger.info(f'获取周期的用例名称{CaseName}信息异常' + repr(e))
-        return _list
+            logger.info(f'通过用例名称获取用例key失败: \n用例名：%s' % str(case_name))
+            set_system_key(Constant.CASE_NAME_NO_FIX + case_name, jira_key)
+        return jira_key
 
     @classmethod
-    def syncCaseJiraMysql(self, _caseNameList, result):
-        logger.info("初始化需要运行的测试用例并同步到数据库")
-        for _case in _caseNameList:
-            _caseMete = ATFPlatForm.getCaseInfo(_case['caseid'])
-            if _caseMete['type'] == Constant.CASE_TYPE_AUTO and _caseMete['key'] != '00000':
-                _runid = _case['caserunid']
-                ATFPlatForm.updateByRunid(_runid, result, "")
-
-
-    @classmethod
-    def get_test_autotest_run_byStatus(self, result):
-        _list = []
-        if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)) and DataProcess.isNotNull(
-                get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            _list = MysqlPlatForm.get_test_autotest_run(get_system_key(Constant.ISSUE_KEY),
-                                                        get_system_key(Constant.TEST_SRTCYCLE_ID), result)
-        return _list
+    def getCaseInfo(self, jira_key):
+        try:
+            case_link = f'{Constant.JIRA_URL}/browse/'
+            case_priority = "P1"
+            case_model = "未关联用例模块"
+            case_name = "未关联用例名称"
+            case_suit = "未关联测试集"
+            case_type = "手工"
+            case_story_id = ""
+            case_story_name = "未关联需求名称"
+            case_story_link = f'{Constant.JIRA_URL}/browse/'
+            content = json.loads(JiraPlatForm.
+                                 getJiraIssueInfo(jira_key+'?fields=summary,customfield_14901,customfield_11758,customfield_10300,customfield_10301,customfield_14903')
+                                 .content)['fields']
+            case_link = f'{Constant.JIRA_URL}/browse/{jira_key}'
+            case_name = content['summary']
+            if JiraPlatForm._isNotNull(content['customfield_14901']):
+                case_priority = content['customfield_14901']['value']
+            if JiraPlatForm._isNotNull(content['customfield_11758']):
+                case_model = content['customfield_11758']['value']
+            if JiraPlatForm._isNotNull(content['customfield_10300']):
+                case_suit = content['customfield_10300']
+            if JiraPlatForm._isNotNull(content['customfield_10301']):
+                case_story_id_list = content['customfield_10301']
+                if JiraPlatForm._isNotNull(str(case_story_id_list).replace("\t","").strip()):
+                    case_story_id = str(case_story_id_list.split(",")[0]).replace("\t","").strip()
+                    case_story_link = f'{Constant.JIRA_URL}/browse/{case_story_id}'
+                    case_story_name = json.loads(JiraPlatForm.getJiraIssueInfo(case_story_id+'?fields=summary').content)['fields']['summary']
+            if JiraPlatForm._isNotNull(content['customfield_14903']):
+                case_type = content['customfield_14903']['value']
+        except Exception as e:
+            logger.info(f'获取用例key用例信息失败，用例的Key:{jira_key}')
+        return jira_key, case_name, case_link, case_priority, case_model, case_suit, case_story_id, case_story_name, case_story_link, case_type
 
     @classmethod
-    def getCycleByCaseID(self, caseId: str):
-        _list = []
+    def _isNotNull(self, data):
         try:
-            _listCase = caseId.split(";")
-            if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)) and DataProcess.isNotNull(
-                    get_system_key(Constant.TEST_SRTCYCLE_ID)):
-                for _temp in _listCase:
-                    _dict = MysqlPlatForm.get_test_case_info_ByID(get_system_key(Constant.ISSUE_KEY),
-                                                             get_system_key(Constant.TEST_SRTCYCLE_ID),
-                                                             _temp)
-                    if len(_dict) > 0:
-                        _list.append(_dict[0])
+            if data is None:
+                return False
+            if isinstance(data, str):
+                _data = data
+            else:
+                _data = str(data)
+            if _data.strip() == '':
+                return False
+            else:
+                return True
         except Exception as e:
-            logger.info(f'获取周期的用例编号{caseId}信息异常'+repr(e))
-        return _list
+            logger.info('判断数据是否为空异常,数据：' + data)
+            return True
 
     @classmethod
-    def getCycleByResult(self,  restult: str = "'通过','未执行','失败','自动化执行'"):
-        _list = []
+    def getCaseNameListFromCircleId(self, result=""):
+        """
+        通过Jira的测试计划number，测试周期名字，来获取测试用例列表
+        :param jira_no: 测试计划number
+        :param cycle_id: 测试周期id
+        :param result: 测试用例执行结果进行筛选（通过，失败，未执行等）
+        :return:
+        """
+        case_name_list=[]
         if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)) and DataProcess.isNotNull(
                 get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            _list = MysqlPlatForm.get_test_autotest_run(get_system_key(Constant.ISSUE_KEY),
-                                                         get_system_key(Constant.TEST_SRTCYCLE_ID),
-                                                         restult)
-        return _list
-
-    @classmethod
-    def runSenceCase(self, _caseList):
-        _caseNameList = []
-        _caseScriptList = []
-        for caseName in _caseNameList:
-            caseName = format_caseName(caseName['casename'])
-            _caseNameList.append(caseName)
-        _caseScriptList = MysqlPlatForm.getScriptyPathByCaseNameList(_caseNameList)
-        return _caseNameList, _caseScriptList
-
+            jira_no = get_system_key(Constant.ISSUE_KEY)
+            cycle_id = get_system_key(Constant.TEST_SRTCYCLE_ID)
+            content = APIDriver.http_request(
+                url=f"{Constant.JIRA_URL}/rest/synapse/latest/public/testPlan/{jira_no}/cycle/{cycle_id}/testRunsByCycleId",
+                method='get',
+                _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD))
+            )
+
+            if result != "":
+                case_name_list = []
+                logger.info('result结果：%s' % str(result.split(",")))
+                for result_item in result.split(","):
+                    logger.info('result_item：%s' % str(result_item))
+                    case_list = jsonpath(json.loads(content.content),
+                                               "$..[?(@.status == '%s')].summary" % result_item)
+                    if case_list:
+                        case_name_list += case_list
+            else:
+                case_name_list = jsonpath(json.loads(content.content), "$..summary")
+        return case_name_list
 
     @classmethod
-    def sent_result_byCaseName(self, CaseName, CaseID, result, comment, scriptUrl:str = ""):
+    def updateTestReference(self,testCaseIssueKey, desc):
         try:
-            _case = ATFPlatForm.getCycleByCaseName(CaseName)
-            if len(_case) == 0 and DataProcess.isNotNull(CaseID):
-                _case = ATFPlatForm.getCycleByCaseID(CaseID)
-            if len(_case) > 0:
-                _runid = _case[0]['caserunid']
-                _caseid = _case[0]['caseid']
-                _caseTitle = _case[0]['casename']
-                if scriptUrl != "":
-                    MysqlPlatForm.insert_test_autotest_script(_caseTitle, _caseid, scriptUrl)
-                ATFPlatForm.updateByRunid(_runid,result,comment)
-                logger.info(f'用例名称:{CaseName} 运行ID：{_runid}  结果:{result} 结果描述:{comment} 推送成功')
-            else:
-                logger.info(f'用例名称:{CaseName} 用例编号:{CaseID} 结果:{result} 在测试周期中没有找到')
+            if JiraPlatForm.getTestReference(testCaseIssueKey) != desc.strip():
+               APIDriver.http_request(
+                    url=f"{Constant.JIRA_URL}/rest/synapse/latest/public/testCase/{testCaseIssueKey}/updateTestReference",
+                    method='post',
+                    parametric_key='json',
+                    data={
+                        "automationReference": f"{desc}"
+                    },
+                    _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD))
+                )
         except Exception as e:
-            logger.info(f'用例名称:{CaseName} 用例编号:{CaseID} 结果:{result}  结果描述:{comment} 推送异常:' + repr(e))
+            logger.info(f' 用例Key:{testCaseIssueKey} 自动化引用信息:{desc} 更新用例描述异常:{e}')
 
     @classmethod
-    def syncCycleNameCase(self):
-        ATFPlatForm.syncCycleBasic()
-        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            ATFPlatForm.syncCycleCase(get_system_key(Constant.TEST_SRTCYCLE_ID))
+    def getTestReference(self, testCaseIssueKey):
+        automationReference = ""
+        try:
+            response = APIDriver.http_request(
+                url=f"{Constant.JIRA_URL}/rest/synapse/latest/public/testCase/{testCaseIssueKey}/automationReference",
+                method='get',
+                _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD))
+            )
+            automationReference = json.loads(response.content)['automationReference']
+            return automationReference
+        except Exception as e:
+            logger.info(f' 用例Key:{testCaseIssueKey}  获取用例引用异常:{e}')
+            return automationReference
 
     @classmethod
-    def syncCycleBasic(self):
-        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
-            issueKey =""
-            try:
-                testPlan = ATFPlatForm.getTestPlanInfo(get_system_key(Constant.TEST_SRTCYCLE_ID).strip())
-                set_system_key(Constant.TEST_SRTCYCLE_ID, str(testPlan['cycleId']))
-                set_system_key(Constant.TEST_SRTCYCLE_NAME, testPlan['cycleName'])
-                set_system_key(Constant.TEST_SRTCYCLE_URL, testPlan['cycleUrl'])
-
-                set_system_key(Constant.ISSUE_KEY, testPlan['issueKey'])
-                issueKey = testPlan['issueKey']
-                set_system_key(Constant.TEST_TestPlan_ID, str(testPlan['testPlanId']))
-                set_system_key(Constant.TEST_TestPlan_NAME, testPlan['testPlanName'])
-                set_system_key(Constant.TEST_TestPlan_URL, testPlan['testPlanUrl'])
-            except Exception as e:
-                logger.error(f"获取周期{cycleId}中测试计划:{issueKey}\n 异常:" + repr(e))
-
-        if DataProcess.isNotNull(get_system_key(Constant.PROJECT_NAME)):
-            projectId = get_system_key(Constant.PROJECT_NAME).split("（")[-1].split("）")[0]
-            set_system_key(Constant.PORJECT_ID, projectId)
-
-
+    def updateDescription(self,testCaseIssueKey, desc):
+        try:
+            case_desc = json.loads(JiraPlatForm.getJiraIssueInfo(testCaseIssueKey + '?fields=description').content)['fields']['description']
+            if DataProcess.isNotNull(case_desc) == False or str(case_desc).strip() != desc.strip():
+                APIDriver.http_request(
+                    url=f"{Constant.JIRA_URL}/rest/api/2/issue/{testCaseIssueKey}",
+                    method='put',
+                    parametric_key='json',
+                    data={"fields" : {"description": f"{desc}"}},
+                    _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD))
+                )
+        except Exception as e:
+            logger.info(f' 用例Key:{testCaseIssueKey} 描述信息:{desc} 更新用例描述异常:{e}')
 
     @classmethod
-    def getTestPlanInfo(self,cycleId):
-        return json.loads(APIDriver.http_request(url=f"{Constant.ATF_PYTHON_URL}/jira/plan/get/{cycleId}", method='get').content)
+    def getDataByJql(self, jql, fields):
+        content = list()
+        try:
+            content = APIDriver.http_request(
+                url=f"{Constant.JIRA_URL}/rest/api/2/search",
+                method='post',
+                parametric_key='json',
+                data={
+                    "jql": jql,
+                    "startAt": 0,
+                    "maxResults": 1000,
+                    "fields": fields
+                },
+                _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD))
+            )
+            content = json.loads(content.content)
+            return content
+        except Exception as e:
+            logger.info(f'查询Jql异常：{jql}')
+            return content
 
     @classmethod
-    def updateByRunid(self, runid, result, comment:str = "", steps:str = ""):
-        _dict = {'result': result, 'comment': comment, 'steps': steps}
-        APIDriver.http_request(
-            url=f"{Constant.ATF_PYTHON_URL}/jira/run/update/{runid}",
-            method='post',
-            parametric_key='json',
-            data=json.loads(json.dumps(_dict,ensure_ascii=False))
-        )
+    def saveCaseToTestPlan(self,testPlanIssueKey,jiraKey):
+        content = list()
+        try:
+            content = APIDriver.http_request(
+                url=f"{Constant.JIRA_URL}/rest/synapse/latest/public/testPlan/{testPlanIssueKey}/addMembers",
+                method='post',
+                parametric_key='json',
+                data={
+                    "testCaseKeys": jiraKey
+                },
+                _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD))
+            )
+            content = json.loads(content.content)
+            return content
+        except Exception as e:
+            logger.info(f'添加测试用例到测试计划异常：{jql}')
+            return content
 
     @classmethod
-    def syncCycleCase(self, cycleId):
-        if DataProcess.isNotNull(get_system_key('Result')):
-            _dict = {'status': get_system_key('Result')}
-        else:
-            _dict = {'status': ''}
-        APIDriver.http_request(
-            url=f"{Constant.ATF_PYTHON_URL}/jira/sync/{cycleId}",
-            method='post',
-            parametric_key='json',
-            data=json.loads(json.dumps(_dict, ensure_ascii=False))
-        )
-
-    @classmethod
-    def updateStausByCycleId(self, cycleId, status):
-        _dict = {'status': status}
-        APIDriver.http_request(
-            url=f"{Constant.ATF_PYTHON_URL}/jira/update/cycle/status/{cycleId}",
-            method='post',
-            parametric_key='json',
-            data=json.loads(json.dumps(_dict, ensure_ascii=False))
-        )
-
-    @classmethod
-    def getCaseInfoByNameOrID(self, issueKey, caseName:str=""):
-        info = ATFPlatForm.getCaseInfo(issueKey)
-        if info['key'] == '00000'or caseName != "" :
-            info = ATFPlatForm.getCaseInfo(caseName)
-        return info
-
-    @classmethod
-    def getCaseRunByNameOrID(self, cycleId, name):
-        _dict = {'cycleId': cycleId, 'name': name}
-        content = APIDriver.http_request(
-            url=f"{Constant.ATF_PYTHON_URL}/jira/run/get",
-            method='post',
-            parametric_key='json',
-            data=json.loads(json.dumps(_dict, ensure_ascii=False))
-        )
-        return json.loads(content.content)
-
-
+    def saveCaseToTestPlanByJql(self, testPlanIssueKey, jql):
+        content = JiraPlatForm.getDataByJql(jql,["id", "key"])
+        keys = jsonpath(content, "$.issues[*].key")
+        logger.info(f'添加用例列表：'+str(keys))
+        JiraPlatForm.saveCaseToTestPlan(testPlanIssueKey, keys)
+        logger.info(f'提交到测试计划：' + str(testPlanIssueKey)+'成功')
 
     @classmethod
-    def getCaseRun(self,cycleId, issuekey, name):
-        run = ATFPlatForm.getCaseRunByNameOrID(cycleId, issuekey)
-        if run['caserunid'] == '00000':
-            run = ATFPlatForm.getCaseRunByNameOrID(cycleId, name)
-        return run
-
-    @classmethod
-    def getCaseInfo(self, caseName):
-        _dict = {'name': caseName}
-        _result = ""
+    def getCycleInfoByTestPlanIssueKey(self,testPlanIssueKey, cycle_id):
         try:
-            if DataProcess.isNotNull(get_system_key(Constant.PORJECT_ID)):
-                projectId=get_system_key(Constant.PORJECT_ID)
-                _dict = {'name': caseName, 'projectId': projectId}
-                content = APIDriver.http_request(
-                    url=f"{Constant.ATF_PYTHON_URL}/jira/case/get",
-                    method='post',
-                    parametric_key='json',
-                    data=json.loads(json.dumps(_dict, ensure_ascii=False))
-                )
-            else:
-                content = APIDriver.http_request(
-                    url=f"{Constant.ATF_PYTHON_URL}/jira/case/get",
-                    method='post',
-                    parametric_key='json',
-                    data=json.loads(json.dumps(_dict, ensure_ascii=False))
-                )
-            _result = content.content
-            return json.loads(_result)
+            logger.info(f"获取测试计划{testPlanIssueKey}周期编号{cycle_id}信息")
+            content = APIDriver.http_request(
+                url=f"{Constant.JIRA_URL}/rest/synapse/latest/public/testPlan/{testPlanIssueKey}/cycles",
+                method='get',
+                _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD)))
+            cycleInfo = jsonpath(json.loads(content.content), f'$.[?(@.id=={cycle_id})]')[0]
+            return cycleInfo
         except Exception as e:
-            logger.error(f"获取用例名称:{_dict}  返回内容:{_result} 异常:" + repr(e))
-
-
-
+            logger.info(f'获取测试计划：{testPlanIssueKey}中周期{cycle_id}信息异常信息:'+repr(e))
+            return ""
```

### Comparing `common-test-29.9.25/common/plat/jenkin_platform.py` & `common-test-29.9.31/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/plugin/allure_plugin.py` & `common-test-29.9.31/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/plugin/assert_plugin.py` & `common-test-29.9.31/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/plugin/atf_plugin.py` & `common-test-29.9.31/common/plugin/atf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class ATFPlugin(object):
 
     @classmethod
     def db_ops(self,_key, _sql, env: str=Constant.ENV):
         DataBus.save_init_data()
-        return ATFPlatForm.db_ops(_key, _sql, env)
+        return ServicePlatForm.db_ops(_key, _sql, env)
 
     @classmethod
     def sendResult(self, report_html_path: str = TEST_TARGET_REPORT_PATH):
         if DataProcess.isNotNull(get_system_key('BUILD_URL')):
             DataBus.save_init_data()
             ATFPlatForm.syncCycleBasic()
             _result, _desc = ATFPlugin.getResultData(report_html_path)
@@ -32,30 +32,26 @@
             if DataProcess.isNotNull(get_system_key(Constant.SEND_URSER_LIST)):
                 logger.info('推送结果到MUC')
                 _userList = get_system_key(Constant.SEND_URSER_LIST).split(',')
                 self.sendMsg(_desc, _userList)
             dict = {"issuekey": f'{_result["jirakey"]}', "project": f'{_result["projectName"]}',
                     "result": f'{_result["result"]}'}
             ATFPlatForm.runDeploy("AutoTest-Result", dict)
-            #JiraPlatForm.setJiraComment(_desc)
 
 
     @classmethod
     def sendMsg(self, content, _list):
         for _index in range(len(_list)):
-            _arr = str(_list[_index]).split('&')
+            _arr = str(_list[_index]).split('|')
             os.environ['toUserId'] = str(_arr[0]).lower()
             os.environ['toMail'] = str(_arr[1])
-            DataBus.set_key('content',content)
+            DataBus.set_key('content', content)
             _data = FilePlugin.load_file("muc.xml",file_path=CONFIG_PATH)
             ServicePlatForm.sendMsg(_data)
 
-
-
-
     @classmethod
     def getResultData(self, report_html_path):
         _summary = FilePlugin.load_json(f'{report_html_path}/widgets/summary.json')
         _result = dict()
         _result['projectId'] = ""
         _result['projectName'] = ""
         _result['env'] = get_system_key('env')
@@ -67,16 +63,16 @@
         _result['cycleName'] = ''
         _result['cycleNameInfo'] = ''
         _result['passrate'] = 0
         _result['passrateInfo'] = ''
         _result["cycleLink"] = ''
         _result['reportUrl'] = _result['buildUrl'] +"allure/"
         if DataProcess.isNotNull(get_system_key(Constant.PROJECT_NAME)):
-            _result['projectName'] = get_system_key(Constant.PROJECT_NAME).split("（")[0]
-            _result['projectId'] = get_system_key(Constant.PROJECT_NAME).split("（")[-1].split("）")[0]
+            _result['projectName'] = get_system_key(Constant.PROJECT_NAME)
+            _result['projectId'] = get_system_key(Constant.PORJECT_ID)
         if DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)):
             _result['jiraLink'] = f'计划地址：{get_system_key(Constant.TEST_TestPlan_URL)}\n'
             _result['jirakey'] = get_system_key(Constant.ISSUE_KEY)
         if DataProcess.isNotNull(get_system_key("type")):
             _result['type'] =get_system_key("type")
             _result['typeInfo'] = f'测试类型：{_result["type"]}\n'
         if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_NAME)):
@@ -113,16 +109,16 @@
                 f'通过用例：{_result["passed"]}\n'\
                 f'测试结果：{_result["resultInfo"]}\n'\
                 f'运行时间：{_result["duration"]}S\n'\
                 f'开始时间：{_result["start"]}\n'\
                 f'结束时间：{_result["stop"]}\n'\
                 f'构建详情：{_result["buildUrl"]} \n'\
                 f'{_result["jiraLink"]}' \
-                #f'{_result["cycleLink"]}' \
-                #f'测试报告：{_result["reportUrl"]}\n'
+                f'{_result["cycleLink"]}' \
+                f'测试报告：{_result["reportUrl"]}\n'
         print_info(f'测试结果数据:\n{_result}')
         logger.info(f'测试结果信息:\n{_desc}')
         return _result, _desc
 
     @classmethod
     def syncJiraCase(self,report_html_path: str = TEST_TARGET_REPORT_PATH):
         """
@@ -150,15 +146,15 @@
             logger.info("自动化用例uid" + str(uids))
             for i in range(0, len(caseName)):
                 parentUid = parentUids[i]
                 uid = uids[i]
                 _caseurl = f'{buildurl}allure/#behaviors/{parentUid}/{uid}'
                 _caseTitleList = caseName[i].split(';')
                 for temp in _caseTitleList:
-                    ATFPlatForm.sent_result_byCaseName(temp, "", "", _caseurl, "")
+                    ATFPlatForm.sent_result_byCaseName(temp, "", "", _caseurl)
```

### Comparing `common-test-29.9.25/common/plugin/data_bus.py` & `common-test-29.9.31/common/plugin/data_bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,19 +146,21 @@
 
     @classmethod
     def save_init_data(cls):
         """
         初始化DataBus数据
         :return:
         """
-        cls.save_yaml('common.setting',_replace=False)
-        cls.save_yaml('common')
-        cls.save_yaml(cls.get_env())
-        cls.get_data_atf()
-        cls.get_param()
+        if DataProcess.isNotNull(get_system_key(Constant.Data_init)):
+            cls.save_yaml('common.setting',_replace=False)
+            cls.save_yaml('common')
+            cls.save_yaml(cls.get_env())
+            cls.get_data_atf()
+            cls.get_param()
+            cls.set_key(Constant.Data_init, Constant.Data_init)
 
     @classmethod
     def run_info(cls):
         """
         打印信息
         :return:
         """
```

### Comparing `common-test-29.9.25/common/plugin/data_plugin.py` & `common-test-29.9.31/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/plugin/file_plugin.py` & `common-test-29.9.31/common/plugin/file_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,18 +260,14 @@
         _mysql.close()
         return _list
 
     @classmethod
     def _dict_contain(self,_data,_temp:list):
         _flag = True
         self._get_jenkin_TestCaseMark(_data)
-        # excelCaseList=defaultdict(list)
-        # for single in _data:
-        #     excelCaseList[single[Constant.CASE_TITLE]]
-
         for i, j in _data.items():
             if i in _temp.keys():
                 if j != str(DataProcess.get_key_dic(_temp, i)).strip():
                     _flag = False
         _flag = self._get_jenkin_TestCaseName(_temp,_flag)
         return _flag
 
@@ -296,17 +292,15 @@
                 _flag = True
             else:
                 _flag = False
         return _flag
 
 
 
-if __name__ == '__main__':
-    _xml=FilePlugin.excel_to_dict("data.xls",sheet="Sheet1",_filter={'需求名称':'bocc上传提交'})
-    print(_xml[0].get('上传文件').get('用例编号'))
+
```

### Comparing `common-test-29.9.25/common/plugin/hooks_plugin.py` & `common-test-29.9.31/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/plugin/pytest_playwright.py` & `common-test-29.9.31/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common/plugin/pytest_plugin.py` & `common-test-29.9.31/common/plugin/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,33 @@
 from common.data.handle_common import get_system_key,format_caseName,print_info
 from common.plat.mysql_platform import MysqlPlatForm
 from common.file.handle_system import del_file
 from common.common.constant import Constant
 from common.data.data_process import DataProcess
 from common.plugin.data_bus import DataBus
 from common.plat.ATF_platform import ATFPlatForm
+from common.plat.service_platform import ServicePlatForm
 from common.plugin.atf_plugin import ATFPlugin
 from common.autotest.handle_allure import allure_title,allure_testcase_link,allure_severity
 from os import path
 
 
 class PytestPlugin(object):
 
     @classmethod
     def getCaseNameList(self):
         """
         获取用例列表
         """
         logger.info("获取测试用例和测试脚本")
         case_name_list = []
-        if DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
-            case_name_list = ATFPlatForm.getCycleByCaseName(get_system_key(Constant.TEST_CASE_NAME_LIST))
+        if DataProcess.isNotNull(get_system_key('Result')):
+            case_name_list = ATFPlatForm.getCycleByResult(get_system_key('Result'))
         else:
-            if DataProcess.isNotNull(get_system_key('Result')):
-                case_name_list = ATFPlatForm.getCycleByResult(get_system_key('Result'))
-            else:
-                case_name_list = ATFPlatForm.getCycleByResult()
+            case_name_list = ATFPlatForm.getCycleByResult()
         PytestPlugin.initRunCyleCase()
         return case_name_list
 
     @classmethod
     def insertCaseToPlan(self):
         if DataProcess.isNotNull(get_system_key('addCaseJql')) and DataProcess.isNotNull(get_system_key(Constant.ISSUE_KEY)):
             JiraPlatForm.saveCaseToTestPlanByJql(get_system_key('issueKey'),get_system_key('addCaseJql'))
@@ -107,17 +105,15 @@
                               f'--alluredir={TEST_TARGET_RESULTS_PATH}'])
             else:
                 logger.info(f"------用例编号：{caseId}  用例名称:{caseName}  运行ID: {caserunId} 结果:{caseStatus}  执行完成----")
 
     @classmethod
     def initRunCyleCase(self):
         if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            ATFPlatForm.updateStausByCycleId(get_system_key(Constant.TEST_SRTCYCLE_ID), Constant.STATUS_PRE)
-
-
+            ServicePlatForm.updateStausByCycleId(get_system_key(Constant.TEST_SRTCYCLE_ID), Constant.STATUS_PRE)
 
     @classmethod
     def pytest_run_case(cls, _deleteResult:bool= True):
         """
         运行自动化用例
         :return:
         """
@@ -138,41 +134,40 @@
                     logger.info("无测试用例列表可运行")
                 else:
                     PytestPlugin.runSceneCase(_caseNameList)
             else:
                 logger.info("运行测试文件:" + get_system_key(Constant.TEST_CASE_PATH))
                 PytestPlugin.runPathCase(get_system_key(Constant.TEST_CASE_PATH))
 
-
     @classmethod
     def allure_report(cls):
         """
         生成测试报告
         :return:
         """
 
         if get_system_key(Constant.ALLURE_PATH) is not None:
             ALLURE_PATH = get_system_key(Constant.ALLURE_PATH)
         else:
             ALLURE_PATH = ''
-        if get_system_key(Constant.RUN_TYPE) is None or get_system_key(Constant.RUN_TYPE) != 'jenkins' or get_system_key(Constant.RUN_TYPE) == '':
+        if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)) == False:
             os.system(f'{ALLURE_PATH}allure generate {TEST_TARGET_RESULTS_PATH} -o {TEST_TARGET_REPORT_PATH} --clean')
             logger.success('Allure测试报告已生成')
         ATFPlugin.sendResult()
 
-
     @classmethod
     def change_allure_title(cls,report_html_path: str = TEST_TARGET_REPORT_PATH):
         """
         修改Allure标题
         :param name: 
         :param report_html_path: 
         :return: 
         """
         dict = {}
+        DataBus.save_init_data()
         # 定义为只读模型，并定义名称为f
         with open(f'{report_html_path}/widgets/summary.json', 'rb') as f:
             # 加载json文件中的内容给params
             params = json.load(f)
             # 修改内容
             params['reportName'] = get_system_key("JOB_NAME")
             # 将修改后的内容保存在dict中
@@ -183,29 +178,35 @@
                 json.dump(dict, r, ensure_ascii=False, indent=4)
 
             # 关闭json读模式
             f.close()
             logger.info("修改测试报告完成")
 
     @classmethod
+    def sendReport(self):
+        DataBus.save_init_data()
+        change_allure_title()
+        ATFPlugin.sendResult()
+
+    @classmethod
     def generated_code(self, _url: str = '', _path: str = TEST_UI_PATH):
         if not DataProcess.isNotNull(_url):
             _url = get_system_key('url')
-        # test_case_dir = '{}{}'.format(os.getcwd(), _path)
         test_case_dir = '{}'.format(_path)
         file_list = [os.path.join(test_case_dir, file) for file in os.listdir(test_case_dir) if "test_" in file]
         test_case_num = len(file_list) - 2
         print("{}目录下存在{}测试用例".format(test_case_dir, test_case_num))
         cmd = r"python -m playwright codegen --target pytest -o {}/test_{}.py -b chromium {}". \
             format(_path, str(test_case_num + 1).zfill(3), _url)
         print("执行录制测试用例命令：{}".format(cmd))
         os.system(cmd)
 
     @classmethod
     def pytest_case_meta(self, item: Item):
+        DataBus.save_init_data()
         _caseTitle, _caseNo = PytestPlugin.getCaseName(item)
         PytestPlugin.jira_convert_allure(_caseTitle, _caseNo)
         PytestPlugin.sync_case_Script(item, _caseTitle, _caseNo)
         PytestPlugin.send_case_result(item, Constant.STATUS_AUTOTEST)
 
     @classmethod
     def getCaseName(self, item: Item):
@@ -224,80 +225,89 @@
             temp = item.__dict__['keywords'].__dict__['_markers']['__allure_display_name__']
             if temp != Constant.TEST_DATA_PARAMETER:
                 _caseTitle = temp
         except Exception as e:
             print_info('未通过装饰器title获取到用例信息')
         try:
             if _caseNo == '00000' or _caseNo is None:
-                _caseNo = item.__dict__['keywords'].__dict__['_markers']['pytestmark'][0].__dict__['args']
-                if str(_caseNo).find("(") > -1:
-                    _caseNo = '00000'
+                _caseNo = item.__dict__['keywords'].__dict__['_markers']['pytestmark'][0].__dict__['args'][0]
+                # if str(_caseNo).find("(") > -1:
+                #     _caseNo = '00000'
         except Exception as e:
             print_info('未通过装饰器ID获取到用例信息')
         print_info(f"执行用例名称：{_caseTitle} 用例编号:{_caseNo}")
         print_info(f'用例数据:{_caseData}')
         return _caseTitle, _caseNo
 
-
-
     @classmethod
     def send_case_result(self, item: Item, result):
-        _caseTitle, _caseNo = PytestPlugin.getCaseName(item)
-        _caseurl=""
-        # _caseurl = PytestPlugin.getCaseUrl(item)
-        if DataProcess.isNotNull(_caseTitle):
-            _caseTitleList = _caseTitle.split(';')
-            caseInfoList = ""
-            for temp in _caseTitleList:
-                info = ATFPlatForm.getCaseInfoByNameOrID(_caseNo, temp)
-                caseInfoList = caseInfoList + info['summary'] + "(" + info['key'] + "),"
-                if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)) and result != 'skipped' and info['key']!='00000':
-                    ATFPlatForm.sent_result_byCaseName(temp, _caseNo, result, "", _caseurl)
-            logger.info(f"---用例列表：{caseInfoList}  执行状态:{result}")
-        else:
-            logger.info(f"---用例列表：无用例列表【请检查是否设置用例名称或者编号】 执行状态:{result}")
+            _caseTitle, _caseNo = PytestPlugin.getCaseName(item)
+            if DataProcess.isNotNull(_caseTitle):
+                _caseTitleList = _caseTitle.split(';')
+            if DataProcess.isNotNull(_caseNo):
+                _caseTitleList.extend(_caseNo.split(';'))
+            if DataProcess.isNotNull(_caseTitleList) > 0:
+                caseInfoList = ""
+                for temp in _caseTitleList:
+                    if DataProcess.isNotNull(temp) and temp.strip() != '00000':
+                        info = ATFPlatForm.getCaseInfoByNameOrID(temp)
+                        if result != 'skipped' and info['key'] != '00000':
+                            caseInfoList = caseInfoList + info['summary'] + "(" + info['key'] + "),"
+                            ATFPlatForm.sent_result_byCaseName(info['summary'], info['key'], result, "")
+                        else:
+                            caseInfoList = caseInfoList + temp + "(" + info['key'] + "),"
+                logger.info(f"---用例列表：{caseInfoList}  执行状态:{result}")
+            else:
+                logger.info(f"---用例列表：无用例列表【请检查是否设置用例名称或者编号】 执行状态:{result}")
 
     @classmethod
-    def sync_case_Script(self,item: Item, _caseTitle, _caseNo):
+    def sync_case_Script(self, item: Item, _caseTitle, _caseNo):
         _caseurl = PytestPlugin.getCaseUrl(item)
         if DataProcess.isNotNull(_caseTitle):
             _caseTitleList = _caseTitle.split(';')
+        if DataProcess.isNotNull(_caseNo):
+            _caseTitleList.extend(_caseNo.split(';'))
+        if DataProcess.isNotNull(_caseTitleList):
             caseInfoList = ""
-            for _name in _caseTitleList:
-                info = ATFPlatForm.getCaseInfoByNameOrID(_caseNo, _name)
-                caseInfoList = caseInfoList + info['summary'] + "(" + info['key'] + "),"
-                if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
-                    MysqlPlatForm.sync_autotest_script(info['summary'], info['key'], _caseurl)
-                    logger.info(f"---用例列表：{caseInfoList} 脚本路径:{_caseurl} 开始执行【结果忽略】")
-                    assert "测试用例检查" == "执行结果可忽略"
+            if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
+                logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 【脚本用例同步】")
+                for _name in _caseTitleList:
+                    if DataProcess.isNotNull(_name) and _name !='00000':
+                        info = ATFPlatForm.getCaseInfoByNameOrID(_name)
+                        caseInfoList = caseInfoList + _name + "(" + info['key'] + "),"
+                        MysqlPlatForm.sync_autotest_script(info['summary'], info['key'], _caseurl)
+                logger.info(f"---同步用例列表：{caseInfoList} 脚本路径:{_caseurl}  【脚本用例同步】")
+                assert "测试用例检查" == "脚本用例同步【执行结果可忽略】"
             if PytestPlugin.checkCaseRun(item, _caseTitle, _caseNo) == False:
-                logger.info(f"---用例列表：{caseInfoList} 脚本路径:{_caseurl} 开始执行【结果忽略】")
-                assert "测试用例检查" == "执行结果可忽略"
+                logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 【未在执行周期中】")
+                assert "测试用例检查" == "未在测试周期中【执行中断】"
             else:
-                logger.info(f"---用例列表：{caseInfoList} 脚本路径:{_caseurl} 开始执行")
+                logger.info(f"---用例列表：{_caseTitleList} 脚本路径:{_caseurl} 【开始执行】")
         else:
             logger.info(f"---用例列表：无用例列表【请检查是否设置用例名称或者编号】")
-            assert "测试用例检查" == "执行结果可忽略"
+            assert "测试用例检查" == "无用例列表【执行结果可忽略】"
 
 
     @classmethod
     def checkCaseRun(self,item: Item, _caseTitle, _caseNo):
         isRun = False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-            cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
             _caseurl = PytestPlugin.getCaseUrl(item)
-            _caseTitleList = _caseTitle.split(';')
-            if len(_caseTitleList) > 1:
+            if DataProcess.isNotNull(_caseTitle):
+                _caseTitleList = _caseTitle.split(';')
+            if DataProcess.isNotNull(_caseNo):
+                _caseTitleList.extend(_caseNo.split(';'))
+            if DataProcess.isNotNull(_caseTitleList):
                 for _name in _caseTitleList:
-                    run = ATFPlatForm.getCaseRun(cycleId, _caseNo, _name)
+                    run = ATFPlatForm.getCaseRun(_name)
                     if run['caserunid'] !='00000':
                         isRun=True
             else:
                 _name = _caseTitleList[0]
-                run = ATFPlatForm.getCaseRun(cycleId,_caseNo, _name)
+                run = ATFPlatForm.getCaseRun(_name)
                 if run['caserunid'] != '00000':
                     isRun = True
         else:
             isRun = True
         return isRun
 
     @classmethod
@@ -331,7 +341,10 @@
                     case_link = f'{Constant.JIRA_URL}/browse/'
                     allure_testcase_link(case_link, info['summary']+"【无关联】")
                     allure_severity("P1")
         else:
             allure_title("未关联测试用例【请检查】")
 
 
+
+
+
```

### Comparing `common-test-29.9.25/common_test.egg-info/PKG-INFO` & `common-test-29.9.31/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.25
+Version: 29.9.31
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.25/common_test.egg-info/SOURCES.txt` & `common-test-29.9.31/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/common_test.egg-info/requires.txt` & `common-test-29.9.31/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.25/setup.py` & `common-test-29.9.31/setup.py`

 * *Files identical despite different names*

