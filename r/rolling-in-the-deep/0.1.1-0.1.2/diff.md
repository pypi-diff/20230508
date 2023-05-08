# Comparing `tmp/rolling-in-the-deep-0.1.1.tar.gz` & `tmp/rolling-in-the-deep-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/admin/PycharmProjects/pythonProject/dist/tmpkx4r7zzs/rolling-in-the-deep-0.1.1.tar", last modified: Mon Apr 18 13:32:23 2022, max compression
+gzip compressed data, was "rolling-in-the-deep-0.1.2.tar", last modified: Mon May  8 09:35:39 2023, max compression
```

## Comparing `rolling-in-the-deep-0.1.1.tar` & `rolling-in-the-deep-0.1.2.tar`

### file list

```diff
@@ -1,104 +1,126 @@
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.756935 rolling-in-the-deep-0.1.1/
--rw-r--r--   0 admin      (502) staff       (20)     1073 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/LICENSE
--rw-r--r--   0 admin      (502) staff       (20)     1792 2022-04-18 13:32:23.756534 rolling-in-the-deep-0.1.1/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)     1280 2022-01-26 04:12:07.000000 rolling-in-the-deep-0.1.1/README.md
--rw-r--r--   0 admin      (502) staff       (20)      104 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/pyproject.toml
--rw-r--r--   0 admin      (502) staff       (20)       38 2022-04-18 13:32:23.757116 rolling-in-the-deep-0.1.1/setup.cfg
--rw-r--r--   0 admin      (502) staff       (20)     1841 2022-04-18 13:30:21.000000 rolling-in-the-deep-0.1.1/setup.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.685141 rolling-in-the-deep-0.1.1/src/
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.692573 rolling-in-the-deep-0.1.1/src/example_package/
--rw-r--r--   0 admin      (502) staff       (20)      479 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/example_package/RichTest.py
--rw-r--r--   0 admin      (502) staff       (20)      153 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/example_package/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)      193 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/example_package/example.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.695836 rolling-in-the-deep-0.1.1/src/rolling_in_the_deep.egg-info/
--rw-r--r--   0 admin      (502) staff       (20)     1792 2022-04-18 13:32:23.000000 rolling-in-the-deep-0.1.1/src/rolling_in_the_deep.egg-info/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)     3269 2022-04-18 13:32:23.000000 rolling-in-the-deep-0.1.1/src/rolling_in_the_deep.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2022-04-18 13:32:23.000000 rolling-in-the-deep-0.1.1/src/rolling_in_the_deep.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (502) staff       (20)       35 2022-04-18 13:32:23.000000 rolling-in-the-deep-0.1.1/src/rolling_in_the_deep.egg-info/top_level.txt
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.696445 rolling-in-the-deep-0.1.1/src/rolling_king/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/__init__.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.697032 rolling-in-the-deep-0.1.1/src/rolling_king/jason/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/__init__.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.698385 rolling-in-the-deep-0.1.1/src/rolling_king/jason/autogen/
--rw-r--r--   0 admin      (502) staff       (20)      153 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/autogen/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)     1171 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/autogen/auto_generate.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.699746 rolling-in-the-deep-0.1.1/src/rolling_king/jason/crawler/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/crawler/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)     2035 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/crawler/crawler_urllib.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.701061 rolling-in-the-deep-0.1.1/src/rolling_king/jason/newcore/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/newcore/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)     1041 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/newcore/test_ccc.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.702436 rolling-in-the-deep-0.1.1/src/rolling_king/jason/openpyxl/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/openpyxl/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)     1967 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/openpyxl/excel_util.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.705730 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pypac/
--rw-r--r--   0 admin      (502) staff       (20)      206 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pypac/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)       82 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pypac/pyfile1.py
--rw-r--r--   0 admin      (502) staff       (20)       81 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pypac/pyfile2.py
--rw-r--r--   0 admin      (502) staff       (20)      142 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pypac/test.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.709850 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pytest/
--rw-r--r--   0 admin      (502) staff       (20)      154 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pytest/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)      634 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pytest/conftest.py
--rw-r--r--   0 admin      (502) staff       (20)     1618 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pytest/test_class.py
--rw-r--r--   0 admin      (502) staff       (20)      430 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/pytest/test_sample.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.717147 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/
--rw-r--r--   0 admin      (502) staff       (20)    13268 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/ClassTest.py
--rw-r--r--   0 admin      (502) staff       (20)     1639 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/DbTest.py
--rw-r--r--   0 admin      (502) staff       (20)     1146 2022-03-29 13:07:09.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/MailTest.py
--rw-r--r--   0 admin      (502) staff       (20)    15111 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/MyPyTest.py
--rw-r--r--   0 admin      (502) staff       (20)    14302 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/PythonTest.py
--rw-r--r--   0 admin      (502) staff       (20)     1557 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/QueueTest.py
--rw-r--r--   0 admin      (502) staff       (20)    11731 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/SeniorTest.py
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/__init__.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.719760 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/socket/
--rw-r--r--   0 admin      (502) staff       (20)      424 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/socket/SocketClient.py
--rw-r--r--   0 admin      (502) staff       (20)      670 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/socket/SocketServer.py
--rw-r--r--   0 admin      (502) staff       (20)      154 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/socket/__init__.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.722762 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/thread/
--rw-r--r--   0 admin      (502) staff       (20)     2483 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/thread/ThreadingTest.py
--rw-r--r--   0 admin      (502) staff       (20)      910 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/thread/_ThreadTest.py
--rw-r--r--   0 admin      (502) staff       (20)      154 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/thread/__init__.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.727754 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/
--rw-r--r--   0 admin      (502) staff       (20)     1985 2022-03-29 13:07:09.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/ExcelTest.py
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)     1044 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/xmind_excel_converter.py
--rw-r--r--   0 admin      (502) staff       (20)     4808 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/zy_schedule.py
--rw-r--r--   0 admin      (502) staff       (20)     1161 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/zy_shell.py
--rw-r--r--   0 admin      (502) staff       (20)     1287 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/zy_stamp_tool.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.732514 rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)     3102 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/http_sender_module.py
--rw-r--r--   0 admin      (502) staff       (20)      763 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/test_ccc.py
--rw-r--r--   0 admin      (502) staff       (20)     6463 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/test_http.py
--rw-r--r--   0 admin      (502) staff       (20)     2442 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/test_m_project.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.734500 rolling-in-the-deep-0.1.1/src/rolling_king/jason/webdriver/
--rw-r--r--   0 admin      (502) staff       (20)      149 2022-03-29 13:07:09.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/webdriver/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)    11410 2022-04-02 06:52:57.000000 rolling-in-the-deep-0.1.1/src/rolling_king/jason/webdriver/webdriver_common.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.735706 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/__init__.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.738587 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)    15442 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/db_models.py
--rw-r--r--   0 admin      (502) staff       (20)     3112 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/db_util.py
--rw-r--r--   0 admin      (502) staff       (20)    11222 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/sqlalchemy_util.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.740631 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/requests/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/requests/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)     3338 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/requests/http_sender_module.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.747947 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)    16635 2022-04-18 13:30:21.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/eventcollect.py
--rw-r--r--   0 admin      (502) staff       (20)     2069 2022-04-18 13:30:21.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/get_service_info.py
--rw-r--r--   0 admin      (502) staff       (20)     1368 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py
--rw-r--r--   0 admin      (502) staff       (20)    10903 2022-04-07 07:38:41.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/update_idl.py
--rw-r--r--   0 admin      (502) staff       (20)      435 2022-04-18 13:30:21.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/utils.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.748648 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/
--rw-r--r--   0 admin      (502) staff       (20)      154 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/__init__.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.752526 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/
--rw-r--r--   0 admin      (502) staff       (20)        0 2022-03-29 05:39:13.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)    15835 2022-04-07 07:38:41.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/autotest_generator.py
--rw-r--r--   0 admin      (502) staff       (20)    14001 2022-04-02 07:32:21.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/base_compare.py
--rw-r--r--   0 admin      (502) staff       (20)    12354 2022-04-02 07:32:21.000000 rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/base_test.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2022-04-18 13:32:23.755648 rolling-in-the-deep-0.1.1/src/tests/
--rw-r--r--   0 admin      (502) staff       (20)      149 2022-04-02 06:52:57.000000 rolling-in-the-deep-0.1.1/src/tests/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)      789 2022-04-02 06:52:57.000000 rolling-in-the-deep-0.1.1/src/tests/conftest.py
--rw-r--r--   0 admin      (502) staff       (20)      760 2022-04-02 06:52:57.000000 rolling-in-the-deep-0.1.1/src/tests/test_options.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.641059 rolling-in-the-deep-0.1.2/
+-rw-rw-rw-   0        0        0     1073 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1805 2023-05-08 09:35:39.640058 rolling-in-the-deep-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1280 2022-01-26 04:12:06.000000 rolling-in-the-deep-0.1.2/README.md
+-rw-rw-rw-   0        0        0      104 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 09:35:39.641059 rolling-in-the-deep-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1905 2023-05-08 09:31:51.000000 rolling-in-the-deep-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.456506 rolling-in-the-deep-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.478509 rolling-in-the-deep-0.1.2/src/example_package/
+-rw-rw-rw-   0        0        0      494 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/example_package/RichTest.py
+-rw-rw-rw-   0        0        0      159 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/example_package/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/example_package/example.py
+-rw-rw-rw-   0        0        0     6602 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/example_package/pyecharts_test.py
+-rw-rw-rw-   0        0        0     7022 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/example_package/reportlab_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.486509 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/
+-rw-rw-rw-   0        0        0     1805 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3923 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-08 09:35:39.000000 rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.488510 rolling-in-the-deep-0.1.2/src/rolling_king/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.489510 rolling-in-the-deep-0.1.2/src/rolling_king/jason/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.492510 rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/
+-rw-rw-rw-   0        0        0      153 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/__init__.py
+-rw-rw-rw-   0        0        0     1171 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/auto_generate.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.495510 rolling-in-the-deep-0.1.2/src/rolling_king/jason/chatgpt/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/chatgpt/__init__.py
+-rw-rw-rw-   0        0        0     1885 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/chatgpt/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.499512 rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/__init__.py
+-rw-rw-rw-   0        0        0     1041 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/test_ccc.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.503512 rolling-in-the-deep-0.1.2/src/rolling_king/jason/openpyxl/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/openpyxl/__init__.py
+-rw-rw-rw-   0        0        0     2576 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/openpyxl/excel_util.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.509513 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/__init__.py
+-rw-rw-rw-   0        0        0    15090 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/playwright_common.py
+-rw-rw-rw-   0        0        0     2861 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/test_generate.py
+-rw-rw-rw-   0        0        0     1247 2023-05-08 09:20:22.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/playwright/test_playwright.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.517514 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/
+-rw-rw-rw-   0        0        0      206 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/__init__.py
+-rw-rw-rw-   0        0        0       82 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/pyfile1.py
+-rw-rw-rw-   0        0        0       81 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/pyfile2.py
+-rw-rw-rw-   0        0        0      142 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pypac/test.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.525323 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/
+-rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/__init__.py
+-rw-rw-rw-   0        0        0      634 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/conftest.py
+-rw-rw-rw-   0        0        0     1618 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/test_class.py
+-rw-rw-rw-   0        0        0      455 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.544046 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/
+-rw-rw-rw-   0        0        0    13268 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/ClassTest.py
+-rw-rw-rw-   0        0        0     1639 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/DbTest.py
+-rw-rw-rw-   0        0        0     1146 2022-03-29 13:07:08.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MailTest.py
+-rw-rw-rw-   0        0        0    15111 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MyPyTest.py
+-rw-rw-rw-   0        0        0    14302 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/PythonTest.py
+-rw-rw-rw-   0        0        0     1557 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/QueueTest.py
+-rw-rw-rw-   0        0        0    11731 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/SeniorTest.py
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.550047 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/
+-rw-rw-rw-   0        0        0      424 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/SocketClient.py
+-rw-rw-rw-   0        0        0      670 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/SocketServer.py
+-rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.556048 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/
+-rw-rw-rw-   0        0        0     2483 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/ThreadingTest.py
+-rw-rw-rw-   0        0        0      910 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/_ThreadTest.py
+-rw-rw-rw-   0        0        0      154 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.569050 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/
+-rw-rw-rw-   0        0        0     1985 2022-03-29 13:07:08.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/ExcelTest.py
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/__init__.py
+-rw-rw-rw-   0        0        0     1044 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/xmind_excel_converter.py
+-rw-rw-rw-   0        0        0     4991 2023-05-08 08:41:06.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_schedule.py
+-rw-rw-rw-   0        0        0     1161 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_shell.py
+-rw-rw-rw-   0        0        0     1340 2023-05-08 09:15:00.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_stamp_tool.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.579051 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/
+-rw-rw-rw-   0        0        0        0 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/__init__.py
+-rw-rw-rw-   0        0        0     3102 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/http_sender_module.py
+-rw-rw-rw-   0        0        0      763 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_ccc.py
+-rw-rw-rw-   0        0        0     6463 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_http.py
+-rw-rw-rw-   0        0        0     2442 2022-03-29 05:39:12.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_m_project.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.583051 rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/
+-rw-rw-rw-   0        0        0      155 2023-05-08 09:01:41.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/__init__.py
+-rw-rw-rw-   0        0        0    11714 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/webdriver_common.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.585051 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/
+-rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.591052 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/
+-rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/__init__.py
+-rw-rw-rw-   0        0        0    15845 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_models.py
+-rw-rw-rw-   0        0        0     3204 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_util.py
+-rw-rw-rw-   0        0        0    11495 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/sqlalchemy_util.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.595053 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/requests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/requests/__init__.py
+-rw-rw-rw-   0        0        0     3414 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/requests/http_sender_module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.604054 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/
+-rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/__init__.py
+-rw-rw-rw-   0        0        0    17075 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/eventcollect.py
+-rw-rw-rw-   0        0        0     2127 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/get_service_info.py
+-rw-rw-rw-   0        0        0     1411 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py
+-rw-rw-rw-   0        0        0    11163 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/update_idl.py
+-rw-rw-rw-   0        0        0      458 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.606055 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/
+-rw-rw-rw-   0        0        0      160 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.612055 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/
+-rw-rw-rw-   0        0        0        0 2023-05-08 08:41:07.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/__init__.py
+-rw-rw-rw-   0        0        0    16165 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/autotest_generator.py
+-rw-rw-rw-   0        0        0    14266 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_compare.py
+-rw-rw-rw-   0        0        0    12560 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_test.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.621056 rolling-in-the-deep-0.1.2/src/tests/
+-rw-rw-rw-   0        0        0      155 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.626057 rolling-in-the-deep-0.1.2/src/tests/apscheduler/
+-rw-rw-rw-   0        0        0      155 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/apscheduler/__init__.py
+-rw-rw-rw-   0        0        0     2080 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/apscheduler/backgroud_scheduler.py
+-rw-rw-rw-   0        0        0     7664 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/apscheduler/sample_apscheduler.py
+-rw-rw-rw-   0        0        0      881 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.629057 rolling-in-the-deep-0.1.2/src/tests/excel/
+-rw-rw-rw-   0        0        0      159 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/excel/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/excel/excel_test.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.633057 rolling-in-the-deep-0.1.2/src/tests/hive/
+-rw-rw-rw-   0        0        0      155 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/hive/__init__.py
+-rw-rw-rw-   0        0        0      555 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/hive/pyhive_test.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:35:39.638058 rolling-in-the-deep-0.1.2/src/tests/refresh_page/
+-rw-rw-rw-   0        0        0      159 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/refresh_page/__init__.py
+-rw-rw-rw-   0        0        0      903 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/refresh_page/data_analysis.py
+-rw-rw-rw-   0        0        0     2473 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/refresh_page/temp_refresh.py
+-rw-rw-rw-   0        0        0      788 2023-05-08 09:01:42.000000 rolling-in-the-deep-0.1.2/src/tests/test_options.py
+-rw-rw-rw-   0        0        0     1644 2023-05-08 09:15:01.000000 rolling-in-the-deep-0.1.2/src/tests/upload_file_test.py
```

### Comparing `rolling-in-the-deep-0.1.1/LICENSE` & `rolling-in-the-deep-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/PKG-INFO` & `rolling-in-the-deep-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,35 @@
-Metadata-Version: 2.1
-Name: rolling-in-the-deep
-Version: 0.1.1
-Summary: Python Project For QA Test
-Home-page: https://gitee.com/jason024/python_project
-Author: RollingKing
-Author-email: 386773780@qq.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://gitee.com/jason024/python_project/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pythonProject
-
-#### 介绍
-{**以下是 Gitee 平台说明，您可以替换此简介**
-Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
-无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}
-
-#### 软件架构
-软件架构说明
-
-
-#### 安装教程
-
-1.  xxxx
-2.  xxxx
-3.  xxxx
-
-#### 使用说明
-
-1.  xxxx
-2.  xxxx
-3.  xxxx
-
-#### 参与贡献
-
-1.  JasonZheng
-
-#### 特技
-
-1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
-2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
-3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
-4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
-5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
-6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
-
-
+# pythonProject
+
+#### 介绍
+{**以下是 Gitee 平台说明，您可以替换此简介**
+Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
+无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}
+
+#### 软件架构
+软件架构说明
+
+
+#### 安装教程
+
+1.  xxxx
+2.  xxxx
+3.  xxxx
+
+#### 使用说明
+
+1.  xxxx
+2.  xxxx
+3.  xxxx
+
+#### 参与贡献
+
+1.  JasonZheng
+
+#### 特技
+
+1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
+2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
+3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
+4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
+5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
+6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
```

### Comparing `rolling-in-the-deep-0.1.1/README.md` & `rolling-in-the-deep-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: rolling-in-the-deep
+Version: 0.1.2
+Summary: Python Project For QA Test
+Home-page: https://gitee.com/jason024/python_project
+Author: RollingKing
+Author-email: 386773780@qq.com
+Project-URL: Bug Tracker, https://gitee.com/jason024/python_project/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pythonProject
 
 #### 介绍
 {**以下是 Gitee 平台说明，您可以替换此简介**
 Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
 无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_in_the_deep.egg-info/SOURCES.txt` & `rolling-in-the-deep-0.1.2/src/rolling_in_the_deep.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/example_package/RichTest.py
 src/example_package/__init__.py
 src/example_package/example.py
+src/example_package/pyecharts_test.py
+src/example_package/reportlab_pdf.py
 src/rolling_in_the_deep.egg-info/PKG-INFO
 src/rolling_in_the_deep.egg-info/SOURCES.txt
 src/rolling_in_the_deep.egg-info/dependency_links.txt
 src/rolling_in_the_deep.egg-info/top_level.txt
 src/rolling_king/__init__.py
 src/rolling_king/jason/__init__.py
 src/rolling_king/jason/autogen/__init__.py
 src/rolling_king/jason/autogen/auto_generate.py
-src/rolling_king/jason/crawler/__init__.py
-src/rolling_king/jason/crawler/crawler_urllib.py
+src/rolling_king/jason/chatgpt/__init__.py
+src/rolling_king/jason/chatgpt/openai.py
 src/rolling_king/jason/newcore/__init__.py
 src/rolling_king/jason/newcore/test_ccc.py
 src/rolling_king/jason/openpyxl/__init__.py
 src/rolling_king/jason/openpyxl/excel_util.py
+src/rolling_king/jason/playwright/__init__.py
+src/rolling_king/jason/playwright/playwright_common.py
+src/rolling_king/jason/playwright/test_generate.py
+src/rolling_king/jason/playwright/test_playwright.py
 src/rolling_king/jason/pypac/__init__.py
 src/rolling_king/jason/pypac/pyfile1.py
 src/rolling_king/jason/pypac/pyfile2.py
 src/rolling_king/jason/pypac/test.py
 src/rolling_king/jason/pytest/__init__.py
 src/rolling_king/jason/pytest/conftest.py
 src/rolling_king/jason/pytest/test_class.py
@@ -70,8 +76,19 @@
 src/rolling_king/zijie/tests/__init__.py
 src/rolling_king/zijie/tests/base/__init__.py
 src/rolling_king/zijie/tests/base/autotest_generator.py
 src/rolling_king/zijie/tests/base/base_compare.py
 src/rolling_king/zijie/tests/base/base_test.py
 src/tests/__init__.py
 src/tests/conftest.py
-src/tests/test_options.py
+src/tests/test_options.py
+src/tests/upload_file_test.py
+src/tests/apscheduler/__init__.py
+src/tests/apscheduler/backgroud_scheduler.py
+src/tests/apscheduler/sample_apscheduler.py
+src/tests/excel/__init__.py
+src/tests/excel/excel_test.py
+src/tests/hive/__init__.py
+src/tests/hive/pyhive_test.py
+src/tests/refresh_page/__init__.py
+src/tests/refresh_page/data_analysis.py
+src/tests/refresh_page/temp_refresh.py
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/autogen/auto_generate.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/autogen/auto_generate.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/newcore/test_ccc.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/newcore/test_ccc.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/pytest/conftest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/conftest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/pytest/test_class.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/pytest/test_class.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/ClassTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/ClassTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/DbTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/DbTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/MailTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MailTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/MyPyTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/MyPyTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/PythonTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/PythonTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/QueueTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/QueueTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/SeniorTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/SeniorTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/socket/SocketServer.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/socket/SocketServer.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/thread/ThreadingTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/ThreadingTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/thread/_ThreadTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/thread/_ThreadTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/ExcelTest.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/ExcelTest.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/xmind_excel_converter.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/xmind_excel_converter.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/zy_schedule.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_schedule.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2022/1/28 4:20 下午
-# @Author  : zhengyu.0985
-# @FileName: zy_schedule.py
-# @Software: PyCharm
-
-import schedule
-import time
-import threading
-import functools
-import logging
-
-logging.basicConfig(level=logging.DEBUG,
-                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
-logger = logging.getLogger('com.zijie.db.sqlalchemy_util')
-
-
-# def job():
-#     print("I'm working...")
-#
-#
-# schedule.every(10).seconds.do(job)
-#
-# while True:
-#     schedule.run_pending()  # 检测是否执行
-#     time.sleep(1)
-#     logger.info("Waiting for 1 second...")
-
-def job():
-    print("I'm working...")
-
-
-# 每十分钟执行任务
-schedule.every(10).minutes.do(job)
-# 每个小时执行任务
-schedule.every().hour.do(job)
-# 每天的10:30执行任务
-schedule.every().day.at("10:30").do(job)
-# 每个月执行任务
-schedule.every().monday.do(job)
-# 每个星期三的13:15分执行任务
-schedule.every().wednesday.at("13:15").do(job)
-# 每分钟的第17秒执行任务
-schedule.every().minute.at(":17").do(job)
-
-while True:
-    schedule.run_pending()
-    time.sleep(1)
-
-
-# 只运行一次
-def job_that_executes_once():
-    # 此处编写的任务只会执行一次...
-    return schedule.CancelJob
-
-
-schedule.every().day.at('22:30').do(job_that_executes_once)
-
-while True:
-    schedule.run_pending()
-    time.sleep(1)
-
-
-# 参数传递
-def greet(name):
-    print('Hello', name)
-
-
-# do() 将额外的参数传递给job函数
-schedule.every(2).seconds.do(greet, name='Alice')
-schedule.every(4).seconds.do(greet, name='Bob')
-
-
-# 获取所有作业 and 取消所有作业
-def hello():
-    print('Hello world')
-
-
-schedule.every().second.do(hello)
-
-all_jobs = schedule.get_jobs()  # 获取
-schedule.clear()  # 取消
-
-
-# .tag 打标签
-schedule.every().day.do(greet, 'Andrea').tag('daily-tasks', 'friend')
-schedule.every().hour.do(greet, 'John').tag('hourly-tasks', 'friend')
-schedule.every().hour.do(greet, 'Monica').tag('hourly-tasks', 'customer')
-schedule.every().day.do(greet, 'Derek').tag('daily-tasks', 'guest')
-
-# get_jobs(标签)：可以获取所有该标签的任务
-friends = schedule.get_jobs('friend')
-
-# 取消所有 daily-tasks 标签的任务
-schedule.clear('daily-tasks')
-
-
-# 设定截止时间
-# 每个小时运行作业，18:30后停止
-schedule.every(1).hours.until("18:30").do(job)
-
-# 每个小时运行作业，2030-01-01 18:33 today
-schedule.every(1).hours.until("2030-01-01 18:33").do(job)
-
-# 每个小时运行作业，8个小时后停止
-schedule.every(1).hours.until(timedelta(hours=8)).do(job)
-
-# 每个小时运行作业，11:32:42后停止
-schedule.every(1).hours.until(time(11, 33, 42)).do(job)
-
-# 每个小时运行作业，2020-5-17 11:36:20后停止
-schedule.every(1).hours.until(datetime(2020, 5, 17, 11, 36, 20)).do(job)
-
-
-# 立即运行所有作业，而不管其安排如何
-schedule.run_all()
-# 立即运行所有作业，每次作业间隔10秒
-schedule.run_all(delay_seconds=10)
-
-
-# 装饰器安排作业
-# 此装饰器效果等同于 schedule.every(10).minutes.do(job)
-@repeat(every(10).minutes)
-def job():
-    print("I am a scheduled job")
-
-
-while True:
-    run_pending()
-    time.sleep(1)
-
-
-# 并行执行
-# 默认情况下，Schedule 按顺序执行所有作业
-# 通过多线程的形式来并行每个作业
-
-def job1():
-    print("I'm running on thread %s" % threading.current_thread())
-def job2():
-    print("I'm running on thread %s" % threading.current_thread())
-def job3():
-    print("I'm running on thread %s" % threading.current_thread())
-
-def run_threaded(job_func):
-    job_thread = threading.Thread(target=job_func)
-    job_thread.start()
-
-
-schedule.every(10).seconds.do(run_threaded, job1)
-schedule.every(10).seconds.do(run_threaded, job2)
-schedule.every(10).seconds.do(run_threaded, job3)
-
-while True:
-    schedule.run_pending()
-    time.sleep(1)
-
-
-# 异常处理
-# Schedule 不会自动捕捉异常，它遇到异常会直接抛出
-
-def catch_exceptions(cancel_on_failure=False):
-    def catch_exceptions_decorator(job_func):
-        @functools.wraps(job_func)
-        def wrapper(*args, **kwargs):
-            try:
-                return job_func(*args, **kwargs)
-            except:
-                import traceback
-                print(traceback.format_exc())
-                if cancel_on_failure:
-                    return schedule.CancelJob
-        return wrapper
-    return catch_exceptions_decorator
-
-
-@catch_exceptions(cancel_on_failure=True)
-def bad_task():
-    return 1 / 0
-
-
-# 这样，bad_task 在执行时遇到的任何错误，都会被 catch_exceptions  捕获，这点在保证调度任务正常运转的时候非常关键。
-schedule.every(5).minutes.do(bad_task)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2022/1/28 4:20 下午
+# @Author  : zhengyu.0985
+# @FileName: zy_schedule.py
+# @Software: PyCharm
+
+import schedule
+import time
+import threading
+import functools
+import logging
+
+logging.basicConfig(level=logging.DEBUG,
+                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
+logger = logging.getLogger('com.zijie.db.sqlalchemy_util')
+
+
+# def job():
+#     print("I'm working...")
+#
+#
+# schedule.every(10).seconds.do(job)
+#
+# while True:
+#     schedule.run_pending()  # 检测是否执行
+#     time.sleep(1)
+#     logger.info("Waiting for 1 second...")
+
+def job():
+    print("I'm working...")
+
+
+# 每十分钟执行任务
+schedule.every(10).minutes.do(job)
+# 每个小时执行任务
+schedule.every().hour.do(job)
+# 每天的10:30执行任务
+schedule.every().day.at("10:30").do(job)
+# 每个月执行任务
+schedule.every().monday.do(job)
+# 每个星期三的13:15分执行任务
+schedule.every().wednesday.at("13:15").do(job)
+# 每分钟的第17秒执行任务
+schedule.every().minute.at(":17").do(job)
+
+while True:
+    schedule.run_pending()
+    time.sleep(1)
+
+
+# 只运行一次
+def job_that_executes_once():
+    # 此处编写的任务只会执行一次...
+    return schedule.CancelJob
+
+
+schedule.every().day.at('22:30').do(job_that_executes_once)
+
+while True:
+    schedule.run_pending()
+    time.sleep(1)
+
+
+# 参数传递
+def greet(name):
+    print('Hello', name)
+
+
+# do() 将额外的参数传递给job函数
+schedule.every(2).seconds.do(greet, name='Alice')
+schedule.every(4).seconds.do(greet, name='Bob')
+
+
+# 获取所有作业 and 取消所有作业
+def hello():
+    print('Hello world')
+
+
+schedule.every().second.do(hello)
+
+all_jobs = schedule.get_jobs()  # 获取
+schedule.clear()  # 取消
+
+
+# .tag 打标签
+schedule.every().day.do(greet, 'Andrea').tag('daily-tasks', 'friend')
+schedule.every().hour.do(greet, 'John').tag('hourly-tasks', 'friend')
+schedule.every().hour.do(greet, 'Monica').tag('hourly-tasks', 'customer')
+schedule.every().day.do(greet, 'Derek').tag('daily-tasks', 'guest')
+
+# get_jobs(标签)：可以获取所有该标签的任务
+friends = schedule.get_jobs('friend')
+
+# 取消所有 daily-tasks 标签的任务
+schedule.clear('daily-tasks')
+
+
+# 设定截止时间
+# 每个小时运行作业，18:30后停止
+schedule.every(1).hours.until("18:30").do(job)
+
+# 每个小时运行作业，2030-01-01 18:33 today
+schedule.every(1).hours.until("2030-01-01 18:33").do(job)
+
+# 每个小时运行作业，8个小时后停止
+schedule.every(1).hours.until(timedelta(hours=8)).do(job)
+
+# 每个小时运行作业，11:32:42后停止
+schedule.every(1).hours.until(time(11, 33, 42)).do(job)
+
+# 每个小时运行作业，2020-5-17 11:36:20后停止
+schedule.every(1).hours.until(datetime(2020, 5, 17, 11, 36, 20)).do(job)
+
+
+# 立即运行所有作业，而不管其安排如何
+schedule.run_all()
+# 立即运行所有作业，每次作业间隔10秒
+schedule.run_all(delay_seconds=10)
+
+
+# 装饰器安排作业
+# 此装饰器效果等同于 schedule.every(10).minutes.do(job)
+@repeat(every(10).minutes)
+def job():
+    print("I am a scheduled job")
+
+
+while True:
+    run_pending()
+    time.sleep(1)
+
+
+# 并行执行
+# 默认情况下，Schedule 按顺序执行所有作业
+# 通过多线程的形式来并行每个作业
+
+def job1():
+    print("I'm running on thread %s" % threading.current_thread())
+def job2():
+    print("I'm running on thread %s" % threading.current_thread())
+def job3():
+    print("I'm running on thread %s" % threading.current_thread())
+
+def run_threaded(job_func):
+    job_thread = threading.Thread(target=job_func)
+    job_thread.start()
+
+
+schedule.every(10).seconds.do(run_threaded, job1)
+schedule.every(10).seconds.do(run_threaded, job2)
+schedule.every(10).seconds.do(run_threaded, job3)
+
+while True:
+    schedule.run_pending()
+    time.sleep(1)
+
+
+# 异常处理
+# Schedule 不会自动捕捉异常，它遇到异常会直接抛出
+
+def catch_exceptions(cancel_on_failure=False):
+    def catch_exceptions_decorator(job_func):
+        @functools.wraps(job_func)
+        def wrapper(*args, **kwargs):
+            try:
+                return job_func(*args, **kwargs)
+            except:
+                import traceback
+                print(traceback.format_exc())
+                if cancel_on_failure:
+                    return schedule.CancelJob
+        return wrapper
+    return catch_exceptions_decorator
+
+
+@catch_exceptions(cancel_on_failure=True)
+def bad_task():
+    return 1 / 0
+
+
+# 这样，bad_task 在执行时遇到的任何错误，都会被 catch_exceptions  捕获，这点在保证调度任务正常运转的时候非常关键。
+schedule.every(5).minutes.do(bad_task)
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/zy_shell.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_shell.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/python/tools/zy_stamp_tool.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/python/tools/zy_stamp_tool.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2022/3/8 4:08 下午
-# @Author  : zhengyu.0985
-# @FileName: zy_stamp_tool.py
-# @Software: PyCharm
-
-from datetime import datetime
-import time
-
-
-class TimeStampExchange(object):
-
-    @staticmethod
-    def stamp2datetime(stamp_val=None):
-        if stamp_val is None:
-            return datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        elif len(str(stamp_val)) == 13:
-            return datetime.fromtimestamp(stamp_val/1000).strftime('%Y-%m-%d %H:%M:%S')
-        else:
-            return datetime.fromtimestamp(stamp_val).strftime('%Y-%m-%d %H:%M:%S')
-
-    @staticmethod
-    def datetime2stamp(date_time_str=None, stamp_digits=10):
-        if date_time_str is None:
-            date_time_str = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        date_time_obj = datetime.strptime(date_time_str, '%Y-%m-%d %H:%M:%S')
-        if stamp_digits == 13:
-            return int(time.mktime(date_time_obj.timetuple()) * 1000 + date_time_obj.microsecond / 1000)
-        else:
-            return int(date_time_obj.timestamp())
-
-
-if __name__ == '__main__':
-    val = TimeStampExchange.stamp2datetime(1646201351000)
-    print(val)
-    print('-----------')
-    val = TimeStampExchange.datetime2stamp("2022-03-02 14:09:11", 13)
-    print(val)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2022/3/8 4:08 下午
+# @Author  : zhengyu.0985
+# @FileName: zy_stamp_tool.py
+# @Software: PyCharm
+
+from datetime import datetime
+import time
+
+
+class TimeStampExchange(object):
+
+    @staticmethod
+    def stamp2datetime(stamp_val=None) -> str:
+        if stamp_val is None:
+            return datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        elif len(str(stamp_val)) == 13:
+            return datetime.fromtimestamp(stamp_val/1000).strftime('%Y-%m-%d %H:%M:%S')
+        else:
+            return datetime.fromtimestamp(stamp_val).strftime('%Y-%m-%d %H:%M:%S')
+
+    @staticmethod
+    def datetime2stamp(date_time_str=None, stamp_digits=10) -> int:
+        if date_time_str is None:
+            date_time_str = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        date_time_obj = datetime.strptime(date_time_str, '%Y-%m-%d %H:%M:%S')
+        if stamp_digits == 13:
+            return int(time.mktime(date_time_obj.timetuple()) * 1000 + date_time_obj.microsecond / 1000)
+        else:
+            return int(date_time_obj.timestamp())
+
+
+if __name__ == '__main__':
+    val = TimeStampExchange.stamp2datetime(1646201351000)
+    print(val)
+    print('-----------')
+    val = TimeStampExchange.datetime2stamp("2022-03-02 14:09:11", 13)
+    print(val)
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/http_sender_module.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/http_sender_module.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/test_ccc.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_ccc.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/test_http.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_http.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/requests/test_m_project.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/requests/test_m_project.py`

 * *Files identical despite different names*

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/jason/webdriver/webdriver_common.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/jason/webdriver/webdriver_common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,260 +1,261 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2022/3/29 1:43 PM
-# @Author  : zhengyu.0985
-# @FileName: webdriver_common.py
-# @Software: PyCharm
-
-import logging
-import time
-
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from selenium.webdriver.chrome.service import Service
-from selenium.webdriver.common.action_chains import ActionChains
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.wait import WebDriverWait
-from selenium.webdriver.remote.webelement import WebElement
-from selenium.webdriver.common.keys import Keys
-from typing import List
-
-logging.basicConfig(level=logging.DEBUG,
-                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')
-logger = logging.getLogger("my_driver")
-
-
-class WebDriverCommon(object):
-    driver = None
-    action = None
-
-    @classmethod
-    def _browser_options(cls, browser_type='Chrome'):
-        if browser_type == 'Firefox':
-            options = webdriver.FirefoxOptions()
-        elif browser_type == 'IE':
-            options = webdriver.IeOptions()
-        else:
-            options = webdriver.ChromeOptions()
-        # 像Options中添加实验选项。
-        options.add_experimental_option(name="excludeSwitches", value=["enable-automation"])
-        return options
-
-    @classmethod
-    def init_driver(cls, driver_type='Chrome', executable_path=None):
-        if cls.driver is None:
-            if executable_path is None:
-                if driver_type == 'Firefox':
-                    cls.driver = webdriver.Firefox(options=cls._browser_options(browser_type=driver_type))
-                elif driver_type == 'IE':
-                    cls.driver = webdriver.Ie(options=cls._browser_options(browser_type=driver_type))
-                else:
-                    cls.driver = webdriver.Chrome(options=cls._browser_options())
-            else:
-                service_obj = Service(executable_path=executable_path)
-                # Chrome类的初始化，executable_path已不建议使用，所以使用Service对象。
-                if driver_type == 'Firefox':
-                    cls.driver = webdriver.Firefox(service=service_obj,
-                                                   options=cls._browser_options(browser_type=driver_type))
-                elif driver_type == 'IE':
-                    cls.driver = webdriver.Ie(service=service_obj,
-                                              options=cls._browser_options(browser_type=driver_type))
-                else:
-                    cls.driver = webdriver.Chrome(service=service_obj, options=cls._browser_options())
-
-            logger.info('The driver object of WebDriverCommon class was successfully initialized.')
-        else:
-            logger.warning('The driver object of WebDriverCommon class has been already initialized.')
-
-    @classmethod
-    def navigate(cls, url):
-        cls.driver.get(url)
-
-    @classmethod
-    def refresh(cls):
-        cls.driver.refresh()
-
-    @classmethod
-    def max_window(cls):
-        cls.driver.maximize_window()
-
-    @classmethod
-    def min_window(cls):
-        cls.driver.minimize_window()
-
-    @classmethod
-    def set_action(cls):
-        if cls.driver is None:
-            logger.error("Driver is None, so cannot initialize ActionChains.")
-        else:
-            cls.action = ActionChains(cls.driver)
-            logger.info("Initialize ActionChains successfully by Driver.")
-
-    @classmethod
-    def is_ele_exist(cls, by_locator: str, locator_value: str) -> bool:
-        # e.g: element = driver.find_element(By.ID, 'foo')
-        try:
-            web_ele = cls.driver.find_element(by_locator, locator_value)
-            if web_ele is None:
-                logger.warning("[失败]：{}={}, 未能定位到WebElement".format(by_locator, locator_value))
-                return False
-            else:
-                logger.info("[成功]：{}={}, 成功定位到WebElement".format(by_locator, locator_value))
-                return True
-        except Exception as e:
-            logger.warning("[异常]：{}={}, 未能定位到WebElement".format(by_locator, locator_value))
-            logger.warning(e.args)
-            return False
-        finally:
-            logger.info("is_ele_exist class func has been executed.")
-
-    @classmethod
-    def switch_to_new_window(cls):
-        handles_list = cls.driver.window_handles()
-        for handle in handles_list:
-            if handle == cls.driver.current_window_handle:
-                pass
-            else:
-                cls.driver.switch_to.window(handle)
-
-    @classmethod
-    def wait_implicitly(cls, time_in_seconds):
-        cls.driver.implicitly_wait(time_to_wait=time_in_seconds)
-
-    @classmethod
-    def wait_for_load(cls, tuple_locator: tuple, presence_or_visibility='visibility', time_out=10, frequency=0.5) -> WebElement:
-        try:
-            web_driver_wait = WebDriverWait(cls.driver, timeout=time_out, poll_frequency=frequency)
-            if presence_or_visibility == 'visibility':
-                result = web_driver_wait.until(method=EC.visibility_of_element_located(tuple_locator),
-                                               message="超时未找到")
-            elif presence_or_visibility == 'presence':
-                result = web_driver_wait.until(method=EC.presence_of_element_located(tuple_locator),
-                                               message="超时未找到")
-            else:
-                logger.warning("presence_or_visibility only supports visibility or presence.")
-                result = None
-            if isinstance(result, WebElement):
-                logger.info("Locator={}, 元素已成功加载。".format(tuple_locator))
-            else:
-                logger.warning("未等到元素加载。")
-                logger.info("result={}".format(result))
-            return result
-        except Exception as e:
-            logger.error(e.args)
-            logger.error(e)
-        finally:
-            logger.info("wait_for_load method has been executed.")
-
-    @classmethod
-    def find_element(cls, by_locator: str, locator_value: str, curr_web_ele=None) -> WebElement:
-        try:
-            if curr_web_ele is None:
-                web_ele = cls.driver.find_element(by_locator, locator_value)
-                logger.info("[成功]：{}={}, 成功定位到WebElement".format(by_locator, locator_value))
-            elif isinstance(curr_web_ele, WebElement):
-                web_ele = curr_web_ele.find_element(by_locator, locator_value)
-                logger.info("[成功]：基于当前Element[{}], 通过 {}={}, 成功定位到WebElement".format(curr_web_ele, by_locator, locator_value))
-            else:
-                logger.info("所传参数curr_web_ele类型错误，必须是WebElement类型。")
-                web_ele = None
-        except Exception as e:
-            logger.error(e.args)
-            web_ele = None
-        finally:
-            logger.info("find_element method has been executed.")
-        return web_ele
-
-    @classmethod
-    def find_element_list(cls, by_locator: str, locator_value: str, curr_web_ele=None) -> List[WebElement]:
-        try:
-            if curr_web_ele is None:
-                web_ele_list = cls.driver.find_elements(by_locator, locator_value)
-                logger.info("[成功]：{}={}, 成功获取到WebElement List。".format(by_locator, locator_value))
-            elif isinstance(curr_web_ele, WebElement):
-                web_ele_list = curr_web_ele.find_elements(by_locator, locator_value)
-                logger.info("[成功]：基于当前Element[{}], 通过 {}={}, 成功获取到WebElement List。".format(curr_web_ele, by_locator, locator_value))
-            else:
-                logger.info("所传参数curr_web_ele类型错误，必须是WebElement类型。")
-                web_ele_list = []
-        except Exception as e:
-            logger.error(e.args)
-            web_ele_list = []
-        finally:
-            logger.info("find_element_list method has been executed.")
-        return web_ele_list
-
-    @classmethod
-    def switch_to_iframe(cls, frame_id_name_ele):
-        # driver.switch_to.frame('frame_name')
-        # driver.switch_to.frame(1)
-        # driver.switch_to.frame(driver.find_elements(By.TAG_NAME, "iframe")[0])
-        try:
-            if isinstance(frame_id_name_ele, int):
-                cls.driver.switch_to.frame(frame_id_name_ele)
-                logger.info("通过Integer Index={}, 进入iFrame。".format(frame_id_name_ele))
-            elif isinstance(frame_id_name_ele, str):
-                cls.driver.switch_to.frame(frame_id_name_ele)
-                logger.info("通过iFrame Name={}, 进入iFrame。".format(frame_id_name_ele))
-            elif isinstance(frame_id_name_ele, WebElement):
-                cls.driver.switch_to.frame(frame_id_name_ele)
-                logger.info("通过iFrame WebElement={}, 进入iFrame。".format(frame_id_name_ele))
-            else:
-                logger.warning("frame_id_name_ele参数，仅支持int、str、WebElement类型。")
-        except Exception as e:
-            logger.error(e.args)
-        finally:
-            logger.info("switch_to_iFrame method has been executed.")
-
-    @classmethod
-    def switch_to_default_content(cls):
-        cls.driver.switch_to.default_content()
-
-    @classmethod
-    def right_click(cls, on_web_ele, int_down_times):
-        if cls.action is None:
-            logger.error("尚未未初始化ActionChains对象action.")
-        else:
-            cls.action.context_click(on_element=on_web_ele).perform()
-            for i in range(int_down_times):  # 当前点击向下键无反应。
-                # cls.action.send_keys(Keys.ARROW_DOWN)
-                cls.action.key_down(Keys.ARROW_DOWN)
-                cls.wait_implicitly(1)
-                cls.action.key_up(Keys.ARROW_DOWN)
-                logger.info("第{}次点击向下键。".format(i))
-            cls.action.send_keys(Keys.ENTER)
-            logger.info("回车选中。")
-
-    @classmethod
-    def move_to_ele(cls, web_ele, x_off_set=None, y_off_set=None):
-        if web_ele is None:
-            logger.error("给定WebElement is None.")
-            return None
-        elif x_off_set is None or y_off_set is None:
-            return cls.action.move_to_element(web_ele)
-        else:
-            return cls.action.move_to_element_with_offset(web_ele, xoffset=x_off_set, yoffset=y_off_set)
-
-    @classmethod
-    def close_driver(cls):
-        cls.driver.close()
-        logger.info("成功关闭WebDriver")
-
-
-if __name__ == '__main__':
-    WebDriverCommon.init_driver(executable_path='./chromedriver')
-    WebDriverCommon.navigate("https://www.baidu.com")
-    WebDriverCommon.refresh()
-    WebDriverCommon.max_window()
-    logger.info(WebDriverCommon.is_ele_exist(By.ID, "s-top-left"))
-    ele = WebDriverCommon.wait_for_load((By.XPATH, "//div[@id='s-top-left']/a[1]"))
-    logger.info(type(ele))
-    logger.info(ele)
-    WebDriverCommon.set_action()
-    # WebDriverCommon.right_click(ele, 3)  # 该功能有Bug
-    WebDriverCommon.wait_implicitly(3)  # 该功能不生效
-    search_input = (By.ID, 'kw')
-    search_button = (By.ID, 'su')
-    WebDriverCommon.find_element(*search_input).send_keys("郑宇")
-    WebDriverCommon.find_element(*search_button).click()
-    time.sleep(3)
-    WebDriverCommon.close_driver()
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2022/3/29 1:43 PM
+# @Author  : zhengyu.0985
+# @FileName: webdriver_common.py
+# @Software: PyCharm
+
+import logging
+import time
+
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.common.action_chains import ActionChains
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.remote.webelement import WebElement
+from selenium.webdriver.common.keys import Keys
+from typing import List
+
+logging.basicConfig(level=logging.DEBUG,
+                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')
+logger = logging.getLogger("my_driver")
+
+
+class WebDriverCommon(object):
+    driver = None
+    action = None
+
+    @classmethod
+    def _browser_options(cls, browser_type='Chrome'):
+        if browser_type == 'Firefox':
+            options = webdriver.FirefoxOptions()
+        elif browser_type == 'IE':
+            options = webdriver.IeOptions()
+        else:
+            options = webdriver.ChromeOptions()
+        # 像Options中添加实验选项。
+        options.add_experimental_option(name="excludeSwitches", value=["enable-automation"])
+        options.add_argument("--headless")
+        return options
+
+    @classmethod
+    def init_driver(cls, driver_type='Chrome', executable_path=None):
+        if cls.driver is None:
+            if executable_path is None:
+                if driver_type == 'Firefox':
+                    cls.driver = webdriver.Firefox(options=cls._browser_options(browser_type=driver_type))
+                elif driver_type == 'IE':
+                    cls.driver = webdriver.Ie(options=cls._browser_options(browser_type=driver_type))
+                else:
+                    cls.driver = webdriver.Chrome(options=cls._browser_options())
+            else:
+                service_obj = Service(executable_path=executable_path)
+                # Chrome类的初始化，executable_path已不建议使用，所以使用Service对象。
+                if driver_type == 'Firefox':
+                    cls.driver = webdriver.Firefox(service=service_obj,
+                                                   options=cls._browser_options(browser_type=driver_type))
+                elif driver_type == 'IE':
+                    cls.driver = webdriver.Ie(service=service_obj,
+                                              options=cls._browser_options(browser_type=driver_type))
+                else:
+                    cls.driver = webdriver.Chrome(service=service_obj, options=cls._browser_options())
+
+            logger.info('The driver object of WebDriverCommon class was successfully initialized.')
+        else:
+            logger.warning('The driver object of WebDriverCommon class has been already initialized.')
+
+    @classmethod
+    def navigate(cls, url):
+        cls.driver.get(url)
+
+    @classmethod
+    def refresh(cls):
+        cls.driver.refresh()
+
+    @classmethod
+    def max_window(cls):
+        cls.driver.maximize_window()
+
+    @classmethod
+    def min_window(cls):
+        cls.driver.minimize_window()
+
+    @classmethod
+    def set_action(cls):
+        if cls.driver is None:
+            logger.error("Driver is None, so cannot initialize ActionChains.")
+        else:
+            cls.action = ActionChains(cls.driver)
+            logger.info("Initialize ActionChains successfully by Driver.")
+
+    @classmethod
+    def is_ele_exist(cls, by_locator: str, locator_value: str) -> bool:
+        # e.g: element = driver.find_element(By.ID, 'foo')
+        try:
+            web_ele = cls.driver.find_element(by_locator, locator_value)
+            if web_ele is None:
+                logger.warning("[失败]：{}={}, 未能定位到WebElement".format(by_locator, locator_value))
+                return False
+            else:
+                logger.info("[成功]：{}={}, 成功定位到WebElement".format(by_locator, locator_value))
+                return True
+        except Exception as e:
+            logger.warning("[异常]：{}={}, 未能定位到WebElement".format(by_locator, locator_value))
+            logger.warning(e.args)
+            return False
+        finally:
+            logger.info("is_ele_exist class func has been executed.")
+
+    @classmethod
+    def switch_to_new_window(cls):
+        handles_list = cls.driver.window_handles()
+        for handle in handles_list:
+            if handle == cls.driver.current_window_handle:
+                pass
+            else:
+                cls.driver.switch_to.window(handle)
+
+    @classmethod
+    def wait_implicitly(cls, time_in_seconds):
+        cls.driver.implicitly_wait(time_to_wait=time_in_seconds)
+
+    @classmethod
+    def wait_for_load(cls, tuple_locator: tuple, presence_or_visibility='visibility', time_out=10, frequency=0.5) -> WebElement:
+        try:
+            web_driver_wait = WebDriverWait(cls.driver, timeout=time_out, poll_frequency=frequency)
+            if presence_or_visibility == 'visibility':
+                result = web_driver_wait.until(method=EC.visibility_of_element_located(tuple_locator),
+                                               message="超时未找到")
+            elif presence_or_visibility == 'presence':
+                result = web_driver_wait.until(method=EC.presence_of_element_located(tuple_locator),
+                                               message="超时未找到")
+            else:
+                logger.warning("presence_or_visibility only supports visibility or presence.")
+                result = None
+            if isinstance(result, WebElement):
+                logger.info("Locator={}, 元素已成功加载。".format(tuple_locator))
+            else:
+                logger.warning("未等到元素加载。")
+                logger.info("result={}".format(result))
+            return result
+        except Exception as e:
+            logger.error(e.args)
+            logger.error(e)
+        finally:
+            logger.info("wait_for_load method has been executed.")
+
+    @classmethod
+    def find_element(cls, by_locator: str, locator_value: str, curr_web_ele=None) -> WebElement:
+        try:
+            if curr_web_ele is None:
+                web_ele = cls.driver.find_element(by_locator, locator_value)
+                logger.info("[成功]：{}={}, 成功定位到WebElement".format(by_locator, locator_value))
+            elif isinstance(curr_web_ele, WebElement):
+                web_ele = curr_web_ele.find_element(by_locator, locator_value)
+                logger.info("[成功]：基于当前Element[{}], 通过 {}={}, 成功定位到WebElement".format(curr_web_ele, by_locator, locator_value))
+            else:
+                logger.info("所传参数curr_web_ele类型错误，必须是WebElement类型。")
+                web_ele = None
+        except Exception as e:
+            logger.error(e.args)
+            web_ele = None
+        finally:
+            logger.info("find_element method has been executed.")
+        return web_ele
+
+    @classmethod
+    def find_element_list(cls, by_locator: str, locator_value: str, curr_web_ele=None) -> List[WebElement]:
+        try:
+            if curr_web_ele is None:
+                web_ele_list = cls.driver.find_elements(by_locator, locator_value)
+                logger.info("[成功]：{}={}, 成功获取到WebElement List。".format(by_locator, locator_value))
+            elif isinstance(curr_web_ele, WebElement):
+                web_ele_list = curr_web_ele.find_elements(by_locator, locator_value)
+                logger.info("[成功]：基于当前Element[{}], 通过 {}={}, 成功获取到WebElement List。".format(curr_web_ele, by_locator, locator_value))
+            else:
+                logger.info("所传参数curr_web_ele类型错误，必须是WebElement类型。")
+                web_ele_list = []
+        except Exception as e:
+            logger.error(e.args)
+            web_ele_list = []
+        finally:
+            logger.info("find_element_list method has been executed.")
+        return web_ele_list
+
+    @classmethod
+    def switch_to_iframe(cls, frame_id_name_ele):
+        # driver.switch_to.frame('frame_name')
+        # driver.switch_to.frame(1)
+        # driver.switch_to.frame(driver.find_elements(By.TAG_NAME, "iframe")[0])
+        try:
+            if isinstance(frame_id_name_ele, int):
+                cls.driver.switch_to.frame(frame_id_name_ele)
+                logger.info("通过Integer Index={}, 进入iFrame。".format(frame_id_name_ele))
+            elif isinstance(frame_id_name_ele, str):
+                cls.driver.switch_to.frame(frame_id_name_ele)
+                logger.info("通过iFrame Name={}, 进入iFrame。".format(frame_id_name_ele))
+            elif isinstance(frame_id_name_ele, WebElement):
+                cls.driver.switch_to.frame(frame_id_name_ele)
+                logger.info("通过iFrame WebElement={}, 进入iFrame。".format(frame_id_name_ele))
+            else:
+                logger.warning("frame_id_name_ele参数，仅支持int、str、WebElement类型。")
+        except Exception as e:
+            logger.error(e.args)
+        finally:
+            logger.info("switch_to_iFrame method has been executed.")
+
+    @classmethod
+    def switch_to_default_content(cls):
+        cls.driver.switch_to.default_content()
+
+    @classmethod
+    def right_click(cls, on_web_ele, int_down_times):
+        if cls.action is None:
+            logger.error("尚未未初始化ActionChains对象action.")
+        else:
+            cls.action.context_click(on_element=on_web_ele).perform()
+            for i in range(int_down_times):  # 当前点击向下键无反应。
+                # cls.action.send_keys(Keys.ARROW_DOWN)
+                cls.action.key_down(Keys.ARROW_DOWN)
+                cls.wait_implicitly(1)
+                cls.action.key_up(Keys.ARROW_DOWN)
+                logger.info("第{}次点击向下键。".format(i))
+            cls.action.send_keys(Keys.ENTER)
+            logger.info("回车选中。")
+
+    @classmethod
+    def move_to_ele(cls, web_ele, x_off_set=None, y_off_set=None):
+        if web_ele is None:
+            logger.error("给定WebElement is None.")
+            return None
+        elif x_off_set is None or y_off_set is None:
+            return cls.action.move_to_element(web_ele)
+        else:
+            return cls.action.move_to_element_with_offset(web_ele, xoffset=x_off_set, yoffset=y_off_set)
+
+    @classmethod
+    def close_driver(cls):
+        cls.driver.close()
+        logger.info("成功关闭WebDriver")
+
+
+if __name__ == '__main__':
+    WebDriverCommon.init_driver(executable_path='./chromedriver')
+    WebDriverCommon.navigate("https://www.baidu.com")
+    WebDriverCommon.refresh()
+    WebDriverCommon.max_window()
+    logger.info(WebDriverCommon.is_ele_exist(By.ID, "s-top-left"))
+    ele = WebDriverCommon.wait_for_load((By.XPATH, "//div[@id='s-top-left']/a[1]"))
+    logger.info(type(ele))
+    logger.info(ele)
+    WebDriverCommon.set_action()
+    # WebDriverCommon.right_click(ele, 3)  # 该功能有Bug
+    WebDriverCommon.wait_implicitly(3)  # 该功能不生效
+    search_input = (By.ID, 'kw')
+    search_button = (By.ID, 'su')
+    WebDriverCommon.find_element(*search_input).send_keys("郑宇")
+    WebDriverCommon.find_element(*search_button).click()
+    time.sleep(3)
+    WebDriverCommon.close_driver()
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/db_models.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_models.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,403 +1,403 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2021/12/8 3:26 下午
-# @Author  : zhengyu.0985
-# @FileName: db_models.py
-# @Software: PyCharm
-
-from rolling_king.zijie.db.sqlalchemy_util import AlchemyUtil
-from sqlalchemy import Column, Integer, String, Text, ForeignKey, DateTime, UniqueConstraint, Index
-import datetime
-import json
-import re
-
-
-class CaseRecordModel(AlchemyUtil.Base):
-
-    __tablename__ = 'pytest_case_record'
-
-    uid = Column(Integer, primary_key=True, autoincrement=True)  # '测试用例唯一标识'
-    test_project_name = Column(String(64))  # 'QA的Python测试项目名称'
-    test_psm = Column(String(32))  # '被测PSM'
-    test_interface = Column(String(64))  # '被测接口: Http接口是subrui, Thrift接口是Service.Method'
-    test_inter_type = Column(String(8))  # '接口协议类型'
-    test_class = Column(String(64))  # 'Pytest的测试类：package.Class'
-    test_method = Column(String(64))  # 'Pytest的测试方法名'
-    test_description = Column(String(128))  # '测试用例描述'
-    version = Column(Integer)  # '用例版本号'
-    gmt_create = Column(DateTime, default=datetime.datetime.now)  # '记录创建时间'
-    gmt_modify = Column(DateTime, default=datetime.datetime.now)  # '记录修改时间'
-
-    def to_json(self):
-        dict = self.__dict__
-        if "_sa_instance_state" in dict:
-            del dict["_sa_instance_state"]
-        return dict
-
-
-# 重写JSONEncoder的default方法，object转换成dict
-class CaseRecordEncoder(json.JSONEncoder):
-    # 重写default方法
-    def default(self, obj):
-        """
-        把【Object】转成【Dict字典】
-        :param obj:
-        :return:
-        """
-        if isinstance(obj, CaseRecordModel):
-            return {
-                'uid': obj.uid,
-                'test_project_name': obj.test_project_name,
-                'test_psm': obj.test_psm,
-                'test_interface': obj.test_interface,
-                'test_inter_type': obj.test_inter_type,
-                'test_class': obj.test_class,
-                'test_method': obj.test_method,
-                'test_description': obj.test_description,
-                'version': obj.version,
-                'gmt_create': obj.gmt_create,
-                'gmt_modify': obj.gmt_modify
-            }
-        else:
-            return json.JSONEncoder.default(self, obj)
-
-    # 重写encode方法
-    def encode(self, obj):
-        """
-        把【Object】转成【Dict字典】再转成【String】
-        :param obj:
-        :return:
-        """
-        if isinstance(obj, CaseRecordModel):
-            dict_val = {
-                'uid': obj.uid,
-                'test_project_name': obj.test_project_name,
-                'test_psm': obj.test_psm,
-                'test_interface': obj.test_interface,
-                'test_inter_type': obj.test_inter_type,
-                'test_class': obj.test_class,
-                'test_method': obj.test_method,
-                'test_description': obj.test_description,
-                'version': obj.version,
-                'gmt_create': obj.gmt_create,
-                'gmt_modify': obj.gmt_modify
-            }
-            return str(dict_val)
-        else:
-            return json.JSONEncoder.encode(self, obj)
-
-
-# 重写JSONDecoder的decode方法，dict转换成object
-class CaseRecordDecoder(json.JSONDecoder):
-
-    def decode(self, dict_str):
-        """
-        把【字符串】转成【字典】再转成【Object】
-        :param dict_str: 字典的字符串
-        :return:
-        """
-        dict_val = super().decode(dict_str)  # 先把str转dict
-        # 下面是dict转object
-        CaseRecordDecoder.dict_to_obj(dict_val)
-
-    @staticmethod
-    def dict_to_obj(dict_val):
-        """
-        把【字典Dict】直接转成对应的【Object】
-        :param dict_val:
-        :return:
-        """
-        case_record_model = CaseRecordModel()
-        if 'uid' in dict_val.keys():
-            case_record_model.uid = dict_val['uid']
-        else:
-            case_record_model.uid = 0
-        case_record_model.test_project_name = dict_val['test_project_name']
-        case_record_model.test_psm = dict_val['test_psm']
-        case_record_model.test_interface = dict_val['test_interface']
-        case_record_model.test_inter_type = dict_val['test_inter_type']
-        case_record_model.test_class = dict_val['test_class']
-        case_record_model.test_method = dict_val['test_method']
-        case_record_model.test_description = dict_val['test_description']
-        case_record_model.version = dict_val['version']
-        return case_record_model
-
-############################################################################
-
-
-class ExecutionRecordModel(AlchemyUtil.Base):
-
-    __tablename__ = 'pytest_execution_record'
-
-    uid = Column(Integer, primary_key=True, autoincrement=True)  # '测试记录每一个TestCase的唯一标识'
-    test_unique_tag = Column(String(64))  # '一次整体测试的唯一标签'
-    test_project_name = Column(String(64))  # 'QA的Python测试项目名称'
-    test_psm = Column(String(32))  # '被测PSM'
-    test_interface = Column(String(64))  # '被测接口: Http接口是subrui, Thrift接口是Service.Method'
-    test_inter_type = Column(String(8))  # '接口协议类型'
-    test_class = Column(String(64))  # 'Pytest的测试类：package.Class'
-    test_method = Column(String(64))  # 'Pytest的测试方法名'
-    test_result = Column(String(8))  # '测试用例执行结果'
-    test_params = Column(String(64))  # 'Pytest的测试方法入参'
-    test_duration = Column(Integer)  # '测试用例执行耗时'
-    test_start_time = Column(String(64))  # '测试用例执行起始时间'
-    test_finish_time = Column(String(64))  # '测试用例执行完成时间'
-    test_assert = Column(String(8))  # '测试用例是否使用Assert断言'
-    test_error_msg = Column(String(32))  # '测试用例失败信息'
-    gmt_create = Column(DateTime, default=datetime.datetime.now)  # '记录创建时间'
-    gmt_modify = Column(DateTime, default=datetime.datetime.now)  # '记录修改时间'
-
-    def to_json(self):
-        dict = self.__dict__
-        if "_sa_instance_state" in dict:
-            del dict["_sa_instance_state"]
-        return dict
-
-
-# 重写JSONEncoder的default方法，object转换成dict
-class ExecutionRecordEncoder(json.JSONEncoder):
-    # 重写default方法
-    def default(self, execution_obj):
-        """
-        把【Object】转成【Dict字典】
-        :param execution_obj:
-        :return:
-        """
-        if isinstance(execution_obj, ExecutionRecordModel):
-            return {
-                'uid': execution_obj.uid,
-                'test_unique_tag': execution_obj.test_unique_tag,
-                'test_project_name': execution_obj.test_project_name,
-                'test_psm': execution_obj.test_psm,
-                'test_interface': execution_obj.test_interface,
-                'test_inter_type': execution_obj.test_inter_type,
-                'test_class': execution_obj.test_class,
-                'test_method': execution_obj.test_method,
-                'test_result': execution_obj.test_result,
-                'test_params': execution_obj.test_params,
-                'test_duration': execution_obj.test_duration,
-                'test_start_time': execution_obj.test_start_time,
-                'test_finish_time': execution_obj.test_finish_time,
-                'test_assert': execution_obj.test_assert,
-                'test_error_msg': execution_obj.test_error_msg,
-                'gmt_create': execution_obj.gmt_create,
-                'gmt_modify': execution_obj.gmt_modify
-            }
-        else:
-            return json.JSONEncoder.default(self, execution_obj)
-
-    # 重写encode方法
-    def encode(self, execution_obj):
-        """
-        把【Object】转成【Dict字典】再转成【String】
-        :param execution_obj:
-        :return:
-        """
-        if isinstance(execution_obj, CaseRecordModel):
-            return str(ExecutionRecordEncoder.default(execution_obj))
-        else:
-            return json.JSONEncoder.encode(self, execution_obj)
-
-
-# 重写JSONDecoder的decode方法，dict转换成object
-class ExecutionRecordDecoder(json.JSONDecoder):
-
-    def decode(self, dict_str):
-        """
-        把【字符串】转成【字典】再转成【Object】
-        :param dict_str: 字典的字符串
-        :return:
-        """
-        dict_val = super().decode(dict_str)  # 先把str转dict
-        # 下面是dict转object
-        ExecutionRecordDecoder.dict_to_obj(dict_val)
-
-    @staticmethod
-    def dict_to_obj(dict_val):
-        """
-        把【字典Dict】直接转成对应的【Object】
-        :param dict_val:
-        :return:
-        """
-        execution_record_model = ExecutionRecordModel()
-        if 'uid' in dict_val.keys():
-            execution_record_model.uid = dict_val['uid']
-        else:
-            execution_record_model.uid = 0
-        execution_record_model.test_unique_tag = dict_val['test_unique_tag']
-        execution_record_model.test_project_name = dict_val['test_project_name']
-        execution_record_model.test_psm = dict_val['test_psm']
-        execution_record_model.test_interface = dict_val['test_interface']
-        execution_record_model.test_inter_type = dict_val['test_inter_type']
-        execution_record_model.test_class = dict_val['test_class']
-        execution_record_model.test_method = dict_val['test_method']
-        execution_record_model.test_result = dict_val['test_result']
-        execution_record_model.test_params = dict_val['test_params']
-        execution_record_model.test_duration = dict_val['test_duration']
-        execution_record_model.test_start_time = dict_val['test_start_time']
-        execution_record_model.test_finish_time = dict_val['test_finish_time']
-        execution_record_model.test_assert = dict_val['test_assert']
-        execution_record_model.test_error_msg = dict_val['test_error_msg']
-        return execution_record_model
-
-
-#################################################################################
-###### 下方是全部接口Model：BamInterModel 和 未覆盖接口Model：NonCovInterModel ######
-
-FLAGS = re.VERBOSE | re.MULTILINE | re.DOTALL
-WHITESPACE = re.compile(r'[ \t\n\r]*', FLAGS)
-
-
-def gen_unique_key():
-    dt = datetime.datetime.now()
-    dt_str = dt.strftime('%Y%m%d%H%M%S')
-    ts = datetime.datetime.timestamp(dt)
-    ts_str = str(int(ts * 1000000))
-    unique_key = dt_str + ts_str
-    return unique_key
-
-
-class BamInterModel(AlchemyUtil.Base):
-
-    __bind_key__ = "site_reldb"  # 若不指定，则使用默认数据库。
-    __tablename__ = 'psm_inter_info'
-
-    id = Column(String(32), primary_key=True)
-    psm = Column(String(64), nullable=False)
-    endpoint_id = Column(String(64), nullable=False)
-    method = Column(String(8))
-    path = Column(String(128))
-    level = Column(Integer)
-    name = Column(String(64))
-    note = Column(String(64))
-    rpc_method = Column(String(64))
-    creator = Column(String(16))
-    updater = Column(String(32))
-    modify_time = Column(String(32))
-    create_time = Column(String(32))
-    publish_status = Column(Integer)
-    priority = Column(Integer)
-    version = Column(String(8))
-    gmt_create = Column(DateTime, default=datetime.datetime.now)
-
-    def to_json(self):
-        dict = self.__dict__
-        if "_sa_instance_state" in dict:
-            del dict["_sa_instance_state"]
-        return dict
-
-
-# 重写JSONEncoder的default方法，object转换成dict
-class BamInterEncoder(json.JSONEncoder):
-    # 重写default方法
-    def default(self, obj):
-        """
-        把【Object】转成【Dict字典】
-        :param obj:
-        :return:
-        """
-        if isinstance(obj, BamInterModel):
-            return {
-                'id': obj.id,
-                'psm': obj.psm,
-                'endpoint_id': obj.endpoint_id,
-                'method': obj.method,
-                'path': obj.path,
-                'level': obj.level,
-                'name': obj.name,
-                'note': obj.note,
-                'rpc_method': obj.rpc_method,
-                'creator': obj.creator,
-                'updater': obj.updater,
-                'create_time': obj.create_time,
-                'modify_time': obj.modify_time,
-                'publish_status': obj.publish_status,
-                'priority': obj.priority,
-                'version': obj.version,
-                'gmt_create': obj.gmt_create
-            }
-        else:
-            return json.JSONEncoder.default(self, obj)
-
-    # 重写encode方法
-    def encode(self, obj):
-        """
-        把【Object】转成【Dict字典】再转成【String】
-        :param obj:
-        :return:
-        """
-        if isinstance(obj, BamInterModel):
-            return str(self.default(obj))
-        else:
-            return json.JSONEncoder.encode(self, obj)
-
-
-# 重写JSONDecoder的decode方法，dict转换成object
-class BamInterDecoder(json.JSONDecoder):
-
-    def decode(self, dict_str, _w=WHITESPACE.match):
-        """
-        把【字符串】转成【字典】再转成【Object】
-        :param dict_str: 字典的字符串
-        :param _w:
-        :return:
-        """
-        dict_val = super().decode(dict_str)  # 先把str转dict
-        # 下面是dict转object
-        self.dict_to_obj(dict_val)
-
-    @staticmethod
-    def dict_to_obj(dict_val):
-        """
-        把【字典Dict】直接转成对应的【Object】
-        :param dict_val:
-        :return:
-        """
-        bam_inter_model = BamInterModel()
-        if 'uid' in dict_val.keys():
-            bam_inter_model.id = dict_val['id']
-        else:
-            bam_inter_model.id = gen_unique_key()
-        bam_inter_model.psm = dict_val['psm']
-        bam_inter_model.endpoint_id = dict_val['endpoint_id']
-        bam_inter_model.method = dict_val['method']
-        bam_inter_model.path = dict_val['path']
-        bam_inter_model.level = dict_val['level']
-        bam_inter_model.name = dict_val['name']
-        bam_inter_model.note = dict_val['note']
-        bam_inter_model.rpc_method = dict_val['rpc_method']
-        bam_inter_model.creator = dict_val['creator']
-        bam_inter_model.updater = dict_val['updater']
-        bam_inter_model.create_time = dict_val['create_time']
-        bam_inter_model.modify_time = dict_val['modify_time']
-        bam_inter_model.publish_status = dict_val['publish_status']
-        bam_inter_model.priority = dict_val['priority']
-        bam_inter_model.version = dict_val['version']
-        if 'gmt_create' in dict_val.keys():
-            bam_inter_model.gmt_create = dict_val['gmt_create']
-        return bam_inter_model
-
-
-class NonCovInterModel(AlchemyUtil.Base):
-
-    __bind_key__ = "site_reldb"  # 若不指定，则使用默认数据库。
-    __tablename__ = 'psm_non_cov_inter'
-
-    id = Column(String(32), primary_key=True)
-    psm = Column(String(64), nullable=False)
-    endpoint_id = Column(String(64), nullable=False)
-    method = Column(String(8))
-    path = Column(String(128))
-    name = Column(String(64))
-    note = Column(String(64))
-    rpc_method = Column(String(64))
-    version = Column(String(8))
-    gmt_create = Column(DateTime, default=datetime.datetime.now)
-
-    def to_json(self):
-        dict = self.__dict__
-        if "_sa_instance_state" in dict:
-            del dict["_sa_instance_state"]
-        return dict
-
-
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2021/12/8 3:26 下午
+# @Author  : zhengyu.0985
+# @FileName: db_models.py
+# @Software: PyCharm
+
+from rolling_king.zijie.db.sqlalchemy_util import AlchemyUtil
+from sqlalchemy import Column, Integer, String, Text, ForeignKey, DateTime, UniqueConstraint, Index
+import datetime
+import json
+import re
+
+
+class CaseRecordModel(AlchemyUtil.Base):
+
+    __tablename__ = 'pytest_case_record'
+
+    uid = Column(Integer, primary_key=True, autoincrement=True)  # '测试用例唯一标识'
+    test_project_name = Column(String(64))  # 'QA的Python测试项目名称'
+    test_psm = Column(String(32))  # '被测PSM'
+    test_interface = Column(String(64))  # '被测接口: Http接口是subrui, Thrift接口是Service.Method'
+    test_inter_type = Column(String(8))  # '接口协议类型'
+    test_class = Column(String(64))  # 'Pytest的测试类：package.Class'
+    test_method = Column(String(64))  # 'Pytest的测试方法名'
+    test_description = Column(String(128))  # '测试用例描述'
+    version = Column(Integer)  # '用例版本号'
+    gmt_create = Column(DateTime, default=datetime.datetime.now)  # '记录创建时间'
+    gmt_modify = Column(DateTime, default=datetime.datetime.now)  # '记录修改时间'
+
+    def to_json(self):
+        dict = self.__dict__
+        if "_sa_instance_state" in dict:
+            del dict["_sa_instance_state"]
+        return dict
+
+
+# 重写JSONEncoder的default方法，object转换成dict
+class CaseRecordEncoder(json.JSONEncoder):
+    # 重写default方法
+    def default(self, obj):
+        """
+        把【Object】转成【Dict字典】
+        :param obj:
+        :return:
+        """
+        if isinstance(obj, CaseRecordModel):
+            return {
+                'uid': obj.uid,
+                'test_project_name': obj.test_project_name,
+                'test_psm': obj.test_psm,
+                'test_interface': obj.test_interface,
+                'test_inter_type': obj.test_inter_type,
+                'test_class': obj.test_class,
+                'test_method': obj.test_method,
+                'test_description': obj.test_description,
+                'version': obj.version,
+                'gmt_create': obj.gmt_create,
+                'gmt_modify': obj.gmt_modify
+            }
+        else:
+            return json.JSONEncoder.default(self, obj)
+
+    # 重写encode方法
+    def encode(self, obj):
+        """
+        把【Object】转成【Dict字典】再转成【String】
+        :param obj:
+        :return:
+        """
+        if isinstance(obj, CaseRecordModel):
+            dict_val = {
+                'uid': obj.uid,
+                'test_project_name': obj.test_project_name,
+                'test_psm': obj.test_psm,
+                'test_interface': obj.test_interface,
+                'test_inter_type': obj.test_inter_type,
+                'test_class': obj.test_class,
+                'test_method': obj.test_method,
+                'test_description': obj.test_description,
+                'version': obj.version,
+                'gmt_create': obj.gmt_create,
+                'gmt_modify': obj.gmt_modify
+            }
+            return str(dict_val)
+        else:
+            return json.JSONEncoder.encode(self, obj)
+
+
+# 重写JSONDecoder的decode方法，dict转换成object
+class CaseRecordDecoder(json.JSONDecoder):
+
+    def decode(self, dict_str):
+        """
+        把【字符串】转成【字典】再转成【Object】
+        :param dict_str: 字典的字符串
+        :return:
+        """
+        dict_val = super().decode(dict_str)  # 先把str转dict
+        # 下面是dict转object
+        CaseRecordDecoder.dict_to_obj(dict_val)
+
+    @staticmethod
+    def dict_to_obj(dict_val):
+        """
+        把【字典Dict】直接转成对应的【Object】
+        :param dict_val:
+        :return:
+        """
+        case_record_model = CaseRecordModel()
+        if 'uid' in dict_val.keys():
+            case_record_model.uid = dict_val['uid']
+        else:
+            case_record_model.uid = 0
+        case_record_model.test_project_name = dict_val['test_project_name']
+        case_record_model.test_psm = dict_val['test_psm']
+        case_record_model.test_interface = dict_val['test_interface']
+        case_record_model.test_inter_type = dict_val['test_inter_type']
+        case_record_model.test_class = dict_val['test_class']
+        case_record_model.test_method = dict_val['test_method']
+        case_record_model.test_description = dict_val['test_description']
+        case_record_model.version = dict_val['version']
+        return case_record_model
+
+############################################################################
+
+
+class ExecutionRecordModel(AlchemyUtil.Base):
+
+    __tablename__ = 'pytest_execution_record'
+
+    uid = Column(Integer, primary_key=True, autoincrement=True)  # '测试记录每一个TestCase的唯一标识'
+    test_unique_tag = Column(String(64))  # '一次整体测试的唯一标签'
+    test_project_name = Column(String(64))  # 'QA的Python测试项目名称'
+    test_psm = Column(String(32))  # '被测PSM'
+    test_interface = Column(String(64))  # '被测接口: Http接口是subrui, Thrift接口是Service.Method'
+    test_inter_type = Column(String(8))  # '接口协议类型'
+    test_class = Column(String(64))  # 'Pytest的测试类：package.Class'
+    test_method = Column(String(64))  # 'Pytest的测试方法名'
+    test_result = Column(String(8))  # '测试用例执行结果'
+    test_params = Column(String(64))  # 'Pytest的测试方法入参'
+    test_duration = Column(Integer)  # '测试用例执行耗时'
+    test_start_time = Column(String(64))  # '测试用例执行起始时间'
+    test_finish_time = Column(String(64))  # '测试用例执行完成时间'
+    test_assert = Column(String(8))  # '测试用例是否使用Assert断言'
+    test_error_msg = Column(String(32))  # '测试用例失败信息'
+    gmt_create = Column(DateTime, default=datetime.datetime.now)  # '记录创建时间'
+    gmt_modify = Column(DateTime, default=datetime.datetime.now)  # '记录修改时间'
+
+    def to_json(self):
+        dict = self.__dict__
+        if "_sa_instance_state" in dict:
+            del dict["_sa_instance_state"]
+        return dict
+
+
+# 重写JSONEncoder的default方法，object转换成dict
+class ExecutionRecordEncoder(json.JSONEncoder):
+    # 重写default方法
+    def default(self, execution_obj):
+        """
+        把【Object】转成【Dict字典】
+        :param execution_obj:
+        :return:
+        """
+        if isinstance(execution_obj, ExecutionRecordModel):
+            return {
+                'uid': execution_obj.uid,
+                'test_unique_tag': execution_obj.test_unique_tag,
+                'test_project_name': execution_obj.test_project_name,
+                'test_psm': execution_obj.test_psm,
+                'test_interface': execution_obj.test_interface,
+                'test_inter_type': execution_obj.test_inter_type,
+                'test_class': execution_obj.test_class,
+                'test_method': execution_obj.test_method,
+                'test_result': execution_obj.test_result,
+                'test_params': execution_obj.test_params,
+                'test_duration': execution_obj.test_duration,
+                'test_start_time': execution_obj.test_start_time,
+                'test_finish_time': execution_obj.test_finish_time,
+                'test_assert': execution_obj.test_assert,
+                'test_error_msg': execution_obj.test_error_msg,
+                'gmt_create': execution_obj.gmt_create,
+                'gmt_modify': execution_obj.gmt_modify
+            }
+        else:
+            return json.JSONEncoder.default(self, execution_obj)
+
+    # 重写encode方法
+    def encode(self, execution_obj):
+        """
+        把【Object】转成【Dict字典】再转成【String】
+        :param execution_obj:
+        :return:
+        """
+        if isinstance(execution_obj, CaseRecordModel):
+            return str(ExecutionRecordEncoder.default(execution_obj))
+        else:
+            return json.JSONEncoder.encode(self, execution_obj)
+
+
+# 重写JSONDecoder的decode方法，dict转换成object
+class ExecutionRecordDecoder(json.JSONDecoder):
+
+    def decode(self, dict_str):
+        """
+        把【字符串】转成【字典】再转成【Object】
+        :param dict_str: 字典的字符串
+        :return:
+        """
+        dict_val = super().decode(dict_str)  # 先把str转dict
+        # 下面是dict转object
+        ExecutionRecordDecoder.dict_to_obj(dict_val)
+
+    @staticmethod
+    def dict_to_obj(dict_val):
+        """
+        把【字典Dict】直接转成对应的【Object】
+        :param dict_val:
+        :return:
+        """
+        execution_record_model = ExecutionRecordModel()
+        if 'uid' in dict_val.keys():
+            execution_record_model.uid = dict_val['uid']
+        else:
+            execution_record_model.uid = 0
+        execution_record_model.test_unique_tag = dict_val['test_unique_tag']
+        execution_record_model.test_project_name = dict_val['test_project_name']
+        execution_record_model.test_psm = dict_val['test_psm']
+        execution_record_model.test_interface = dict_val['test_interface']
+        execution_record_model.test_inter_type = dict_val['test_inter_type']
+        execution_record_model.test_class = dict_val['test_class']
+        execution_record_model.test_method = dict_val['test_method']
+        execution_record_model.test_result = dict_val['test_result']
+        execution_record_model.test_params = dict_val['test_params']
+        execution_record_model.test_duration = dict_val['test_duration']
+        execution_record_model.test_start_time = dict_val['test_start_time']
+        execution_record_model.test_finish_time = dict_val['test_finish_time']
+        execution_record_model.test_assert = dict_val['test_assert']
+        execution_record_model.test_error_msg = dict_val['test_error_msg']
+        return execution_record_model
+
+
+#################################################################################
+###### 下方是全部接口Model：BamInterModel 和 未覆盖接口Model：NonCovInterModel ######
+
+FLAGS = re.VERBOSE | re.MULTILINE | re.DOTALL
+WHITESPACE = re.compile(r'[ \t\n\r]*', FLAGS)
+
+
+def gen_unique_key():
+    dt = datetime.datetime.now()
+    dt_str = dt.strftime('%Y%m%d%H%M%S')
+    ts = datetime.datetime.timestamp(dt)
+    ts_str = str(int(ts * 1000000))
+    unique_key = dt_str + ts_str
+    return unique_key
+
+
+class BamInterModel(AlchemyUtil.Base):
+
+    __bind_key__ = "site_reldb"  # 若不指定，则使用默认数据库。
+    __tablename__ = 'psm_inter_info'
+
+    id = Column(String(32), primary_key=True)
+    psm = Column(String(64), nullable=False)
+    endpoint_id = Column(String(64), nullable=False)
+    method = Column(String(8))
+    path = Column(String(128))
+    level = Column(Integer)
+    name = Column(String(64))
+    note = Column(String(64))
+    rpc_method = Column(String(64))
+    creator = Column(String(16))
+    updater = Column(String(32))
+    modify_time = Column(String(32))
+    create_time = Column(String(32))
+    publish_status = Column(Integer)
+    priority = Column(Integer)
+    version = Column(String(8))
+    gmt_create = Column(DateTime, default=datetime.datetime.now)
+
+    def to_json(self):
+        dict = self.__dict__
+        if "_sa_instance_state" in dict:
+            del dict["_sa_instance_state"]
+        return dict
+
+
+# 重写JSONEncoder的default方法，object转换成dict
+class BamInterEncoder(json.JSONEncoder):
+    # 重写default方法
+    def default(self, obj):
+        """
+        把【Object】转成【Dict字典】
+        :param obj:
+        :return:
+        """
+        if isinstance(obj, BamInterModel):
+            return {
+                'id': obj.id,
+                'psm': obj.psm,
+                'endpoint_id': obj.endpoint_id,
+                'method': obj.method,
+                'path': obj.path,
+                'level': obj.level,
+                'name': obj.name,
+                'note': obj.note,
+                'rpc_method': obj.rpc_method,
+                'creator': obj.creator,
+                'updater': obj.updater,
+                'create_time': obj.create_time,
+                'modify_time': obj.modify_time,
+                'publish_status': obj.publish_status,
+                'priority': obj.priority,
+                'version': obj.version,
+                'gmt_create': obj.gmt_create
+            }
+        else:
+            return json.JSONEncoder.default(self, obj)
+
+    # 重写encode方法
+    def encode(self, obj):
+        """
+        把【Object】转成【Dict字典】再转成【String】
+        :param obj:
+        :return:
+        """
+        if isinstance(obj, BamInterModel):
+            return str(self.default(obj))
+        else:
+            return json.JSONEncoder.encode(self, obj)
+
+
+# 重写JSONDecoder的decode方法，dict转换成object
+class BamInterDecoder(json.JSONDecoder):
+
+    def decode(self, dict_str, _w=WHITESPACE.match):
+        """
+        把【字符串】转成【字典】再转成【Object】
+        :param dict_str: 字典的字符串
+        :param _w:
+        :return:
+        """
+        dict_val = super().decode(dict_str)  # 先把str转dict
+        # 下面是dict转object
+        self.dict_to_obj(dict_val)
+
+    @staticmethod
+    def dict_to_obj(dict_val):
+        """
+        把【字典Dict】直接转成对应的【Object】
+        :param dict_val:
+        :return:
+        """
+        bam_inter_model = BamInterModel()
+        if 'uid' in dict_val.keys():
+            bam_inter_model.id = dict_val['id']
+        else:
+            bam_inter_model.id = gen_unique_key()
+        bam_inter_model.psm = dict_val['psm']
+        bam_inter_model.endpoint_id = dict_val['endpoint_id']
+        bam_inter_model.method = dict_val['method']
+        bam_inter_model.path = dict_val['path']
+        bam_inter_model.level = dict_val['level']
+        bam_inter_model.name = dict_val['name']
+        bam_inter_model.note = dict_val['note']
+        bam_inter_model.rpc_method = dict_val['rpc_method']
+        bam_inter_model.creator = dict_val['creator']
+        bam_inter_model.updater = dict_val['updater']
+        bam_inter_model.create_time = dict_val['create_time']
+        bam_inter_model.modify_time = dict_val['modify_time']
+        bam_inter_model.publish_status = dict_val['publish_status']
+        bam_inter_model.priority = dict_val['priority']
+        bam_inter_model.version = dict_val['version']
+        if 'gmt_create' in dict_val.keys():
+            bam_inter_model.gmt_create = dict_val['gmt_create']
+        return bam_inter_model
+
+
+class NonCovInterModel(AlchemyUtil.Base):
+
+    __bind_key__ = "site_reldb"  # 若不指定，则使用默认数据库。
+    __tablename__ = 'psm_non_cov_inter'
+
+    id = Column(String(32), primary_key=True)
+    psm = Column(String(64), nullable=False)
+    endpoint_id = Column(String(64), nullable=False)
+    method = Column(String(8))
+    path = Column(String(128))
+    name = Column(String(64))
+    note = Column(String(64))
+    rpc_method = Column(String(64))
+    version = Column(String(8))
+    gmt_create = Column(DateTime, default=datetime.datetime.now)
+
+    def to_json(self):
+        dict = self.__dict__
+        if "_sa_instance_state" in dict:
+            del dict["_sa_instance_state"]
+        return dict
+
+
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/db_util.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/db_util.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2021/12/8 3:26 下午
-# @Author  : zhengyu.0985
-# @FileName: db_util.py
-# @Software: PyCharm
-
-import pymysql
-import configparser
-import json
-import sys
-
-
-# 定义一个db链接类
-class DBConn:
-    """
-    使用cnn进行db连接
-    """
-    def __init__(self, db_key, db_conf_relative_path):
-        self.db_key = db_key
-        conf_file = open(db_conf_relative_path)
-        cf = configparser.ConfigParser()
-        cf.read_file(conf_file)
-        json_str = cf.get("mysql", db_key)
-        print(json_str)
-        dict_val = json.loads(json_str)
-        host = dict_val['db_host']
-        user = dict_val['db_user']
-        passwd = dict_val['db_passwd']
-        db = dict_val['db_db']
-        charset = dict_val['db_charset']
-        port = dict_val['db_port']
-        print("host = {0}".format(host))
-        print("user = {0}".format(user))
-        print("passwd = {0}".format(passwd))
-        print("db = {0}".format(db))
-        print("charset = {0}".format(charset))
-        print("port = {0}".format(port))
-
-        self.conn = pymysql.connect(host=host,
-                                    user=user,
-                                    passwd=passwd,
-                                    db=db,
-                                    charset=charset,
-                                    port=int(port),
-                                    )
-        print("成功连接{0}数据库。".format(self.db_key))
-
-    def query_db(self, sql_str):
-        cur = self.conn.cursor()
-        try:
-            affected_row = cur.execute(sql_str)
-            print("【{0}】SQL语句返回{1}条数据".format(sql_str, affected_row))
-            self.conn.commit()
-            return cur.fetchall()
-        except Exception as e:
-            print(e.with_traceback(sys.exc_info()[2]))
-        finally:
-            cur.close()
-
-    def update_db(self, sql_str):
-        cur = self.conn.cursor()
-        try:
-            affected_row = cur.execute(sql_str)
-            self.conn.commit()
-            print("【{0}】SQL语句共影响{1}条数据".format(sql_str, affected_row))
-            return affected_row
-        except Exception as e:
-            print(e.with_traceback(sys.exc_info()[2]))
-        finally:
-            cur.close()
-
-    def close_db(self):
-        self.conn.close()
-        print("与{0}的数据库连接已关闭。".format(self.db_key))
-
-
-if __name__ == "__main__":
-    # 建立连接
-    conn = DBConn("DB_BOE_Site_Reldb", "../../conf/db.conf")
-    # 执行SELECT
-    tuple_result = conn.query_db("select * from union_media where id in (45535, 45532, 45507, 259);")
-    print(tuple_result)
-    for row_result in tuple_result:
-        print("当前行元祖为：", row_result)
-        print("当前行共{0}个字段".format(len(row_result)))
-        print("当前行第一个字段值=", row_result[0])
-    # 执行UPDATE
-    affected_row_num = conn.update_db("update union_media_function_rel set function_id = 35 where id = '111287';")
-    print("更新了{0}行。".format(affected_row_num))
-    # 关闭连接
-    conn.close_db()
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2021/12/8 3:26 下午
+# @Author  : zhengyu.0985
+# @FileName: db_util.py
+# @Software: PyCharm
+
+import pymysql
+import configparser
+import json
+import sys
+
+
+# 定义一个db链接类
+class DBConn:
+    """
+    使用cnn进行db连接
+    """
+    def __init__(self, db_key, db_conf_relative_path):
+        self.db_key = db_key
+        conf_file = open(db_conf_relative_path)
+        cf = configparser.ConfigParser()
+        cf.read_file(conf_file)
+        json_str = cf.get("mysql", db_key)
+        print(json_str)
+        dict_val = json.loads(json_str)
+        host = dict_val['db_host']
+        user = dict_val['db_user']
+        passwd = dict_val['db_passwd']
+        db = dict_val['db_db']
+        charset = dict_val['db_charset']
+        port = dict_val['db_port']
+        print("host = {0}".format(host))
+        print("user = {0}".format(user))
+        print("passwd = {0}".format(passwd))
+        print("db = {0}".format(db))
+        print("charset = {0}".format(charset))
+        print("port = {0}".format(port))
+
+        self.conn = pymysql.connect(host=host,
+                                    user=user,
+                                    passwd=passwd,
+                                    db=db,
+                                    charset=charset,
+                                    port=int(port),
+                                    )
+        print("成功连接{0}数据库。".format(self.db_key))
+
+    def query_db(self, sql_str):
+        cur = self.conn.cursor()
+        try:
+            affected_row = cur.execute(sql_str)
+            print("【{0}】SQL语句返回{1}条数据".format(sql_str, affected_row))
+            self.conn.commit()
+            return cur.fetchall()
+        except Exception as e:
+            print(e.with_traceback(sys.exc_info()[2]))
+        finally:
+            cur.close()
+
+    def update_db(self, sql_str):
+        cur = self.conn.cursor()
+        try:
+            affected_row = cur.execute(sql_str)
+            self.conn.commit()
+            print("【{0}】SQL语句共影响{1}条数据".format(sql_str, affected_row))
+            return affected_row
+        except Exception as e:
+            print(e.with_traceback(sys.exc_info()[2]))
+        finally:
+            cur.close()
+
+    def close_db(self):
+        self.conn.close()
+        print("与{0}的数据库连接已关闭。".format(self.db_key))
+
+
+if __name__ == "__main__":
+    # 建立连接
+    conn = DBConn("DB_BOE_Site_Reldb", "../../conf/db.conf")
+    # 执行SELECT
+    tuple_result = conn.query_db("select * from union_media where id in (45535, 45532, 45507, 259);")
+    print(tuple_result)
+    for row_result in tuple_result:
+        print("当前行元祖为：", row_result)
+        print("当前行共{0}个字段".format(len(row_result)))
+        print("当前行第一个字段值=", row_result[0])
+    # 执行UPDATE
+    affected_row_num = conn.update_db("update union_media_function_rel set function_id = 35 where id = '111287';")
+    print("更新了{0}行。".format(affected_row_num))
+    # 关闭连接
+    conn.close_db()
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/db/sqlalchemy_util.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/db/sqlalchemy_util.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2021/12/8 3:26 下午
-# @Author  : zhengyu.0985
-# @FileName: sqlalchemy_util.py
-# @Software: PyCharm
-
-import configparser
-import json
-from sqlalchemy import create_engine
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import sessionmaker
-import logging
-import traceback
-import datetime
-
-logging.basicConfig(level=logging.DEBUG,
-                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
-logger = logging.getLogger('com.zijie.db.sqlalchemy_util')
-
-
-class AlchemyUtil(object):
-
-    # 基类
-    Base = declarative_base()
-
-    @classmethod
-    def get_db_param_dict(cls, db_key, db_conf_relative_path):
-        conf_file = open(db_conf_relative_path)
-        cf = configparser.ConfigParser()
-        cf.read_file(conf_file)
-        json_str = cf.get("mysql", db_key)
-        dict_val = json.loads(json_str)
-        logger.info("%s = %s" % (db_key, dict_val))
-        return dict_val
-
-    @classmethod
-    def init_engine(cls, db_param_dict):
-        """
-        根据数据库连接串创建MySQL数据库的engine。
-        :param db_param_dict: 数据连接串的各项参数的字典。
-        :return: MySQL数据库的engine。
-        """
-        host = db_param_dict['db_host']
-        user = db_param_dict['db_user']
-        passwd = db_param_dict['db_passwd']
-        db = db_param_dict['db_db']
-        charset = db_param_dict['db_charset']
-        port = db_param_dict['db_port']
-        logger.info("host = {0}".format(host))
-        logger.info("user = {0}".format(user))
-        logger.info("passwd = {0}".format(passwd))
-        logger.info("db = {0}".format(db))
-        logger.info("charset = {0}".format(charset))
-        logger.info("port = {0}".format(port))
-        mysql_engine = create_engine(
-            "mysql+pymysql://"+ user +":"+ passwd +"@"+ host +":" + port +"/"+ db +"?charset="+charset,
-            max_overflow=0,  # 超过连接池大小外最多创建的连接
-            pool_size=5,  # 连接池大小
-            pool_timeout=30,  # 池中没有线程最多等待的时间，否则报错
-            pool_recycle=-1  # 多久之后对线程池中的线程进行一次连接的回收（重置）
-        )
-        logger.info("[%s] engine has been created successfully." % mysql_engine.name)
-        return mysql_engine
-
-    @classmethod
-    def init_db(cls, mysql_engine):
-        """
-        根据类创建数据库表
-        :return:
-        """
-        AlchemyUtil.Base.metadata.create_all(mysql_engine)
-
-    @classmethod
-    def drop_db(cls, mysql_engine):
-        """
-        根据类删除数据库表
-        :return:
-        """
-        AlchemyUtil.Base.metadata.drop_all(mysql_engine)
-
-    @classmethod
-    def init_db_by_flask(cls, db, bind_key=None):
-        if bind_key is None:
-            db.create_all()
-        else:
-            # 下面这句不能初始化Flask中的SQLAlchemy Table，因为里面是调用 create_all() of MetaData in sqlalchemy.sql.schema。
-            # AlchemyUtil.init_db(db.get_engine(bind="site_reldb"))
-            db.create_all(bind=bind_key)  # 这个是create_all() of SQLAlchemy in flask_sqlalchemy
-
-    @classmethod
-    def get_session(cls, mysql_engine):
-        db_session = sessionmaker(bind=mysql_engine)  # Session是<class 'sqlalchemy.orm.session.sessionmaker'>
-        return db_session()
-
-    @classmethod
-    def insert_list_with_flush_only(cls, session, obj_list):
-        try:
-            for obj in obj_list:
-                session.add(obj)
-                session.flush()
-            logger.info("【Success】一共插入 %d 条记录 by [insert_list_with_flush_only] method." % len(obj_list))
-        finally:
-            logger.info("[insert_list_with_flush_only] method has done, but has not been committed yet.")
-
-    @classmethod
-    def insert_obj_with_commit(cls, session, obj):
-        try:
-            session.add(obj)
-            session.commit()
-            logger.info("【Success】插入一条记录：%s" % obj.__dict__)
-        finally:
-            session.close()
-            logger.info("[insert_obj_with_commit] method has done and session has been closed.")
-
-    @classmethod
-    def insert_obj_without_commit(cls, session, obj):
-        try:
-            session.add(obj)
-            session.flush()
-            logger.info("【Success】插入一条记录：%s" % obj.__dict__)
-        finally:
-            logger.info("[insert_obj_without_commit] method has done but not committed yet.")
-
-    @classmethod
-    def do_commit_only(cls, session):
-        try:
-            session.commit()
-            logger.info("session has been committed.")
-        finally:
-            session.close()
-            logger.info("do_commit_only method has done and session has been closed.")
-
-    @classmethod
-    def query_first(cls, session, clazz, criteria_set=None):
-        try:
-            if criteria_set is None or len(criteria_set) == 0:
-                sql = session.query(clazz)
-                logger.info("执行全量查询SQL = %s" % sql)
-            else:
-                sql = session.query(clazz).filter(*criteria_set)
-                logger.info("执行条件查询SQL = %s" % sql)
-            record = sql.one_or_none()  # 真正执行该查询。
-            return record
-        finally:
-            session.close()
-            logger.info("[query_first] method has done and session has been closed.")
-
-    @classmethod
-    def query_obj_list(cls, session, clazz, criteria_set=None):
-        try:
-            if criteria_set is None or len(criteria_set) == 0:
-                sql = session.query(clazz)
-                logger.info("执行全量查询SQL = %s" % sql)
-            else:
-                sql = session.query(clazz).filter(*criteria_set)
-                logger.info("执行条件查询SQL = %s" % sql)
-            record_list = sql.all()  # 真正执行该查询。
-            logger.info("查询获取到 %d 条记录。" % len(record_list))
-            return record_list
-        finally:
-            session.close()
-            logger.info("[query_obj_list] method has done and session has been closed.")
-
-    @classmethod
-    def query_field_list(cls, session, entities, criteria_set=None):
-        try:
-            if criteria_set is None or len(criteria_set) == 0:
-                sql = session.query(*entities)
-                logger.info("执行全量查询SQL = %s" % sql)
-            else:
-                sql = session.query(*entities).filter(*criteria_set)
-                logger.info("执行条件查询SQL = %s" % sql)
-            fields_record_list = sql.all()  # 真正执行该查询。
-            logger.info("查询获取到 %d 条记录。" % len(fields_record_list))
-            return fields_record_list
-        finally:
-            session.close()
-            logger.info("[query_field_list] method has done and seesion has been closed.")
-
-    @classmethod
-    def query_field_list_with_distinct(cls, session, entities, criteria_set=None, distinct_columns=None):
-        try:
-            if criteria_set is None or len(criteria_set) == 0:
-                if distinct_columns is None or len(distinct_columns) == 0:
-                    sql = session.query(*entities)
-                else:
-                    sql = session.query(*entities).distinct(*distinct_columns)
-                logger.info("执行全量查询SQL = %s" % sql)
-            else:
-                if distinct_columns is None or len(distinct_columns) == 0:
-                    sql = session.query(*entities).filter(*criteria_set)
-                else:
-                    sql = session.query(*entities).filter(*criteria_set).distinct(*distinct_columns)
-                logger.info("执行条件查询SQL = %s" % sql)
-            fields_record_list = sql.all()  # 真正执行该查询。
-            logger.info("查询获取到 %d 条记录。" % len(fields_record_list))
-            return fields_record_list
-        finally:
-            session.close()
-            logger.info("[query_field_list_with_distinct] method has done and seesion has been closed.")
-
-    @classmethod
-    def update_for_criteria_with_commit(cls, session, clazz, criteria_set=None, update_dict={}):
-        """
-        :param session: db_session
-        :param clazz: db_model_name
-        :param criteria_set: query's criteria
-        :param update_dict: update's field-value pairs
-        :return: row count of updated records
-        """
-        if len(update_dict) > 0:
-            try:
-                if criteria_set is None or len(criteria_set) == 0:
-                    sql = session.query(clazz)
-                    logger.info("执行全量查询SQL = %s" % sql)
-                else:
-                    sql = session.query(clazz).filter(*criteria_set)
-                    logger.info("执行条件查询SQL = %s" % sql)
-                affected_row = sql.update(update_dict)  # 真正执行更新，返回更新的记录条数。
-                session.commit()
-                logger.info("【Success】一共更新 %d 行记录。" % affected_row)
-                return affected_row
-            except:
-                session.rollback()
-                logger.warning("出现异常")
-                logger.error(traceback.format_exc())
-            finally:
-                session.close()
-        else:
-            logger.warning("依据update_dict参数，传入的需要更新的字段个数为零，无法更新。")
-
-    @classmethod
-    def delete_for_criteria_commit(cls, session, clazz, criteria_set=None):
-        """
-        :param session: db_session
-        :param clazz: db_model_name
-        :param criteria_set: query's criteria
-        :return: row count of deleted records
-        """
-        try:
-            if criteria_set is None or len(criteria_set) == 0:
-                logger.info("criteria_set 为空，不可删除全部记录，有风险。")
-                return 0
-            else:
-                sql = session.query(clazz).filter(*criteria_set)
-                logger.info("执行条件查询SQL = %s" % sql)
-                affected_row = sql.delete()  # 真正执行删除，返回删除的记录条数。
-                session.commit()
-                logger.info("【Success】一共删除 %d 行记录，依据条件：%s" % (affected_row, *criteria_set))
-                return affected_row
-        except:
-            session.rollback()
-            logger.warning("出现异常")
-            logger.error(traceback.format_exc())
-        finally:
-            session.close()
-
-    @classmethod
-    def gen_unique_key(cls):
-        dt = datetime.datetime.now()
-        dt_str = dt.strftime('%Y%m%d%H%M%S')
-        ts = datetime.datetime.timestamp(dt)
-        ts_str = str(int(ts * 1000000))
-        unique_key = dt_str + ts_str
-        return unique_key
-
-
-if __name__ == "__main__":
-    dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", "../../conf/db.conf")
-    engine = AlchemyUtil.init_engine(dict_val)
-    AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
-    site_rel_db_session = AlchemyUtil.get_session(engine)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2021/12/8 3:26 下午
+# @Author  : zhengyu.0985
+# @FileName: sqlalchemy_util.py
+# @Software: PyCharm
+
+import configparser
+import json
+from sqlalchemy import create_engine
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import sessionmaker
+import logging
+import traceback
+import datetime
+
+logging.basicConfig(level=logging.DEBUG,
+                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
+logger = logging.getLogger('com.zijie.db.sqlalchemy_util')
+
+
+class AlchemyUtil(object):
+
+    # 基类
+    Base = declarative_base()
+
+    @classmethod
+    def get_db_param_dict(cls, db_key, db_conf_relative_path):
+        conf_file = open(db_conf_relative_path)
+        cf = configparser.ConfigParser()
+        cf.read_file(conf_file)
+        json_str = cf.get("mysql", db_key)
+        dict_val = json.loads(json_str)
+        logger.info("%s = %s" % (db_key, dict_val))
+        return dict_val
+
+    @classmethod
+    def init_engine(cls, db_param_dict):
+        """
+        根据数据库连接串创建MySQL数据库的engine。
+        :param db_param_dict: 数据连接串的各项参数的字典。
+        :return: MySQL数据库的engine。
+        """
+        host = db_param_dict['db_host']
+        user = db_param_dict['db_user']
+        passwd = db_param_dict['db_passwd']
+        db = db_param_dict['db_db']
+        charset = db_param_dict['db_charset']
+        port = db_param_dict['db_port']
+        logger.info("host = {0}".format(host))
+        logger.info("user = {0}".format(user))
+        logger.info("passwd = {0}".format(passwd))
+        logger.info("db = {0}".format(db))
+        logger.info("charset = {0}".format(charset))
+        logger.info("port = {0}".format(port))
+        mysql_engine = create_engine(
+            "mysql+pymysql://"+ user +":"+ passwd +"@"+ host +":" + port +"/"+ db +"?charset="+charset,
+            max_overflow=0,  # 超过连接池大小外最多创建的连接
+            pool_size=5,  # 连接池大小
+            pool_timeout=30,  # 池中没有线程最多等待的时间，否则报错
+            pool_recycle=-1  # 多久之后对线程池中的线程进行一次连接的回收（重置）
+        )
+        logger.info("[%s] engine has been created successfully." % mysql_engine.name)
+        return mysql_engine
+
+    @classmethod
+    def init_db(cls, mysql_engine):
+        """
+        根据类创建数据库表
+        :return:
+        """
+        AlchemyUtil.Base.metadata.create_all(mysql_engine)
+
+    @classmethod
+    def drop_db(cls, mysql_engine):
+        """
+        根据类删除数据库表
+        :return:
+        """
+        AlchemyUtil.Base.metadata.drop_all(mysql_engine)
+
+    @classmethod
+    def init_db_by_flask(cls, db, bind_key=None):
+        if bind_key is None:
+            db.create_all()
+        else:
+            # 下面这句不能初始化Flask中的SQLAlchemy Table，因为里面是调用 create_all() of MetaData in sqlalchemy.sql.schema。
+            # AlchemyUtil.init_db(db.get_engine(bind="site_reldb"))
+            db.create_all(bind=bind_key)  # 这个是create_all() of SQLAlchemy in flask_sqlalchemy
+
+    @classmethod
+    def get_session(cls, mysql_engine):
+        db_session = sessionmaker(bind=mysql_engine)  # Session是<class 'sqlalchemy.orm.session.sessionmaker'>
+        return db_session()
+
+    @classmethod
+    def insert_list_with_flush_only(cls, session, obj_list):
+        try:
+            for obj in obj_list:
+                session.add(obj)
+                session.flush()
+            logger.info("【Success】一共插入 %d 条记录 by [insert_list_with_flush_only] method." % len(obj_list))
+        finally:
+            logger.info("[insert_list_with_flush_only] method has done, but has not been committed yet.")
+
+    @classmethod
+    def insert_obj_with_commit(cls, session, obj):
+        try:
+            session.add(obj)
+            session.commit()
+            logger.info("【Success】插入一条记录：%s" % obj.__dict__)
+        finally:
+            session.close()
+            logger.info("[insert_obj_with_commit] method has done and session has been closed.")
+
+    @classmethod
+    def insert_obj_without_commit(cls, session, obj):
+        try:
+            session.add(obj)
+            session.flush()
+            logger.info("【Success】插入一条记录：%s" % obj.__dict__)
+        finally:
+            logger.info("[insert_obj_without_commit] method has done but not committed yet.")
+
+    @classmethod
+    def do_commit_only(cls, session):
+        try:
+            session.commit()
+            logger.info("session has been committed.")
+        finally:
+            session.close()
+            logger.info("do_commit_only method has done and session has been closed.")
+
+    @classmethod
+    def query_first(cls, session, clazz, criteria_set=None):
+        try:
+            if criteria_set is None or len(criteria_set) == 0:
+                sql = session.query(clazz)
+                logger.info("执行全量查询SQL = %s" % sql)
+            else:
+                sql = session.query(clazz).filter(*criteria_set)
+                logger.info("执行条件查询SQL = %s" % sql)
+            record = sql.one_or_none()  # 真正执行该查询。
+            return record
+        finally:
+            session.close()
+            logger.info("[query_first] method has done and session has been closed.")
+
+    @classmethod
+    def query_obj_list(cls, session, clazz, criteria_set=None):
+        try:
+            if criteria_set is None or len(criteria_set) == 0:
+                sql = session.query(clazz)
+                logger.info("执行全量查询SQL = %s" % sql)
+            else:
+                sql = session.query(clazz).filter(*criteria_set)
+                logger.info("执行条件查询SQL = %s" % sql)
+            record_list = sql.all()  # 真正执行该查询。
+            logger.info("查询获取到 %d 条记录。" % len(record_list))
+            return record_list
+        finally:
+            session.close()
+            logger.info("[query_obj_list] method has done and session has been closed.")
+
+    @classmethod
+    def query_field_list(cls, session, entities, criteria_set=None):
+        try:
+            if criteria_set is None or len(criteria_set) == 0:
+                sql = session.query(*entities)
+                logger.info("执行全量查询SQL = %s" % sql)
+            else:
+                sql = session.query(*entities).filter(*criteria_set)
+                logger.info("执行条件查询SQL = %s" % sql)
+            fields_record_list = sql.all()  # 真正执行该查询。
+            logger.info("查询获取到 %d 条记录。" % len(fields_record_list))
+            return fields_record_list
+        finally:
+            session.close()
+            logger.info("[query_field_list] method has done and seesion has been closed.")
+
+    @classmethod
+    def query_field_list_with_distinct(cls, session, entities, criteria_set=None, distinct_columns=None):
+        try:
+            if criteria_set is None or len(criteria_set) == 0:
+                if distinct_columns is None or len(distinct_columns) == 0:
+                    sql = session.query(*entities)
+                else:
+                    sql = session.query(*entities).distinct(*distinct_columns)
+                logger.info("执行全量查询SQL = %s" % sql)
+            else:
+                if distinct_columns is None or len(distinct_columns) == 0:
+                    sql = session.query(*entities).filter(*criteria_set)
+                else:
+                    sql = session.query(*entities).filter(*criteria_set).distinct(*distinct_columns)
+                logger.info("执行条件查询SQL = %s" % sql)
+            fields_record_list = sql.all()  # 真正执行该查询。
+            logger.info("查询获取到 %d 条记录。" % len(fields_record_list))
+            return fields_record_list
+        finally:
+            session.close()
+            logger.info("[query_field_list_with_distinct] method has done and seesion has been closed.")
+
+    @classmethod
+    def update_for_criteria_with_commit(cls, session, clazz, criteria_set=None, update_dict={}):
+        """
+        :param session: db_session
+        :param clazz: db_model_name
+        :param criteria_set: query's criteria
+        :param update_dict: update's field-value pairs
+        :return: row count of updated records
+        """
+        if len(update_dict) > 0:
+            try:
+                if criteria_set is None or len(criteria_set) == 0:
+                    sql = session.query(clazz)
+                    logger.info("执行全量查询SQL = %s" % sql)
+                else:
+                    sql = session.query(clazz).filter(*criteria_set)
+                    logger.info("执行条件查询SQL = %s" % sql)
+                affected_row = sql.update(update_dict)  # 真正执行更新，返回更新的记录条数。
+                session.commit()
+                logger.info("【Success】一共更新 %d 行记录。" % affected_row)
+                return affected_row
+            except:
+                session.rollback()
+                logger.warning("出现异常")
+                logger.error(traceback.format_exc())
+            finally:
+                session.close()
+        else:
+            logger.warning("依据update_dict参数，传入的需要更新的字段个数为零，无法更新。")
+
+    @classmethod
+    def delete_for_criteria_commit(cls, session, clazz, criteria_set=None):
+        """
+        :param session: db_session
+        :param clazz: db_model_name
+        :param criteria_set: query's criteria
+        :return: row count of deleted records
+        """
+        try:
+            if criteria_set is None or len(criteria_set) == 0:
+                logger.info("criteria_set 为空，不可删除全部记录，有风险。")
+                return 0
+            else:
+                sql = session.query(clazz).filter(*criteria_set)
+                logger.info("执行条件查询SQL = %s" % sql)
+                affected_row = sql.delete()  # 真正执行删除，返回删除的记录条数。
+                session.commit()
+                logger.info("【Success】一共删除 %d 行记录，依据条件：%s" % (affected_row, *criteria_set))
+                return affected_row
+        except:
+            session.rollback()
+            logger.warning("出现异常")
+            logger.error(traceback.format_exc())
+        finally:
+            session.close()
+
+    @classmethod
+    def gen_unique_key(cls):
+        dt = datetime.datetime.now()
+        dt_str = dt.strftime('%Y%m%d%H%M%S')
+        ts = datetime.datetime.timestamp(dt)
+        ts_str = str(int(ts * 1000000))
+        unique_key = dt_str + ts_str
+        return unique_key
+
+
+if __name__ == "__main__":
+    dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", "../../conf/db.conf")
+    engine = AlchemyUtil.init_engine(dict_val)
+    AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
+    site_rel_db_session = AlchemyUtil.get_session(engine)
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/requests/http_sender_module.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/requests/http_sender_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2021/2/8 3:26 下午
-# @Author  : zhengyu.0985
-# @FileName: http_sender_module.py
-# @Software: PyCharm
-
-import requests
-
-
-class HttpSender(object):
-    get_response = ""
-    post_response = ""
-    hostname = ""  # 公有的类属性
-    __cookies = {}  # 私有的类属性
-
-    # def __init__(self):
-    #     print("HttpSender Default Constructor has been called.")
-
-    def __init__(self, hostname, headers=None):
-        print("HttpSender Parameter Constructor has been called.")
-        self.hostname = hostname
-        self.headers = headers  # self.headers的这个headers是实例属性，可以用实例直接方法。
-        print("self.headers = {0}".format(self.headers))
-
-    def set_headers(self, headers):
-        self.headers = headers
-        print("成员方法设置请求头：self.headers = {0}".format(self.headers))
-        print("self.headers = {0}".format(self.headers))
-
-    # 类方法，用classmethod来进行修饰
-    # 注：类方法和实例方法同名，则类方法会覆盖实例方法。所以改个名字。
-    @classmethod
-    # def set_headers(cls, headers):
-    def set_cls_headers(cls, headers):
-        cls.headers = headers
-        print("类方法设置请求头：cls.headers = {0}".format(cls.headers))
-
-    def send_get_request(self, full_get_url):
-        self.get_response = requests.get(full_get_url, headers=self.headers)
-        print("响应：", self.get_response.text)
-
-    def send_get_request_by_suburi(self, sub_uri, input_params):
-        full_url = self.hostname + sub_uri
-        self.get_response = requests.get(full_url, params=input_params, headers=self.headers)
-        print("full_url = %s" % self.get_response.url)
-
-    def send_post_request(self, full_post_url, param_data=None):
-        self.post_response = requests.post(full_post_url, param_data, headers=self.headers)
-
-    def send_json_post_request(self, full_post_url, json_data=None):
-        self.post_response = requests.post(full_post_url, json=json_data, headers=self.headers)
-        print("响应={0}".format(self.post_response.text))
-
-    # 静态方法
-    @staticmethod
-    def send_json_post_request_with_headers_cookies(self, full_post_url, json_data=None, header_data=None, cookie_data=None):
-        # 在静态方法中引用类属性的话，必须通过类实例对象来引用
-        # print(self.hostname)
-        self.post_response = requests.post(full_post_url, json=json_data, headers=header_data, cookies=cookie_data)
-
-    def send_json_post_request_by_suburi(self, sub_uri, json_data=None):
-        full_url = self.hostname + sub_uri
-        print("full_url={0}".format(full_url))
-        print("json_data={0}".format(json_data))
-        self.post_response = requests.post(full_url, json=json_data, headers=self.headers)
-
-# *args 和 **kwargs 都代表 1个 或 多个 参数的意思。*args 传入tuple 类型的无名参数，而 **kwargs 传入的参数是 dict 类型.
-# 可变参数 (Variable Argument) 的方法：使用*args和**kwargs语法。# 其中，*args是可变的positional arguments列表，**kwargs是可变的keyword arguments列表。
-# 并且，*args必须位于**kwargs之前，因为positional arguments必须位于keyword arguments之前。
-
-#
-# r = requests.get("http://www.baidu.com")
-# print(r.text)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2021/2/8 3:26 下午
+# @Author  : zhengyu.0985
+# @FileName: http_sender_module.py
+# @Software: PyCharm
+
+import requests
+
+
+class HttpSender(object):
+    get_response = ""
+    post_response = ""
+    hostname = ""  # 公有的类属性
+    __cookies = {}  # 私有的类属性
+
+    # def __init__(self):
+    #     print("HttpSender Default Constructor has been called.")
+
+    def __init__(self, hostname, headers=None):
+        print("HttpSender Parameter Constructor has been called.")
+        self.hostname = hostname
+        self.headers = headers  # self.headers的这个headers是实例属性，可以用实例直接方法。
+        print("self.headers = {0}".format(self.headers))
+
+    def set_headers(self, headers):
+        self.headers = headers
+        print("成员方法设置请求头：self.headers = {0}".format(self.headers))
+        print("self.headers = {0}".format(self.headers))
+
+    # 类方法，用classmethod来进行修饰
+    # 注：类方法和实例方法同名，则类方法会覆盖实例方法。所以改个名字。
+    @classmethod
+    # def set_headers(cls, headers):
+    def set_cls_headers(cls, headers):
+        cls.headers = headers
+        print("类方法设置请求头：cls.headers = {0}".format(cls.headers))
+
+    def send_get_request(self, full_get_url):
+        self.get_response = requests.get(full_get_url, headers=self.headers)
+        # print("响应：", self.get_response.text)
+
+    def send_get_request_by_suburi(self, sub_uri, input_params):
+        full_url = self.hostname + sub_uri
+        self.get_response = requests.get(full_url, params=input_params, headers=self.headers)
+        print("full_url = %s" % self.get_response.url)
+
+    def send_post_request(self, full_post_url, param_data=None):
+        self.post_response = requests.post(full_post_url, param_data, headers=self.headers)
+
+    def send_json_post_request(self, full_post_url, json_data=None):
+        self.post_response = requests.post(full_post_url, json=json_data, headers=self.headers)
+        print("响应={0}".format(self.post_response.text))
+
+    # 静态方法
+    @staticmethod
+    def send_json_post_request_with_headers_cookies(self, full_post_url, json_data=None, header_data=None, cookie_data=None):
+        # 在静态方法中引用类属性的话，必须通过类实例对象来引用
+        # print(self.hostname)
+        self.post_response = requests.post(full_post_url, json=json_data, headers=header_data, cookies=cookie_data)
+
+    def send_json_post_request_by_suburi(self, sub_uri, json_data=None):
+        full_url = self.hostname + sub_uri
+        print("full_url={0}".format(full_url))
+        print("json_data={0}".format(json_data))
+        self.post_response = requests.post(full_url, json=json_data, headers=self.headers)
+
+# *args 和 **kwargs 都代表 1个 或 多个 参数的意思。*args 传入tuple 类型的无名参数，而 **kwargs 传入的参数是 dict 类型.
+# 可变参数 (Variable Argument) 的方法：使用*args和**kwargs语法。# 其中，*args是可变的positional arguments列表，**kwargs是可变的keyword arguments列表。
+# 并且，*args必须位于**kwargs之前，因为positional arguments必须位于keyword arguments之前。
+
+#
+# r = requests.get("http://www.baidu.com")
+# print(r.text)
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/thrift_rpc_util.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2021/3/8 3:26 下午
-# @Author  : zhengyu.0985
-# @FileName: thrift_rpc_util.py
-# @Software: PyCharm
-
-import thriftpy2
-import os
-from thriftpy2.rpc import make_aio_client, make_client
-
-
-class ThriftUtil(object):
-    BASE_DIR = ""
-    THRIFT_PATH = ""
-
-    def __init__(self, thrift_file_path, module_name):
-        print("ThriftUtil Parameter Constructor has been called.")
-        self.sync_task_thrift = thriftpy2.load(thrift_file_path, module_name=module_name)
-
-    def get_sync_task_thrift(self):
-        return self.sync_task_thrift
-
-    @staticmethod
-    def make_sync_client(service, ip, port):
-        client = make_client(service, ip, port)
-        return client
-
-
-if __name__ == '__main__':
-    BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-    print(BASE_DIR)
-    THRIFT_PATH = os.path.join(BASE_DIR, "tests/thrift/files", "union_account.thrift")
-    print(THRIFT_PATH)
-    thrift_util_obj = ThriftUtil(THRIFT_PATH, "UnionAccountService_thrift")
-    sync_task_thrift = thrift_util_obj.get_sync_task_thrift()
-    sync_client = ThriftUtil.make_sync_client(sync_task_thrift.UnionAccountService, '10.225.112.217', 9685)
-    param = sync_task_thrift.QueryUserInfoRequest()
-    param.CoreUserId = 140381073185863
-    response = sync_client.QueryUserInfo(param)
-    print(response)
-
-
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2021/3/8 3:26 下午
+# @Author  : zhengyu.0985
+# @FileName: thrift_rpc_util.py
+# @Software: PyCharm
+
+import thriftpy2
+import os
+from thriftpy2.rpc import make_aio_client, make_client
+
+
+class ThriftUtil(object):
+    BASE_DIR = ""
+    THRIFT_PATH = ""
+
+    def __init__(self, thrift_file_path, module_name):
+        print("ThriftUtil Parameter Constructor has been called.")
+        self.sync_task_thrift = thriftpy2.load(thrift_file_path, module_name=module_name)
+
+    def get_sync_task_thrift(self):
+        return self.sync_task_thrift
+
+    @staticmethod
+    def make_sync_client(service, ip, port):
+        client = make_client(service, ip, port)
+        return client
+
+
+if __name__ == '__main__':
+    BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+    print(BASE_DIR)
+    THRIFT_PATH = os.path.join(BASE_DIR, "tests/thrift/files", "union_account.thrift")
+    print(THRIFT_PATH)
+    thrift_util_obj = ThriftUtil(THRIFT_PATH, "UnionAccountService_thrift")
+    sync_task_thrift = thrift_util_obj.get_sync_task_thrift()
+    sync_client = ThriftUtil.make_sync_client(sync_task_thrift.UnionAccountService, '10.225.112.217', 9685)
+    param = sync_task_thrift.QueryUserInfoRequest()
+    param.CoreUserId = 140381073185863
+    response = sync_client.QueryUserInfo(param)
+    print(response)
+
+
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/rpc_thrift/update_idl.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/rpc_thrift/update_idl.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-"""下载idl
-
-使用手册：https://bytedance.feishu.cn/docs/doccnSuhygJAzwis5ryxOWUt0le
-非中idl文件归档在group idl和cpputil/service_rpc_idl这两处
-每个库的工程结构是不一样的：
-    group idl下归档的idl以group idl的父目录作为构建根目录，引用范围涉及group idl下的所有库
-    service_rpc_idl内的idl以service_rpc_idl库作为构建根目录，一般采用相对当前idl路径引用的方式引用其他idl文件，引用文件都在service_rpc_idl库下
-"""
-import os
-import re
-import logging
-import subprocess
-
-from copy import deepcopy
-
-logger = logging.getLogger(__name__)
-
-
-class UpdateIdl(object):
-
-    def update_idl(self, idl_file_remote, idl_path_local, branch, repo, token):
-        need_update = os.getenv('NEED_UPDATE_IDL') != '0' and True or False
-        if not need_update:
-            idl_local = self.simplifyPath(idl_path_local + str.split(repo, ".")[0] + "/" + idl_file_remote)
-            return idl_local
-        idl_path = os.path.split(idl_file_remote)[0]
-        idl_sub_path = idl_path_local + str.split(repo, ".")[0] + "/" + idl_path
-        logger.debug("idl_sub_path: %s", idl_sub_path)
-        if not os.path.exists(idl_sub_path):
-            os.makedirs(idl_sub_path)
-        idl_local = self.simplifyPath(idl_path_local + str.split(repo, ".")[0] + "/" + idl_file_remote)
-        logger.debug("idl_local: %s", idl_local)
-        idl_file_remote = self.simplifyPath(idl_file_remote)
-        logger.debug("idl_file_remote: %s", idl_file_remote)
-        self.idl_update_os(token, repo, branch, idl_file_remote, idl_local)
-        with open(idl_local, 'r') as idl_file_local:
-            for line in idl_file_local:
-                find_include = re.search("^include *", line)
-                if find_include:
-                    if (len(str.split(line, '"'))) > 1:
-                        next_idl_name = str.split(line, '"')[1]
-                        if (next_idl_name.startswith(".") == False) & ("/" in next_idl_name):
-                            repo, next_idl_file = self.idl_file_in_other_repo(next_idl_name)
-                        else:
-                            next_idl_file = idl_path + '/' + next_idl_name
-                        self.update_idl(next_idl_file.lstrip('/'), idl_path_local, branch, repo, token)
-        logger.debug("idl_file_local=%s", idl_file_local.name)
-        return idl_file_local.name
-
-    def idl_file_in_other_repo(self, idl):
-        repo_out = str.split(idl, '/', 2)[0] + '/' + str.split(idl, '/', 2)[1]
-        idl_new = str.split(idl, '/', 2)[2]
-        return repo_out, idl_new
-
-    def idl_update_os(self, token, repo, branch, idl_file_remote, idl_local):
-        logger.debug("repo=%s, branch=%s, idl_file_remote=%s, idl_local=%s", repo, branch, idl_file_remote, idl_local)
-        repo_encode = repo.replace('/', '%2F')
-        idl_file_remote_encode = idl_file_remote.replace('/', '%2F')
-        idl_copy = "curl --request GET --header 'PRIVATE-TOKEN: "+token+"' 'https://code.byted.org/api/v4/projects/" + repo_encode + "/repository/files/" + idl_file_remote_encode + "/raw?ref=" + branch + "' >> " + idl_local
-        logger.debug("idl_copy: %s", idl_copy)
-        if os.path.exists(idl_local):
-            os.remove(idl_local)
-        logger.debug("curl results: %s", os.popen(idl_copy).read())
-
-    def simplifyPath(self, path):
-        """
-        :type path: str
-        :rtype: str
-        """
-        logger.debug("path before simplify: %s", path)
-        path.replace('//', '/')
-        list = path.split('/')
-        res = []
-        for i in range(len(list)):
-            if list[i] == '..' and len(res) > 0:
-                res = res[:-1]
-            elif list[i] != '' and list[i] != '.' and list[i] != '..':
-                res.append(list[i])
-        simplifyPath = '/' + '/'.join(res)
-        logger.debug("path after simplify: %s", simplifyPath)
-        return simplifyPath
-
-
-def update(token, idl, branch='master', dst='.'):
-    """
-    token: self access token, used for gitlab authentication, configured on gitlab
-    idl: idl url, e.g. https://code.byted.org/idl/i18n_ad/ad_understanding/ad_understanding.thrift
-    branch: git branch
-    dst: destination directory of idl downloaded, e.g. ../tmp. directory struct unchanged, e.g. ${dst}/idl/i18n_ad/...
-    """
-    need_update = os.getenv('NEED_UPDATE_IDL') != '0' and True or False
-    if not need_update:
-        return True
-    tmp = re.search(r'\w+\.\w+\.\w+/(?P<repo>\w+/\w+)/(blob/master/|blob/{}/|)(?P<idl>.+\.thrift)'.format(branch), idl)
-    if tmp is None:
-        logger.error('{} is not valid'.format(idl))
-        return False
-    repo = tmp.group('repo')
-    idl = tmp.group('idl')
-    repo_type = get_repo_type(repo)
-    if repo_type == 'service_rpc_idl':
-        include_paths = ['cpputil/service_rpc_idl']
-    elif repo_type == 'idl/':
-        include_paths = ['']
-    else:
-        include_paths = [repo]
-    updated_files = set()
-    return download_idls(repo, idl, token, dst, branch, include_paths, updated_files)
-
-
-def get_repo_type(repo):
-    """获取git repo name
-    判断待下载idl归档的库，进而决定采用哪种方式下载
-    """
-    if 'service_rpc_idl' in repo:
-        return 'service_rpc_idl'
-    elif repo.startswith('idl/'):
-        return 'idl/'
-    return None
-
-
-def download_idls(repo, idl, token, dst='.', branch='master', include_paths=[], updated_files=set()):
-    """下载当前.thrift文件，及其引用到的其他.thrift文件"""
-    # 下载当前idl
-    dst_file = os.path.join(dst, repo, idl)
-    if dst_file in updated_files:
-        return True
-    updated_files.add(dst_file)
-    content = download_single_idl(token, repo, idl, branch)
-    if content is None:
-        logger.error('update {}/{} failed'.format(repo, idl))
-        return False
-    output(content, dst_file)
-    logger.debug('update {}/{} success'.format(repo, idl))
-    # 获取当前idl引用到的其他idl
-    idls_to_update = get_idl_to_update(content)
-    # 根据引用方式的不同，采用不同方式递归下载其他引用到的idl
-    for next_idl in idls_to_update:
-        if re.match(r'[.]{1,2}/.*', next_idl) or re.match(r'\w+\.thrift', next_idl):  # 相对当前文件
-            abs_idl = os.path.normpath(os.path.join(repo, os.path.dirname(idl), next_idl))
-            tmp = abs_idl.split('/')
-            next_repo = '/'.join(tmp[:2])
-            next_idl = '/'.join(tmp[2:])
-            if not download_idls(next_repo, next_idl, token, dst, branch, include_paths, updated_files):
-                return False
-        elif re.match(r'[\w]+/.*', next_idl):
-            cur_include_paths = deepcopy(include_paths)
-            cur_include_paths.append(os.path.join(repo, os.path.dirname(idl)))
-            for path in cur_include_paths:
-                tmp = os.path.normpath(os.path.join(path, next_idl)).split('/')
-                next_repo = '/'.join(tmp[:2])
-                next_idl = '/'.join(tmp[2:])
-                if download_idls(next_repo, next_idl, token, dst, branch, include_paths, updated_files):
-                    break
-            else:
-                return False
-        else:
-            return False
-    return True
-
-
-def download_single_idl(token, repo, idl, branch):
-    branches = ['master']
-    if branch != 'master':
-        branches.insert(0, branch)
-    for br in branches:
-        cmd = ("curl --request GET "
-               "--header 'PRIVATE-TOKEN: {token}' "
-               "'https://code.byted.org/api/v4/projects/{repo}/repository/files/{idl}/raw?"
-               "ref={branch}'").format(
-            token=token,
-            repo=repo.replace('/', '%2F'),
-            idl=idl.replace('/', '%2F'),
-            branch=br
-        )
-        content = shell_command(cmd)
-        if content is None or re.search(r'"404.*Not Found"', content):
-            logger.warning('download {}/{} on branch {} failed:{}'.format(repo, idl, branch, content))
-            continue
-        return content
-    return None
-
-
-def shell_command(cmd):
-    res = subprocess.run(cmd, shell=True, capture_output=True)
-    if res.returncode != 0:
-        logger.error('"{}" exec failed'.format(cmd))
-        logger.error('reason: {}'.format(res.stderr.decode()))
-        return None
-    return res.stdout.decode()
-
-
-def get_idl_to_update(content):
-    """获取当前文件引用到的.thrift文件"""
-    res = []
-    for o in re.finditer(r'^\s*include\s+[\'"](?P<file>.*)[\'"]', content, flags=re.MULTILINE):
-        path = o.group('file')
-        res.append(path)
-    return res
-
-
-def output(content, dst_file):
-    # todo: 文件锁
-    d = os.path.dirname(dst_file)
-    os.makedirs(d, exist_ok=True)
-    if os.path.exists(dst_file):
-        with open(dst_file) as fd:
-            tmp = fd.read()
-        if content == tmp:
-            return True
-        else:
-            os.remove(dst_file)
-    with open(dst_file, mode='w') as fd:
-        fd.write(content)
-    return True
-
-
-def get_psm_idls(idl_remote, git_token):
-    """
-    使用文档: https://bytedance.feishu.cn/docs/doccnSuhygJAzwis5ryxOWUt0le
-    """
-    psm_idl = ""
-    if idl_remote is not None:
-        logger.info(f"psm idl_remote: {idl_remote}")
-        logger.info(f"git_token: {git_token}")
-        updater = UpdateIdl()
-        psm_idl = updater.update_idl(idl_file_remote=idl_remote["idl_file"],
-                                     idl_path_local='{}'.format(
-                                         # os.path.dirname(os.path.abspath(__file__)) + '/../idls/'),  # 在导入包时该路径则在包中，而不在测试项目中。
-                                         get_idl_location()),  # 所以要使用该方法。
-                                     branch=idl_remote["branch"],
-                                     repo=idl_remote["repo"],
-                                     token=git_token)
-        logger.info("psm idl path: %s", psm_idl)
-    return psm_idl
-
-
-def get_idl_location():
-    curr_sys_path = os.getcwd()
-    index_of_com = curr_sys_path.find("com")
-    if index_of_com != -1:
-        # 下面一行是绝对路径传入获取配置文件的方法。
-        return curr_sys_path[0:index_of_com] + "com/zijie/tests/thrift/idls/"
-    else:
-        return curr_sys_path + "/com/zijie/tests/thrift/idls/"
-
-
-if __name__ == '__main__':
-    logger.debug(update(idl='https://code.byted.org/idl/i18n_ad/style/engine.thrift',
-                 branch='master',
-                 token='xxx',
-                 dst='tmp'))
-    logger.debug(update(idl='https://code.byted.org/cpputil/service_rpc_idl/blob/master/ad/lego.thrift',
-                 branch='master',
-                 token='xxx',
-                 dst='tmp'))
-    logger.debug(update(idl='https://code.byted.org/cpputil/service_rpc_idl/blob/master/ad/tetris/instant_page_interface_i18n.thrift',
-                 branch='master',
-                 token='xxx',
-                 dst='tmp'))
+"""下载idl
+
+使用手册：https://bytedance.feishu.cn/docs/doccnSuhygJAzwis5ryxOWUt0le
+非中idl文件归档在group idl和cpputil/service_rpc_idl这两处
+每个库的工程结构是不一样的：
+    group idl下归档的idl以group idl的父目录作为构建根目录，引用范围涉及group idl下的所有库
+    service_rpc_idl内的idl以service_rpc_idl库作为构建根目录，一般采用相对当前idl路径引用的方式引用其他idl文件，引用文件都在service_rpc_idl库下
+"""
+import os
+import re
+import logging
+import subprocess
+
+from copy import deepcopy
+
+logger = logging.getLogger(__name__)
+
+
+class UpdateIdl(object):
+
+    def update_idl(self, idl_file_remote, idl_path_local, branch, repo, token):
+        need_update = os.getenv('NEED_UPDATE_IDL') != '0' and True or False
+        if not need_update:
+            idl_local = self.simplifyPath(idl_path_local + str.split(repo, ".")[0] + "/" + idl_file_remote)
+            return idl_local
+        idl_path = os.path.split(idl_file_remote)[0]
+        idl_sub_path = idl_path_local + str.split(repo, ".")[0] + "/" + idl_path
+        logger.debug("idl_sub_path: %s", idl_sub_path)
+        if not os.path.exists(idl_sub_path):
+            os.makedirs(idl_sub_path)
+        idl_local = self.simplifyPath(idl_path_local + str.split(repo, ".")[0] + "/" + idl_file_remote)
+        logger.debug("idl_local: %s", idl_local)
+        idl_file_remote = self.simplifyPath(idl_file_remote)
+        logger.debug("idl_file_remote: %s", idl_file_remote)
+        self.idl_update_os(token, repo, branch, idl_file_remote, idl_local)
+        with open(idl_local, 'r') as idl_file_local:
+            for line in idl_file_local:
+                find_include = re.search("^include *", line)
+                if find_include:
+                    if (len(str.split(line, '"'))) > 1:
+                        next_idl_name = str.split(line, '"')[1]
+                        if (next_idl_name.startswith(".") == False) & ("/" in next_idl_name):
+                            repo, next_idl_file = self.idl_file_in_other_repo(next_idl_name)
+                        else:
+                            next_idl_file = idl_path + '/' + next_idl_name
+                        self.update_idl(next_idl_file.lstrip('/'), idl_path_local, branch, repo, token)
+        logger.debug("idl_file_local=%s", idl_file_local.name)
+        return idl_file_local.name
+
+    def idl_file_in_other_repo(self, idl):
+        repo_out = str.split(idl, '/', 2)[0] + '/' + str.split(idl, '/', 2)[1]
+        idl_new = str.split(idl, '/', 2)[2]
+        return repo_out, idl_new
+
+    def idl_update_os(self, token, repo, branch, idl_file_remote, idl_local):
+        logger.debug("repo=%s, branch=%s, idl_file_remote=%s, idl_local=%s", repo, branch, idl_file_remote, idl_local)
+        repo_encode = repo.replace('/', '%2F')
+        idl_file_remote_encode = idl_file_remote.replace('/', '%2F')
+        idl_copy = "curl --request GET --header 'PRIVATE-TOKEN: "+token+"' 'https://code.byted.org/api/v4/projects/" + repo_encode + "/repository/files/" + idl_file_remote_encode + "/raw?ref=" + branch + "' >> " + idl_local
+        logger.debug("idl_copy: %s", idl_copy)
+        if os.path.exists(idl_local):
+            os.remove(idl_local)
+        logger.debug("curl results: %s", os.popen(idl_copy).read())
+
+    def simplifyPath(self, path):
+        """
+        :type path: str
+        :rtype: str
+        """
+        logger.debug("path before simplify: %s", path)
+        path.replace('//', '/')
+        list = path.split('/')
+        res = []
+        for i in range(len(list)):
+            if list[i] == '..' and len(res) > 0:
+                res = res[:-1]
+            elif list[i] != '' and list[i] != '.' and list[i] != '..':
+                res.append(list[i])
+        simplifyPath = '/' + '/'.join(res)
+        logger.debug("path after simplify: %s", simplifyPath)
+        return simplifyPath
+
+
+def update(token, idl, branch='master', dst='.'):
+    """
+    token: self access token, used for gitlab authentication, configured on gitlab
+    idl: idl url, e.g. https://code.byted.org/idl/i18n_ad/ad_understanding/ad_understanding.thrift
+    branch: git branch
+    dst: destination directory of idl downloaded, e.g. ../tmp. directory struct unchanged, e.g. ${dst}/idl/i18n_ad/...
+    """
+    need_update = os.getenv('NEED_UPDATE_IDL') != '0' and True or False
+    if not need_update:
+        return True
+    tmp = re.search(r'\w+\.\w+\.\w+/(?P<repo>\w+/\w+)/(blob/master/|blob/{}/|)(?P<idl>.+\.thrift)'.format(branch), idl)
+    if tmp is None:
+        logger.error('{} is not valid'.format(idl))
+        return False
+    repo = tmp.group('repo')
+    idl = tmp.group('idl')
+    repo_type = get_repo_type(repo)
+    if repo_type == 'service_rpc_idl':
+        include_paths = ['cpputil/service_rpc_idl']
+    elif repo_type == 'idl/':
+        include_paths = ['']
+    else:
+        include_paths = [repo]
+    updated_files = set()
+    return download_idls(repo, idl, token, dst, branch, include_paths, updated_files)
+
+
+def get_repo_type(repo):
+    """获取git repo name
+    判断待下载idl归档的库，进而决定采用哪种方式下载
+    """
+    if 'service_rpc_idl' in repo:
+        return 'service_rpc_idl'
+    elif repo.startswith('idl/'):
+        return 'idl/'
+    return None
+
+
+def download_idls(repo, idl, token, dst='.', branch='master', include_paths=[], updated_files=set()):
+    """下载当前.thrift文件，及其引用到的其他.thrift文件"""
+    # 下载当前idl
+    dst_file = os.path.join(dst, repo, idl)
+    if dst_file in updated_files:
+        return True
+    updated_files.add(dst_file)
+    content = download_single_idl(token, repo, idl, branch)
+    if content is None:
+        logger.error('update {}/{} failed'.format(repo, idl))
+        return False
+    output(content, dst_file)
+    logger.debug('update {}/{} success'.format(repo, idl))
+    # 获取当前idl引用到的其他idl
+    idls_to_update = get_idl_to_update(content)
+    # 根据引用方式的不同，采用不同方式递归下载其他引用到的idl
+    for next_idl in idls_to_update:
+        if re.match(r'[.]{1,2}/.*', next_idl) or re.match(r'\w+\.thrift', next_idl):  # 相对当前文件
+            abs_idl = os.path.normpath(os.path.join(repo, os.path.dirname(idl), next_idl))
+            tmp = abs_idl.split('/')
+            next_repo = '/'.join(tmp[:2])
+            next_idl = '/'.join(tmp[2:])
+            if not download_idls(next_repo, next_idl, token, dst, branch, include_paths, updated_files):
+                return False
+        elif re.match(r'[\w]+/.*', next_idl):
+            cur_include_paths = deepcopy(include_paths)
+            cur_include_paths.append(os.path.join(repo, os.path.dirname(idl)))
+            for path in cur_include_paths:
+                tmp = os.path.normpath(os.path.join(path, next_idl)).split('/')
+                next_repo = '/'.join(tmp[:2])
+                next_idl = '/'.join(tmp[2:])
+                if download_idls(next_repo, next_idl, token, dst, branch, include_paths, updated_files):
+                    break
+            else:
+                return False
+        else:
+            return False
+    return True
+
+
+def download_single_idl(token, repo, idl, branch):
+    branches = ['master']
+    if branch != 'master':
+        branches.insert(0, branch)
+    for br in branches:
+        cmd = ("curl --request GET "
+               "--header 'PRIVATE-TOKEN: {token}' "
+               "'https://code.byted.org/api/v4/projects/{repo}/repository/files/{idl}/raw?"
+               "ref={branch}'").format(
+            token=token,
+            repo=repo.replace('/', '%2F'),
+            idl=idl.replace('/', '%2F'),
+            branch=br
+        )
+        content = shell_command(cmd)
+        if content is None or re.search(r'"404.*Not Found"', content):
+            logger.warning('download {}/{} on branch {} failed:{}'.format(repo, idl, branch, content))
+            continue
+        return content
+    return None
+
+
+def shell_command(cmd):
+    res = subprocess.run(cmd, shell=True, capture_output=True)
+    if res.returncode != 0:
+        logger.error('"{}" exec failed'.format(cmd))
+        logger.error('reason: {}'.format(res.stderr.decode()))
+        return None
+    return res.stdout.decode()
+
+
+def get_idl_to_update(content):
+    """获取当前文件引用到的.thrift文件"""
+    res = []
+    for o in re.finditer(r'^\s*include\s+[\'"](?P<file>.*)[\'"]', content, flags=re.MULTILINE):
+        path = o.group('file')
+        res.append(path)
+    return res
+
+
+def output(content, dst_file):
+    # todo: 文件锁
+    d = os.path.dirname(dst_file)
+    os.makedirs(d, exist_ok=True)
+    if os.path.exists(dst_file):
+        with open(dst_file) as fd:
+            tmp = fd.read()
+        if content == tmp:
+            return True
+        else:
+            os.remove(dst_file)
+    with open(dst_file, mode='w') as fd:
+        fd.write(content)
+    return True
+
+
+def get_psm_idls(idl_remote, git_token):
+    """
+    使用文档: https://bytedance.feishu.cn/docs/doccnSuhygJAzwis5ryxOWUt0le
+    """
+    psm_idl = ""
+    if idl_remote is not None:
+        logger.info(f"psm idl_remote: {idl_remote}")
+        logger.info(f"git_token: {git_token}")
+        updater = UpdateIdl()
+        psm_idl = updater.update_idl(idl_file_remote=idl_remote["idl_file"],
+                                     idl_path_local='{}'.format(
+                                         # os.path.dirname(os.path.abspath(__file__)) + '/../idls/'),  # 在导入包时该路径则在包中，而不在测试项目中。
+                                         get_idl_location()),  # 所以要使用该方法。
+                                     branch=idl_remote["branch"],
+                                     repo=idl_remote["repo"],
+                                     token=git_token)
+        logger.info("psm idl path: %s", psm_idl)
+    return psm_idl
+
+
+def get_idl_location():
+    curr_sys_path = os.getcwd()
+    index_of_com = curr_sys_path.find("com")
+    if index_of_com != -1:
+        # 下面一行是绝对路径传入获取配置文件的方法。
+        return curr_sys_path[0:index_of_com] + "com/zijie/tests/thrift/idls/"
+    else:
+        return curr_sys_path + "/com/zijie/tests/thrift/idls/"
+
+
+if __name__ == '__main__':
+    logger.debug(update(idl='https://code.byted.org/idl/i18n_ad/style/engine.thrift',
+                 branch='master',
+                 token='xxx',
+                 dst='tmp'))
+    logger.debug(update(idl='https://code.byted.org/cpputil/service_rpc_idl/blob/master/ad/lego.thrift',
+                 branch='master',
+                 token='xxx',
+                 dst='tmp'))
+    logger.debug(update(idl='https://code.byted.org/cpputil/service_rpc_idl/blob/master/ad/tetris/instant_page_interface_i18n.thrift',
+                 branch='master',
+                 token='xxx',
+                 dst='tmp'))
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/autotest_generator.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/autotest_generator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2022/1/11 3:51 下午
-# @Author  : zhengyu.0985
-# @FileName: autotest_generator.py
-# @Software: PyCharm
-
-import os
-import json
-from string import Template
-import logging
-logging.basicConfig(level=logging.DEBUG,
-                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
-logger = logging.getLogger('com.zijie.tests.base.autotest_generator')
-
-
-class TestGenerator(object):
-
-    @staticmethod
-    def rest_generate(rest_test_file_path='',
-                      test_class_name='TestXXX',
-                      domain_host_url='https://boe-pangle-ssr.bytedance.net',
-                      case_info_dict_list=[]):
-        """
-        :param rest_test_file_path: com.zijie.tests.rest.之后的路径到.py结束。
-        :param test_class_name: 测试类的名称，必须以Test开头，以符合PyTest规范。
-        :param domain_host_url: Restful请求的域名地址。
-        :param case_info_dict_list: 测试用例信息列表，元素要求为dict类型。
-        :return:
-        """
-
-        # 获取待生成的目标python文件
-        template_path = TestGenerator.__get_template_path("rest")
-        # py_file_path = template_path + "../../zijie/tests/rest/" + rest_test_file_path
-        py_file_path = TestGenerator._get_com_path() + "zijie/tests/rest/" + rest_test_file_path
-        py_file = open(py_file_path, 'w')
-        # 组装测试类
-        setup_file_path = template_path + "restful_setup.template"
-        setup_template_file = open(setup_file_path)
-        setup_template = Template(setup_template_file.read())
-        # setup模版替换
-        lines = [setup_template.substitute(
-            rest_test_file_path=rest_test_file_path,
-            test_class_name=test_class_name,
-            domain_host_url=domain_host_url)]
-
-        # 用例模板替换
-        lines.extend(TestGenerator._get_test_cases(case_info_dict_list))
-        # teardown模板替换
-        teardown_file_path = template_path + "restful_teardown.template"
-        teardown_template_file = open(teardown_file_path)
-        teardown_template = Template(teardown_template_file.read())
-        lines.extend(teardown_template.substitute(rest_test_file_path=rest_test_file_path))
-        # 输出至python文件并保存。
-        py_file.writelines(lines)
-        py_file.close()
-        logger.info('[Success] Generate %s. ~ ~' % py_file_path)
-
-    @staticmethod
-    def rpc_generate(thrift_test_file_path='',
-                     test_class_name='TestXXX',
-                     thrift_file_name='thrift_file_name',
-                     idl_settings=None,
-                     case_info_dict_list=[]):
-        """
-        :param thrift_test_file_path: com.zijie.tests.thrift.之后的路径到.py结束。
-        :param test_class_name: 测试类的名称，必须以Test开头，以符合PyTest规范。
-        :param thrift_file_name: thrift文件名。
-        :param idl_settings: idl自动下载的配置。
-        :param case_info_dict_list: 测试用例信息列表，元素要求为dict类型。
-        :return:
-        """
-
-        # 获取待生成的目标python文件
-        template_path = TestGenerator.__get_template_path("thrift")
-        py_file_path = TestGenerator._get_com_path() + "zijie/tests/thrift/" + thrift_test_file_path
-        py_file = open(py_file_path, 'w')
-        # 组装测试类
-        if idl_settings is None:
-            setup_file_path = template_path + "thrift_setup.template"
-            setup_template_file = open(setup_file_path)
-            setup_template = Template(setup_template_file.read())
-            # setup模版替换
-            lines = [setup_template.substitute(
-                thrift_test_file_path=thrift_test_file_path,
-                test_class_name=test_class_name,
-                thrift_file_name=thrift_file_name)]
-        else:
-            setup_file_path = template_path + "thrift_advanced_setup.template"
-            setup_template_file = open(setup_file_path)
-            setup_template = Template(setup_template_file.read())
-            # setup模版替换
-            lines = [setup_template.substitute(
-                thrift_test_file_path=thrift_test_file_path,
-                test_class_name=test_class_name,
-                idl_remote=idl_settings['idl_remote'],
-                git_token=idl_settings['git_token']
-            )]
-
-        # 用例模板替换
-        lines.extend(TestGenerator._get_test_cases(case_info_dict_list))
-
-        # teardown模板替换
-        teardown_file_path = template_path + "thrift_teardown.template"
-        teardown_template_file = open(teardown_file_path)
-        teardown_template = Template(teardown_template_file.read())
-        lines.extend(teardown_template.substitute(thrift_test_file_path=thrift_test_file_path))
-
-        # 输出至python文件并保存。
-        py_file.writelines(lines)
-        py_file.close()
-        logger.info('[Success] Generate %s. ~ ~' % py_file_path)
-        pass
-
-    @staticmethod
-    def _get_test_cases(case_info_dict_list):
-        lines = []
-        if len(case_info_dict_list) == 0:
-            pass
-        else:
-            for case_info_dict in case_info_dict_list:
-                lines.append(TestGenerator._get_one_case(case_info_dict))
-                lines.append("\n")
-        return lines
-
-    @staticmethod
-    def _get_one_case(curr_case_dict):
-        if type(curr_case_dict) == dict:
-            order = 1
-            test_method_name = "test_method_name"
-            inter_name = "inter_name"
-            protocol_type = "HTTP"
-            method_name = "thrift_method_name"  # for thrift api only
-            inter_path = "/suburi"
-            cookie = ""
-            http_method = ""
-            http_method_call = ""
-            param_class_name = ""  # for thrift api only
-            if "order" in curr_case_dict.keys():
-                order = curr_case_dict['order']
-            if "test_method_name" in curr_case_dict.keys():
-                test_method_name = curr_case_dict['test_method_name']
-            if "inter_name" in curr_case_dict.keys():
-                inter_name = curr_case_dict['inter_name']
-            if "protocol_type" in curr_case_dict.keys():
-                protocol_type = curr_case_dict['protocol_type']
-            if "method_name" in curr_case_dict.keys():
-                method_name = curr_case_dict['method_name']
-            if "inter_path" in curr_case_dict.keys():
-                inter_path = curr_case_dict['inter_path']
-            if "cookie" in curr_case_dict.keys():
-                cookie = curr_case_dict['cookie']
-            if "http_method" in curr_case_dict.keys():
-                http_method = curr_case_dict['http_method'].lower()
-                if http_method == "get":
-                    http_method_call = "send_get_request_by_suburi"
-                elif http_method == "post":
-                    http_method_call = "send_json_post_request_by_suburi"
-                else:
-                    http_method_call = "不支持GET或POST以外的请求"
-                    logger.info("当前用例自动生成仅支持GET和POST请求。")
-            if "param_class_name" in curr_case_dict.keys():
-                param_class_name = curr_case_dict['param_class_name']
-            # 准备组装Template
-            # 下面开始判断该用例是否是参数化的
-            if "parameters" in curr_case_dict.keys() and len(curr_case_dict['parameters']) > 0:
-                parameters = curr_case_dict['parameters']
-                if "," in parameters:
-                    param_list = parameters.split(",")
-                    values_tuples = "("
-                    for param in param_list:
-                        values_tuples = values_tuples + param.strip() + "_value0, "
-                    values_tuples = values_tuples + ")"
-                else:
-                    values_tuples = "(" + parameters.strip() + "_value0)"
-                # 真正开始组装Template
-                # 判断是HTTP接口还是THRIFT接口
-                if protocol_type.lower() == "http" or protocol_type.lower() == "rest":
-                    template_path = TestGenerator.__get_template_path("rest")
-                    parameter_case_file_path = template_path + "restful_parameter_case.template"
-                    parameter_case_template_file = open(parameter_case_file_path)
-                    template = Template(parameter_case_template_file.read())
-                    result = template.substitute(
-                        order=order,
-                        test_method_name=test_method_name,
-                        inter_name=inter_name,
-                        protocol_type=protocol_type,
-                        inter_path=inter_path,
-                        cookie=cookie,
-                        http_method=http_method,
-                        http_method_call=http_method_call,
-                        parameters=parameters,
-                        values_tuples=values_tuples
-                    )
-                elif protocol_type.lower() == "thrift" or protocol_type.lower() == "rpc":
-                    template_path = TestGenerator.__get_template_path("thrift")
-                    parameter_case_file_path = template_path + "thrift_parameter_case.template"
-                    parameter_case_template_file = open(parameter_case_file_path)
-                    template = Template(parameter_case_template_file.read())
-                    result = template.substitute(
-                        order=order,
-                        test_method_name=test_method_name,
-                        inter_name=inter_name,
-                        protocol_type=protocol_type,
-                        method_name=method_name,
-                        cookie=cookie,
-                        param_class_name=param_class_name,
-                        parameters=parameters,
-                        values_tuples=values_tuples
-                    )
-                else:
-                    result = ""
-                    logger.warning("当前仅支持接口协议为HTTP和THRIFT。")
-            else:  # 该else代表该用例是非参数化执行。
-                if protocol_type.lower() == "http" or protocol_type.lower() == "rest":
-                    template_path = TestGenerator.__get_template_path("rest")
-                    restful_case_file_path = template_path + "restful_case.template"
-                    restful_case_template_file = open(restful_case_file_path)
-                    template = Template(restful_case_template_file.read())
-                    result = template.substitute(
-                        order=order,
-                        test_method_name=test_method_name,
-                        inter_name=inter_name,
-                        protocol_type=protocol_type,
-                        inter_path=inter_path,
-                        cookie=cookie,
-                        http_method=http_method,
-                        http_method_call=http_method_call
-                    )
-                elif protocol_type.lower() == "thrift" or protocol_type.lower() == "rpc":
-                    template_path = TestGenerator.__get_template_path("thrift")
-                    thrift_case_file_path = template_path + "thrift_case.template"
-                    thrift_case_template_file = open(thrift_case_file_path)
-                    template = Template(thrift_case_template_file.read())
-                    result = template.substitute(
-                        order=order,
-                        test_method_name=test_method_name,
-                        inter_name=inter_name,
-                        protocol_type=protocol_type,
-                        method_name=method_name,
-                        cookie=cookie,
-                        param_class_name=param_class_name,
-                    )
-                else:
-                    result = ""
-                    logger.warning("当前仅支持接口协议为HTTP和THRIFT。")
-            return result
-        else:
-            logger.error('case_info_dict_list的元素不是dict类型。')
-            return ""
-
-    @staticmethod
-    def __get_template_path(rest_or_thrift):
-        return TestGenerator._get_com_path() + "templates/" + rest_or_thrift + "/"
-
-    @staticmethod
-    def _get_com_path():
-        curr_path = os.getcwd()
-        index_of_com = curr_path.find("com")
-        if index_of_com != -1:
-            # 下面一行是绝对路径传入获取配置文件的方法。
-            return curr_path[0:index_of_com] + "com/"
-        else:
-            # 下面一行的相对路径会随测试py文件位置而变化，仅在测试文件绝对路径中不包含com时，做默认三层情况使用。
-            return "../../../"
-
-    @staticmethod
-    def generate(config_file_name):
-        test_config_file_path = TestGenerator._get_com_path() + "zijie/tests/case_config/" + config_file_name
-        test_config_file = open(test_config_file_path, 'r')
-        str_val = test_config_file.read()
-        dict_array = json.loads(str_val)
-        if "rest" in config_file_name.lower() or "http" in config_file_name.lower():
-            for test_dict in dict_array:
-                # 每一个dict是一个测试文件。
-                TestGenerator.rest_generate(
-                    rest_test_file_path=test_dict['rest_test_file_path'],
-                    test_class_name=test_dict['test_class_name'],
-                    domain_host_url=test_dict['domain_host_url'],
-                    case_info_dict_list=test_dict['case_info_dict_list']
-                )
-        elif "rpc" in config_file_name.lower() or "thrift" in config_file_name.lower():
-            for test_dict in dict_array:
-                # 每一个dict是一个测试文件。
-                if 'idl_settings' in test_dict.keys() and len(test_dict['idl_settings']) > 0:
-                    TestGenerator.rpc_generate(
-                        thrift_test_file_path=test_dict['thrift_test_file_path'],
-                        test_class_name=test_dict['test_class_name'],
-                        thrift_file_name=test_dict['thrift_file_name'],
-                        idl_settings=test_dict['idl_settings'],
-                        case_info_dict_list=test_dict['case_info_dict_list']
-                    )
-                else:
-                    TestGenerator.rpc_generate(
-                        thrift_test_file_path=test_dict['thrift_test_file_path'],
-                        test_class_name=test_dict['test_class_name'],
-                        thrift_file_name=test_dict['thrift_file_name'],
-                        case_info_dict_list=test_dict['case_info_dict_list']
-                    )
-
-
-if __name__ == "__main__":
-    TestGenerator.generate("restful_case_config.json")
-    TestGenerator.generate("thrift_case_config.json")
-
-    # case_info_dict_list = [
-    #     {
-    #         "order": 1,
-    #         "test_method_name": "test_case",
-    #         "inter_name": "被测接口",
-    #         "protocol_type": "HTTP",
-    #         "inter_path": "/union_pangle",
-    #         "http_method": "GET"
-    #     },
-    #     {
-    #         "order": 2,
-    #         "test_method_name": "test_parameter_case",
-    #         "inter_name": "被测接口1",
-    #         "protocol_type": "HTTP",
-    #         "inter_path": "/union_pangle/parameter",
-    #         "http_method": "POST",
-    #         "parameters": "var, param",
-    #     },
-    # ]
-    # TestGenerator.rest_generate(
-    #     rest_test_file_path="auto_test.py",
-    #     test_class_name="TestAuto",
-    #     domain_host_url="https://boe-pangle-ssr.bytedance.net",
-    #     case_info_dict_list=case_info_dict_list
-    # )
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2022/1/11 3:51 下午
+# @Author  : zhengyu.0985
+# @FileName: autotest_generator.py
+# @Software: PyCharm
+
+import os
+import json
+from string import Template
+import logging
+logging.basicConfig(level=logging.DEBUG,
+                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
+logger = logging.getLogger('com.zijie.tests.base.autotest_generator')
+
+
+class TestGenerator(object):
+
+    @staticmethod
+    def rest_generate(rest_test_file_path='',
+                      test_class_name='TestXXX',
+                      domain_host_url='https://boe-pangle-ssr.bytedance.net',
+                      case_info_dict_list=[]):
+        """
+        :param rest_test_file_path: com.zijie.tests.rest.之后的路径到.py结束。
+        :param test_class_name: 测试类的名称，必须以Test开头，以符合PyTest规范。
+        :param domain_host_url: Restful请求的域名地址。
+        :param case_info_dict_list: 测试用例信息列表，元素要求为dict类型。
+        :return:
+        """
+
+        # 获取待生成的目标python文件
+        template_path = TestGenerator.__get_template_path("rest")
+        # py_file_path = template_path + "../../zijie/tests/rest/" + rest_test_file_path
+        py_file_path = TestGenerator._get_com_path() + "zijie/tests/rest/" + rest_test_file_path
+        py_file = open(py_file_path, 'w')
+        # 组装测试类
+        setup_file_path = template_path + "restful_setup.template"
+        setup_template_file = open(setup_file_path)
+        setup_template = Template(setup_template_file.read())
+        # setup模版替换
+        lines = [setup_template.substitute(
+            rest_test_file_path=rest_test_file_path,
+            test_class_name=test_class_name,
+            domain_host_url=domain_host_url)]
+
+        # 用例模板替换
+        lines.extend(TestGenerator._get_test_cases(case_info_dict_list))
+        # teardown模板替换
+        teardown_file_path = template_path + "restful_teardown.template"
+        teardown_template_file = open(teardown_file_path)
+        teardown_template = Template(teardown_template_file.read())
+        lines.extend(teardown_template.substitute(rest_test_file_path=rest_test_file_path))
+        # 输出至python文件并保存。
+        py_file.writelines(lines)
+        py_file.close()
+        logger.info('[Success] Generate %s. ~ ~' % py_file_path)
+
+    @staticmethod
+    def rpc_generate(thrift_test_file_path='',
+                     test_class_name='TestXXX',
+                     thrift_file_name='thrift_file_name',
+                     idl_settings=None,
+                     case_info_dict_list=[]):
+        """
+        :param thrift_test_file_path: com.zijie.tests.thrift.之后的路径到.py结束。
+        :param test_class_name: 测试类的名称，必须以Test开头，以符合PyTest规范。
+        :param thrift_file_name: thrift文件名。
+        :param idl_settings: idl自动下载的配置。
+        :param case_info_dict_list: 测试用例信息列表，元素要求为dict类型。
+        :return:
+        """
+
+        # 获取待生成的目标python文件
+        template_path = TestGenerator.__get_template_path("thrift")
+        py_file_path = TestGenerator._get_com_path() + "zijie/tests/thrift/" + thrift_test_file_path
+        py_file = open(py_file_path, 'w')
+        # 组装测试类
+        if idl_settings is None:
+            setup_file_path = template_path + "thrift_setup.template"
+            setup_template_file = open(setup_file_path)
+            setup_template = Template(setup_template_file.read())
+            # setup模版替换
+            lines = [setup_template.substitute(
+                thrift_test_file_path=thrift_test_file_path,
+                test_class_name=test_class_name,
+                thrift_file_name=thrift_file_name)]
+        else:
+            setup_file_path = template_path + "thrift_advanced_setup.template"
+            setup_template_file = open(setup_file_path)
+            setup_template = Template(setup_template_file.read())
+            # setup模版替换
+            lines = [setup_template.substitute(
+                thrift_test_file_path=thrift_test_file_path,
+                test_class_name=test_class_name,
+                idl_remote=idl_settings['idl_remote'],
+                git_token=idl_settings['git_token']
+            )]
+
+        # 用例模板替换
+        lines.extend(TestGenerator._get_test_cases(case_info_dict_list))
+
+        # teardown模板替换
+        teardown_file_path = template_path + "thrift_teardown.template"
+        teardown_template_file = open(teardown_file_path)
+        teardown_template = Template(teardown_template_file.read())
+        lines.extend(teardown_template.substitute(thrift_test_file_path=thrift_test_file_path))
+
+        # 输出至python文件并保存。
+        py_file.writelines(lines)
+        py_file.close()
+        logger.info('[Success] Generate %s. ~ ~' % py_file_path)
+        pass
+
+    @staticmethod
+    def _get_test_cases(case_info_dict_list):
+        lines = []
+        if len(case_info_dict_list) == 0:
+            pass
+        else:
+            for case_info_dict in case_info_dict_list:
+                lines.append(TestGenerator._get_one_case(case_info_dict))
+                lines.append("\n")
+        return lines
+
+    @staticmethod
+    def _get_one_case(curr_case_dict):
+        if type(curr_case_dict) == dict:
+            order = 1
+            test_method_name = "test_method_name"
+            inter_name = "inter_name"
+            protocol_type = "HTTP"
+            method_name = "thrift_method_name"  # for thrift api only
+            inter_path = "/suburi"
+            cookie = ""
+            http_method = ""
+            http_method_call = ""
+            param_class_name = ""  # for thrift api only
+            if "order" in curr_case_dict.keys():
+                order = curr_case_dict['order']
+            if "test_method_name" in curr_case_dict.keys():
+                test_method_name = curr_case_dict['test_method_name']
+            if "inter_name" in curr_case_dict.keys():
+                inter_name = curr_case_dict['inter_name']
+            if "protocol_type" in curr_case_dict.keys():
+                protocol_type = curr_case_dict['protocol_type']
+            if "method_name" in curr_case_dict.keys():
+                method_name = curr_case_dict['method_name']
+            if "inter_path" in curr_case_dict.keys():
+                inter_path = curr_case_dict['inter_path']
+            if "cookie" in curr_case_dict.keys():
+                cookie = curr_case_dict['cookie']
+            if "http_method" in curr_case_dict.keys():
+                http_method = curr_case_dict['http_method'].lower()
+                if http_method == "get":
+                    http_method_call = "send_get_request_by_suburi"
+                elif http_method == "post":
+                    http_method_call = "send_json_post_request_by_suburi"
+                else:
+                    http_method_call = "不支持GET或POST以外的请求"
+                    logger.info("当前用例自动生成仅支持GET和POST请求。")
+            if "param_class_name" in curr_case_dict.keys():
+                param_class_name = curr_case_dict['param_class_name']
+            # 准备组装Template
+            # 下面开始判断该用例是否是参数化的
+            if "parameters" in curr_case_dict.keys() and len(curr_case_dict['parameters']) > 0:
+                parameters = curr_case_dict['parameters']
+                if "," in parameters:
+                    param_list = parameters.split(",")
+                    values_tuples = "("
+                    for param in param_list:
+                        values_tuples = values_tuples + param.strip() + "_value0, "
+                    values_tuples = values_tuples + ")"
+                else:
+                    values_tuples = "(" + parameters.strip() + "_value0)"
+                # 真正开始组装Template
+                # 判断是HTTP接口还是THRIFT接口
+                if protocol_type.lower() == "http" or protocol_type.lower() == "rest":
+                    template_path = TestGenerator.__get_template_path("rest")
+                    parameter_case_file_path = template_path + "restful_parameter_case.template"
+                    parameter_case_template_file = open(parameter_case_file_path)
+                    template = Template(parameter_case_template_file.read())
+                    result = template.substitute(
+                        order=order,
+                        test_method_name=test_method_name,
+                        inter_name=inter_name,
+                        protocol_type=protocol_type,
+                        inter_path=inter_path,
+                        cookie=cookie,
+                        http_method=http_method,
+                        http_method_call=http_method_call,
+                        parameters=parameters,
+                        values_tuples=values_tuples
+                    )
+                elif protocol_type.lower() == "thrift" or protocol_type.lower() == "rpc":
+                    template_path = TestGenerator.__get_template_path("thrift")
+                    parameter_case_file_path = template_path + "thrift_parameter_case.template"
+                    parameter_case_template_file = open(parameter_case_file_path)
+                    template = Template(parameter_case_template_file.read())
+                    result = template.substitute(
+                        order=order,
+                        test_method_name=test_method_name,
+                        inter_name=inter_name,
+                        protocol_type=protocol_type,
+                        method_name=method_name,
+                        cookie=cookie,
+                        param_class_name=param_class_name,
+                        parameters=parameters,
+                        values_tuples=values_tuples
+                    )
+                else:
+                    result = ""
+                    logger.warning("当前仅支持接口协议为HTTP和THRIFT。")
+            else:  # 该else代表该用例是非参数化执行。
+                if protocol_type.lower() == "http" or protocol_type.lower() == "rest":
+                    template_path = TestGenerator.__get_template_path("rest")
+                    restful_case_file_path = template_path + "restful_case.template"
+                    restful_case_template_file = open(restful_case_file_path)
+                    template = Template(restful_case_template_file.read())
+                    result = template.substitute(
+                        order=order,
+                        test_method_name=test_method_name,
+                        inter_name=inter_name,
+                        protocol_type=protocol_type,
+                        inter_path=inter_path,
+                        cookie=cookie,
+                        http_method=http_method,
+                        http_method_call=http_method_call
+                    )
+                elif protocol_type.lower() == "thrift" or protocol_type.lower() == "rpc":
+                    template_path = TestGenerator.__get_template_path("thrift")
+                    thrift_case_file_path = template_path + "thrift_case.template"
+                    thrift_case_template_file = open(thrift_case_file_path)
+                    template = Template(thrift_case_template_file.read())
+                    result = template.substitute(
+                        order=order,
+                        test_method_name=test_method_name,
+                        inter_name=inter_name,
+                        protocol_type=protocol_type,
+                        method_name=method_name,
+                        cookie=cookie,
+                        param_class_name=param_class_name,
+                    )
+                else:
+                    result = ""
+                    logger.warning("当前仅支持接口协议为HTTP和THRIFT。")
+            return result
+        else:
+            logger.error('case_info_dict_list的元素不是dict类型。')
+            return ""
+
+    @staticmethod
+    def __get_template_path(rest_or_thrift):
+        return TestGenerator._get_com_path() + "templates/" + rest_or_thrift + "/"
+
+    @staticmethod
+    def _get_com_path():
+        curr_path = os.getcwd()
+        index_of_com = curr_path.find("com")
+        if index_of_com != -1:
+            # 下面一行是绝对路径传入获取配置文件的方法。
+            return curr_path[0:index_of_com] + "com/"
+        else:
+            # 下面一行的相对路径会随测试py文件位置而变化，仅在测试文件绝对路径中不包含com时，做默认三层情况使用。
+            return "../../../"
+
+    @staticmethod
+    def generate(config_file_name):
+        test_config_file_path = TestGenerator._get_com_path() + "zijie/tests/case_config/" + config_file_name
+        test_config_file = open(test_config_file_path, 'r')
+        str_val = test_config_file.read()
+        dict_array = json.loads(str_val)
+        if "rest" in config_file_name.lower() or "http" in config_file_name.lower():
+            for test_dict in dict_array:
+                # 每一个dict是一个测试文件。
+                TestGenerator.rest_generate(
+                    rest_test_file_path=test_dict['rest_test_file_path'],
+                    test_class_name=test_dict['test_class_name'],
+                    domain_host_url=test_dict['domain_host_url'],
+                    case_info_dict_list=test_dict['case_info_dict_list']
+                )
+        elif "rpc" in config_file_name.lower() or "thrift" in config_file_name.lower():
+            for test_dict in dict_array:
+                # 每一个dict是一个测试文件。
+                if 'idl_settings' in test_dict.keys() and len(test_dict['idl_settings']) > 0:
+                    TestGenerator.rpc_generate(
+                        thrift_test_file_path=test_dict['thrift_test_file_path'],
+                        test_class_name=test_dict['test_class_name'],
+                        thrift_file_name=test_dict['thrift_file_name'],
+                        idl_settings=test_dict['idl_settings'],
+                        case_info_dict_list=test_dict['case_info_dict_list']
+                    )
+                else:
+                    TestGenerator.rpc_generate(
+                        thrift_test_file_path=test_dict['thrift_test_file_path'],
+                        test_class_name=test_dict['test_class_name'],
+                        thrift_file_name=test_dict['thrift_file_name'],
+                        case_info_dict_list=test_dict['case_info_dict_list']
+                    )
+
+
+if __name__ == "__main__":
+    TestGenerator.generate("restful_case_config.json")
+    TestGenerator.generate("thrift_case_config.json")
+
+    # case_info_dict_list = [
+    #     {
+    #         "order": 1,
+    #         "test_method_name": "test_case",
+    #         "inter_name": "被测接口",
+    #         "protocol_type": "HTTP",
+    #         "inter_path": "/union_pangle",
+    #         "http_method": "GET"
+    #     },
+    #     {
+    #         "order": 2,
+    #         "test_method_name": "test_parameter_case",
+    #         "inter_name": "被测接口1",
+    #         "protocol_type": "HTTP",
+    #         "inter_path": "/union_pangle/parameter",
+    #         "http_method": "POST",
+    #         "parameters": "var, param",
+    #     },
+    # ]
+    # TestGenerator.rest_generate(
+    #     rest_test_file_path="auto_test.py",
+    #     test_class_name="TestAuto",
+    #     domain_host_url="https://boe-pangle-ssr.bytedance.net",
+    #     case_info_dict_list=case_info_dict_list
+    # )
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/base_compare.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_compare.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2021/12/13 2:41 下午
-# @Author  : zhengyu.0985
-# @FileName: base_compare.py
-# @Software: PyCharm
-
-from rolling_king.zijie.db.db_models import CaseRecordModel, BamInterModel, NonCovInterModel
-from rolling_king.zijie.db.sqlalchemy_util import AlchemyUtil
-from rolling_king.zijie.tests.base.base_test import BaseTest
-import logging
-import os
-
-logger = logging.getLogger("base_compare")
-
-
-class CoverDiff(object):
-
-    @staticmethod
-    def _get_db_conf_path():
-        curr_sys_path = os.getcwd()
-        logger.info(f"file_path={curr_sys_path}")
-        index_of_com = curr_sys_path.find("com")
-        if index_of_com != -1:
-            # 下面一行是绝对路径传入获取配置文件的方法。
-            conf_absolute_path = curr_sys_path[0:index_of_com] + "com/conf/"
-            db_conf_file_path = conf_absolute_path + "db.conf"
-        else:
-            # 下面一行的相对路径会随测试py文件位置而变化，仅在测试文件绝对路径中不包含com时，做默认三层情况使用。
-            db_conf_file_path = curr_sys_path + "/com/conf/db.conf"
-        return db_conf_file_path
-
-    @staticmethod
-    def get_diff_result(psm=None, test_project_name=None, protocol="BOTH"):
-        db_conf_dict = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", CoverDiff._get_db_conf_path())
-        engine = AlchemyUtil.init_engine(db_conf_dict)
-        AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
-        site_rel_db_session = AlchemyUtil.get_session(engine)
-        # 判断已测试（分子）的查询范围。
-        if psm is None and test_project_name is None:
-            project_conf_dict = BaseTest.get_project_conf_dict()
-            psm = project_conf_dict['test_psm']
-            test_project_name = project_conf_dict['test_project_name']
-            tested_criteria_set = {  # 这是<class 'set'>类型。
-                CaseRecordModel.test_psm == psm,  # 被测PSM
-                CaseRecordModel.test_project_name == test_project_name  # 测试项目名
-            }
-        elif psm is None:
-            project_conf_dict = BaseTest.get_project_conf_dict()
-            psm = project_conf_dict['test_psm']
-            tested_criteria_set = {  # 这是<class 'set'>类型。
-                CaseRecordModel.test_psm == psm,  # 被测PSM
-                CaseRecordModel.test_project_name == test_project_name  # 测试项目名
-            }
-        elif test_project_name is None:  # 只传入PSM，证明与被测项目无关，全局进行查询。
-            logger.info("test_project_name is None")
-            tested_criteria_set = {  # 这是<class 'set'>类型。
-                CaseRecordModel.test_psm == psm,  # 被测PSM
-            }
-        else:
-            tested_criteria_set = {  # 这是<class 'set'>类型。
-                CaseRecordModel.test_psm == psm,  # 被测PSM
-                CaseRecordModel.test_project_name == test_project_name  # 测试项目名
-            }
-
-        # 获取已测试列表
-        tested_list = AlchemyUtil.query_obj_list(site_rel_db_session, CaseRecordModel, tested_criteria_set)
-
-        # 下面查询总接口数（分母）
-
-        # 查询总接口的若干字段
-        collum_tuple = (BamInterModel.psm, BamInterModel.name, BamInterModel.method, BamInterModel.path,\
-                        BamInterModel.rpc_method, BamInterModel.note, BamInterModel.endpoint_id, BamInterModel.version)
-
-        # 依据想要对比的接口协议类型，进行对比。
-        if protocol == "HTTP" or protocol == "REST":
-            logger.info("仅对比HTTP接口")
-            total_criteria_set = {  # 这是<class 'set'>类型。
-                BamInterModel.psm == psm,
-                BamInterModel.path != '',
-                BamInterModel.method != ''
-            }
-            total_list = AlchemyUtil.query_field_list(site_rel_db_session, collum_tuple,
-                                                      criteria_set=total_criteria_set)
-            if len(tested_list) == 0:
-                logger.info("tested_list：为空")
-                if len(total_list) > 0:
-                    CoverDiff._delete_non_cov_records(psm, total_list)
-                    CoverDiff._insert_non_cov_to_db(psm, total_list)
-            elif len(total_list) == 0:
-                logger.info("total_list：为空")
-            else:
-                diff_tuple_list = CoverDiff._compare_http(tested_list, total_list)
-                CoverDiff._delete_non_cov_records(psm, diff_tuple_list)
-                CoverDiff._insert_non_cov_to_db(psm, diff_tuple_list)
-                return len(diff_tuple_list)
-        elif protocol == "RPC" or protocol == "THRIFT":
-            logger.info("仅对比RPC接口")
-            total_criteria_set = {  # 这是<class 'set'>类型。
-                BamInterModel.psm == psm,
-                BamInterModel.path == '',
-                BamInterModel.method == ''
-            }
-            total_list = AlchemyUtil.query_field_list(site_rel_db_session, collum_tuple,
-                                                      criteria_set=total_criteria_set)
-            if len(tested_list) == 0:
-                logger.info("tested_list：为空")
-                if len(total_list) > 0:
-                    CoverDiff._delete_non_cov_records(psm, total_list)
-                    CoverDiff._insert_non_cov_to_db(psm, total_list)
-            elif len(total_list) == 0:
-                logger.info("total_list：为空")
-            else:
-                diff_tuple_list = CoverDiff._compare_rpc(tested_list, total_list)
-                CoverDiff._delete_non_cov_records(psm, diff_tuple_list)
-                CoverDiff._insert_non_cov_to_db(psm, diff_tuple_list)
-                return len(diff_tuple_list)
-        else:
-            logger.info("HTTP and RPC 接口均对比")
-            total_criteria_set = {  # 这是<class 'set'>类型。
-                BamInterModel.psm == psm,
-            }
-            total_list = AlchemyUtil.query_field_list(site_rel_db_session, collum_tuple,
-                                                      criteria_set=total_criteria_set)
-            if len(tested_list) == 0:
-                logger.info("tested_list：为空")
-                if len(total_list) > 0:
-                    CoverDiff._delete_non_cov_records(psm, total_list)
-                    CoverDiff._insert_non_cov_to_db(psm, total_list)
-            elif len(total_list) == 0:
-                logger.info("total_list：为空")
-            else:
-                diff_tuple_list = CoverDiff._compare_both(tested_list, total_list)
-                CoverDiff._delete_non_cov_records(psm, diff_tuple_list)
-                CoverDiff._insert_non_cov_to_db(psm, diff_tuple_list)
-                return len(diff_tuple_list)
-        # 返回数量
-        return 0
-
-    @staticmethod
-    def _compare_rpc(tested_list, total_list):
-        logger.info("一共 %d 个接口。" % len(total_list))
-        for curr_test in tested_list:
-            curr_rpc_method = curr_test.__dict__['test_interface'].split(".")[1]
-            for curr_db_record in total_list:
-                if curr_rpc_method == curr_db_record[4]:
-                    logger.info("curr_db_record = %s" % curr_db_record)
-                    logger.info("[RPC] %s 已被 %s 项目的 %s 测试用例覆盖。" % (curr_rpc_method, curr_test.test_project_name, curr_test.test_method))
-                    total_list.remove(curr_db_record)
-                    break
-                else:
-                    pass
-        logger.info("未覆盖 %d 个接口" % len(total_list))
-        return total_list
-
-    @staticmethod
-    def _compare_http(tested_list, total_list):
-        logger.info("一共 %d 个接口。" % len(total_list))
-        for curr_test in tested_list:
-            curr_http_uri = curr_test.__dict__['test_interface'].split("::")[1]
-            for curr_db_record in total_list:
-                if curr_http_uri == curr_db_record[3]:
-                    logger.info("curr_db_record = %s" % curr_db_record)
-                    logger.info("[REST] %s 已被 %s 项目的 %s 测试用例覆盖。" % (curr_http_uri, curr_test.test_project_name, curr_test.test_method))
-                    total_list.remove(curr_db_record)
-                    break
-                else:
-                    pass
-        logger.info("未覆盖 %d 个接口" % len(total_list))
-        return total_list
-
-    @staticmethod
-    def _compare_both(tested_list, total_list):
-        logger.info("一共 %d 个接口。" % len(total_list))
-        for curr_test in tested_list:
-            if curr_test.test_inter_type == 'HTTP':
-                curr_http_uri = curr_test.__dict__['test_interface'].split("::")[1]
-                for curr_db_record in total_list:
-                    if curr_http_uri == curr_db_record[3]:
-                        logger.info("curr_db_record = %s" % curr_db_record)
-                        logger.info("[REST] %s 已被 %s 项目的 %s 测试用例覆盖。" % (
-                        curr_http_uri, curr_test.test_project_name, curr_test.test_method))
-                        total_list.remove(curr_db_record)
-                        break
-                    else:
-                        pass
-                # End For
-            elif curr_test.test_inter_type == 'THRIFT':
-                curr_rpc_method = curr_test.__dict__['test_interface'].split(".")[1]
-                for curr_db_record in total_list:
-                    if curr_rpc_method == curr_db_record[4]:
-                        logger.info("curr_db_record = %s" % curr_db_record)
-                        logger.info("[RPC] %s 已被 %s 项目的 %s 测试用例覆盖。" % (
-                        curr_rpc_method, curr_test.test_project_name, curr_test.test_method))
-                        total_list.remove(curr_db_record)
-                        break
-                    else:
-                        pass
-                # End For
-            else:
-                pass
-        logger.info("未覆盖 %d 个接口" % len(total_list))
-        return total_list
-
-    @staticmethod
-    def _insert_non_cov_to_db(psm, non_cov_tuple_list):
-        if non_cov_tuple_list is not None and len(non_cov_tuple_list) > 0:
-            logger.info("PSM=[%s]，需要 插入 %d 条记录。" % (psm, len(non_cov_tuple_list)))
-            non_cov_inter_model_list = []
-            for curr_non_cov_tuple in non_cov_tuple_list:
-                curr_non_cov_inter = NonCovInterModel()
-                curr_non_cov_inter.id = AlchemyUtil.gen_unique_key()
-                curr_non_cov_inter.psm = curr_non_cov_tuple[0],
-                curr_non_cov_inter.name = curr_non_cov_tuple[1],
-                curr_non_cov_inter.method = curr_non_cov_tuple[2],
-                curr_non_cov_inter.path = curr_non_cov_tuple[3],
-                curr_non_cov_inter.rpc_method = curr_non_cov_tuple[4],
-                curr_non_cov_inter.note = curr_non_cov_tuple[5],
-                curr_non_cov_inter.endpoint_id = curr_non_cov_tuple[6],
-                curr_non_cov_inter.version = curr_non_cov_tuple[7]
-                non_cov_inter_model_list.append(curr_non_cov_inter)
-            dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", CoverDiff._get_db_conf_path())
-            engine = AlchemyUtil.init_engine(dict_val)
-            AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
-            site_rel_db_session = AlchemyUtil.get_session(engine)
-            AlchemyUtil.insert_list_with_flush_only(site_rel_db_session, non_cov_inter_model_list)
-            AlchemyUtil.do_commit_only(site_rel_db_session)
-        else:
-            logger.info("[无需插入]：non_cov_tuple_list 为空，无需插入。")
-
-    @staticmethod
-    def _delete_non_cov_records(psm, diff_tuple_list):
-        if psm is not None:
-            dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", CoverDiff._get_db_conf_path())
-            engine = AlchemyUtil.init_engine(dict_val)
-            AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
-            site_rel_db_session = AlchemyUtil.get_session(engine)
-            if diff_tuple_list is None:
-                AlchemyUtil.delete_for_criteria_commit(site_rel_db_session, NonCovInterModel, {NonCovInterModel.psm == psm})
-            else:
-                existing_non_cov_list_in_db = AlchemyUtil.query_field_list(site_rel_db_session,\
-                                                                                    (NonCovInterModel.endpoint_id,
-                                                                                     NonCovInterModel.name),\
-                                                                                    {NonCovInterModel.psm == psm})
-                already_cov_endpoint_list = []
-                for non_cov_tuple_in_db in existing_non_cov_list_in_db:
-                    found = False
-                    curr_endpoint = non_cov_tuple_in_db[0]
-                    for curr_diff_tuple in diff_tuple_list:
-                        if curr_endpoint == curr_diff_tuple[6]:
-                            diff_tuple_list.remove(curr_diff_tuple)
-                            found = True
-                            break
-                        else:
-                            pass
-                    if not found:
-                        already_cov_endpoint_list.append(curr_endpoint)
-                # End For
-                logger.info("PSM=[%s]，需要 删除 %d 条记录。" % (psm, len(already_cov_endpoint_list)))
-                if len(already_cov_endpoint_list) > 0:
-                    AlchemyUtil.delete_for_criteria_commit(site_rel_db_session, NonCovInterModel, {NonCovInterModel.endpoint_id in already_cov_endpoint_list})
-                    logger.info("【Success】PSM=[%s]，成功 删除 %d 条记录。" % (psm, len(already_cov_endpoint_list)))
-        else:
-            logger.info("psm is None.")
-            pass
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2021/12/13 2:41 下午
+# @Author  : zhengyu.0985
+# @FileName: base_compare.py
+# @Software: PyCharm
+
+from rolling_king.zijie.db.db_models import CaseRecordModel, BamInterModel, NonCovInterModel
+from rolling_king.zijie.db.sqlalchemy_util import AlchemyUtil
+from rolling_king.zijie.tests.base.base_test import BaseTest
+import logging
+import os
+
+logger = logging.getLogger("base_compare")
+
+
+class CoverDiff(object):
+
+    @staticmethod
+    def _get_db_conf_path():
+        curr_sys_path = os.getcwd()
+        logger.info(f"file_path={curr_sys_path}")
+        index_of_com = curr_sys_path.find("com")
+        if index_of_com != -1:
+            # 下面一行是绝对路径传入获取配置文件的方法。
+            conf_absolute_path = curr_sys_path[0:index_of_com] + "com/conf/"
+            db_conf_file_path = conf_absolute_path + "db.conf"
+        else:
+            # 下面一行的相对路径会随测试py文件位置而变化，仅在测试文件绝对路径中不包含com时，做默认三层情况使用。
+            db_conf_file_path = curr_sys_path + "/com/conf/db.conf"
+        return db_conf_file_path
+
+    @staticmethod
+    def get_diff_result(psm=None, test_project_name=None, protocol="BOTH"):
+        db_conf_dict = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", CoverDiff._get_db_conf_path())
+        engine = AlchemyUtil.init_engine(db_conf_dict)
+        AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
+        site_rel_db_session = AlchemyUtil.get_session(engine)
+        # 判断已测试（分子）的查询范围。
+        if psm is None and test_project_name is None:
+            project_conf_dict = BaseTest.get_project_conf_dict()
+            psm = project_conf_dict['test_psm']
+            test_project_name = project_conf_dict['test_project_name']
+            tested_criteria_set = {  # 这是<class 'set'>类型。
+                CaseRecordModel.test_psm == psm,  # 被测PSM
+                CaseRecordModel.test_project_name == test_project_name  # 测试项目名
+            }
+        elif psm is None:
+            project_conf_dict = BaseTest.get_project_conf_dict()
+            psm = project_conf_dict['test_psm']
+            tested_criteria_set = {  # 这是<class 'set'>类型。
+                CaseRecordModel.test_psm == psm,  # 被测PSM
+                CaseRecordModel.test_project_name == test_project_name  # 测试项目名
+            }
+        elif test_project_name is None:  # 只传入PSM，证明与被测项目无关，全局进行查询。
+            logger.info("test_project_name is None")
+            tested_criteria_set = {  # 这是<class 'set'>类型。
+                CaseRecordModel.test_psm == psm,  # 被测PSM
+            }
+        else:
+            tested_criteria_set = {  # 这是<class 'set'>类型。
+                CaseRecordModel.test_psm == psm,  # 被测PSM
+                CaseRecordModel.test_project_name == test_project_name  # 测试项目名
+            }
+
+        # 获取已测试列表
+        tested_list = AlchemyUtil.query_obj_list(site_rel_db_session, CaseRecordModel, tested_criteria_set)
+
+        # 下面查询总接口数（分母）
+
+        # 查询总接口的若干字段
+        collum_tuple = (BamInterModel.psm, BamInterModel.name, BamInterModel.method, BamInterModel.path,\
+                        BamInterModel.rpc_method, BamInterModel.note, BamInterModel.endpoint_id, BamInterModel.version)
+
+        # 依据想要对比的接口协议类型，进行对比。
+        if protocol == "HTTP" or protocol == "REST":
+            logger.info("仅对比HTTP接口")
+            total_criteria_set = {  # 这是<class 'set'>类型。
+                BamInterModel.psm == psm,
+                BamInterModel.path != '',
+                BamInterModel.method != ''
+            }
+            total_list = AlchemyUtil.query_field_list(site_rel_db_session, collum_tuple,
+                                                      criteria_set=total_criteria_set)
+            if len(tested_list) == 0:
+                logger.info("tested_list：为空")
+                if len(total_list) > 0:
+                    CoverDiff._delete_non_cov_records(psm, total_list)
+                    CoverDiff._insert_non_cov_to_db(psm, total_list)
+            elif len(total_list) == 0:
+                logger.info("total_list：为空")
+            else:
+                diff_tuple_list = CoverDiff._compare_http(tested_list, total_list)
+                CoverDiff._delete_non_cov_records(psm, diff_tuple_list)
+                CoverDiff._insert_non_cov_to_db(psm, diff_tuple_list)
+                return len(diff_tuple_list)
+        elif protocol == "RPC" or protocol == "THRIFT":
+            logger.info("仅对比RPC接口")
+            total_criteria_set = {  # 这是<class 'set'>类型。
+                BamInterModel.psm == psm,
+                BamInterModel.path == '',
+                BamInterModel.method == ''
+            }
+            total_list = AlchemyUtil.query_field_list(site_rel_db_session, collum_tuple,
+                                                      criteria_set=total_criteria_set)
+            if len(tested_list) == 0:
+                logger.info("tested_list：为空")
+                if len(total_list) > 0:
+                    CoverDiff._delete_non_cov_records(psm, total_list)
+                    CoverDiff._insert_non_cov_to_db(psm, total_list)
+            elif len(total_list) == 0:
+                logger.info("total_list：为空")
+            else:
+                diff_tuple_list = CoverDiff._compare_rpc(tested_list, total_list)
+                CoverDiff._delete_non_cov_records(psm, diff_tuple_list)
+                CoverDiff._insert_non_cov_to_db(psm, diff_tuple_list)
+                return len(diff_tuple_list)
+        else:
+            logger.info("HTTP and RPC 接口均对比")
+            total_criteria_set = {  # 这是<class 'set'>类型。
+                BamInterModel.psm == psm,
+            }
+            total_list = AlchemyUtil.query_field_list(site_rel_db_session, collum_tuple,
+                                                      criteria_set=total_criteria_set)
+            if len(tested_list) == 0:
+                logger.info("tested_list：为空")
+                if len(total_list) > 0:
+                    CoverDiff._delete_non_cov_records(psm, total_list)
+                    CoverDiff._insert_non_cov_to_db(psm, total_list)
+            elif len(total_list) == 0:
+                logger.info("total_list：为空")
+            else:
+                diff_tuple_list = CoverDiff._compare_both(tested_list, total_list)
+                CoverDiff._delete_non_cov_records(psm, diff_tuple_list)
+                CoverDiff._insert_non_cov_to_db(psm, diff_tuple_list)
+                return len(diff_tuple_list)
+        # 返回数量
+        return 0
+
+    @staticmethod
+    def _compare_rpc(tested_list, total_list):
+        logger.info("一共 %d 个接口。" % len(total_list))
+        for curr_test in tested_list:
+            curr_rpc_method = curr_test.__dict__['test_interface'].split(".")[1]
+            for curr_db_record in total_list:
+                if curr_rpc_method == curr_db_record[4]:
+                    logger.info("curr_db_record = %s" % curr_db_record)
+                    logger.info("[RPC] %s 已被 %s 项目的 %s 测试用例覆盖。" % (curr_rpc_method, curr_test.test_project_name, curr_test.test_method))
+                    total_list.remove(curr_db_record)
+                    break
+                else:
+                    pass
+        logger.info("未覆盖 %d 个接口" % len(total_list))
+        return total_list
+
+    @staticmethod
+    def _compare_http(tested_list, total_list):
+        logger.info("一共 %d 个接口。" % len(total_list))
+        for curr_test in tested_list:
+            curr_http_uri = curr_test.__dict__['test_interface'].split("::")[1]
+            for curr_db_record in total_list:
+                if curr_http_uri == curr_db_record[3]:
+                    logger.info("curr_db_record = %s" % curr_db_record)
+                    logger.info("[REST] %s 已被 %s 项目的 %s 测试用例覆盖。" % (curr_http_uri, curr_test.test_project_name, curr_test.test_method))
+                    total_list.remove(curr_db_record)
+                    break
+                else:
+                    pass
+        logger.info("未覆盖 %d 个接口" % len(total_list))
+        return total_list
+
+    @staticmethod
+    def _compare_both(tested_list, total_list):
+        logger.info("一共 %d 个接口。" % len(total_list))
+        for curr_test in tested_list:
+            if curr_test.test_inter_type == 'HTTP':
+                curr_http_uri = curr_test.__dict__['test_interface'].split("::")[1]
+                for curr_db_record in total_list:
+                    if curr_http_uri == curr_db_record[3]:
+                        logger.info("curr_db_record = %s" % curr_db_record)
+                        logger.info("[REST] %s 已被 %s 项目的 %s 测试用例覆盖。" % (
+                        curr_http_uri, curr_test.test_project_name, curr_test.test_method))
+                        total_list.remove(curr_db_record)
+                        break
+                    else:
+                        pass
+                # End For
+            elif curr_test.test_inter_type == 'THRIFT':
+                curr_rpc_method = curr_test.__dict__['test_interface'].split(".")[1]
+                for curr_db_record in total_list:
+                    if curr_rpc_method == curr_db_record[4]:
+                        logger.info("curr_db_record = %s" % curr_db_record)
+                        logger.info("[RPC] %s 已被 %s 项目的 %s 测试用例覆盖。" % (
+                        curr_rpc_method, curr_test.test_project_name, curr_test.test_method))
+                        total_list.remove(curr_db_record)
+                        break
+                    else:
+                        pass
+                # End For
+            else:
+                pass
+        logger.info("未覆盖 %d 个接口" % len(total_list))
+        return total_list
+
+    @staticmethod
+    def _insert_non_cov_to_db(psm, non_cov_tuple_list):
+        if non_cov_tuple_list is not None and len(non_cov_tuple_list) > 0:
+            logger.info("PSM=[%s]，需要 插入 %d 条记录。" % (psm, len(non_cov_tuple_list)))
+            non_cov_inter_model_list = []
+            for curr_non_cov_tuple in non_cov_tuple_list:
+                curr_non_cov_inter = NonCovInterModel()
+                curr_non_cov_inter.id = AlchemyUtil.gen_unique_key()
+                curr_non_cov_inter.psm = curr_non_cov_tuple[0],
+                curr_non_cov_inter.name = curr_non_cov_tuple[1],
+                curr_non_cov_inter.method = curr_non_cov_tuple[2],
+                curr_non_cov_inter.path = curr_non_cov_tuple[3],
+                curr_non_cov_inter.rpc_method = curr_non_cov_tuple[4],
+                curr_non_cov_inter.note = curr_non_cov_tuple[5],
+                curr_non_cov_inter.endpoint_id = curr_non_cov_tuple[6],
+                curr_non_cov_inter.version = curr_non_cov_tuple[7]
+                non_cov_inter_model_list.append(curr_non_cov_inter)
+            dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", CoverDiff._get_db_conf_path())
+            engine = AlchemyUtil.init_engine(dict_val)
+            AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
+            site_rel_db_session = AlchemyUtil.get_session(engine)
+            AlchemyUtil.insert_list_with_flush_only(site_rel_db_session, non_cov_inter_model_list)
+            AlchemyUtil.do_commit_only(site_rel_db_session)
+        else:
+            logger.info("[无需插入]：non_cov_tuple_list 为空，无需插入。")
+
+    @staticmethod
+    def _delete_non_cov_records(psm, diff_tuple_list):
+        if psm is not None:
+            dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", CoverDiff._get_db_conf_path())
+            engine = AlchemyUtil.init_engine(dict_val)
+            AlchemyUtil.init_db(engine)  # 创建表（存在则不创建）
+            site_rel_db_session = AlchemyUtil.get_session(engine)
+            if diff_tuple_list is None:
+                AlchemyUtil.delete_for_criteria_commit(site_rel_db_session, NonCovInterModel, {NonCovInterModel.psm == psm})
+            else:
+                existing_non_cov_list_in_db = AlchemyUtil.query_field_list(site_rel_db_session,\
+                                                                                    (NonCovInterModel.endpoint_id,
+                                                                                     NonCovInterModel.name),\
+                                                                                    {NonCovInterModel.psm == psm})
+                already_cov_endpoint_list = []
+                for non_cov_tuple_in_db in existing_non_cov_list_in_db:
+                    found = False
+                    curr_endpoint = non_cov_tuple_in_db[0]
+                    for curr_diff_tuple in diff_tuple_list:
+                        if curr_endpoint == curr_diff_tuple[6]:
+                            diff_tuple_list.remove(curr_diff_tuple)
+                            found = True
+                            break
+                        else:
+                            pass
+                    if not found:
+                        already_cov_endpoint_list.append(curr_endpoint)
+                # End For
+                logger.info("PSM=[%s]，需要 删除 %d 条记录。" % (psm, len(already_cov_endpoint_list)))
+                if len(already_cov_endpoint_list) > 0:
+                    AlchemyUtil.delete_for_criteria_commit(site_rel_db_session, NonCovInterModel, {NonCovInterModel.endpoint_id in already_cov_endpoint_list})
+                    logger.info("【Success】PSM=[%s]，成功 删除 %d 条记录。" % (psm, len(already_cov_endpoint_list)))
+        else:
+            logger.info("psm is None.")
+            pass
```

### Comparing `rolling-in-the-deep-0.1.1/src/rolling_king/zijie/tests/base/base_test.py` & `rolling-in-the-deep-0.1.2/src/rolling_king/zijie/tests/base/base_test.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2021/12/8 3:26 下午
-# @Author  : zhengyu.0985
-# @FileName: base_test.py
-# @Software: PyCharm
-
-from rolling_king.zijie.db.sqlalchemy_util import AlchemyUtil
-from rolling_king.zijie.db.db_models import CaseRecordDecoder, CaseRecordModel, ExecutionRecordDecoder
-import logging
-import configparser
-import json
-import os
-import time
-
-logging.basicConfig(level=logging.DEBUG,
-                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
-logger = logging.getLogger('com.zijie.tests.base_test')
-
-
-class BaseTest(object):
-
-    conf_absolute_path = "../../../conf/"  # 默认值是一个相对路径，但若测试类的python文件绝对路径包含com，则会被修改为绝对路径以适用。
-    case_record_dict_list = []  # 每次测试执行收集测试用例信息的列表。
-    # 以下属性是测试执行记录所用到
-    unique_tag = None  # 每次测试执行的唯一标识。
-    execution_record_dict_list = []  # 每次测试执行收集测试执行结果的列表。
-
-    @staticmethod
-    def _get_project_param_dict(project_conf_file_path):
-        project_conf_file = open(project_conf_file_path)
-        cf = configparser.ConfigParser()
-        cf.read_file(project_conf_file)
-        logger.info("从 %s 读取到 %d 个配置项。" % (project_conf_file_path, len(cf.items())))
-        dict_val = {
-            "test_project_name": cf.get("project", "TEST_PROJECT_NAME"),
-            "test_psm": cf.get("project", "TEST_PSM")
-        }
-        logger.info("项目参数 = %s" % dict_val)
-        return dict_val
-
-    @staticmethod
-    def get_project_conf_dict():
-        curr_sys_path = os.getcwd()
-        index_of_com = curr_sys_path.find("com")
-        if index_of_com != -1:
-            # 下面一行是绝对路径传入获取配置文件的方法。
-            BaseTest.conf_absolute_path = curr_sys_path[0:index_of_com] + "com/conf/"
-            project_param_dict = BaseTest._get_project_param_dict(BaseTest.conf_absolute_path + "project.conf")
-        else:
-            # 下面一行的相对路径会随测试py文件位置而变化，仅在测试文件绝对路径中不包含com时，做默认三层情况使用。
-            project_param_dict = BaseTest._get_project_param_dict(curr_sys_path + "/com/conf/project.conf")
-        return project_param_dict
-
-    @staticmethod
-    def analyze_func_desc(entire_desc):
-        tested_inter_dict_val = {
-            "test_interface": "",
-            "test_inter_type": "",
-            "test_description": "",
-        }
-        desc_list = entire_desc.split("\n")
-        for seg in desc_list:
-            if seg.find("desc") != -1:
-                start_index_desc = seg.find("desc") + 5
-                test_description = seg[start_index_desc:].strip()
-                tested_inter_dict_val['test_description'] = test_description
-            if seg.find("api_info") != -1:
-                start_index_api_info = seg.find("api_info") + 9
-                desc_dict_str = seg[start_index_api_info:].strip()
-                api_dict = json.loads(desc_dict_str)
-                protocol = api_dict['protocol_type']
-                tested_inter_dict_val['test_inter_type'] = protocol
-                if protocol == "HTTP":
-                    tested_inter_dict_val['test_interface'] = api_dict['inter_name'] + "::" + api_dict['inter_path']
-                elif protocol == "THRIFT":
-                    tested_inter_dict_val['test_interface'] = api_dict['inter_name'] + "." + api_dict['method_name']
-                else:
-                    logger.error("传入的protocol既不是HTTP也不是THRIFT。")
-        logger.info("被测接口 = %s" % tested_inter_dict_val)
-        return tested_inter_dict_val
-
-    @staticmethod
-    def _get_db_rela_conf_path(db_conf_path=None):
-        if db_conf_path is not None:
-            return db_conf_path
-        else:
-            curr_sys_path = os.getcwd()
-            logger.info(f"curr_sys_path={curr_sys_path}")
-            index_of_com = curr_sys_path.find("com")
-            if index_of_com != -1:
-                # 下面一行是绝对路径传入获取配置文件的方法。
-                BaseTest.conf_absolute_path = curr_sys_path[0:index_of_com] + "com/conf/"
-            else:
-                logger.warning("被测路径不包含com。")
-                BaseTest.conf_absolute_path = curr_sys_path + "/com/conf/"
-            return BaseTest.conf_absolute_path + "db.conf"
-
-    @staticmethod
-    def insert_update_delete():
-        dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", BaseTest._get_db_rela_conf_path())
-        site_rel_db_engine = AlchemyUtil.init_engine(dict_val)
-        site_rel_db_session = AlchemyUtil.get_session(site_rel_db_engine)
-        case_change_flag = False  # 用来判断是否本次执行相对于DB中的已存记录有变化（新增了或者删除了用例）
-        project_conf_dict = BaseTest.get_project_conf_dict()
-        # 查询
-        criteria_set = {  # 这是<class 'set'>类型。
-            CaseRecordModel.test_psm == project_conf_dict['test_psm'],  # 被测PSM
-            CaseRecordModel.test_project_name == project_conf_dict['test_project_name']  #测试项目名
-        }
-        # 获取DB中的test_psm和test_project_name条件的用例记录。
-        db_case_record_model_list = AlchemyUtil.query_obj_list(site_rel_db_session, CaseRecordModel, criteria_set=criteria_set)
-        # 获取本次TEST的用例记录。
-        test_case_record_model_list = []
-        for curr_case_dict in BaseTest.case_record_dict_list:
-            test_case_record_model_list.append(CaseRecordDecoder.dict_to_obj(curr_case_dict))
-        # 将TEST与DB所存的用例记录做对比，以判断是要插入还是更新还是删除。
-        logger.info("DB中现有记录：%d 个。" % len(db_case_record_model_list))
-        logger.info("本次测试记录：%s 个。" % len(test_case_record_model_list))
-        if len(db_case_record_model_list) == 0:  # DB中没有现存记录，全是新增，直接插入即可。
-            AlchemyUtil.insert_list_with_flush_only(site_rel_db_session, test_case_record_model_list)
-            AlchemyUtil.do_commit_only(site_rel_db_session)
-        elif len(test_case_record_model_list) > 0:  # DB中有现有记录且本次测试用例数>0
-            curr_version_in_db = db_case_record_model_list[0].version  # 获取当前DB中相关用例的版本号。
-            matched_db_record_uid_list = []
-            disuse_db_record_uid_list = []
-            for db_case_model in db_case_record_model_list:
-                logger.info("***当前 db_case_model: test_class=%s, test_method=%s, uid=%d" % (db_case_model.test_class, db_case_model.test_method, db_case_model.uid))
-                for test_case_model in test_case_record_model_list:
-                    # 当前db记录跟每一个测试记录比较。
-                    logger.info("---当前 test_case_model: test_class=%s, test_method=%s" % (test_case_model.test_class, test_case_model.test_method))
-                    if db_case_model.test_class == test_case_model.test_class and db_case_model.test_method == test_case_model.test_method:
-                        logger.info("找到 test_class=%s, test_method=%s 的 uid=%d DB记录：%s" % (db_case_model.test_class, db_case_model.test_method, db_case_model.uid, db_case_model.to_json()))
-                        test_case_model.uid = db_case_model.uid  # 原本test_case_model.uid=0，找到匹配的就存DB中的uid的值。
-                        logger.info("当前 test_case_model: test_class=%s, test_method=%s 设为 uid=%d" % (test_case_model.test_class, test_case_model.test_method, test_case_model.uid))
-                        matched_db_record_uid_list.append(db_case_model.uid)
-                        logger.info("当前 db_case_model uid=%d 加入匹配列表中" % db_case_model.uid)
-                        break
-                    else:
-                        pass
-                    # End Inner For Loop
-                if db_case_model.uid not in matched_db_record_uid_list:  # 跟所有测试记录比对之后还未匹配，说明该条DB记录跟所有测试记录都不匹配，已经作废。
-                    case_change_flag = True
-                    disuse_db_record_uid_list.append(db_case_model.uid)
-                    logger.info("DB中的 uid = %d 的记录作废，并加入作废列表中。" % db_case_model.uid)
-                    del_row = AlchemyUtil.delete_for_criteria_commit(site_rel_db_session, CaseRecordModel, {CaseRecordModel.uid == db_case_model.uid})  # 从数据库中也删除。
-                    logger.info("DB中的 uid = %d 的 %d 条记录从DB数据库中删除：" % (db_case_model.uid, del_row))
-                else:
-                    pass
-                # End Outer For Loop
-            # 因全部循环已结束，所以打印匹配列表中的uid，看一看。
-            logger.info("匹配列表中的uid如下:")
-            for matched_uid in matched_db_record_uid_list:
-                logger.info("matched_uid = %d" % matched_uid)
-            logger.info("作废列表中的uid如下:")
-            # 因全部循环已结束，所以打印作废列表中的uid，看一看。
-            for disuse_uid in disuse_db_record_uid_list:
-                logger.info("disuse_uid = %d" % disuse_uid)
-            logger.info("本次测试一共作废 %d 个DB中的用例记录。" % len(disuse_db_record_uid_list))
-            # 下面处理本次测试新增的用例情况。
-            # test_case_record_model_list 中剩下的（没有匹配到的，也就是uid依然=0的那部分）是DB中没有的，也就是新增的，需要插入数据库。
-            new_case_count = 0
-            for test_case_model in test_case_record_model_list:
-                if test_case_model.uid == 0:
-                    case_change_flag = True
-                    AlchemyUtil.insert_obj_with_commit(site_rel_db_session, test_case_model)
-                    new_case_count += 1
-                else:
-                    pass
-            logger.info("本次测试一共新增 %d 个测试用例。" % new_case_count)
-            # 依据 case_change_flag 标志位判断是否有用例的新增或删除，有变化则全部相关用例version增1
-            if case_change_flag:
-                logger.info("本次测试用例有变化。")
-                new_version = curr_version_in_db + 1
-                logger.info("new_version = %d" % new_version)
-                update_dict = {
-                    'version': new_version,
-                    'gmt_modify': time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
-                }
-                affected_row = AlchemyUtil.update_for_criteria_with_commit(site_rel_db_session, CaseRecordModel, criteria_set, update_dict)
-                logger.info("【Success】Totally, {0} Records have been updated with version = {1}.".format(affected_row, new_version))
-            else:
-                logger.info("本次测试毫无变化，无用例新增、无用例删除。")
-            # End Elif
-        else:
-            logger.info("本次测试不包含任何测试用例。")
-        # End Of insert_update_delete Method
-
-    @staticmethod
-    def insert_execution_record():
-        dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", BaseTest.conf_absolute_path + "db.conf")
-        site_rel_db_engine = AlchemyUtil.init_engine(dict_val)
-        site_rel_db_session = AlchemyUtil.get_session(site_rel_db_engine)
-        for curr_execution_dict in BaseTest.execution_record_dict_list:
-            logger.info("curr_execution_dict = %s" % curr_execution_dict)
-            curr_execution_model = ExecutionRecordDecoder.dict_to_obj(curr_execution_dict)
-            AlchemyUtil.insert_obj_without_commit(session=site_rel_db_session, obj=curr_execution_model)
-        AlchemyUtil.do_commit_only(site_rel_db_session)
-        logger.info("本次新增 %d 条测试执行记录并插入至DB。" % len(BaseTest.execution_record_dict_list))
-
-
-###############################################################################
-
-
-if __name__ == "__main__":
-    base_test = BaseTest()
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2021/12/8 3:26 下午
+# @Author  : zhengyu.0985
+# @FileName: base_test.py
+# @Software: PyCharm
+
+from rolling_king.zijie.db.sqlalchemy_util import AlchemyUtil
+from rolling_king.zijie.db.db_models import CaseRecordDecoder, CaseRecordModel, ExecutionRecordDecoder
+import logging
+import configparser
+import json
+import os
+import time
+
+logging.basicConfig(level=logging.DEBUG,
+                    format='%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s')  # logging.basicConfig函数对日志的输出格式及方式做相关配置
+logger = logging.getLogger('com.zijie.tests.base_test')
+
+
+class BaseTest(object):
+
+    conf_absolute_path = "../../../conf/"  # 默认值是一个相对路径，但若测试类的python文件绝对路径包含com，则会被修改为绝对路径以适用。
+    case_record_dict_list = []  # 每次测试执行收集测试用例信息的列表。
+    # 以下属性是测试执行记录所用到
+    unique_tag = None  # 每次测试执行的唯一标识。
+    execution_record_dict_list = []  # 每次测试执行收集测试执行结果的列表。
+
+    @staticmethod
+    def _get_project_param_dict(project_conf_file_path):
+        project_conf_file = open(project_conf_file_path)
+        cf = configparser.ConfigParser()
+        cf.read_file(project_conf_file)
+        logger.info("从 %s 读取到 %d 个配置项。" % (project_conf_file_path, len(cf.items())))
+        dict_val = {
+            "test_project_name": cf.get("project", "TEST_PROJECT_NAME"),
+            "test_psm": cf.get("project", "TEST_PSM")
+        }
+        logger.info("项目参数 = %s" % dict_val)
+        return dict_val
+
+    @staticmethod
+    def get_project_conf_dict():
+        curr_sys_path = os.getcwd()
+        index_of_com = curr_sys_path.find("com")
+        if index_of_com != -1:
+            # 下面一行是绝对路径传入获取配置文件的方法。
+            BaseTest.conf_absolute_path = curr_sys_path[0:index_of_com] + "com/conf/"
+            project_param_dict = BaseTest._get_project_param_dict(BaseTest.conf_absolute_path + "project.conf")
+        else:
+            # 下面一行的相对路径会随测试py文件位置而变化，仅在测试文件绝对路径中不包含com时，做默认三层情况使用。
+            project_param_dict = BaseTest._get_project_param_dict(curr_sys_path + "/com/conf/project.conf")
+        return project_param_dict
+
+    @staticmethod
+    def analyze_func_desc(entire_desc):
+        tested_inter_dict_val = {
+            "test_interface": "",
+            "test_inter_type": "",
+            "test_description": "",
+        }
+        desc_list = entire_desc.split("\n")
+        for seg in desc_list:
+            if seg.find("desc") != -1:
+                start_index_desc = seg.find("desc") + 5
+                test_description = seg[start_index_desc:].strip()
+                tested_inter_dict_val['test_description'] = test_description
+            if seg.find("api_info") != -1:
+                start_index_api_info = seg.find("api_info") + 9
+                desc_dict_str = seg[start_index_api_info:].strip()
+                api_dict = json.loads(desc_dict_str)
+                protocol = api_dict['protocol_type']
+                tested_inter_dict_val['test_inter_type'] = protocol
+                if protocol == "HTTP":
+                    tested_inter_dict_val['test_interface'] = api_dict['inter_name'] + "::" + api_dict['inter_path']
+                elif protocol == "THRIFT":
+                    tested_inter_dict_val['test_interface'] = api_dict['inter_name'] + "." + api_dict['method_name']
+                else:
+                    logger.error("传入的protocol既不是HTTP也不是THRIFT。")
+        logger.info("被测接口 = %s" % tested_inter_dict_val)
+        return tested_inter_dict_val
+
+    @staticmethod
+    def _get_db_rela_conf_path(db_conf_path=None):
+        if db_conf_path is not None:
+            return db_conf_path
+        else:
+            curr_sys_path = os.getcwd()
+            logger.info(f"curr_sys_path={curr_sys_path}")
+            index_of_com = curr_sys_path.find("com")
+            if index_of_com != -1:
+                # 下面一行是绝对路径传入获取配置文件的方法。
+                BaseTest.conf_absolute_path = curr_sys_path[0:index_of_com] + "com/conf/"
+            else:
+                logger.warning("被测路径不包含com。")
+                BaseTest.conf_absolute_path = curr_sys_path + "/com/conf/"
+            return BaseTest.conf_absolute_path + "db.conf"
+
+    @staticmethod
+    def insert_update_delete():
+        dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", BaseTest._get_db_rela_conf_path())
+        site_rel_db_engine = AlchemyUtil.init_engine(dict_val)
+        site_rel_db_session = AlchemyUtil.get_session(site_rel_db_engine)
+        case_change_flag = False  # 用来判断是否本次执行相对于DB中的已存记录有变化（新增了或者删除了用例）
+        project_conf_dict = BaseTest.get_project_conf_dict()
+        # 查询
+        criteria_set = {  # 这是<class 'set'>类型。
+            CaseRecordModel.test_psm == project_conf_dict['test_psm'],  # 被测PSM
+            CaseRecordModel.test_project_name == project_conf_dict['test_project_name']  #测试项目名
+        }
+        # 获取DB中的test_psm和test_project_name条件的用例记录。
+        db_case_record_model_list = AlchemyUtil.query_obj_list(site_rel_db_session, CaseRecordModel, criteria_set=criteria_set)
+        # 获取本次TEST的用例记录。
+        test_case_record_model_list = []
+        for curr_case_dict in BaseTest.case_record_dict_list:
+            test_case_record_model_list.append(CaseRecordDecoder.dict_to_obj(curr_case_dict))
+        # 将TEST与DB所存的用例记录做对比，以判断是要插入还是更新还是删除。
+        logger.info("DB中现有记录：%d 个。" % len(db_case_record_model_list))
+        logger.info("本次测试记录：%s 个。" % len(test_case_record_model_list))
+        if len(db_case_record_model_list) == 0:  # DB中没有现存记录，全是新增，直接插入即可。
+            AlchemyUtil.insert_list_with_flush_only(site_rel_db_session, test_case_record_model_list)
+            AlchemyUtil.do_commit_only(site_rel_db_session)
+        elif len(test_case_record_model_list) > 0:  # DB中有现有记录且本次测试用例数>0
+            curr_version_in_db = db_case_record_model_list[0].version  # 获取当前DB中相关用例的版本号。
+            matched_db_record_uid_list = []
+            disuse_db_record_uid_list = []
+            for db_case_model in db_case_record_model_list:
+                logger.info("***当前 db_case_model: test_class=%s, test_method=%s, uid=%d" % (db_case_model.test_class, db_case_model.test_method, db_case_model.uid))
+                for test_case_model in test_case_record_model_list:
+                    # 当前db记录跟每一个测试记录比较。
+                    logger.info("---当前 test_case_model: test_class=%s, test_method=%s" % (test_case_model.test_class, test_case_model.test_method))
+                    if db_case_model.test_class == test_case_model.test_class and db_case_model.test_method == test_case_model.test_method:
+                        logger.info("找到 test_class=%s, test_method=%s 的 uid=%d DB记录：%s" % (db_case_model.test_class, db_case_model.test_method, db_case_model.uid, db_case_model.to_json()))
+                        test_case_model.uid = db_case_model.uid  # 原本test_case_model.uid=0，找到匹配的就存DB中的uid的值。
+                        logger.info("当前 test_case_model: test_class=%s, test_method=%s 设为 uid=%d" % (test_case_model.test_class, test_case_model.test_method, test_case_model.uid))
+                        matched_db_record_uid_list.append(db_case_model.uid)
+                        logger.info("当前 db_case_model uid=%d 加入匹配列表中" % db_case_model.uid)
+                        break
+                    else:
+                        pass
+                    # End Inner For Loop
+                if db_case_model.uid not in matched_db_record_uid_list:  # 跟所有测试记录比对之后还未匹配，说明该条DB记录跟所有测试记录都不匹配，已经作废。
+                    case_change_flag = True
+                    disuse_db_record_uid_list.append(db_case_model.uid)
+                    logger.info("DB中的 uid = %d 的记录作废，并加入作废列表中。" % db_case_model.uid)
+                    del_row = AlchemyUtil.delete_for_criteria_commit(site_rel_db_session, CaseRecordModel, {CaseRecordModel.uid == db_case_model.uid})  # 从数据库中也删除。
+                    logger.info("DB中的 uid = %d 的 %d 条记录从DB数据库中删除：" % (db_case_model.uid, del_row))
+                else:
+                    pass
+                # End Outer For Loop
+            # 因全部循环已结束，所以打印匹配列表中的uid，看一看。
+            logger.info("匹配列表中的uid如下:")
+            for matched_uid in matched_db_record_uid_list:
+                logger.info("matched_uid = %d" % matched_uid)
+            logger.info("作废列表中的uid如下:")
+            # 因全部循环已结束，所以打印作废列表中的uid，看一看。
+            for disuse_uid in disuse_db_record_uid_list:
+                logger.info("disuse_uid = %d" % disuse_uid)
+            logger.info("本次测试一共作废 %d 个DB中的用例记录。" % len(disuse_db_record_uid_list))
+            # 下面处理本次测试新增的用例情况。
+            # test_case_record_model_list 中剩下的（没有匹配到的，也就是uid依然=0的那部分）是DB中没有的，也就是新增的，需要插入数据库。
+            new_case_count = 0
+            for test_case_model in test_case_record_model_list:
+                if test_case_model.uid == 0:
+                    case_change_flag = True
+                    AlchemyUtil.insert_obj_with_commit(site_rel_db_session, test_case_model)
+                    new_case_count += 1
+                else:
+                    pass
+            logger.info("本次测试一共新增 %d 个测试用例。" % new_case_count)
+            # 依据 case_change_flag 标志位判断是否有用例的新增或删除，有变化则全部相关用例version增1
+            if case_change_flag:
+                logger.info("本次测试用例有变化。")
+                new_version = curr_version_in_db + 1
+                logger.info("new_version = %d" % new_version)
+                update_dict = {
+                    'version': new_version,
+                    'gmt_modify': time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+                }
+                affected_row = AlchemyUtil.update_for_criteria_with_commit(site_rel_db_session, CaseRecordModel, criteria_set, update_dict)
+                logger.info("【Success】Totally, {0} Records have been updated with version = {1}.".format(affected_row, new_version))
+            else:
+                logger.info("本次测试毫无变化，无用例新增、无用例删除。")
+            # End Elif
+        else:
+            logger.info("本次测试不包含任何测试用例。")
+        # End Of insert_update_delete Method
+
+    @staticmethod
+    def insert_execution_record():
+        dict_val = AlchemyUtil.get_db_param_dict("DB_BOE_Site_Reldb", BaseTest.conf_absolute_path + "db.conf")
+        site_rel_db_engine = AlchemyUtil.init_engine(dict_val)
+        site_rel_db_session = AlchemyUtil.get_session(site_rel_db_engine)
+        for curr_execution_dict in BaseTest.execution_record_dict_list:
+            logger.info("curr_execution_dict = %s" % curr_execution_dict)
+            curr_execution_model = ExecutionRecordDecoder.dict_to_obj(curr_execution_dict)
+            AlchemyUtil.insert_obj_without_commit(session=site_rel_db_session, obj=curr_execution_model)
+        AlchemyUtil.do_commit_only(site_rel_db_session)
+        logger.info("本次新增 %d 条测试执行记录并插入至DB。" % len(BaseTest.execution_record_dict_list))
+
+
+###############################################################################
+
+
+if __name__ == "__main__":
+    base_test = BaseTest()
```

### Comparing `rolling-in-the-deep-0.1.1/src/tests/conftest.py` & `rolling-in-the-deep-0.1.2/src/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# @Time    : 2022/4/2 10:37 AM
-# @Author  : zhengyu.0985
-# @FileName: conftest.py
-# @Software: PyCharm
-
-import pytest
-
-
-def pytest_addoption(parser):
-    print("pytest_addoption func executes...")
-    parser.addoption(
-        "--cmdopt", action="store", default="type1", help="my option: type1 or type2"
-    )
-    parser.addoption(
-        "--env", action="store", default="dev", help="env：表示测试环境，默认dev环境"
-    )
-
-
-# @pytest.fixture(scope="module")
-# def cmdopt(pytestconfig):
-#     return pytestconfig.getoption("cmdopt")
-
-@pytest.fixture(scope="module")
-def cmdopt(request):
-    return request.config.getoption("--cmdopt")
-
-
-@pytest.fixture(scope="module")
-def env(request):
-    return request.config.getoption("--env")
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# @Time    : 2022/4/2 10:37 AM
+# @Author  : zhengyu.0985
+# @FileName: conftest.py
+# @Software: PyCharm
+
+import pytest
+
+
+def pytest_addoption(parser):
+    print("pytest_addoption func executes...")
+    parser.addoption(
+        "--cmdopt", action="store", default="type1", help="my option: type1 or type2"
+    )
+    parser.addoption(
+        "--env", action="store", default="dev", choices=['dev', 'test'], type=str, help="env：表示测试环境，默认dev环境"
+    )
+
+
+# @pytest.fixture(scope="module")
+# def cmdopt(pytestconfig):
+#     return pytestconfig.getoption("cmdopt")
+
+@pytest.fixture(scope="module")
+def cmdopt(request):
+    return request.config.getoption("--cmdopt")
+
+
+@pytest.fixture(scope="module")
+def env(request):
+    print("execute...")
+    return request.config.getoption("--env")
```

