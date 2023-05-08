# Comparing `tmp/router_log_preprocessor-0.1.5.tar.gz` & `tmp/router_log_preprocessor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "router_log_preprocessor-0.1.5.tar", max compression
+gzip compressed data, was "router_log_preprocessor-0.1.6.tar", max compression
```

## Comparing `router_log_preprocessor-0.1.5.tar` & `router_log_preprocessor-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/LICENSE
--rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.5/README.md
--rw-r--r--   0        0        0      794 2023-04-17 19:20:50.639422 router_log_preprocessor-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/router_log_preprocessor/__init__.py
--rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/router_log_preprocessor/__main__.py
--rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__init__.py
--rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
--rw-r--r--   0        0        0     1317 2023-04-14 18:44:34.268234 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
--rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_dnsmasq_dhcp.py
--rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_message.py
--rw-r--r--   0        0        0     1560 2023-04-14 18:44:28.564220 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_wlc.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__init__.py
--rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
--rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/abc.py
--rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__init__.py
--rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
--rw-r--r--   0        0        0     1898 2023-04-14 18:44:34.272234 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
--rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
--rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_known_clients.py
--rw-r--r--   0        0        0     2644 2023-04-14 18:44:28.588220 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_mapper.py
--rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_trapper.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__init__.py
--rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
--rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
--rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/handler.py
--rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/server.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__init__.py
--rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
--rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
--rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
--rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/typing.py
--rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/wlc.py
--rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.5/router_log_preprocessor/settings.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__init__.py
--rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
--rw-r--r--   0        0        0     3125 2023-04-17 19:09:25.191263 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
--rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/util/logging.py
--rw-r--r--   0        0        0     3860 2023-04-17 19:18:08.344018 router_log_preprocessor-0.1.5/router_log_preprocessor/util/rfc3164_parser.py
--rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.5/setup.py
--rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.6/README.md
+-rw-r--r--   0        0        0      794 2023-05-08 20:04:15.581444 router_log_preprocessor-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.6/router_log_preprocessor/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.6/router_log_preprocessor/__main__.py
+-rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
+-rw-r--r--   0        0        0     1317 2023-04-14 18:44:34.268234 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
+-rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/_dnsmasq_dhcp.py
+-rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/_message.py
+-rw-r--r--   0        0        0     1560 2023-04-14 18:44:28.564220 router_log_preprocessor-0.1.6/router_log_preprocessor/domain/_wlc.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
+-rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/abc.py
+-rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
+-rw-r--r--   0        0        0     1898 2023-04-14 18:44:34.272234 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
+-rw-r--r--   0        0        0     5050 2023-05-08 19:49:19.761228 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
+-rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/_known_clients.py
+-rw-r--r--   0        0        0     2644 2023-04-14 18:44:28.588220 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/_mapper.py
+-rw-r--r--   0        0        0     6776 2023-05-08 20:03:53.929175 router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/_trapper.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
+-rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
+-rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/handler.py
+-rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/server.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
+-rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
+-rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
+-rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/typing.py
+-rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/wlc.py
+-rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.6/router_log_preprocessor/settings.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/util/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.6/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.6/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
+-rw-r--r--   0        0        0     3125 2023-05-03 09:15:23.649248 router_log_preprocessor-0.1.6/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.6/router_log_preprocessor/util/logging.py
+-rw-r--r--   0        0        0     3860 2023-04-17 19:18:08.344018 router_log_preprocessor-0.1.6/router_log_preprocessor/util/rfc3164_parser.py
+-rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.6/setup.py
+-rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.6/PKG-INFO
```

### Comparing `router_log_preprocessor-0.1.5/LICENSE` & `router_log_preprocessor-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/README.md` & `router_log_preprocessor-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/pyproject.toml` & `router_log_preprocessor-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "router-log-preprocessor"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 repository = "https://github.com/mastdi/router-log-preprocessor"
 authors = ["Martin Storgaard Dieu <martin@storgaarddieu.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "router_log_preprocessor"}]
```

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/__init__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/__main__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__init__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/_dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_message.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/_message.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_wlc.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/domain/_wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__init__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/abc.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/abc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__init__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 13 12:50:17 2023 UTC, .py size: 5820 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,264 +1,316 @@
-00000000: 550d 0d0a 0000 0000 89fa 3764 bc16 0000  U.........7d....
+00000000: 550d 0d0a 0000 0000 0851 5964 781a 0000  U........QYdx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c05 6d06 0200 0100 6d07  ..d.d.l.m.....m.
 00000060: 5a07 0100 6400 6401 6c08 6d06 0200 0100  Z...d.d.l.m.....
 00000070: 6d09 0200 0100 6d0a 5a0b 0100 6400 6401  m.....m.Z...d.d.
 00000080: 6c0c 6d06 0200 0100 6d09 0200 0100 6d0d  l.m.....m.....m.
 00000090: 5a0e 0100 6400 6401 6c0f 6d10 0200 0100  Z...d.d.l.m.....
 000000a0: 6d11 5a11 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
 000000b0: 6507 6a12 8303 5a13 6401 5300 2904 e900  e.j...Z.d.S.)...
 000000c0: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
-000000d0: 0000 0000 0004 0000 0000 0000 0073 5000  .............sP.
-000000e0: 0000 6500 5a01 6400 5a02 640b 8700 6601  ..e.Z.d.Z.d...f.
+000000d0: 0000 0000 0004 0000 0000 0000 0073 5800  .............sX.
+000000e0: 0000 6500 5a01 6400 5a02 640d 8700 6601  ..e.Z.d.Z.d...f.
 000000f0: 6403 6404 8409 5a03 6504 6a05 6506 6a07  d.d...Z.e.j.e.j.
 00000100: 6504 6a08 1900 6405 6406 9c03 6407 6408  e.j...d.d...d.d.
 00000110: 8404 5a09 6504 6a05 6504 6a08 650a 6406  ..Z.e.j.e.j.e.d.
-00000120: 9c03 6409 640a 8404 5a0b 8700 0400 5a0c  ..d.d...Z.....Z.
-00000130: 5300 290c da0d 5a61 6262 6978 5472 6170  S.)...ZabbixTrap
-00000140: 7065 72e9 3200 0000 e90a 0000 0063 0400  per.2........c..
-00000150: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00000160: 0000 0300 0000 733c 0000 0074 0083 00a0  ......s<...t....
-00000170: 01a1 0001 007c 017c 005f 027c 027c 005f  .....|.|._.|.|._
-00000180: 0374 04a0 057c 02a1 017c 005f 067c 037c  .t...|...|._.|.|
-00000190: 005f 0764 017c 005f 0874 09a0 0aa1 007c  ._.d.|._.t.....|
-000001a0: 005f 0b64 0053 0029 024e 4629 0cda 0573  ._.d.S.).NF)...s
-000001b0: 7570 6572 da08 5f5f 696e 6974 5f5f da07  uper..__init__..
-000001c0: 5f73 656e 6465 72da 1b5f 636c 6965 6e74  _sender.._client
-000001d0: 5f64 6973 636f 7665 7279 5f77 6169 745f  _discovery_wait_
-000001e0: 7469 6d65 da0d 6b6e 6f77 6e5f 636c 6965  time..known_clie
-000001f0: 6e74 735a 0c4b 6e6f 776e 436c 6965 6e74  ntsZ.KnownClient
-00000200: 73da 0e5f 6b6e 6f77 6e5f 636c 6965 6e74  s.._known_client
-00000210: 73da 1d5f 6d65 6173 7572 656d 656e 745f  s.._measurement_
-00000220: 6275 6e64 6c65 5f77 6169 745f 7469 6d65  bundle_wait_time
-00000230: da19 5f69 735f 6275 6e64 6c69 6e67 5f6d  .._is_bundling_m
-00000240: 6561 7375 7265 6d65 6e74 73da 1561 7379  easurements..asy
-00000250: 6e63 696f 5f7a 6162 6269 785f 7365 6e64  ncio_zabbix_send
-00000260: 6572 da0c 4d65 6173 7572 656d 656e 7473  er..Measurements
-00000270: da0d 5f6d 6561 7375 7265 6d65 6e74 7329  .._measurements)
-00000280: 04da 0473 656c 66da 0673 656e 6465 725a  ...self..senderZ
-00000290: 1a63 6c69 656e 745f 6469 7363 6f76 6572  .client_discover
-000002a0: 795f 7761 6974 5f74 696d 655a 1c6d 6561  y_wait_timeZ.mea
-000002b0: 7375 7265 6d65 6e74 5f62 756e 646c 655f  surement_bundle_
-000002c0: 7761 6974 5f74 696d 65a9 01da 095f 5f63  wait_time....__c
-000002d0: 6c61 7373 5f5f a900 fa6a 2f68 6f6d 652f  lass__...j/home/
-000002e0: 6d79 732f 446f 6375 6d65 6e74 732f 4769  mys/Documents/Gi
-000002f0: 7448 7562 2f6d 6173 7464 692f 726f 7574  tHub/mastdi/rout
-00000300: 6572 2d6c 6f67 2d70 7265 7072 6f63 6573  er-log-preproces
-00000310: 736f 722f 726f 7574 6572 5f6c 6f67 5f70  sor/router_log_p
-00000320: 7265 7072 6f63 6573 736f 722f 686f 6f6b  reprocessor/hook
-00000330: 732f 7a61 6262 6978 2f5f 7472 6170 7065  s/zabbix/_trappe
-00000340: 722e 7079 7206 0000 001b 0000 0073 0e00  r.pyr........s..
-00000350: 0000 0003 0a01 0601 0601 0c01 0601 0601  ................
-00000360: 7a16 5a61 6262 6978 5472 6170 7065 722e  z.ZabbixTrapper.
-00000370: 5f5f 696e 6974 5f5f 4e29 03da 0672 6563  __init__N)...rec
-00000380: 6f72 64da 076d 6573 7361 6765 da06 7265  ord..message..re
-00000390: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
-000003a0: 0007 0000 0006 0000 00c3 0000 0073 d400  .............s..
-000003b0: 0000 7c02 6401 6b08 720c 6401 5300 7c00  ..|.d.k.r.d.S.|.
-000003c0: a000 7c01 7c02 a102 4900 6401 4800 7d03  ..|.|...I.d.H.}.
-000003d0: 7c03 6402 6b04 724c 7401 6a02 a003 6403  |.d.k.rLt.j...d.
-000003e0: 7c02 6a04 7c01 6a05 7c03 a104 0100 7406  |.j.|.j.|.....t.
-000003f0: a007 7c03 a101 4900 6401 4800 0100 7408  ..|...I.d.H...t.
-00000400: a009 7c01 7c02 a102 4400 5d10 7d04 7c00  ..|.|...D.].}.|.
-00000410: 6a0a a00b 7c04 a101 0100 7158 7c00 6a0c  j...|.....qX|.j.
-00000420: 7274 6401 5300 6404 7c00 5f0c 7406 a007  rtd.S.d.|._.t...
-00000430: 7c00 6a0d a101 4900 6401 4800 0100 6405  |.j...I.d.H...d.
-00000440: 7c00 5f0c 7c00 6a0a 7d05 740e a00f a100  |._.|.j.}.t.....
-00000450: 7c00 5f0a 7401 6a02 a010 6406 7c05 a102  |._.t.j...d.|...
-00000460: 0100 7c00 6a11 a012 7c05 a101 4900 6401  ..|.j...|...I.d.
-00000470: 4800 7d06 7401 6a02 a010 6407 7c06 a102  H.}.t.j...d.|...
-00000480: 0100 6401 5300 2908 61fe 0100 0053 656e  ..d.S.).a....Sen
-00000490: 6420 7468 6520 7072 6570 726f 6365 7373  d the preprocess
-000004a0: 6564 206d 6573 7361 6765 2074 6f20 7468  ed message to th
-000004b0: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-000004c0: 5a61 6262 6978 2054 7261 7070 6572 2069  Zabbix Trapper i
-000004d0: 7465 6d28 7329 2e0a 0a20 2020 2020 2020  tem(s)...       
-000004e0: 2046 6f72 2063 6c69 656e 7420 6d65 7373   For client mess
-000004f0: 6167 6573 2061 206c 6f77 2d6c 6576 656c  ages a low-level
-00000500: 2064 6973 636f 7665 7279 2077 696c 6c20   discovery will 
-00000510: 6265 2073 656e 7420 6669 7273 7420 616e  be sent first an
-00000520: 6420 7468 650a 2020 2020 2020 2020 636f  d the.        co
-00000530: 7272 6573 706f 6e64 696e 6720 5a61 6262  rresponding Zabb
-00000540: 6978 2054 7261 7070 6572 2069 7465 6d28  ix Trapper item(
-00000550: 7329 2077 696c 6c20 6265 2064 656c 6179  s) will be delay
-00000560: 6564 2075 6e74 696c 205a 6162 6269 7820  ed until Zabbix 
-00000570: 6861 7665 2062 6565 6e0a 2020 2020 2020  have been.      
-00000580: 2020 6769 7665 6e20 7469 6d65 2074 6f20    given time to 
-00000590: 7379 6e63 6872 6f6e 697a 6520 6361 6368  synchronize cach
-000005a0: 6573 2e0a 0a20 2020 2020 2020 2049 6620  es...        If 
-000005b0: 7468 6520 6d65 7373 6167 6520 6973 204e  the message is N
-000005c0: 6f6e 652c 2074 6865 6e20 7468 6973 206d  one, then this m
-000005d0: 6574 686f 6420 7265 7475 726e 7320 696d  ethod returns im
-000005e0: 6d65 6469 6174 656c 792e 0a0a 2020 2020  mediately...    
-000005f0: 2020 2020 3a70 6172 616d 2072 6563 6f72      :param recor
-00000600: 643a 2054 6865 206c 6f67 2072 6563 6f72  d: The log recor
-00000610: 6420 636f 6e74 6169 6e69 6e67 2068 6f73  d containing hos
-00000620: 746e 616d 652c 2070 726f 6365 7373 206e  tname, process n
-00000630: 616d 6520 616e 6420 7469 6d65 7374 616d  ame and timestam
-00000640: 702e 0a20 2020 2020 2020 203a 7061 7261  p..        :para
-00000650: 6d20 6d65 7373 6167 653a 2054 6865 206d  m message: The m
-00000660: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
-00000670: 6720 7468 6520 6d61 6320 6164 6472 6573  g the mac addres
-00000680: 732e 0a20 2020 2020 2020 204e 7201 0000  s..        Nr...
-00000690: 007a 3750 656e 6469 6e67 2064 6973 636f  .z7Pending disco
-000006a0: 7665 7279 2065 7665 6e74 206f 6620 2573  very event of %s
-000006b0: 206f 6e20 2573 2e20 5761 6974 696e 6720   on %s. Waiting 
-000006c0: 2566 2073 6563 6f6e 6473 5446 7a10 5365  %f secondsTFz.Se
-000006d0: 6e64 696e 6720 6461 7461 3a20 2572 fa0c  nding data: %r..
-000006e0: 5265 7370 6f6e 7365 3a20 2572 2913 da0f  Response: %r)...
-000006f0: 6469 7363 6f76 6572 5f63 6c69 656e 74da  discover_client.
-00000700: 076c 6f67 6769 6e67 da06 6c6f 6767 6572  .logging..logger
-00000710: da05 6465 6275 67da 0b6d 6163 5f61 6464  ..debug..mac_add
-00000720: 7265 7373 da07 7072 6f63 6573 73da 0561  ress..process..a
-00000730: 6e79 696f da05 736c 6565 70da 066d 6170  nyio..sleep..map
-00000740: 7065 725a 126d 6170 5f63 6c69 656e 745f  perZ.map_client_
-00000750: 6d65 7373 6167 6572 0f00 0000 da0f 6164  messager......ad
-00000760: 645f 6d65 6173 7572 656d 656e 7472 0c00  d_measurementr..
-00000770: 0000 720b 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000780: 00da 0469 6e66 6f72 0700 0000 da04 7365  ...infor......se
-00000790: 6e64 2907 7210 0000 0072 1600 0000 7217  nd).r....r....r.
-000007a0: 0000 005a 1873 6563 6f6e 6473 5f75 6e74  ...Z.seconds_unt
-000007b0: 696c 5f64 6973 636f 7665 7265 64da 0b6d  il_discovered..m
-000007c0: 6561 7375 7265 6d65 6e74 da0c 6d65 6173  easurement..meas
-000007d0: 7572 656d 656e 7473 da08 7265 7370 6f6e  urements..respon
-000007e0: 7365 7214 0000 0072 1400 0000 7215 0000  ser....r....r...
-000007f0: 0072 2500 0000 2600 0000 732e 0000 0000  .r%...&...s.....
-00000800: 0e08 0104 0112 0108 0206 0102 0104 0104  ................
-00000810: 0102 fc04 0610 0210 010e 0206 0304 0306  ................
-00000820: 0112 0506 0106 010a 020e 0112 017a 125a  .............z.Z
-00000830: 6162 6269 7854 7261 7070 6572 2e73 656e  abbixTrapper.sen
-00000840: 6463 0300 0000 0000 0000 0000 0000 0500  dc..............
-00000850: 0000 0400 0000 c300 0000 7398 0000 007c  ..........s....|
-00000860: 016a 0064 016b 0973 0e74 0182 017c 006a  .j.d.k.s.t...|.j
-00000870: 02a0 037c 016a 007c 026a 04a1 0272 327c  ...|.j.|.j...r2|
-00000880: 006a 02a0 057c 016a 007c 026a 04a1 0253  .j...|.j.|.j...S
-00000890: 007c 006a 02a0 067c 016a 007c 026a 04a1  .|.j...|.j.|.j..
-000008a0: 0201 0074 07a0 087c 017c 006a 02a1 027d  ...t...|.|.j...}
-000008b0: 0374 096a 0aa0 0b64 027c 03a1 0201 007c  .t.j...d.|.....|
-000008c0: 006a 0ca0 0d7c 03a1 0149 0064 0148 007d  .j...|...I.d.H.}
-000008d0: 0474 096a 0aa0 0b64 037c 04a1 0201 007c  .t.j...d.|.....|
-000008e0: 046a 0e64 046b 0273 9274 017c 0483 0182  .j.d.k.s.t.|....
-000008f0: 017c 006a 0f53 0029 0561 3a04 0000 4469  .|.j.S.).a:...Di
-00000900: 7363 6f76 6572 2061 206e 6577 2063 6c69  scover a new cli
-00000910: 656e 7420 6261 7365 6420 6f6e 2074 6865  ent based on the
-00000920: 206d 6163 2061 6464 7265 7373 2069 6e20   mac address in 
-00000930: 7468 6520 6d65 7373 6167 652e 0a0a 2020  the message...  
-00000940: 2020 2020 2020 5468 6572 6520 6172 6520        There are 
-00000950: 7468 7265 6520 6361 7365 7320 6f66 2063  three cases of c
-00000960: 6c69 656e 7420 6469 7363 6f76 6572 793a  lient discovery:
-00000970: 0a20 2020 2020 2020 2031 2920 5468 6520  .        1) The 
-00000980: 636c 6965 6e74 2068 6176 6520 6e6f 7420  client have not 
-00000990: 6265 656e 2064 6973 636f 7665 7265 6420  been discovered 
-000009a0: 6265 666f 7265 0a20 2020 2020 2020 2032  before.        2
-000009b0: 2920 5468 6520 636c 6965 6e74 2068 6176  ) The client hav
-000009c0: 6520 7265 6365 6e74 6c79 2062 6565 6e20  e recently been 
-000009d0: 6469 7363 6f76 6572 6564 0a20 2020 2020  discovered.     
-000009e0: 2020 2033 2920 5468 6520 636c 6965 6e74     3) The client
-000009f0: 2068 6176 6520 6265 656e 2064 6973 636f   have been disco
-00000a00: 7665 7265 6420 666f 7220 6120 6c6f 6e67  vered for a long
-00000a10: 2074 696d 650a 0a20 2020 2020 2020 2041   time..        A
-00000a20: 2064 6973 636f 7665 7279 2070 6163 6b65   discovery packe
-00000a30: 7420 7769 6c6c 206f 6e6c 7920 6265 2073  t will only be s
-00000a40: 656e 7420 746f 205a 6162 6269 7820 696e  ent to Zabbix in
-00000a50: 2074 6865 2066 6972 7374 2063 6173 6520   the first case 
-00000a60: 616e 6420 7468 6520 6361 6c6c 6565 0a20  and the callee. 
-00000a70: 2020 2020 2020 2077 696c 6c20 6265 2069         will be i
-00000a80: 6e73 7472 7563 7465 6420 746f 2077 6169  nstructed to wai
-00000a90: 7420 666f 7220 7468 6520 6675 6c6c 2064  t for the full d
-00000aa0: 6566 6175 6c74 5f77 6169 745f 7469 6d65  efault_wait_time
-00000ab0: 2070 6572 696f 6420 6265 666f 7265 2073   period before s
-00000ac0: 656e 6469 6e67 0a20 2020 2020 2020 2074  ending.        t
-00000ad0: 6865 2061 6374 7561 6c20 6461 7461 2074  he actual data t
-00000ae0: 6f20 5a61 6262 6978 2e20 5468 6973 2065  o Zabbix. This e
-00000af0: 6e73 7572 6573 2074 6861 7420 7468 6520  nsures that the 
-00000b00: 5a61 6262 6978 2054 7261 7070 6572 2070  Zabbix Trapper p
-00000b10: 726f 6365 7373 2069 7320 6177 6172 650a  rocess is aware.
-00000b20: 2020 2020 2020 2020 6f66 2074 6865 2028          of the (
-00000b30: 6e65 776c 7920 6372 6561 7465 6429 2069  newly created) i
-00000b40: 7465 6d20 7072 6f74 6f74 7970 6528 7329  tem prototype(s)
-00000b50: 2e0a 0a20 2020 2020 2020 2049 6620 6120  ...        If a 
-00000b60: 636c 6965 6e74 2068 6176 6520 7265 6365  client have rece
-00000b70: 6e74 6c79 2062 6565 6e20 6469 7363 6f76  ntly been discov
-00000b80: 6572 6564 2074 6865 2063 616c 6c65 6520  ered the callee 
-00000b90: 7769 6c6c 2062 6520 696e 7374 7275 6374  will be instruct
-00000ba0: 6564 2074 6f20 7761 6974 0a20 2020 2020  ed to wait.     
-00000bb0: 2020 2074 6865 2072 656d 6169 6e69 6e67     the remaining
-00000bc0: 2074 696d 6520 6f66 2074 6865 2064 6566   time of the def
-00000bd0: 6175 6c74 5f77 6169 745f 7469 6d65 2062  ault_wait_time b
-00000be0: 6566 6f72 6520 7365 6e64 696e 6720 7468  efore sending th
-00000bf0: 6520 6163 7475 616c 2064 6174 6120 746f  e actual data to
-00000c00: 0a20 2020 2020 2020 205a 6162 6269 782e  .        Zabbix.
-00000c10: 0a0a 2020 2020 2020 2020 466f 7220 7468  ..        For th
-00000c20: 6520 6c61 7374 2063 6173 6520 7468 6520  e last case the 
-00000c30: 6361 6c6c 6565 2077 696c 6c20 6265 2069  callee will be i
-00000c40: 6e73 7472 7563 7465 6420 746f 2077 6169  nstructed to wai
-00000c50: 7420 3020 7365 636f 6e64 732c 2069 2e65  t 0 seconds, i.e
-00000c60: 2e20 7468 6579 2063 616e 0a20 2020 2020  . they can.     
-00000c70: 2020 2073 656e 6420 7468 6520 6461 7461     send the data
-00000c80: 2074 6f20 5a61 6262 6978 2069 6d6d 6564   to Zabbix immed
-00000c90: 6961 7465 6c79 2e0a 0a20 2020 2020 2020  iately...       
-00000ca0: 203a 7061 7261 6d20 7265 636f 7264 3a20   :param record: 
-00000cb0: 5468 6520 6c6f 6720 7265 636f 7264 2063  The log record c
-00000cc0: 6f6e 7461 696e 696e 6720 686f 7374 6e61  ontaining hostna
-00000cd0: 6d65 2c20 7072 6f63 6573 7320 6e61 6d65  me, process name
-00000ce0: 2061 6e64 2074 696d 6573 7461 6d70 2e0a   and timestamp..
-00000cf0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
-00000d00: 6573 7361 6765 3a20 5468 6520 6d65 7373  essage: The mess
-00000d10: 6167 6520 636f 6e74 6169 6e69 6e67 2074  age containing t
-00000d20: 6865 206d 6163 2061 6464 7265 7373 2e0a  he mac address..
-00000d30: 2020 2020 2020 2020 4e7a 0f44 6973 636f          Nz.Disco
-00000d40: 7665 7269 6e67 3a20 2572 7219 0000 00e9  vering: %rr.....
-00000d50: 0100 0000 2910 721f 0000 00da 0e41 7373  ....).r......Ass
-00000d60: 6572 7469 6f6e 4572 726f 7272 0a00 0000  ertionErrorr....
-00000d70: 5a0f 6973 5f63 6c69 656e 745f 6b6e 6f77  Z.is_client_know
-00000d80: 6e72 1e00 0000 5a13 7265 6d61 696e 696e  nr....Z.remainin
-00000d90: 675f 7761 6974 5f74 696d 655a 0a61 6464  g_wait_timeZ.add
-00000da0: 5f63 6c69 656e 7472 2200 0000 5a14 6d61  _clientr"...Z.ma
-00000db0: 705f 636c 6965 6e74 5f64 6973 636f 7665  p_client_discove
-00000dc0: 7279 721b 0000 0072 1c00 0000 7224 0000  ryr....r....r$..
-00000dd0: 0072 0700 0000 7225 0000 00da 0970 726f  .r....r%.....pro
-00000de0: 6365 7373 6564 7208 0000 0029 0572 1000  cessedr....).r..
-00000df0: 0000 7216 0000 0072 1700 0000 7227 0000  ..r....r....r'..
-00000e00: 0072 2800 0000 7214 0000 0072 1400 0000  .r(...r....r....
-00000e10: 7215 0000 0072 1a00 0000 5800 0000 731a  r....r....X...s.
-00000e20: 0000 0000 190e 0112 0306 0104 0004 ff04  ................
-00000e30: 0412 020e 020e 0112 010e 0112 017a 1d5a  .............z.Z
-00000e40: 6162 6269 7854 7261 7070 6572 2e64 6973  abbixTrapper.dis
-00000e50: 636f 7665 725f 636c 6965 6e74 2902 7203  cover_client).r.
-00000e60: 0000 0072 0400 0000 290d da08 5f5f 6e61  ...r....)...__na
-00000e70: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000e80: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7206  ..__qualname__r.
-00000e90: 0000 00da 0664 6f6d 6169 6eda 094c 6f67  .....domain..Log
-00000ea0: 5265 636f 7264 da06 7479 7069 6e67 da08  Record..typing..
-00000eb0: 4f70 7469 6f6e 616c da07 4d65 7373 6167  Optional..Messag
-00000ec0: 6572 2500 0000 da05 666c 6f61 7472 1a00  er%.....floatr..
-00000ed0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00000ee0: 5f72 1400 0000 7214 0000 0072 1200 0000  _r....r....r....
-00000ef0: 7215 0000 0072 0200 0000 1a00 0000 7316  r....r........s.
-00000f00: 0000 0008 0200 0000 ff0e 0c04 000a 0102  ................
-00000f10: fe0c 3304 0004 0102 fe72 0200 0000 2914  ..3......r....).
-00000f20: 7231 0000 0072 2000 0000 720d 0000 005a  r1...r ...r....Z
-00000f30: 1e72 6f75 7465 725f 6c6f 675f 7072 6570  .router_log_prep
-00000f40: 726f 6365 7373 6f72 2e64 6f6d 6169 6e72  rocessor.domainr
-00000f50: 2f00 0000 5a21 726f 7574 6572 5f6c 6f67  /...Z!router_log
-00000f60: 5f70 7265 7072 6f63 6573 736f 722e 686f  _preprocessor.ho
-00000f70: 6f6b 732e 6162 63da 0568 6f6f 6b73 da03  oks.abc..hooks..
-00000f80: 6162 635a 3372 6f75 7465 725f 6c6f 675f  abcZ3router_log_
-00000f90: 7072 6570 726f 6365 7373 6f72 2e68 6f6f  preprocessor.hoo
-00000fa0: 6b73 2e7a 6162 6269 782e 5f6b 6e6f 776e  ks.zabbix._known
-00000fb0: 5f63 6c69 656e 7473 da06 7a61 6262 6978  _clients..zabbix
-00000fc0: 720a 0000 0072 0900 0000 5a2c 726f 7574  r....r....Z,rout
-00000fd0: 6572 5f6c 6f67 5f70 7265 7072 6f63 6573  er_log_preproces
-00000fe0: 736f 722e 686f 6f6b 732e 7a61 6262 6978  sor.hooks.zabbix
-00000ff0: 2e5f 6d61 7070 6572 5a07 5f6d 6170 7065  ._mapperZ._mappe
-00001000: 7272 2200 0000 da24 726f 7574 6572 5f6c  rr"....$router_l
-00001010: 6f67 5f70 7265 7072 6f63 6573 736f 722e  og_preprocessor.
-00001020: 7574 696c 2e6c 6f67 6769 6e67 da04 7574  util.logging..ut
-00001030: 696c 721b 0000 005a 0448 6f6f 6b72 0200  ilr....Z.Hookr..
-00001040: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00001050: 0072 1500 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001060: 0e00 0000 7310 0000 0008 0208 0108 020c  ....s...........
-00001070: 0112 0118 0118 0112 03                   .........
+00000120: 9c03 6409 640a 8404 5a0b 640b 640c 8400  ..d.d...Z.d.d...
+00000130: 5a0c 8700 0400 5a0d 5300 290e da0d 5a61  Z.....Z.S.)...Za
+00000140: 6262 6978 5472 6170 7065 72e9 3200 0000  bbixTrapper.2...
+00000150: e90a 0000 0063 0400 0000 0000 0000 0000  .....c..........
+00000160: 0000 0400 0000 0300 0000 0300 0000 733c  ..............s<
+00000170: 0000 0074 0083 00a0 01a1 0001 007c 017c  ...t.........|.|
+00000180: 005f 027c 027c 005f 0374 04a0 057c 02a1  ._.|.|._.t...|..
+00000190: 017c 005f 067c 037c 005f 0764 017c 005f  .|._.|.|._.d.|._
+000001a0: 0874 09a0 0aa1 007c 005f 0b64 0053 0029  .t.....|._.d.S.)
+000001b0: 024e 4629 0cda 0573 7570 6572 da08 5f5f  .NF)...super..__
+000001c0: 696e 6974 5f5f da07 5f73 656e 6465 72da  init__.._sender.
+000001d0: 1b5f 636c 6965 6e74 5f64 6973 636f 7665  ._client_discove
+000001e0: 7279 5f77 6169 745f 7469 6d65 da0d 6b6e  ry_wait_time..kn
+000001f0: 6f77 6e5f 636c 6965 6e74 735a 0c4b 6e6f  own_clientsZ.Kno
+00000200: 776e 436c 6965 6e74 73da 0e5f 6b6e 6f77  wnClients.._know
+00000210: 6e5f 636c 6965 6e74 73da 1d5f 6d65 6173  n_clients.._meas
+00000220: 7572 656d 656e 745f 6275 6e64 6c65 5f77  urement_bundle_w
+00000230: 6169 745f 7469 6d65 da19 5f69 735f 6275  ait_time.._is_bu
+00000240: 6e64 6c69 6e67 5f6d 6561 7375 7265 6d65  ndling_measureme
+00000250: 6e74 73da 1561 7379 6e63 696f 5f7a 6162  nts..asyncio_zab
+00000260: 6269 785f 7365 6e64 6572 da0c 4d65 6173  bix_sender..Meas
+00000270: 7572 656d 656e 7473 da0d 5f6d 6561 7375  urements.._measu
+00000280: 7265 6d65 6e74 7329 04da 0473 656c 66da  rements)...self.
+00000290: 0673 656e 6465 725a 1a63 6c69 656e 745f  .senderZ.client_
+000002a0: 6469 7363 6f76 6572 795f 7761 6974 5f74  discovery_wait_t
+000002b0: 696d 655a 1c6d 6561 7375 7265 6d65 6e74  imeZ.measurement
+000002c0: 5f62 756e 646c 655f 7761 6974 5f74 696d  _bundle_wait_tim
+000002d0: 65a9 01da 095f 5f63 6c61 7373 5f5f a900  e....__class__..
+000002e0: fa6a 2f68 6f6d 652f 6d79 732f 446f 6375  .j/home/mys/Docu
+000002f0: 6d65 6e74 732f 4769 7448 7562 2f6d 6173  ments/GitHub/mas
+00000300: 7464 692f 726f 7574 6572 2d6c 6f67 2d70  tdi/router-log-p
+00000310: 7265 7072 6f63 6573 736f 722f 726f 7574  reprocessor/rout
+00000320: 6572 5f6c 6f67 5f70 7265 7072 6f63 6573  er_log_preproces
+00000330: 736f 722f 686f 6f6b 732f 7a61 6262 6978  sor/hooks/zabbix
+00000340: 2f5f 7472 6170 7065 722e 7079 7206 0000  /_trapper.pyr...
+00000350: 001b 0000 0073 0e00 0000 0003 0a01 0601  .....s..........
+00000360: 0601 0c01 0601 0601 7a16 5a61 6262 6978  ........z.Zabbix
+00000370: 5472 6170 7065 722e 5f5f 696e 6974 5f5f  Trapper.__init__
+00000380: 4e29 03da 0672 6563 6f72 64da 076d 6573  N)...record..mes
+00000390: 7361 6765 da06 7265 7475 726e 6303 0000  sage..returnc...
+000003a0: 0000 0000 0000 0000 0005 0000 0006 0000  ................
+000003b0: 00c3 0000 0073 7c00 0000 7c02 6401 6b08  .....s|...|.d.k.
+000003c0: 720c 6401 5300 7c00 a000 7c01 7c02 a102  r.d.S.|...|.|...
+000003d0: 4900 6401 4800 7d03 7c03 6402 6b04 724c  I.d.H.}.|.d.k.rL
+000003e0: 7401 6a02 a003 6403 7c02 6a04 7c01 6a05  t.j...d.|.j.|.j.
+000003f0: 7c03 a104 0100 7406 a007 7c03 a101 4900  |.....t...|...I.
+00000400: 6401 4800 0100 7408 a009 7c01 7c02 a102  d.H...t...|.|...
+00000410: 4400 5d10 7d04 7c00 6a0a a00b 7c04 a101  D.].}.|.j...|...
+00000420: 0100 7158 7c00 a00c a100 4900 6401 4800  ..qX|.....I.d.H.
+00000430: 0100 6401 5300 2904 61fe 0100 0053 656e  ..d.S.).a....Sen
+00000440: 6420 7468 6520 7072 6570 726f 6365 7373  d the preprocess
+00000450: 6564 206d 6573 7361 6765 2074 6f20 7468  ed message to th
+00000460: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
+00000470: 5a61 6262 6978 2054 7261 7070 6572 2069  Zabbix Trapper i
+00000480: 7465 6d28 7329 2e0a 0a20 2020 2020 2020  tem(s)...       
+00000490: 2046 6f72 2063 6c69 656e 7420 6d65 7373   For client mess
+000004a0: 6167 6573 2061 206c 6f77 2d6c 6576 656c  ages a low-level
+000004b0: 2064 6973 636f 7665 7279 2077 696c 6c20   discovery will 
+000004c0: 6265 2073 656e 7420 6669 7273 7420 616e  be sent first an
+000004d0: 6420 7468 650a 2020 2020 2020 2020 636f  d the.        co
+000004e0: 7272 6573 706f 6e64 696e 6720 5a61 6262  rresponding Zabb
+000004f0: 6978 2054 7261 7070 6572 2069 7465 6d28  ix Trapper item(
+00000500: 7329 2077 696c 6c20 6265 2064 656c 6179  s) will be delay
+00000510: 6564 2075 6e74 696c 205a 6162 6269 7820  ed until Zabbix 
+00000520: 6861 7665 2062 6565 6e0a 2020 2020 2020  have been.      
+00000530: 2020 6769 7665 6e20 7469 6d65 2074 6f20    given time to 
+00000540: 7379 6e63 6872 6f6e 697a 6520 6361 6368  synchronize cach
+00000550: 6573 2e0a 0a20 2020 2020 2020 2049 6620  es...        If 
+00000560: 7468 6520 6d65 7373 6167 6520 6973 204e  the message is N
+00000570: 6f6e 652c 2074 6865 6e20 7468 6973 206d  one, then this m
+00000580: 6574 686f 6420 7265 7475 726e 7320 696d  ethod returns im
+00000590: 6d65 6469 6174 656c 792e 0a0a 2020 2020  mediately...    
+000005a0: 2020 2020 3a70 6172 616d 2072 6563 6f72      :param recor
+000005b0: 643a 2054 6865 206c 6f67 2072 6563 6f72  d: The log recor
+000005c0: 6420 636f 6e74 6169 6e69 6e67 2068 6f73  d containing hos
+000005d0: 746e 616d 652c 2070 726f 6365 7373 206e  tname, process n
+000005e0: 616d 6520 616e 6420 7469 6d65 7374 616d  ame and timestam
+000005f0: 702e 0a20 2020 2020 2020 203a 7061 7261  p..        :para
+00000600: 6d20 6d65 7373 6167 653a 2054 6865 206d  m message: The m
+00000610: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
+00000620: 6720 7468 6520 6d61 6320 6164 6472 6573  g the mac addres
+00000630: 732e 0a20 2020 2020 2020 204e 7201 0000  s..        Nr...
+00000640: 007a 3750 656e 6469 6e67 2064 6973 636f  .z7Pending disco
+00000650: 7665 7279 2065 7665 6e74 206f 6620 2573  very event of %s
+00000660: 206f 6e20 2573 2e20 5761 6974 696e 6720   on %s. Waiting 
+00000670: 2566 2073 6563 6f6e 6473 290d da0f 6469  %f seconds)...di
+00000680: 7363 6f76 6572 5f63 6c69 656e 74da 076c  scover_client..l
+00000690: 6f67 6769 6e67 da06 6c6f 6767 6572 da05  ogging..logger..
+000006a0: 6465 6275 67da 0b6d 6163 5f61 6464 7265  debug..mac_addre
+000006b0: 7373 da07 7072 6f63 6573 73da 0561 6e79  ss..process..any
+000006c0: 696f da05 736c 6565 70da 066d 6170 7065  io..sleep..mappe
+000006d0: 725a 126d 6170 5f63 6c69 656e 745f 6d65  rZ.map_client_me
+000006e0: 7373 6167 6572 0f00 0000 da0f 6164 645f  ssager......add_
+000006f0: 6d65 6173 7572 656d 656e 74da 0f5f 7374  measurement.._st
+00000700: 6172 745f 6275 6e64 6c69 6e67 2905 7210  art_bundling).r.
+00000710: 0000 0072 1600 0000 7217 0000 005a 1873  ...r....r....Z.s
+00000720: 6563 6f6e 6473 5f75 6e74 696c 5f64 6973  econds_until_dis
+00000730: 636f 7665 7265 64da 0b6d 6561 7375 7265  covered..measure
+00000740: 6d65 6e74 7214 0000 0072 1400 0000 7215  mentr....r....r.
+00000750: 0000 00da 0473 656e 6426 0000 0073 1c00  .....send&...s..
+00000760: 0000 000e 0801 0401 1201 0802 0601 0201  ................
+00000770: 0401 0401 02fc 0406 1002 1001 0e02 7a12  ..............z.
+00000780: 5a61 6262 6978 5472 6170 7065 722e 7365  ZabbixTrapper.se
+00000790: 6e64 6303 0000 0000 0000 0000 0000 0005  ndc.............
+000007a0: 0000 0004 0000 00c3 0000 0073 9800 0000  ...........s....
+000007b0: 7c01 6a00 6401 6b09 730e 7401 8201 7c00  |.j.d.k.s.t...|.
+000007c0: 6a02 a003 7c01 6a00 7c02 6a04 a102 7232  j...|.j.|.j...r2
+000007d0: 7c00 6a02 a005 7c01 6a00 7c02 6a04 a102  |.j...|.j.|.j...
+000007e0: 5300 7c00 6a02 a006 7c01 6a00 7c02 6a04  S.|.j...|.j.|.j.
+000007f0: a102 0100 7407 a008 7c01 7c00 6a02 a102  ....t...|.|.j...
+00000800: 7d03 7409 6a0a a00b 6402 7c03 a102 0100  }.t.j...d.|.....
+00000810: 7c00 6a0c a00d 7c03 a101 4900 6401 4800  |.j...|...I.d.H.
+00000820: 7d04 7409 6a0a a00b 6403 7c04 a102 0100  }.t.j...d.|.....
+00000830: 7c04 6a0e 6404 6b02 7392 7401 7c04 8301  |.j.d.k.s.t.|...
+00000840: 8201 7c00 6a0f 5300 2905 613a 0400 0044  ..|.j.S.).a:...D
+00000850: 6973 636f 7665 7220 6120 6e65 7720 636c  iscover a new cl
+00000860: 6965 6e74 2062 6173 6564 206f 6e20 7468  ient based on th
+00000870: 6520 6d61 6320 6164 6472 6573 7320 696e  e mac address in
+00000880: 2074 6865 206d 6573 7361 6765 2e0a 0a20   the message... 
+00000890: 2020 2020 2020 2054 6865 7265 2061 7265         There are
+000008a0: 2074 6872 6565 2063 6173 6573 206f 6620   three cases of 
+000008b0: 636c 6965 6e74 2064 6973 636f 7665 7279  client discovery
+000008c0: 3a0a 2020 2020 2020 2020 3129 2054 6865  :.        1) The
+000008d0: 2063 6c69 656e 7420 6861 7665 206e 6f74   client have not
+000008e0: 2062 6565 6e20 6469 7363 6f76 6572 6564   been discovered
+000008f0: 2062 6566 6f72 650a 2020 2020 2020 2020   before.        
+00000900: 3229 2054 6865 2063 6c69 656e 7420 6861  2) The client ha
+00000910: 7665 2072 6563 656e 746c 7920 6265 656e  ve recently been
+00000920: 2064 6973 636f 7665 7265 640a 2020 2020   discovered.    
+00000930: 2020 2020 3329 2054 6865 2063 6c69 656e      3) The clien
+00000940: 7420 6861 7665 2062 6565 6e20 6469 7363  t have been disc
+00000950: 6f76 6572 6564 2066 6f72 2061 206c 6f6e  overed for a lon
+00000960: 6720 7469 6d65 0a0a 2020 2020 2020 2020  g time..        
+00000970: 4120 6469 7363 6f76 6572 7920 7061 636b  A discovery pack
+00000980: 6574 2077 696c 6c20 6f6e 6c79 2062 6520  et will only be 
+00000990: 7365 6e74 2074 6f20 5a61 6262 6978 2069  sent to Zabbix i
+000009a0: 6e20 7468 6520 6669 7273 7420 6361 7365  n the first case
+000009b0: 2061 6e64 2074 6865 2063 616c 6c65 650a   and the callee.
+000009c0: 2020 2020 2020 2020 7769 6c6c 2062 6520          will be 
+000009d0: 696e 7374 7275 6374 6564 2074 6f20 7761  instructed to wa
+000009e0: 6974 2066 6f72 2074 6865 2066 756c 6c20  it for the full 
+000009f0: 6465 6661 756c 745f 7761 6974 5f74 696d  default_wait_tim
+00000a00: 6520 7065 7269 6f64 2062 6566 6f72 6520  e period before 
+00000a10: 7365 6e64 696e 670a 2020 2020 2020 2020  sending.        
+00000a20: 7468 6520 6163 7475 616c 2064 6174 6120  the actual data 
+00000a30: 746f 205a 6162 6269 782e 2054 6869 7320  to Zabbix. This 
+00000a40: 656e 7375 7265 7320 7468 6174 2074 6865  ensures that the
+00000a50: 205a 6162 6269 7820 5472 6170 7065 7220   Zabbix Trapper 
+00000a60: 7072 6f63 6573 7320 6973 2061 7761 7265  process is aware
+00000a70: 0a20 2020 2020 2020 206f 6620 7468 6520  .        of the 
+00000a80: 286e 6577 6c79 2063 7265 6174 6564 2920  (newly created) 
+00000a90: 6974 656d 2070 726f 746f 7479 7065 2873  item prototype(s
+00000aa0: 292e 0a0a 2020 2020 2020 2020 4966 2061  )...        If a
+00000ab0: 2063 6c69 656e 7420 6861 7665 2072 6563   client have rec
+00000ac0: 656e 746c 7920 6265 656e 2064 6973 636f  ently been disco
+00000ad0: 7665 7265 6420 7468 6520 6361 6c6c 6565  vered the callee
+00000ae0: 2077 696c 6c20 6265 2069 6e73 7472 7563   will be instruc
+00000af0: 7465 6420 746f 2077 6169 740a 2020 2020  ted to wait.    
+00000b00: 2020 2020 7468 6520 7265 6d61 696e 696e      the remainin
+00000b10: 6720 7469 6d65 206f 6620 7468 6520 6465  g time of the de
+00000b20: 6661 756c 745f 7761 6974 5f74 696d 6520  fault_wait_time 
+00000b30: 6265 666f 7265 2073 656e 6469 6e67 2074  before sending t
+00000b40: 6865 2061 6374 7561 6c20 6461 7461 2074  he actual data t
+00000b50: 6f0a 2020 2020 2020 2020 5a61 6262 6978  o.        Zabbix
+00000b60: 2e0a 0a20 2020 2020 2020 2046 6f72 2074  ...        For t
+00000b70: 6865 206c 6173 7420 6361 7365 2074 6865  he last case the
+00000b80: 2063 616c 6c65 6520 7769 6c6c 2062 6520   callee will be 
+00000b90: 696e 7374 7275 6374 6564 2074 6f20 7761  instructed to wa
+00000ba0: 6974 2030 2073 6563 6f6e 6473 2c20 692e  it 0 seconds, i.
+00000bb0: 652e 2074 6865 7920 6361 6e0a 2020 2020  e. they can.    
+00000bc0: 2020 2020 7365 6e64 2074 6865 2064 6174      send the dat
+00000bd0: 6120 746f 205a 6162 6269 7820 696d 6d65  a to Zabbix imme
+00000be0: 6469 6174 656c 792e 0a0a 2020 2020 2020  diately...      
+00000bf0: 2020 3a70 6172 616d 2072 6563 6f72 643a    :param record:
+00000c00: 2054 6865 206c 6f67 2072 6563 6f72 6420   The log record 
+00000c10: 636f 6e74 6169 6e69 6e67 2068 6f73 746e  containing hostn
+00000c20: 616d 652c 2070 726f 6365 7373 206e 616d  ame, process nam
+00000c30: 6520 616e 6420 7469 6d65 7374 616d 702e  e and timestamp.
+00000c40: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000c50: 6d65 7373 6167 653a 2054 6865 206d 6573  message: The mes
+00000c60: 7361 6765 2063 6f6e 7461 696e 696e 6720  sage containing 
+00000c70: 7468 6520 6d61 6320 6164 6472 6573 732e  the mac address.
+00000c80: 0a20 2020 2020 2020 204e 7a0f 4469 7363  .        Nz.Disc
+00000c90: 6f76 6572 696e 673a 2025 72fa 0c52 6573  overing: %r..Res
+00000ca0: 706f 6e73 653a 2025 72e9 0100 0000 2910  ponse: %r.....).
+00000cb0: 721e 0000 00da 0e41 7373 6572 7469 6f6e  r......Assertion
+00000cc0: 4572 726f 7272 0a00 0000 5a0f 6973 5f63  Errorr....Z.is_c
+00000cd0: 6c69 656e 745f 6b6e 6f77 6e72 1d00 0000  lient_knownr....
+00000ce0: 5a13 7265 6d61 696e 696e 675f 7761 6974  Z.remaining_wait
+00000cf0: 5f74 696d 655a 0a61 6464 5f63 6c69 656e  _timeZ.add_clien
+00000d00: 7472 2100 0000 5a14 6d61 705f 636c 6965  tr!...Z.map_clie
+00000d10: 6e74 5f64 6973 636f 7665 7279 721a 0000  nt_discoveryr...
+00000d20: 0072 1b00 0000 da04 696e 666f 7207 0000  .r......infor...
+00000d30: 0072 2500 0000 da09 7072 6f63 6573 7365  .r%.....processe
+00000d40: 6472 0800 0000 2905 7210 0000 0072 1600  dr....).r....r..
+00000d50: 0000 7217 0000 00da 0c6d 6561 7375 7265  ..r......measure
+00000d60: 6d65 6e74 73da 0872 6573 706f 6e73 6572  ments..responser
+00000d70: 1400 0000 7214 0000 0072 1500 0000 7219  ....r....r....r.
+00000d80: 0000 0046 0000 0073 1a00 0000 0019 0e01  ...F...s........
+00000d90: 1203 0601 0400 04ff 0404 1202 0e02 0e01  ................
+00000da0: 1201 0e01 1201 7a1d 5a61 6262 6978 5472  ......z.ZabbixTr
+00000db0: 6170 7065 722e 6469 7363 6f76 6572 5f63  apper.discover_c
+00000dc0: 6c69 656e 7463 0100 0000 0000 0000 0000  lientc..........
+00000dd0: 0000 0500 0000 0a00 0000 c300 0000 73c4  ..............s.
+00000de0: 0000 007c 006a 0072 0a64 0153 0064 027c  ...|.j.r.d.S.d.|
+00000df0: 005f 0074 01a0 027c 006a 03a1 0149 0064  ._.t...|.j...I.d
+00000e00: 0148 0001 0064 037c 005f 007c 006a 047d  .H...d.|._.|.j.}
+00000e10: 0174 05a0 06a1 007c 005f 047a 3274 076a  .t.....|._.z2t.j
+00000e20: 08a0 0964 047c 01a1 0201 007c 006a 0aa0  ...d.|.....|.j..
+00000e30: 0b7c 01a1 0149 0064 0148 007d 0274 076a  .|...I.d.H.}.t.j
+00000e40: 08a0 0964 057c 02a1 0201 0057 006e 5404  ...d.|.....W.nT.
+00000e50: 0074 0c6b 0a72 be01 007d 0301 007a 3674  .t.k.r...}...z6t
+00000e60: 076a 08a0 0d64 067c 03a1 0201 007c 0144  .j...d.|.....|.D
+00000e70: 005d 107d 047c 006a 04a0 0e7c 04a1 0101  .].}.|.j...|....
+00000e80: 0071 8e7c 00a0 0fa1 0049 0064 0148 0001  .q.|.....I.d.H..
+00000e90: 0057 0035 0064 017d 037e 0358 0059 006e  .W.5.d.}.~.X.Y.n
+00000ea0: 0258 0064 0153 0029 0761 bb01 0000 456e  .X.d.S.).a....En
+00000eb0: 7375 7265 2074 6861 7420 6275 6e64 6c69  sure that bundli
+00000ec0: 6e67 206f 6620 6d65 6173 7572 656d 656e  ng of measuremen
+00000ed0: 7473 2068 6173 2073 7461 7274 6564 2e0a  ts has started..
+00000ee0: 0a20 2020 2020 2020 2049 6620 616e 6f74  .        If anot
+00000ef0: 6865 7220 7072 6f63 6573 7320 616c 7265  her process alre
+00000f00: 6164 7920 7374 6172 7465 6420 7468 6520  ady started the 
+00000f10: 6275 6e64 6c69 6e67 206f 6620 6d65 6173  bundling of meas
+00000f20: 7572 656d 656e 7473 2c20 7468 656e 206e  urements, then n
+00000f30: 6f74 6869 6e67 0a20 2020 2020 2020 2066  othing.        f
+00000f40: 7572 7468 6572 2069 7320 646f 6e65 2e20  urther is done. 
+00000f50: 4f74 6865 7277 6973 652c 2074 6869 7320  Otherwise, this 
+00000f60: 7769 6c6c 2074 616b 6520 7265 7370 6f6e  will take respon
+00000f70: 7369 6269 6c69 7479 206f 6620 626f 7468  sibility of both
+00000f80: 2062 756e 646c 696e 6720 7468 650a 2020   bundling the.  
+00000f90: 2020 2020 2020 6d65 6173 7572 656d 656e        measuremen
+00000fa0: 7473 2061 6e64 2073 656e 6469 6e67 2074  ts and sending t
+00000fb0: 6865 206d 6561 7375 7265 6d65 6e74 7320  he measurements 
+00000fc0: 746f 205a 6162 6269 7820 6166 7465 7220  to Zabbix after 
+00000fd0: 7468 650a 2020 2020 2020 2020 606d 6561  the.        `mea
+00000fe0: 7375 7265 6d65 6e74 5f62 756e 646c 655f  surement_bundle_
+00000ff0: 7761 6974 5f74 696d 6560 2068 6173 2065  wait_time` has e
+00001000: 6c61 7073 6564 2e0a 0a20 2020 2020 2020  lapsed...       
+00001010: 2049 6620 7468 6520 7365 6e64 696e 6720   If the sending 
+00001020: 6f66 206d 6561 7375 7265 6d65 6e74 7320  of measurements 
+00001030: 6661 696c 732c 2074 6865 6e20 7468 6520  fails, then the 
+00001040: 7072 6f63 6573 7320 6973 2072 6574 7269  process is retri
+00001050: 6564 2069 6e64 6566 696e 6974 656c 792e  ed indefinitely.
+00001060: 0a20 2020 2020 2020 204e 5446 7a10 5365  .        NTFz.Se
+00001070: 6e64 696e 6720 6461 7461 3a20 2572 7226  nding data: %rr&
+00001080: 0000 007a 2543 6f6e 6e65 6374 696f 6e20  ...z%Connection 
+00001090: 6572 726f 7220 746f 205a 6162 6269 7820  error to Zabbix 
+000010a0: 7365 7276 6572 3a20 2572 2910 720c 0000  server: %r).r...
+000010b0: 0072 1f00 0000 7220 0000 0072 0b00 0000  .r....r ...r....
+000010c0: 720f 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+000010d0: 1a00 0000 721b 0000 0072 2900 0000 7207  ....r....r)...r.
+000010e0: 0000 0072 2500 0000 da0f 436f 6e6e 6563  ...r%.....Connec
+000010f0: 7469 6f6e 4572 726f 72da 0777 6172 6e69  tionError..warni
+00001100: 6e67 7222 0000 0072 2300 0000 2905 7210  ngr"...r#...).r.
+00001110: 0000 0072 2b00 0000 722c 0000 005a 1063  ...r+...r,...Z.c
+00001120: 6f6e 6e65 6374 696f 6e5f 6572 726f 7272  onnection_errorr
+00001130: 2400 0000 7214 0000 0072 1400 0000 7215  $...r....r....r.
+00001140: 0000 0072 2300 0000 7100 0000 7326 0000  ...r#...q...s&..
+00001150: 0000 0a06 0304 0306 0112 0506 0106 010a  ................
+00001160: 0202 010e 0112 0112 0110 0106 0102 0102  ................
+00001170: fe04 0508 010e 017a 1d5a 6162 6269 7854  .......z.ZabbixT
+00001180: 7261 7070 6572 2e5f 7374 6172 745f 6275  rapper._start_bu
+00001190: 6e64 6c69 6e67 2902 7203 0000 0072 0400  ndling).r....r..
+000011a0: 0000 290e da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+000011b0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000011c0: 616c 6e61 6d65 5f5f 7206 0000 00da 0664  alname__r......d
+000011d0: 6f6d 6169 6eda 094c 6f67 5265 636f 7264  omain..LogRecord
+000011e0: da06 7479 7069 6e67 da08 4f70 7469 6f6e  ..typing..Option
+000011f0: 616c da07 4d65 7373 6167 6572 2500 0000  al..Messager%...
+00001200: da05 666c 6f61 7472 1900 0000 7223 0000  ..floatr....r#..
+00001210: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00001220: 7214 0000 0072 1400 0000 7212 0000 0072  r....r....r....r
+00001230: 1500 0000 7202 0000 001a 0000 0073 1800  ....r........s..
+00001240: 0000 0802 0000 00ff 0e0c 0400 0a01 02fe  ................
+00001250: 0c21 0400 0401 02fe 0c2b 7202 0000 0029  .!.......+r....)
+00001260: 1472 3400 0000 721f 0000 0072 0d00 0000  .r4...r....r....
+00001270: 5a1e 726f 7574 6572 5f6c 6f67 5f70 7265  Z.router_log_pre
+00001280: 7072 6f63 6573 736f 722e 646f 6d61 696e  processor.domain
+00001290: 7232 0000 005a 2172 6f75 7465 725f 6c6f  r2...Z!router_lo
+000012a0: 675f 7072 6570 726f 6365 7373 6f72 2e68  g_preprocessor.h
+000012b0: 6f6f 6b73 2e61 6263 da05 686f 6f6b 73da  ooks.abc..hooks.
+000012c0: 0361 6263 5a33 726f 7574 6572 5f6c 6f67  .abcZ3router_log
+000012d0: 5f70 7265 7072 6f63 6573 736f 722e 686f  _preprocessor.ho
+000012e0: 6f6b 732e 7a61 6262 6978 2e5f 6b6e 6f77  oks.zabbix._know
+000012f0: 6e5f 636c 6965 6e74 73da 067a 6162 6269  n_clients..zabbi
+00001300: 7872 0a00 0000 7209 0000 005a 2c72 6f75  xr....r....Z,rou
+00001310: 7465 725f 6c6f 675f 7072 6570 726f 6365  ter_log_preproce
+00001320: 7373 6f72 2e68 6f6f 6b73 2e7a 6162 6269  ssor.hooks.zabbi
+00001330: 782e 5f6d 6170 7065 725a 075f 6d61 7070  x._mapperZ._mapp
+00001340: 6572 7221 0000 00da 2472 6f75 7465 725f  err!....$router_
+00001350: 6c6f 675f 7072 6570 726f 6365 7373 6f72  log_preprocessor
+00001360: 2e75 7469 6c2e 6c6f 6767 696e 67da 0475  .util.logging..u
+00001370: 7469 6c72 1a00 0000 5a04 486f 6f6b 7202  tilr....Z.Hookr.
+00001380: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
+00001390: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000013a0: 3e0e 0000 0073 1000 0000 0802 0801 0802  >....s..........
+000013b0: 0c01 1201 1801 1801 1203                 ..........
```

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_known_clients.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/_known_clients.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_mapper.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/_mapper.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_trapper.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/hooks/zabbix/_trapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,33 +61,15 @@
                 seconds_until_discovered,
             )
             await anyio.sleep(seconds_until_discovered)
 
         for measurement in mapper.map_client_message(record, message):
             self._measurements.add_measurement(measurement)
 
