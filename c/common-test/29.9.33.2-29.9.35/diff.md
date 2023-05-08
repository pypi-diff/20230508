# Comparing `tmp/common-test-29.9.33.2.tar.gz` & `tmp/common-test-29.9.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.33.2.tar", last modified: Mon May  8 05:48:34 2023, max compression
+gzip compressed data, was "common-test-29.9.35.tar", last modified: Mon May  8 06:50:54 2023, max compression
```

## Comparing `common-test-29.9.33.2.tar` & `common-test-29.9.35.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.105064 common-test-29.9.33.2/
--rw-r--r--   0 edz        (502) staff       (20)      625 2023-05-08 05:48:34.105209 common-test-29.9.33.2/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.069204 common-test-29.9.33.2/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.33.2/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.071194 common-test-29.9.33.2/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.33.2/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7021 2023-05-06 02:44:55.000000 common-test-29.9.33.2/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.33.2/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.073649 common-test-29.9.33.2/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.33.2/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.33.2/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.33.2/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.074549 common-test-29.9.33.2/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.33.2/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.33.2/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.076895 common-test-29.9.33.2/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.33.2/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.33.2/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.33.2/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.080896 common-test-29.9.33.2/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.33.2/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.33.2/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.086338 common-test-29.9.33.2/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.33.2/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.33.2/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.33.2/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.087272 common-test-29.9.33.2/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.33.2/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.33.2/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.091462 common-test-29.9.33.2/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3531 2023-05-08 04:08:54.000000 common-test-29.9.33.2/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.33.2/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.33.2/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13609 2023-05-05 06:58:50.000000 common-test-29.9.33.2/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.33.2/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8570 2023-05-08 05:47:33.000000 common-test-29.9.33.2/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.100811 common-test-29.9.33.2/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.33.2/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.33.2/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.33.2/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7903 2023-05-08 05:41:27.000000 common-test-29.9.33.2/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6706 2023-05-08 05:48:27.000000 common-test-29.9.33.2/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.33.2/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.33.2/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.33.2/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.33.2/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    16834 2023-05-08 03:28:26.000000 common-test-29.9.33.2/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 05:48:34.104614 common-test-29.9.33.2/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      625 2023-05-08 05:48:33.000000 common-test-29.9.33.2/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-08 05:48:33.000000 common-test-29.9.33.2/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-08 05:48:33.000000 common-test-29.9.33.2/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-08 05:48:33.000000 common-test-29.9.33.2/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-08 05:48:33.000000 common-test-29.9.33.2/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-08 05:48:33.000000 common-test-29.9.33.2/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      442 2023-05-08 05:48:34.105962 common-test-29.9.33.2/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.33.2/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.055615 common-test-29.9.35/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 06:50:54.055764 common-test-29.9.35/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.014014 common-test-29.9.35/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.35/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.016545 common-test-29.9.35/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.35/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7021 2023-05-06 02:44:55.000000 common-test-29.9.35/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.35/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.35/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.019196 common-test-29.9.35/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.35/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.35/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.35/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.35/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.020214 common-test-29.9.35/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.35/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.35/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.022625 common-test-29.9.35/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.35/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.35/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.35/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.026926 common-test-29.9.35/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.35/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.35/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.35/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.35/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.35/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.35/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.032454 common-test-29.9.35/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.35/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.35/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.35/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.35/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.35/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.35/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.35/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.033553 common-test-29.9.35/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.35/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.35/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.037665 common-test-29.9.35/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3531 2023-05-08 04:08:54.000000 common-test-29.9.35/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.35/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.35/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13609 2023-05-05 06:58:50.000000 common-test-29.9.35/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.35/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8570 2023-05-08 05:47:33.000000 common-test-29.9.35/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.048702 common-test-29.9.35/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.35/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.35/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.35/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7907 2023-05-08 06:33:14.000000 common-test-29.9.35/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6706 2023-05-08 05:48:27.000000 common-test-29.9.35/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.35/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.35/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.35/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.35/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    16834 2023-05-08 03:28:26.000000 common-test-29.9.35/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-08 06:50:54.055215 common-test-29.9.35/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-08 06:50:53.000000 common-test-29.9.35/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-08 06:50:53.000000 common-test-29.9.35/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-08 06:50:53.000000 common-test-29.9.35/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-08 06:50:53.000000 common-test-29.9.35/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-08 06:50:53.000000 common-test-29.9.35/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-08 06:50:53.000000 common-test-29.9.35/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-08 06:50:54.056574 common-test-29.9.35/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.35/setup.py
```

### Comparing `common-test-29.9.33.2/PKG-INFO` & `common-test-29.9.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.33.2
+Version: 29.9.35
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.33.2/common/autotest/base_requests.py` & `common-test-29.9.35/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/autotest/handle_allure.py` & `common-test-29.9.35/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/autotest/handle_assert.py` & `common-test-29.9.35/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/common/api_driver.py` & `common-test-29.9.35/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/common/constant.py` & `common-test-29.9.35/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/common/test.py` & `common-test-29.9.35/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/config/config.py` & `common-test-29.9.35/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/data/data_process.py` & `common-test-29.9.35/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/data/handle_common.py` & `common-test-29.9.35/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/db/handle_db.py` & `common-test-29.9.35/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/db/handle_db_batch.py` & `common-test-29.9.35/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/db/handle_mysqldb.py` & `common-test-29.9.35/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/db/handle_oracle.py` & `common-test-29.9.35/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/db/handle_sqlserver.py` & `common-test-29.9.35/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/file/ReadFile.py` & `common-test-29.9.35/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/file/handle_excel.py` & `common-test-29.9.35/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/file/handle_file.py` & `common-test-29.9.35/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/file/handle_reques.py` & `common-test-29.9.35/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/file/handle_system.py` & `common-test-29.9.35/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/file/handle_yaml.py` & `common-test-29.9.35/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/mq/handle_rabbit.py` & `common-test-29.9.35/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plat/ATF_platform.py` & `common-test-29.9.35/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plat/jenkin_platform.py` & `common-test-29.9.35/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plat/jira_platform.py` & `common-test-29.9.35/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plat/mysql_platform.py` & `common-test-29.9.35/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plat/service_platform.py` & `common-test-29.9.35/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/allure_plugin.py` & `common-test-29.9.35/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/assert_plugin.py` & `common-test-29.9.35/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/atf_plugin.py` & `common-test-29.9.35/common/plugin/atf_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             if _result['result'] == 'success':
                 JiraPlatForm.setJiraFlowStatus("2551")
             if DataProcess.isNotNull(get_system_key(Constant.SEND_URSER_LIST)):
                 _userList = get_system_key(Constant.SEND_URSER_LIST).split(',')
                 self.sendMsg(_desc, _userList)
             dict = {"issuekey": f'{_result["jirakey"]}', "project": f'{_result["projectName"]}',
                     "result": f'{_result["result"]}'}
-            ATFPlatForm.runDeploy("AutoTest-Result", dict)
+            ServicePlatForm.runDeploy("AutoTest-Result", dict)
 
 
     @classmethod
     def sendMsg(self, content, _list):
         for _index in range(len(_list)):
             _arr = str(_list[_index]).split('|')
             os.environ['toUserId'] = str(_arr[0]).lower()
```

### Comparing `common-test-29.9.33.2/common/plugin/data_bus.py` & `common-test-29.9.35/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/data_plugin.py` & `common-test-29.9.35/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/file_plugin.py` & `common-test-29.9.35/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/hooks_plugin.py` & `common-test-29.9.35/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/pytest_playwright.py` & `common-test-29.9.35/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common/plugin/pytest_plugin.py` & `common-test-29.9.35/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common_test.egg-info/PKG-INFO` & `common-test-29.9.35/common_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.33.2
+Version: 29.9.35
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.33.2/common_test.egg-info/SOURCES.txt` & `common-test-29.9.35/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/common_test.egg-info/requires.txt` & `common-test-29.9.35/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.33.2/setup.py` & `common-test-29.9.35/setup.py`

 * *Files identical despite different names*

