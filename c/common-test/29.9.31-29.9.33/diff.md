# Comparing `tmp/common-test-29.9.31.tar.gz` & `tmp/common-test-29.9.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.31.tar", last modified: Mon May  8 02:04:26 2023, max compression
+gzip compressed data, was "common-test-29.9.33.tar", last modified: Mon May  8 02:59:31 2023, max compression
```

## Comparing `common-test-29.9.31.tar` & `common-test-29.9.33.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.205552 common-test-29.9.31/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 02:04:26.205759 common-test-29.9.31/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.186705 common-test-29.9.31/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.31/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.188507 common-test-29.9.31/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.31/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7021 2023-05-06 02:44:55.000000 common-test-29.9.31/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.31/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.31/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.189864 common-test-29.9.31/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.31/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.31/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.31/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.31/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.190428 common-test-29.9.31/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.31/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.31/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.191433 common-test-29.9.31/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.31/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.31/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.31/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.193789 common-test-29.9.31/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.31/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.31/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.31/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.196299 common-test-29.9.31/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.31/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.31/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.31/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.31/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.196960 common-test-29.9.31/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.31/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.31/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.199109 common-test-29.9.31/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3594 2023-05-08 01:30:00.000000 common-test-29.9.31/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.31/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.31/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13609 2023-05-05 06:58:50.000000 common-test-29.9.31/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.31/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8671 2023-05-06 06:54:30.000000 common-test-29.9.31/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.202587 common-test-29.9.31/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.31/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.31/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.31/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7879 2023-05-05 07:35:27.000000 common-test-29.9.31/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6886 2023-05-08 02:03:18.000000 common-test-29.9.31/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.31/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.31/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.31/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.31/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    16627 2023-05-08 02:04:19.000000 common-test-29.9.31/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:04:26.205110 common-test-29.9.31/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-08 02:04:26.000000 common-test-29.9.31/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-08 02:04:26.206675 common-test-29.9.31/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.31/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.387913 common-test-29.9.33/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 02:59:31.388053 common-test-29.9.33/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.368802 common-test-29.9.33/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.33/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.369932 common-test-29.9.33/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.33/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7021 2023-05-06 02:44:55.000000 common-test-29.9.33/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.33/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.33/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.371570 common-test-29.9.33/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.33/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.33/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.33/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.33/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.372105 common-test-29.9.33/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.33/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.33/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.373085 common-test-29.9.33/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.33/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.33/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.33/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.375239 common-test-29.9.33/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.33/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.33/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.33/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.33/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.33/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.33/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.378031 common-test-29.9.33/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.33/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.33/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.33/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.33/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.33/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.33/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.33/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.378736 common-test-29.9.33/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.33/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.33/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.380997 common-test-29.9.33/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3594 2023-05-08 01:30:00.000000 common-test-29.9.33/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.33/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.33/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13609 2023-05-05 06:58:50.000000 common-test-29.9.33/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.33/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8671 2023-05-06 06:54:30.000000 common-test-29.9.33/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.384920 common-test-29.9.33/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.33/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.33/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.33/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7879 2023-05-05 07:35:27.000000 common-test-29.9.33/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6833 2023-05-08 02:36:24.000000 common-test-29.9.33/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.33/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.33/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.33/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.33/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    16745 2023-05-08 02:59:24.000000 common-test-29.9.33/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 02:59:31.387527 common-test-29.9.33/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 02:59:31.000000 common-test-29.9.33/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-08 02:59:31.000000 common-test-29.9.33/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-08 02:59:31.000000 common-test-29.9.33/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-08 02:59:31.000000 common-test-29.9.33/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-08 02:59:31.000000 common-test-29.9.33/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-08 02:59:31.000000 common-test-29.9.33/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-08 02:59:31.389263 common-test-29.9.33/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.33/setup.py
```

### Comparing `common-test-29.9.31/PKG-INFO` & `common-test-29.9.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.31
+Version: 29.9.33
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.31/common/autotest/base_requests.py` & `common-test-29.9.33/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/autotest/handle_allure.py` & `common-test-29.9.33/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/autotest/handle_assert.py` & `common-test-29.9.33/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/common/api_driver.py` & `common-test-29.9.33/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/common/constant.py` & `common-test-29.9.33/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/common/test.py` & `common-test-29.9.33/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/config/config.py` & `common-test-29.9.33/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/data/data_process.py` & `common-test-29.9.33/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/data/handle_common.py` & `common-test-29.9.33/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/db/handle_db.py` & `common-test-29.9.33/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/db/handle_db_batch.py` & `common-test-29.9.33/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/db/handle_mysqldb.py` & `common-test-29.9.33/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/db/handle_oracle.py` & `common-test-29.9.33/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/db/handle_sqlserver.py` & `common-test-29.9.33/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/file/ReadFile.py` & `common-test-29.9.33/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/file/handle_excel.py` & `common-test-29.9.33/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/file/handle_file.py` & `common-test-29.9.33/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/file/handle_reques.py` & `common-test-29.9.33/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/file/handle_system.py` & `common-test-29.9.33/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/file/handle_yaml.py` & `common-test-29.9.33/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/mq/handle_rabbit.py` & `common-test-29.9.33/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plat/ATF_platform.py` & `common-test-29.9.33/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plat/jenkin_platform.py` & `common-test-29.9.33/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plat/jira_platform.py` & `common-test-29.9.33/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plat/mysql_platform.py` & `common-test-29.9.33/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plat/service_platform.py` & `common-test-29.9.33/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/allure_plugin.py` & `common-test-29.9.33/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/assert_plugin.py` & `common-test-29.9.33/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/atf_plugin.py` & `common-test-29.9.33/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/data_bus.py` & `common-test-29.9.33/common/plugin/data_bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,21 +146,21 @@
 
     @classmethod
     def save_init_data(cls):
         """
         初始化DataBus数据
         :return:
         """