-        if self._is_bundling_measurements:
-            # This process is done and have handed over the responsibility to send the
-            # measurements to another process
-            return
-
-        # Allow other processes to add measurements while this process sleeps
-        self._is_bundling_measurements = True
-        await anyio.sleep(self._measurement_bundle_wait_time)
-
-        # Get the measurements and prepare an empty measurement container
-        # Once control is handed back to this process we have control of the
-        # measurements until the next await statement
-        self._is_bundling_measurements = False
-        measurements = self._measurements
-        self._measurements = asyncio_zabbix_sender.Measurements()
-
-        logging.logger.info("Sending data: %r", measurements)
-        response = await self._sender.send(measurements)
-        logging.logger.info("Response: %r", response)
+        await self._start_bundling()
 
     async def discover_client(
         self, record: domain.LogRecord, message: domain.Message
     ) -> float:
         """Discover a new client based on the mac address in the message.
 
         There are three cases of client discovery:
@@ -123,7 +105,47 @@
         measurements = mapper.map_client_discovery(record, self._known_clients)
 
         logging.logger.info("Discovering: %r", measurements)
         response = await self._sender.send(measurements)
         logging.logger.info("Response: %r", response)
         assert response.processed == 1, response
         return self._client_discovery_wait_time
+
+    async def _start_bundling(self):
+        """Ensure that bundling of measurements has started.
+
+        If another process already started the bundling of measurements, then nothing
+        further is done. Otherwise, this will take responsibility of both bundling the
+        measurements and sending the measurements to Zabbix after the
+        `measurement_bundle_wait_time` has elapsed.
+
+        If the sending of measurements fails, then the process is retried indefinitely.
+        """
+        if self._is_bundling_measurements:
+            # This process is done and have handed over the responsibility to send the
+            # measurements to another process
+            return
+
+            # Allow other processes to add measurements while this process sleeps
+        self._is_bundling_measurements = True
+        await anyio.sleep(self._measurement_bundle_wait_time)
+
+        # Get the measurements and prepare an empty measurement container
+        # Once control is handed back to this process we have control of the
+        # measurements until the next await statement
+        self._is_bundling_measurements = False
+        measurements = self._measurements
+        self._measurements = asyncio_zabbix_sender.Measurements()
+
+        try:
+            logging.logger.info("Sending data: %r", measurements)
+            response = await self._sender.send(measurements)
+            logging.logger.info("Response: %r", response)
+        except ConnectionError as connection_error:
+            logging.logger.warning(
+                "Connection error to Zabbix server: %r",
+                connection_error
+            )
+            # Add the failed measurements and retry
+            for measurement in measurements:
+                self._measurements.add_measurement(measurement)
+            await self._start_bundling()
```

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__init__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/handler.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/handler.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/server.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/log_server/server.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__init__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/typing.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/typing.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/wlc.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/preprocessors/wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/settings.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/settings.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/util/__init__.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc` & `router_log_preprocessor-0.1.6/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Apr 17 19:09:23 2023 UTC, .py size: 3694 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6399 3d64 6e0e 0000  U.......c.=dn...
+00000000: 550d 0d0a 0000 0000 709b 3d64 140f 0000  U.......p.=d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6502 a005 6403 a101 5a06 6404 6405  ..e...d...Z.d.d.
 00000060: 6406 6407 6408 6409 640a 640b 640c 640d  d.d.d.d.d.d.d.d.
 00000070: 640e 640f 6410 9c0c 5a07 6500 6a08 4700  d.d.d...Z.e.j.G.
@@ -177,15 +177,15 @@
 00000b00: 6469 766d 6f64 7227 0000 0072 1b00 0000  divmodr'...r....
 00000b10: 7237 0000 00da 036c 656e da06 6c73 7472  r7.....len..lstr
 00000b20: 6970 2905 7238 0000 0072 3a00 0000 723c  ip).r8...r:...r<
 00000b30: 0000 0072 1c00 0000 721d 0000 0072 2b00  ...r....r....r+.
 00000b40: 0000 722b 0000 0072 2c00 0000 da05 7061  ..r+...r,.....pa
 00000b50: 7273 655e 0000 0073 1c00 0000 000a 0a01  rse^...s........
 00000b60: 0801 0e01 0802 1601 0201 0201 0201 0e01  ................
-00000b70: 0601 1e01 1a01 06f9 7240 0000 0029 0dda  ........r@...)..
+00000b70: 0603 1e01 1a01 06f7 7240 0000 0029 0dda  ........r@...)..
 00000b80: 0b64 6174 6163 6c61 7373 6573 7229 0000  .dataclassesr)..
 00000b90: 00da 0272 65da 0674 7970 696e 6772 0200  ...re..typingr..
 00000ba0: 0000 da07 636f 6d70 696c 6572 3900 0000  ....compiler9...
 00000bb0: 7236 0000 00da 0964 6174 6163 6c61 7373  r6.....dataclass
 00000bc0: 721b 0000 0072 2a00 0000 7237 0000 0072  r....r*...r7...r
 00000bd0: 4000 0000 722b 0000 0072 2b00 0000 722b  @...r+...r+...r+
 00000be0: 0000 0072 2c00 0000 da08 3c6d 6f64 756c  ...r,.....<modul
```

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/util/logging.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/util/logging.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/router_log_preprocessor/util/rfc3164_parser.py` & `router_log_preprocessor-0.1.6/router_log_preprocessor/util/rfc3164_parser.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.5/setup.py` & `router_log_preprocessor-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 entry_points = \
 {'console_scripts': ['router-log-preprocessor = '
                      'router_log_preprocessor.__main__:main']}
 
 setup_kwargs = {
     'name': 'router-log-preprocessor',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': '# Router Log Preprocessor\n![router-log-preprocessor](https://user-images.githubusercontent.com/105678820/228938795-66dbd955-813b-4fb3-a559-4f3a41f55bb9.png)\n\n> Garbage in, garbage out\n>\n> &mdash; <cite>George Fuechsel</cite>\n\nPreprocessors upcycle garbage input data into well-structured data to ensure reliable and accurate event handling in third-party systems such as Zabbix.\nBy parsing and filtering the input log data, the preprocessor helps to ensure that only high-quality data are sent for further analysis and alerting.\nThis helps to minimize false positives and ensure that network administrators receive reliable and actionable alerts about potential security threats or other issues.\n\n\nKey features:\n- **Wireless LAN Controller event** log entries are parsed to tangible enumerations\n- **DNSMASQ DHCP** log entries are parsed to catch which IP a given client is assigned to\n- **Zabbix** templates are included to ensure that the logs are can lead to actionable alerts\n- **Extendable** preprocessors and hooks to ensure future reliable information to network administrators\n\n## Installation\n```console\n$ pip install router-log-preprocessor\n```\n\nIf needed it can also be installed from sources.\nRequires [Poetry 1.3.2](https://python-poetry.org/).\n```console\n$ git pull https://github.com/mastdi/router-log-preprocessor.git\n$ cd router-log-preprocessor\n$ poetry install\n```\n\n## Usage\nInstalling the package using pip also creates the executable script named `router-log-preprocessor`.\nOn Linux systems the router log preprocessor can be run by\n\n```console\n./router-log-preprocessor\n```\n\nThe configuration solely happens through environment variables or a `.env` configuration file located in the current working directory.\nThe most important variables are documented below. \nA full sample can be found in [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env).\nThe application reads, in order of the least priority to the highest file:\n1. `.env`,\n2. `.env.dev`,\n3. `.env.test`,\n4. `.env.staging`,\n5. `.env.prod`,\n\nmeaning that values stored in `.env.prod` will overwrite any values from other dovenv files.\nParameters stored in environment variables will always take priority over values loaded from a dotenv file.\n\n```dotenv\n# Purpose: Specifies the IP address or hostname of the local interface to which the\n# logging system should bind.\n# Format: A string containing a valid IP address or hostname, such as "192.168.0.1" or\n# "example.com".\nLOG_SERVER_HOST="0.0.0.0"\n\n# Purpose: Specifies the port number of the server to which log data should be sent.\n# Format: An integer representing a valid port number, such as 514.\nLOG_SERVER_PORT=8514\n\n# Purpose: Specifies the hostname or IP address of the Zabbix server to which the\n# Zabbix Sender should send monitoring data.\n# Format: A string containing a valid hostname or IP address, such as "example.com" or\n# "192.168.0.1".\nZABBIX_HOST="example.com"\n\n# Purpose: Specifies the port number on which the Zabbix server is running and to\n# which the Zabbix Sender should send monitoring data.\n# Format: An integer representing a valid port number, such as 10051.\nZABBIX_PORT=10051\n```\n\n## As a service\n\nThis part will go through the steps to set up the Router Log Preprocessor as a service on Ubuntu.\nThe following steps will be explained in details below:\n\n- Create a service user\n- Create a virtual environment\n- Configure environment variables\n- Set up the logging directory\n- Create the service file\n- Start the service and check its status\n- Debugging the service using journalctl\n\n### Prerequisites\n\nTo install and set up the Router Log Preprocessor as a service on Ubuntu, you will need:\n\n- Python 3.8 installed or higher\n- `venv` package (can be installed via `apt-get install python3-venv` command)\n- `pip` package manager (should be included after activating the virtual environment)\n- Internet connection to download the Router Log Preprocessor package from PyPI and the `.env` file from the GitHub repository\n\nNote that some of these prerequisites may already be installed on your Ubuntu system.\nYou can check if Python and pip are installed by running the following commands:\n\n```console\npython3 --version\npip --version\n```\n\nIf both of these commands return the version number of Python and pip, respectively, you\'re good to go.\nOtherwise, you will need to install Python and pip on your Ubuntu system before proceeding.\n\n### Creating a service user\n\nFirst, we will create a service user to run the Router Log Preprocessor.\nThis is a good security practice as running the script as a root user is not needed.\n\nRun the following commands to create a new user called `rlp`:\n\n```console\nsudo adduser rlp --disabled-password --gecos ""\nsudo su rlp\ncd ~\n```\n\nThe first command creates a new user called `rlp` with a disabled password and no additional information. \nThe second command switches to the new user and moves to their home directory.\n\n### Creating a virtual environment\n\nNow that we have a service user set up, we can create a virtual environment to install the Router Log Preprocessor.\nThe following commands create a virtual environment using Python 3.8 and install the Router Log Preprocessor package:\n\n```console\npython3 -m venv venv\ncd venv\nsource bin/activate\npip install router-log-preprocessor\n```\n\nThese commands create a new virtual environment in the venv directory, activate the environment, and install the Router Log Preprocessor package.\n\n### Configuring the environment variables \nWe will create a .env file in the virtual environment directory to store these variables.\nYou can copy the default [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env) file from the Router Log Preprocessor repository and customize it according to your needs:\n```console\ncurl -o .env https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env\nnano .env\n```\nThis will download the .env file from the Router Log Preprocessor repository and open it in the Nano text editor. \nCustomize the file to set the environment variables you need.\n\nWe are done setting up the servie user:\n\n```console\nexit\n```\n\n### Setting up the logging directory\n\nIf you have set the `LOGGING_DIRECTORY` variable in the .env file to `/var/log/rlp`, you need to create the directory and set the ownership to the rlp user:\n\n```console\nsudo mkdir /var/log/rlp\nsudo chown rlp:rlp /var/log/rlp\n```\n\nThese commands will create the `/var/log/rlp` directory and set the ownership to the `rlp` user.\n\n### Creating the service file\n\nThe next step is to create a service file for the Router Log Preprocessor.\nThis file specifies how the service should be started and managed by the system.\nCreate a new file called rlp.service in the /etc/systemd/system/ directory using the following command:\n\n```console\nsudo nano /etc/systemd/system/rlp.service\n```\n\nThis will open the text editor with a new file.\nCopy the following text into the file:\n\n```ini\n[Unit]\nDescription=Router Log Preprocessor service\nAfter=network.target\n\n[Service]\nUser=rlp\nWorkingDirectory=/home/rlp/venv\nEnvironment="PATH=/home/rlp/venv/bin"\nEnvironmentFile=/home/rlp/venv/.env\nExecStart=/home/rlp/venv/bin/router-log-preprocessor\nRestart=on-failure\nRestartSec=5s\nStartLimitInterval=60s\nStartLimitBurst=3\n\n[Install]\nWantedBy=multi-user.target\n```\n\n\n### Starting the service\n\nThe service is now ready to be started.\nThe final step is to start the service, check if it is running, and ensuring that the service starts automatically on system boot.\nStart the service using the following command:\n```console\nsudo systemctl start rlp.service\n```\n\nThis starts the service based on the configuration we just provided.\nCheck that the service is started using the following command:\n\n```console\nsudo systemctl status rlp.service\n```\n\nThis should show `active (running)` in the console.\nTo make sure the service is started on system boot use the following command:\n\n```console\nsudo systemctl enable rlp.service \n```\n\n### Debugging the service creation\n\nTo debug any issues with the service, you can use the `journalctl` command.\nFor example, to view the logs of the `rlp` service, run the following command:\n\n```console\nsudo journalctl -u rlp.service -e\n```\n\nThis will show the logs of the `rlp` service and the `-e` flag will show the end of the logs.\nYou can use other flags like `-f` to follow the logs in real-time, `-n` to specify the number of lines to show, and `-r` to show the logs in reverse order (most recent first).\n\nIf the service crashes, you can also use the `--since` and `--until` flags to show the logs between a specific time range.\nFor example, to show the logs of the last 10 minutes, run the following command:\n\n```console\nsudo journalctl -u rlp.service --since "10 minutes ago"\n```\nThis will show the logs of the `rlp` service that were generated in the last 10 minutes.\nUse this command to debug any issues with the service.',
     'author': 'Martin Storgaard Dieu',
     'author_email': 'martin@storgaarddieu.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mastdi/router-log-preprocessor',
```

### Comparing `router_log_preprocessor-0.1.5/PKG-INFO` & `router_log_preprocessor-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: router-log-preprocessor
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/mastdi/router-log-preprocessor
 License: Apache-2.0
 Author: Martin Storgaard Dieu
 Author-email: martin@storgaarddieu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