-        if DataProcess.isNotNull(get_system_key(Constant.Data_init)):
-            cls.save_yaml('common.setting',_replace=False)
-            cls.save_yaml('common')
-            cls.save_yaml(cls.get_env())
-            cls.get_data_atf()
-            cls.get_param()
-            cls.set_key(Constant.Data_init, Constant.Data_init)
+        cls.save_yaml('common.setting', _replace=False)
+        cls.save_yaml('common')
+        cls.save_yaml(cls.get_env())
+        cls.get_data_atf()
+        cls.get_param()
+        cls.set_key(Constant.Data_init, Constant.Data_init)
+
 
     @classmethod
     def run_info(cls):
         """
         打印信息
         :return:
         """
@@ -185,11 +185,12 @@
         print_databus_info(Constant.SEND_URSER_LIST, "通知人列表")
 
 
 
 if __name__ == '__main__':
     DataBus.set_key('RuntType',"3343434")
     DataBus.save_init_data()
-    print(os.environ.values())
+    print(DataProcess.isNotNull(get_system_key(Constant.Data_init)))
+
```

### Comparing `common-test-29.9.31/common/plugin/data_plugin.py` & `common-test-29.9.33/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/file_plugin.py` & `common-test-29.9.33/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/hooks_plugin.py` & `common-test-29.9.33/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/pytest_playwright.py` & `common-test-29.9.33/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common/plugin/pytest_plugin.py` & `common-test-29.9.33/common/plugin/pytest_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,17 +225,19 @@
             temp = item.__dict__['keywords'].__dict__['_markers']['__allure_display_name__']
             if temp != Constant.TEST_DATA_PARAMETER:
                 _caseTitle = temp
         except Exception as e:
             print_info('未通过装饰器title获取到用例信息')
         try:
             if _caseNo == '00000' or _caseNo is None:
-                _caseNo = item.__dict__['keywords'].__dict__['_markers']['pytestmark'][0].__dict__['args'][0]
-                # if str(_caseNo).find("(") > -1:
-                #     _caseNo = '00000'
+                _args= item.__dict__['keywords'].__dict__['_markers']['pytestmark']
+                for arg in _args:
+                     label_type = arg.__dict__['kwargs']['label_type']
+                     if label_type == 'as_id':
+                         _caseNo = arg.__dict__['args'][0]
         except Exception as e:
             print_info('未通过装饰器ID获取到用例信息')
         print_info(f"执行用例名称：{_caseTitle} 用例编号:{_caseNo}")
         print_info(f'用例数据:{_caseData}')
         return _caseTitle, _caseNo
 
     @classmethod
@@ -260,15 +262,15 @@
                 logger.info(f"---用例列表：无用例列表【请检查是否设置用例名称或者编号】 执行状态:{result}")
 
     @classmethod
     def sync_case_Script(self, item: Item, _caseTitle, _caseNo):
         _caseurl = PytestPlugin.getCaseUrl(item)
         if DataProcess.isNotNull(_caseTitle):
             _caseTitleList = _caseTitle.split(';')
-        if DataProcess.isNotNull(_caseNo):
+        if DataProcess.isNotNull(_caseNo) and _caseNo != '00000':
             _caseTitleList.extend(_caseNo.split(';'))
         if DataProcess.isNotNull(_caseTitleList):
             caseInfoList = ""
             if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
                 logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 【脚本用例同步】")
                 for _name in _caseTitleList:
                     if DataProcess.isNotNull(_name) and _name !='00000':
```

### Comparing `common-test-29.9.31/common_test.egg-info/PKG-INFO` & `common-test-29.9.33/common_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.31
+Version: 29.9.33
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.31/common_test.egg-info/SOURCES.txt` & `common-test-29.9.33/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/common_test.egg-info/requires.txt` & `common-test-29.9.33/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.31/setup.py` & `common-test-29.9.33/setup.py`

 * *Files identical despite different names*

