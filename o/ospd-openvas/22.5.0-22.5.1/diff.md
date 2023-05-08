# Comparing `tmp/ospd_openvas-22.5.0.tar.gz` & `tmp/ospd_openvas-22.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospd_openvas-22.5.0.tar", max compression
+gzip compressed data, was "ospd_openvas-22.5.1.tar", max compression
```

## Comparing `ospd_openvas-22.5.0.tar` & `ospd_openvas-22.5.1.tar`

### file list

```diff
@@ -1,88 +1,86 @@
--rw-r--r--   0        0        0    12468 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    34008 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/COPYING
--rw-r--r--   0        0        0     4883 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/README.md
--rw-r--r--   0        0        0      175 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/config/ospd-openvas.conf
--rw-r--r--   0        0        0      636 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/config/ospd-openvas.service
--rw-r--r--   0        0        0     4972 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/docs/ospd-openvas.8
--rw-r--r--   0        0        0      843 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/__init__.py
--rw-r--r--   0        0        0      844 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/__init__.py
--rw-r--r--   0        0        0    23225 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/command.py
--rw-r--r--   0        0        0     1686 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/initsubclass.py
--rw-r--r--   0        0        0     1130 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/registry.py
--rw-r--r--   0        0        0     1628 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/config.py
--rw-r--r--   0        0        0     5244 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/cvss.py
--rw-r--r--   0        0        0     4889 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/datapickler.py
--rw-r--r--   0        0        0     1835 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/errors.py
--rw-r--r--   0        0        0     3309 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/logger.py
--rw-r--r--   0        0        0     4480 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/main.py
--rw-r--r--   0        0        0     4511 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/misc.py
--rw-r--r--   0        0        0    16214 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/network.py
--rw-r--r--   0        0        0    49500 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/ospd.py
--rw-r--r--   0        0        0    10001 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/parser.py
--rw-r--r--   0        0        0    11393 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/protocol.py
--rw-r--r--   0        0        0     3934 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/resultlist.py
--rw-r--r--   0        0        0    21108 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/scan.py
--rw-r--r--   0        0        0     9188 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/server.py
--rw-r--r--   0        0        0     1867 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/timer.py
--rw-r--r--   0        0        0     4746 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/vtfilter.py
--rw-r--r--   0        0        0     6364 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/vts.py
--rw-r--r--   0        0        0     9266 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/xml.py
--rw-r--r--   0        0        0    12704 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/xmlvt.py
--rw-r--r--   0        0        0      804 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/__init__.py
--rw-r--r--   0        0        0      103 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/__version__.py
--rw-r--r--   0        0        0    44291 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/daemon.py
--rw-r--r--   0        0        0    22646 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/db.py
--rw-r--r--   0        0        0     7104 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/dryrun.py
--rw-r--r--   0        0        0      984 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/errors.py
--rw-r--r--   0        0        0     1316 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/feed.py
--rw-r--r--   0        0        0     4500 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/gpg_sha_verifier.py
--rw-r--r--   0        0        0     3939 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/lock.py
--rw-r--r--   0        0        0      737 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messages/__init__.py
--rw-r--r--   0        0        0     2911 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messages/message.py
--rw-r--r--   0        0        0     2888 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messages/result.py
--rw-r--r--   0        0        0      737 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/__init__.py
--rw-r--r--   0        0        0     5989 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/mqtt.py
--rw-r--r--   0        0        0     1099 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/publisher.py
--rw-r--r--   0        0        0     1203 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/subscriber.py
--rw-r--r--   0        0        0     9119 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/notus.py
--rw-r--r--   0        0        0     9770 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/nvticache.py
--rw-r--r--   0        0        0     6199 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/openvas.py
--rw-r--r--   0        0        0    29260 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/preferencehandler.py
--rw-r--r--   0        0        0     9008 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/vthelper.py
--rw-r--r--   0        0        0    71367 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/poetry.toml
--rw-r--r--   0        0        0     2390 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/__init__.py
--rw-r--r--   0        0        0      742 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/__init__.py
--rw-r--r--   0        0        0     2648 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/test_command.py
--rw-r--r--   0        0        0    17645 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/test_commands.py
--rw-r--r--   0        0        0     2045 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/test_registry.py
--rw-r--r--   0        0        0     6173 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/dummydaemon.py
--rw-r--r--   0        0        0     7066 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/helper.py
--rw-r--r--   0        0        0      737 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messages/__init__.py
--rw-r--r--   0        0        0     4824 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messages/test_message.py
--rw-r--r--   0        0        0     6495 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messages/test_result.py
--rw-r--r--   0        0        0      737 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messaging/__init__.py
--rw-r--r--   0        0        0     3343 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messaging/test_mqtt.py
--rw-r--r--   0        0        0     5383 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_argument_parser.py
--rw-r--r--   0        0        0     1629 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_cvss.py
--rw-r--r--   0        0        0    23632 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_daemon.py
--rw-r--r--   0        0        0     4255 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_datapickler.py
--rw-r--r--   0        0        0    25291 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_db.py
--rw-r--r--   0        0        0     2403 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_errors.py
--rw-r--r--   0        0        0     1563 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_feed.py
--rw-r--r--   0        0        0     3481 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_gpg.py
--rw-r--r--   0        0        0     3632 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_lock.py
--rw-r--r--   0        0        0     7461 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_notus.py
--rw-r--r--   0        0        0    11370 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_nvti_cache.py
--rw-r--r--   0        0        0    10912 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_openvas.py
--rw-r--r--   0        0        0    56911 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_port_convert.py
--rw-r--r--   0        0        0    50659 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_preferencehandler.py
--rw-r--r--   0        0        0     1074 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_protocol.py
--rw-r--r--   0        0        0    55036 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_scan_and_result.py
--rw-r--r--   0        0        0     3875 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_target_convert.py
--rw-r--r--   0        0        0    10284 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_vthelper.py
--rw-r--r--   0        0        0     5518 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_vts.py
--rw-r--r--   0        0        0    15018 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_xml.py
--rw-r--r--   0        0        0      373 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/testing.conf
--rw-r--r--   0        0        0     6447 1970-01-01 00:00:00.000000 ospd_openvas-22.5.0/PKG-INFO
+-rw-r--r--   0        0        0    12468 2023-05-08 11:02:34.054608 ospd_openvas-22.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34008 2023-05-08 11:02:34.054608 ospd_openvas-22.5.1/COPYING
+-rw-r--r--   0        0        0     4883 2023-05-08 11:02:34.054608 ospd_openvas-22.5.1/README.md
+-rw-r--r--   0        0        0      175 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/config/ospd-openvas.conf
+-rw-r--r--   0        0        0      636 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/config/ospd-openvas.service
+-rw-r--r--   0        0        0     4972 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/docs/ospd-openvas.8
+-rw-r--r--   0        0        0      843 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/__init__.py
+-rw-r--r--   0        0        0      844 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/__init__.py
+-rw-r--r--   0        0        0    23225 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/command.py
+-rw-r--r--   0        0        0     1686 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/initsubclass.py
+-rw-r--r--   0        0        0     1130 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/registry.py
+-rw-r--r--   0        0        0     1628 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/config.py
+-rw-r--r--   0        0        0     5244 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/cvss.py
+-rw-r--r--   0        0        0     4889 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/datapickler.py
+-rw-r--r--   0        0        0     1835 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/errors.py
+-rw-r--r--   0        0        0     3309 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/logger.py
+-rw-r--r--   0        0        0     4480 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/main.py
+-rw-r--r--   0        0        0     4511 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/misc.py
+-rw-r--r--   0        0        0    16214 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/network.py
+-rw-r--r--   0        0        0    49500 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/ospd.py
+-rw-r--r--   0        0        0    10001 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/parser.py
+-rw-r--r--   0        0        0    11393 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/protocol.py
+-rw-r--r--   0        0        0     3934 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/resultlist.py
+-rw-r--r--   0        0        0    21108 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/scan.py
+-rw-r--r--   0        0        0     9188 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/server.py
+-rw-r--r--   0        0        0     1867 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/timer.py
+-rw-r--r--   0        0        0     4746 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/vtfilter.py
+-rw-r--r--   0        0        0     6364 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/vts.py
+-rw-r--r--   0        0        0     9266 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/xml.py
+-rw-r--r--   0        0        0    12704 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/xmlvt.py
+-rw-r--r--   0        0        0      804 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/__version__.py
+-rw-r--r--   0        0        0    44267 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/daemon.py
+-rw-r--r--   0        0        0    22646 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/db.py
+-rw-r--r--   0        0        0     7104 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/dryrun.py
+-rw-r--r--   0        0        0      984 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/errors.py
+-rw-r--r--   0        0        0     4500 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/gpg_sha_verifier.py
+-rw-r--r--   0        0        0     3939 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/lock.py
+-rw-r--r--   0        0        0      737 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messages/__init__.py
+-rw-r--r--   0        0        0     2911 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messages/message.py
+-rw-r--r--   0        0        0     2888 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messages/result.py
+-rw-r--r--   0        0        0      737 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/__init__.py
+-rw-r--r--   0        0        0     5989 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/mqtt.py
+-rw-r--r--   0        0        0     1099 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/publisher.py
+-rw-r--r--   0        0        0     1203 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/subscriber.py
+-rw-r--r--   0        0        0     9119 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/notus.py
+-rw-r--r--   0        0        0     9770 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/nvticache.py
+-rw-r--r--   0        0        0     6199 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/openvas.py
+-rw-r--r--   0        0        0    29260 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/preferencehandler.py
+-rw-r--r--   0        0        0     9008 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/vthelper.py
+-rw-r--r--   0        0        0    71446 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/poetry.lock
+-rw-r--r--   0        0        0       32 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/poetry.toml
+-rw-r--r--   0        0        0     2390 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/__init__.py
+-rw-r--r--   0        0        0     2648 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/test_command.py
+-rw-r--r--   0        0        0    17645 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/test_commands.py
+-rw-r--r--   0        0        0     2045 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/test_registry.py
+-rw-r--r--   0        0        0     6173 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/dummydaemon.py
+-rw-r--r--   0        0        0     7066 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/helper.py
+-rw-r--r--   0        0        0      737 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messages/__init__.py
+-rw-r--r--   0        0        0     4824 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messages/test_message.py
+-rw-r--r--   0        0        0     6495 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messages/test_result.py
+-rw-r--r--   0        0        0      737 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messaging/__init__.py
+-rw-r--r--   0        0        0     3343 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messaging/test_mqtt.py
+-rw-r--r--   0        0        0     5383 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_argument_parser.py
+-rw-r--r--   0        0        0     1629 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_cvss.py
+-rw-r--r--   0        0        0    23632 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_daemon.py
+-rw-r--r--   0        0        0     4255 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_datapickler.py
+-rw-r--r--   0        0        0    25291 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_db.py
+-rw-r--r--   0        0        0     2403 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_errors.py
+-rw-r--r--   0        0        0     3481 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_gpg.py
+-rw-r--r--   0        0        0     3632 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_lock.py
+-rw-r--r--   0        0        0     7461 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_notus.py
+-rw-r--r--   0        0        0    11370 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_nvti_cache.py
+-rw-r--r--   0        0        0    10912 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_openvas.py
+-rw-r--r--   0        0        0    56927 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_port_convert.py
+-rw-r--r--   0        0        0    50659 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_preferencehandler.py
+-rw-r--r--   0        0        0     1074 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_protocol.py
+-rw-r--r--   0        0        0    55036 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_scan_and_result.py
+-rw-r--r--   0        0        0     3875 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_target_convert.py
+-rw-r--r--   0        0        0    10284 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_vthelper.py
+-rw-r--r--   0        0        0     5518 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_vts.py
+-rw-r--r--   0        0        0    15018 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_xml.py
+-rw-r--r--   0        0        0      373 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/testing.conf
+-rw-r--r--   0        0        0     6447 1970-01-01 00:00:00.000000 ospd_openvas-22.5.1/PKG-INFO
```

### Comparing `ospd_openvas-22.5.0/CHANGELOG.md` & `ospd_openvas-22.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/COPYING` & `ospd_openvas-22.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/README.md` & `ospd_openvas-22.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/config/ospd-openvas.service` & `ospd_openvas-22.5.1/config/ospd-openvas.service`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/docs/ospd-openvas.8` & `ospd_openvas-22.5.1/docs/ospd-openvas.8`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/__init__.py` & `ospd_openvas-22.5.1/ospd/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/command/__init__.py` & `ospd_openvas-22.5.1/ospd/command/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/command/command.py` & `ospd_openvas-22.5.1/ospd/command/command.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/command/initsubclass.py` & `ospd_openvas-22.5.1/ospd/command/initsubclass.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/command/registry.py` & `ospd_openvas-22.5.1/ospd/command/registry.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/config.py` & `ospd_openvas-22.5.1/ospd/config.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/cvss.py` & `ospd_openvas-22.5.1/ospd/cvss.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/datapickler.py` & `ospd_openvas-22.5.1/ospd/datapickler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/errors.py` & `ospd_openvas-22.5.1/ospd/errors.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/logger.py` & `ospd_openvas-22.5.1/ospd/logger.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/main.py` & `ospd_openvas-22.5.1/ospd/main.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/misc.py` & `ospd_openvas-22.5.1/ospd/misc.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/network.py` & `ospd_openvas-22.5.1/ospd/network.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/ospd.py` & `ospd_openvas-22.5.1/ospd/ospd.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/parser.py` & `ospd_openvas-22.5.1/ospd/parser.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/protocol.py` & `ospd_openvas-22.5.1/ospd/protocol.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/resultlist.py` & `ospd_openvas-22.5.1/ospd/resultlist.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/scan.py` & `ospd_openvas-22.5.1/ospd/scan.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/server.py` & `ospd_openvas-22.5.1/ospd/server.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/timer.py` & `ospd_openvas-22.5.1/ospd/timer.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/vtfilter.py` & `ospd_openvas-22.5.1/ospd/vtfilter.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/vts.py` & `ospd_openvas-22.5.1/ospd/vts.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/xml.py` & `ospd_openvas-22.5.1/ospd/xml.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd/xmlvt.py` & `ospd_openvas-22.5.1/ospd/xmlvt.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/__init__.py` & `ospd_openvas-22.5.1/ospd_openvas/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/daemon.py` & `ospd_openvas-22.5.1/ospd_openvas/daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 from ospd_openvas.nvticache import NVTICache
 from ospd_openvas.db import MainDB, BaseDB
 from ospd_openvas.lock import LockFile
 from ospd_openvas.preferencehandler import PreferenceHandler
 from ospd_openvas.openvas import NASLCli, Openvas
 from ospd_openvas.vthelper import VtHelper
 from ospd_openvas.messaging.mqtt import MQTTClient, MQTTDaemon, MQTTSubscriber
-from ospd_openvas.feed import Feed
 
 SENTRY_DSN_OSPD_OPENVAS = environ.get("SENTRY_DSN_OSPD_OPENVAS")
 if SENTRY_DSN_OSPD_OPENVAS:
     # pylint: disable=import-error
     import sentry_sdk
 
     sentry_sdk.init(  # pylint: disable=abstract-class-instantiated
@@ -651,18 +650,18 @@
                 # It is available
                 if fl.has_lock():
                     feed_status["lockfile_in_use"] = '0'
                 # Locked by another process
                 else:
                     feed_status["lockfile_in_use"] = '1'
 
-        feed = Feed()
-        _exit_error, _error_msg = feed.perform_feed_sync_self_test_success()
-        feed_status["self_test_exit_error"] = str(_exit_error)
-        feed_status["self_test_error_msg"] = _error_msg
+        # The feed self test is not performed any more, but the following
+        # entries are kept for backward compatibility.
+        feed_status["self_test_exit_error"] = "0"
+        feed_status["self_test_error_msg"] = None
 
         return feed_status
 
     def update_vts(self):
         """Updates VTs in redis via the openvas-scanner"""
         logger.info(
             "Loading VTs. Scans will be [requested|queued] until VTs are"
```

### Comparing `ospd_openvas-22.5.0/ospd_openvas/db.py` & `ospd_openvas-22.5.1/ospd_openvas/db.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/dryrun.py` & `ospd_openvas-22.5.1/ospd_openvas/dryrun.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/errors.py` & `ospd_openvas-22.5.1/ospd_openvas/errors.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/gpg_sha_verifier.py` & `ospd_openvas-22.5.1/ospd_openvas/gpg_sha_verifier.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/lock.py` & `ospd_openvas-22.5.1/ospd_openvas/lock.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/messages/__init__.py` & `ospd_openvas-22.5.1/ospd_openvas/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/messages/message.py` & `ospd_openvas-22.5.1/ospd_openvas/messages/message.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/messages/result.py` & `ospd_openvas-22.5.1/ospd_openvas/messages/result.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/messaging/__init__.py` & `ospd_openvas-22.5.1/ospd_openvas/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/messaging/mqtt.py` & `ospd_openvas-22.5.1/ospd_openvas/messaging/mqtt.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/messaging/publisher.py` & `ospd_openvas-22.5.1/ospd_openvas/messaging/publisher.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/messaging/subscriber.py` & `ospd_openvas-22.5.1/ospd_openvas/messaging/subscriber.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/notus.py` & `ospd_openvas-22.5.1/ospd_openvas/notus.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/nvticache.py` & `ospd_openvas-22.5.1/ospd_openvas/nvticache.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/openvas.py` & `ospd_openvas-22.5.1/ospd_openvas/openvas.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/preferencehandler.py` & `ospd_openvas-22.5.1/ospd_openvas/preferencehandler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/ospd_openvas/vthelper.py` & `ospd_openvas-22.5.1/ospd_openvas/vthelper.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/poetry.lock` & `ospd_openvas-22.5.1/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -608,22 +608,22 @@
 files = [
     {file = "mypy_extensions-0.4.3-py2.py3-none-any.whl", hash = "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d"},
     {file = "mypy_extensions-0.4.3.tar.gz", hash = "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.0"
+version = "23.1"
 description = "Core utilities for Python packages"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
-    {file = "packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
+    {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
+    {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "paho-mqtt"
 version = "1.6.1"
 description = "MQTT version 5.0/3.1.1 client class"
 category = "main"
@@ -687,34 +687,34 @@
 rich = ">=12.4.4"
 semver = ">=2.13.0,<3.0.0"
 tomlkit = ">=0.5.11"
 typing-extensions = {version = ">=4.4.0,<5.0.0", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "psutil"
-version = "5.9.4"
+version = "5.9.5"
 description = "Cross-platform lib for process and system monitoring in Python."
 category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
-    {file = "psutil-5.9.4-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:c1ca331af862803a42677c120aff8a814a804e09832f166f226bfd22b56feee8"},
-    {file = "psutil-5.9.4-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:68908971daf802203f3d37e78d3f8831b6d1014864d7a85937941bb35f09aefe"},
-    {file = "psutil-5.9.4-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:3ff89f9b835100a825b14c2808a106b6fdcc4b15483141482a12c725e7f78549"},
-    {file = "psutil-5.9.4-cp27-cp27m-win32.whl", hash = "sha256:852dd5d9f8a47169fe62fd4a971aa07859476c2ba22c2254d4a1baa4e10b95ad"},
-    {file = "psutil-5.9.4-cp27-cp27m-win_amd64.whl", hash = "sha256:9120cd39dca5c5e1c54b59a41d205023d436799b1c8c4d3ff71af18535728e94"},
-    {file = "psutil-5.9.4-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:6b92c532979bafc2df23ddc785ed116fced1f492ad90a6830cf24f4d1ea27d24"},
-    {file = "psutil-5.9.4-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:efeae04f9516907be44904cc7ce08defb6b665128992a56957abc9b61dca94b7"},
-    {file = "psutil-5.9.4-cp36-abi3-macosx_10_9_x86_64.whl", hash = "sha256:54d5b184728298f2ca8567bf83c422b706200bcbbfafdc06718264f9393cfeb7"},
-    {file = "psutil-5.9.4-cp36-abi3-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:16653106f3b59386ffe10e0bad3bb6299e169d5327d3f187614b1cb8f24cf2e1"},
-    {file = "psutil-5.9.4-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:54c0d3d8e0078b7666984e11b12b88af2db11d11249a8ac8920dd5ef68a66e08"},
-    {file = "psutil-5.9.4-cp36-abi3-win32.whl", hash = "sha256:149555f59a69b33f056ba1c4eb22bb7bf24332ce631c44a319cec09f876aaeff"},
-    {file = "psutil-5.9.4-cp36-abi3-win_amd64.whl", hash = "sha256:fd8522436a6ada7b4aad6638662966de0d61d241cb821239b2ae7013d41a43d4"},
-    {file = "psutil-5.9.4-cp38-abi3-macosx_11_0_arm64.whl", hash = "sha256:6001c809253a29599bc0dfd5179d9f8a5779f9dffea1da0f13c53ee568115e1e"},
-    {file = "psutil-5.9.4.tar.gz", hash = "sha256:3d7f9739eb435d4b1338944abe23f49584bde5395f27487d2ee25ad9a8774a62"},
+    {file = "psutil-5.9.5-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:be8929ce4313f9f8146caad4272f6abb8bf99fc6cf59344a3167ecd74f4f203f"},
+    {file = "psutil-5.9.5-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:ab8ed1a1d77c95453db1ae00a3f9c50227ebd955437bcf2a574ba8adbf6a74d5"},
+    {file = "psutil-5.9.5-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4"},
+    {file = "psutil-5.9.5-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:ea8518d152174e1249c4f2a1c89e3e6065941df2fa13a1ab45327716a23c2b48"},
+    {file = "psutil-5.9.5-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:acf2aef9391710afded549ff602b5887d7a2349831ae4c26be7c807c0a39fac4"},
+    {file = "psutil-5.9.5-cp27-none-win32.whl", hash = "sha256:5b9b8cb93f507e8dbaf22af6a2fd0ccbe8244bf30b1baad6b3954e935157ae3f"},
+    {file = "psutil-5.9.5-cp27-none-win_amd64.whl", hash = "sha256:8c5f7c5a052d1d567db4ddd231a9d27a74e8e4a9c3f44b1032762bd7b9fdcd42"},
+    {file = "psutil-5.9.5-cp36-abi3-macosx_10_9_x86_64.whl", hash = "sha256:3c6f686f4225553615612f6d9bc21f1c0e305f75d7d8454f9b46e901778e7217"},
+    {file = "psutil-5.9.5-cp36-abi3-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7a7dd9997128a0d928ed4fb2c2d57e5102bb6089027939f3b722f3a210f9a8da"},
+    {file = "psutil-5.9.5-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:89518112647f1276b03ca97b65cc7f64ca587b1eb0278383017c2a0dcc26cbe4"},
+    {file = "psutil-5.9.5-cp36-abi3-win32.whl", hash = "sha256:104a5cc0e31baa2bcf67900be36acde157756b9c44017b86b2c049f11957887d"},
+    {file = "psutil-5.9.5-cp36-abi3-win_amd64.whl", hash = "sha256:b258c0c1c9d145a1d5ceffab1134441c4c5113b2417fafff7315a917a026c3c9"},
+    {file = "psutil-5.9.5-cp38-abi3-macosx_11_0_arm64.whl", hash = "sha256:c607bb3b57dc779d55e1554846352b4e358c10fff3abf3514a7a6601beebdb30"},
+    {file = "psutil-5.9.5.tar.gz", hash = "sha256:5410638e4df39c54d957fc51ce03048acd8e6d60abc0f5107af51e5fb566eb3c"},
 ]
 
 [package.extras]
 test = ["enum34", "ipaddress", "mock", "pywin32", "wmi"]
 
 [[package]]
 name = "pygments"
@@ -864,29 +864,29 @@
 typing-extensions = {version = ">=4.0.0,<5.0", markers = "python_version < \"3.9\""}
 
 [package.extras]
 jupyter = ["ipywidgets (>=7.5.1,<9)"]
 
 [[package]]
 name = "rope"
-version = "1.7.0"
+version = "1.8.0"
 description = "a python refactoring library..."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "rope-1.7.0-py3-none-any.whl", hash = "sha256:893dd80ba7077fc9f6f42b0a849372076b70f1d6e405b9f0cc52781ffa0e6890"},
-    {file = "rope-1.7.0.tar.gz", hash = "sha256:ba39581d0f8dee4ae8b5b5e82e35d03cebad965ccb127b7eaab9755cdc85e85a"},
+    {file = "rope-1.8.0-py3-none-any.whl", hash = "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd"},
+    {file = "rope-1.8.0.tar.gz", hash = "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"},
 ]
 
 [package.dependencies]
 pytoolconfig = {version = ">=1.2.2", extras = ["global"]}
 
 [package.extras]
-dev = ["build (>=0.7.0)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)"]
+dev = ["build (>=0.7.0)", "pip-tools (>=6.12.1)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)", "toml (>=0.10.2)"]
 doc = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
 
 [[package]]
 name = "semver"
 version = "2.13.0"
 description = "Python helper for Semantic Versioning (http://semver.org/)"
 category = "dev"
@@ -895,39 +895,40 @@
 files = [
     {file = "semver-2.13.0-py2.py3-none-any.whl", hash = "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4"},
     {file = "semver-2.13.0.tar.gz", hash = "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"},
 ]
 
 [[package]]
 name = "sentry-sdk"
-version = "1.18.0"
+version = "1.22.1"
 description = "Python client for Sentry (https://sentry.io)"
 category = "main"
 optional = true
 python-versions = "*"
 files = [
-    {file = "sentry-sdk-1.18.0.tar.gz", hash = "sha256:d07b9569a151033b462f7a7113ada94cc41ecf49daa83d35f5f852a0b9cf3b44"},
-    {file = "sentry_sdk-1.18.0-py2.py3-none-any.whl", hash = "sha256:714203a9adcac4a4a35e348dc9d3e294ad0200a66cdca26c068967d728f34fcb"},
+    {file = "sentry-sdk-1.22.1.tar.gz", hash = "sha256:052dff5069c6f0d836ee014323576824a9b40836fc003fb12489a1f19c60a3c9"},
+    {file = "sentry_sdk-1.22.1-py2.py3-none-any.whl", hash = "sha256:c6c6946f8c927adb00af1c5ab6921df38775b2199b9003816d5935a1310352d5"},
 ]
 
 [package.dependencies]
 certifi = "*"
-urllib3 = {version = ">=1.26.11", markers = "python_version >= \"3.6\""}
+urllib3 = {version = ">=1.26.11,<2.0.0", markers = "python_version >= \"3.6\""}
 
 [package.extras]
 aiohttp = ["aiohttp (>=3.5)"]
 arq = ["arq (>=0.23)"]
 beam = ["apache-beam (>=2.12)"]
 bottle = ["bottle (>=0.12.13)"]
 celery = ["celery (>=3)"]
 chalice = ["chalice (>=1.16.0)"]
 django = ["django (>=1.8)"]
 falcon = ["falcon (>=1.4)"]
 fastapi = ["fastapi (>=0.79.0)"]
 flask = ["blinker (>=1.1)", "flask (>=0.11)"]
+grpcio = ["grpcio (>=1.21.1)"]
 httpx = ["httpx (>=0.16.0)"]
 huey = ["huey (>=2)"]
 opentelemetry = ["opentelemetry-distro (>=0.35b0)"]
 pure-eval = ["asttokens", "executing", "pure-eval"]
 pymongo = ["pymongo (>=3.1)"]
 pyspark = ["pyspark (>=2.4.4)"]
 quart = ["blinker (>=1.1)", "quart (>=0.16.1)"]
@@ -1158,8 +1159,8 @@
 
 [extras]
 tracking = ["sentry-sdk"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.7"
-content-hash = "94d9d5f179101967644d48a72b8ab3cbad09561a4d6522808bbd6fb8e681caea"
+content-hash = "f2c0b0d7ab8865886401522547d31c1fcb2a86d85e335ac1c4a18d35a64ad1fc"
```

### Comparing `ospd_openvas-22.5.0/pyproject.toml` & `ospd_openvas-22.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ospd-openvas"
-version = "22.5.0"
+version = "22.5.1"
 description = "ospd based scanner for openvas"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/ospd-openvas"
 repository = "https://github.com/greenbone/ospd-openvas"
 # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
@@ -52,15 +52,15 @@
 defusedxml = ">=0.6,<0.8"
 deprecated = "^1.2.10"
 paho-mqtt = ">=1.5.1"
 python-gnupg = ">=0.4.8,<0.6.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.13.9"
-rope = "^1.7.0"
+rope = "^1.8.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 pontos = ">=22.7.2"
 black = ">=22.6.0"
 
 [tool.poetry.extras]
 tracking = ["sentry-sdk"]
```

### Comparing `ospd_openvas-22.5.0/tests/command/__init__.py` & `ospd_openvas-22.5.1/tests/command/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/command/test_command.py` & `ospd_openvas-22.5.1/tests/command/test_command.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/command/test_commands.py` & `ospd_openvas-22.5.1/tests/command/test_commands.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/command/test_registry.py` & `ospd_openvas-22.5.1/tests/command/test_registry.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/dummydaemon.py` & `ospd_openvas-22.5.1/tests/dummydaemon.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/helper.py` & `ospd_openvas-22.5.1/tests/helper.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/messages/__init__.py` & `ospd_openvas-22.5.1/tests/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/messages/test_message.py` & `ospd_openvas-22.5.1/tests/messages/test_message.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/messages/test_result.py` & `ospd_openvas-22.5.1/tests/messages/test_result.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/messaging/__init__.py` & `ospd_openvas-22.5.1/tests/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/messaging/test_mqtt.py` & `ospd_openvas-22.5.1/tests/messaging/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_argument_parser.py` & `ospd_openvas-22.5.1/tests/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_cvss.py` & `ospd_openvas-22.5.1/tests/test_cvss.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_daemon.py` & `ospd_openvas-22.5.1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_datapickler.py` & `ospd_openvas-22.5.1/tests/test_datapickler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_db.py` & `ospd_openvas-22.5.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_errors.py` & `ospd_openvas-22.5.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_gpg.py` & `ospd_openvas-22.5.1/tests/test_gpg.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_lock.py` & `ospd_openvas-22.5.1/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_notus.py` & `ospd_openvas-22.5.1/tests/test_notus.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_nvti_cache.py` & `ospd_openvas-22.5.1/tests/test_nvti_cache.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_openvas.py` & `ospd_openvas-22.5.1/tests/test_openvas.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_port_convert.py` & `ospd_openvas-22.5.1/tests/test_port_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "ALL_IANA_ASSIGNED_TCP_AND_UDP_2020_02_12": "T:1-50,52-80,82-99,101-113,115-224,242-248,256-257,259-271,280-284,286-287,308-324,333,344-584,586-658,660-702,704-707,709-715,729-731,741-742,744,747-754,758-765,767,769-777,780,800-802,810,828-833,847-848,853-854,860-862,873,886-888,900-903,910-913,953,989-1001,1010,1021-1027,1029,1033-1108,1110-1490,1492-1782,1784-2193,2197-2258,2260-2368,2370-2377,2379-2681,2683-2793,2795-2824,2826-2872,2874-2924,2926-3091,3093-3125,3127-3300,3302-3321,3326-3366,3372-3402,3405-3545,3547-3693,3695-3993,3995-4047,4049-4143,4145-4193,4197,4199,4300-4314,4316,4320-4323,4325-4336,4340-4362,4366,4368-4379,4389-4396,4400-4423,4425-4433,4441-4458,4484-4488,4500,4534-4538,4545-4559,4563,4566-4570,4573,4590-4605,4621,4646,4658-4692,4700-4704,4711,4725-4733,4737-4747,4749-4756,4774,4784-4791,4800-4804,4827,4837-4851,4867-4871,4876-4885,4888-4889,4894,4899-4902,4912-4915,4936-4937,4940-4942,4949-4953,4969-4971,4980,4984-4991,4999-5015,5020-5034,5042-5075,5078-5087,5092-5094,5099-5107,5111-5112,5114-5117,5120,5133-5137,5145-5146,5150-5157,5161-5168,5172,5190-5197,5200-5203,5209,5215,5221-5237,5245-5254,5264-5265,5269-5272,5280-5282,5298-5310,5312-5318,5320-5321,5343-5344,5349-5364,5397-5437,5443,5445,5450,5453-5456,5461-5465,5470-5475,5500-5507,5550,5553-5557,5565-5569,5573-5575,5579-5586,5597-5605,5618,5627-5639,5646,5666,5670-5684,5687-5689,5693,5696,5700,5705,5713-5730,5741-5748,5750,5755,5757,5766-5771,5777,5780-5787,5793-5794,5813-5814,5841-5842,5859,5863,5868,5883,5900,5910-5913,5963,5968-5969,5984-5993,5999,6064-6066,6068-6077,6080-6088,6099-6118,6121-6124,6130,6133,6140-6149,6159-6163,6200-6201,6209,6222,6241-6244,6251-6253,6267-6269,6300-6301,6306,6315-6317,6320-6322,6324-6326,6343-6344,6346-6347,6350,6355,6360,6363,6370,6379,6382,6389-6390,6417-6421,6432,6442-6446,6455-6456,6464,6471,6480-6489,6500-6503,6505-6511,6513-6515,6543-6544,6547-6551,6558,6566,6568,6579-6583,6600-6602,6619-6629,6632-6636,6640,6653,6655-6657,6670-6673,6678-6679,6687-6690,6696-6697,6701-6706,6714-6716,6767-6771,6777-6778,6784-6791,6801,6817,6831,6841-6842,6850,6868,6888,6900-6901,6924,6935-6936,6946,6951,6961-6966,6969-6970,6997-7026,7030-7031,7040,7070-7073,7080,7088,7095,7099-7101,7107,7117,7121,7128-7129,7161-7174,7181,7200-7202,7215-7216,7227-7229,7235-7237,7244,7262,7272-7283,7365,7391-7395,7397,7400-7402,7410-7411,7420-7421,7426-7431,7437,7443,7471,7473-7474,7478,7491,7500-7501,7508-7511,7542-7551,7560,7563,7566,7569-7570,7574,7588,7606,7624,7626-7631,7633,7648,7663,7672-7677,7680,7683,7687,7689,7697,7700-7701,7707-7708,7720,7724-7728,7734,7738,7741-7744,7747,7775,7777-7779,7781,7784,7786-7787,7789,7794,7797-7802,7810,7845-7847,7869-7872,7878,7880,7887,7900-7903,7913,7932-7933,7962,7967,7979-7982,7997-8009,8015-8016,8019-8023,8025-8026,8032-8034,8040-8044,8051-8060,8066-8067,8070,8074,8077,8080-8084,8086-8088,8090-8091,8097,8100-8102,8111,8115-8118,8121-8122,8128-8132,8140,8148-8149,8153,8160-8162,8181-8184,8190-8192,8194-8195,8199-8202,8204-8208,8211,8230-8232,8243,8266,8270,8276,8280,8282,8292-8294,8300-8301,8313,8320-8322,8351,8376-8380,8383-8384,8400-8405,8415-8417,8423,8442-8445,8450,8457,8470-8474,8500-8503,8554-8555,8567,8600,8609-8615,8665-8666,8675,8686,8688,8699,8710-8711,8732-8733,8750,8763-8770,8778,8786-8787,8793,8800,8804-8805,8807-8809,8873,8880-8881,8883,8888-8894,8899-8901,8910-8913,8937,8953-8954,8980-8981,8989-8991,8997-9002,9005,9007-9011,9020-9026,9050-9051,9060,9080-9081,9083-9093,9100-9107,9111,9119,9122-9123,9131,9160-9164,9191,9200-9217,9222,9255,9277-9287,9292-9295,9300,9306,9312,9318,9321,9339,9343-9346,9374,9380,9387-9390,9396-9397,9400-9402,9418,9443-9445,9450,9500,9522,9535-9536,9555,9592-9600,9612,9614,9616-9618,9628-9632,9640,9666-9668,9694-9695,9700,9747,9750,9753,9762,9800-9802,9875-9878,9888-9889,9898-9900,9903,9909,9911,9925,9950-9956,9966,9978-9979,9981,9987-9988,9990-10010,10020,10023,10050-10051,10055,10080-10081,10100-10104,10107,10110-10111,10113-10117,10125,10128-10129,10160-10162,10200-10201,10252-10253,10260-10261,10288,10321,10439,10443,10500,10540-10544,10548,10631,10800,10805,10809-10810,10860,10880,10933,10990,11000-11001,11095,11103-11106,11108-11112,11161-11165,11171-11175,11201-11202,11208,11211,11319-11321,11367,11371,11430,11489,11600,11623,11720,11723,11751,11796,11876-11877,11967,11971,12000-12010,12012-12013,12109,12121,12168,12172,12300,12302,12321-12322,12345,12753,12865,13160,13216-13218,13223-13224,13400,13720-13722,13724,13782-13783,13785-13786,13818-13823,13894,13929-13930,14000-14002,14033-14034,14141-14143,14145,14149-14150,14154,14250,14414,14500,14936-14937,15000,15002,15118,15345,15363,15555,15660,15740,15998-16003,16020-16021,16161-16162,16309-16311,16360-16361,16367-16368,16384-16385,16619,16665-16666,16789,16900,16950,16991-16995,17007,17184-17185,17219-17225,17234-17235,17500,17555,17729,17754-17756,17777,18000,18104,18136,18181-18187,18241-18243,18262,18463,18634-18635,18668,18769,18881,18888,19000,19007,19020,19191,19194,19220,19283,19315,19398,19410-19412,19539-19541,19788,19998-20003,20005,20012-20014,20034,20046,20048-20049,20057,20167,20202,20222,20480,20670,20999-21000,21010,21212-21213,21221,21553-21554,21590,21800,21845-21849,22000-22005,22125,22128,22222,22273,22305,22335,22343,22347,22350-22351,22537,22555,22763,22800,22951,23000-23005,23053,23272,23294,23333,23400-23402,23456-23457,23546,24000-24006,24242,24249,24321-24323,24386,24465,24554,24577,24666,24676-24678,24680,24754,24850,24922,25000-25009,25576,25604,25793,25900-25903,25954-25955,26000,26133,26208,26257,26260-26263,26486-26487,26489,27010,27017,27345,27442,27504,27782,27876,27999-28001,28010,28119,28200,28240,28589,29118,29167-29168,29999-30004,30100,30260,30400,30832,30999,31016,31020,31029,31400,31416,31457,31620,31685,31765,31948-31949,32034,32249,32400,32483,32635-32636,32767-32777,32801,32811,32896,33000,33060,33123,33331,33333-33334,33434-33435,33656,34249,34378-34379,34567,34962-34964,34980,35000-35006,35100,35354-35357,36001,36411-36412,36422,36462,36524,36602,36700,36865,37475,37483,37601,37654,38000-38002,38201-38203,38412,38422,38462,38472,38800,38865,39681,40000,40023,40404,40841-40843,40853,41111,41121,41230,41794-41797,42508-42510,43000,43188-43191,43210,43438-43441,44123,44321-44323,44444-44445,44544,44553,44600,44818,44900,45000-45002,45045,45054,45514,45678,45824-45825,45966,46336,46998-47001,47100,47557,47624,47806,47808-47809,48000-48005,48048-48050,48128-48129,48556,48619,48653,49000-49001,49150,6000-6063,6665-6669, U:1-50,52-80,82-99,101-113,115-224,242-248,256-257,259-271,280-284,286-287,308-324,333,344-584,586-658,660-702,704-707,709-716,729-731,741-742,744,747-754,758-765,767,769-777,780,800-802,810,828-833,847-848,853-854,860-862,873,886-888,900-903,910-913,953,989-1001,1008,1010,1021-1027,1029,1033-1108,1110-1490,1492-1782,1784-2193,2197-2258,2260-2368,2370-2375,2377,2379-2681,2683-2793,2795-2824,2826-2872,2874-2924,2926-3091,3093-3125,3127-3300,3302-3321,3326-3366,3372-3402,3405-3545,3547-3693,3695-3993,3995-4047,4049-4143,4145-4193,4197,4199,4300-4314,4316,4320-4323,4325-4336,4340-4362,4366,4368-4379,4389-4396,4400-4423,4425-4433,4441-4458,4484-4488,4500,4534-4538,4545-4559,4563,4566-4570,4573,4590-4605,4621,4646,4658-4692,4700-4704,4711,4725-4733,4737-4747,4749-4756,4774,4784-4791,4800-4804,4827,4837-4851,4867-4871,4876-4885,4888-4889,4894,4899-4902,4912,4914-4915,4936-4937,4940-4942,4949-4953,4969-4971,4980,4984-4991,4999-5015,5020-5034,5042-5075,5078-5087,5092-5094,5099-5107,5111-5112,5114-5117,5120,5133-5137,5145-5146,5150-5157,5161-5168,5172,5190-5197,5200-5203,5209,5215,5221-5237,5245-5254,5264-5265,5269-5272,5280-5282,5298-5310,5312-5318,5320-5321,5343-5344,5349-5364,5397-5437,5443,5445,5450,5453-5456,5461-5465,5470-5475,5500-5507,5550,5553-5557,5565-5569,5573-5575,5579-5586,5597-5605,5618,5627-5639,5646,5666,5670-5684,5687-5689,5693,5696,5700,5705,5713-5730,5741-5748,5750,5755,5757,5766-5771,5777,5780-5787,5793-5794,5813-5814,5841-5842,5859,5863,5868,5900,5910-5913,5963,5968-5969,5984-5993,5999,6064-6066,6068-6077,6080-6088,6099-6118,6121-6124,6130,6133,6140-6149,6159-6163,6200-6201,6209,6222,6241-6244,6251-6253,6267-6269,6300-6301,6306,6315-6317,6320-6322,6324-6326,6343-6344,6346-6347,6350,6355,6360,6363,6370,6379,6382,6389-6390,6417-6421,6432,6442-6446,6455-6456,6464,6471,6480-6489,6500-6503,6505-6511,6513-6515,6543-6544,6547-6551,6558,6566,6568,6579-6583,6600-6602,6619-6629,6632-6636,6640,6653,6655-6657,6670-6673,6678-6679,6687-6690,6696-6697,6701-6706,6714-6716,6767-6771,6777-6778,6784-6791,6801,6817,6831,6841-6842,6850,6868,6888,6900-6901,6924,6935-6936,6946,6951,6961-6966,6969-6970,6997-7026,7030-7031,7040,7070-7073,7080,7088,7095,7099-7101,7107,7117,7121,7128-7129,7161-7174,7181,7200-7201,7215-7216,7227-7229,7235-7237,7244,7262,7272-7283,7365,7391-7395,7397,7400-7402,7410-7411,7420-7421,7426-7431,7437,7443,7471,7473-7474,7478,7491,7500-7501,7508-7511,7542-7551,7560,7563,7566,7569-7570,7574,7588,7606,7624,7626-7631,7633,7648,7663,7672-7677,7680,7683,7687,7689,7697,7700-7702,7707-7708,7720,7724-7728,7734,7738,7741-7744,7747,7775,7777-7779,7781,7784,7786-7787,7789,7794,7797-7802,7810,7845-7847,7869-7872,7878,7880,7887,7900-7903,7913,7932-7933,7962,7967,7979-7982,7997-8009,8015-8016,8019-8023,8025-8026,8032-8034,8040-8044,8051-8060,8066-8067,8070,8074,8077,8080-8084,8086-8088,8090-8091,8097,8100-8102,8111,8115-8118,8121-8122,8128-8132,8140,8148-8149,8153,8160-8162,8181-8184,8190-8192,8194-8195,8199-8202,8204-8208,8211,8230-8232,8243,8266,8270,8276,8280,8282,8292-8294,8300-8301,8313,8320-8322,8351,8376-8380,8383-8384,8400-8405,8415-8417,8423,8442-8445,8450,8457,8470-8474,8500-8503,8554-8555,8567,8600,8609-8615,8665-8666,8675,8686,8688,8699,8710-8711,8732-8733,8750,8763-8770,8778,8786-8787,8793,8800,8804-8805,8807-8809,8873,8880-8881,8883,8888-8894,8899-8901,8910-8913,8937,8953-8954,8980-8981,8989-8991,8997-9002,9005,9007-9011,9020-9026,9050-9051,9060,9080-9081,9083-9093,9100-9107,9111,9119,9122-9123,9131,9160-9164,9191,9200-9217,9222,9255,9277-9287,9292-9295,9300,9306,9312,9318,9321,9339,9343-9346,9374,9380,9387-9390,9396-9397,9400-9402,9418,9443-9445,9450,9500,9522,9535-9536,9555,9592-9600,9612,9614,9616-9618,9628-9632,9640,9666-9668,9694-9695,9700,9747,9750,9753,9762,9800-9802,9875,9877-9878,9888-9889,9898-9901,9903,9909,9911,9925,9950-9956,9966,9978-9979,9981,9987-9988,9990-10010,10020,10023,10050-10051,10055,10080-10081,10100-10104,10107,10110-10111,10113-10117,10125,10128-10129,10160-10162,10200-10201,10252-10253,10260-10261,10288,10321,10439,10443,10500,10540-10544,10548,10631,10800,10805,10809-10810,10860,10880,10933,10990,11000-11001,11095,11103-11106,11108-11112,11161-11165,11171-11175,11201-11202,11208,11211,11319-11321,11367,11371,11430,11489,11600,11623,11720,11723,11751,11796,11876-11877,11967,11971,12000-12010,12012-12013,12109,12121,12168,12172,12300,12302,12321-12322,12345,12753,12865,13160,13216-13218,13223-13224,13400,13720-13722,13724,13782-13783,13785-13786,13818-13823,13894,13929-13930,14000-14002,14033-14034,14141-14143,14145,14149-14150,14154,14250,14414,14500,14936-14937,15000,15002,15118,15345,15363,15555,15660,15740,15998-16003,16020-16021,16161-16162,16309-16311,16360-16361,16367-16368,16384-16385,16619,16665-16666,16789,16900,16950,16991-16995,17007,17184-17185,17219-17225,17234-17235,17500,17555,17729,17754-17756,17777,18000,18104,18136,18181-18187,18241-18243,18262,18463,18634-18635,18668,18769,18881,18888,19000,19007,19020,19191,19194,19220,19283,19315,19398,19410-19412,19539-19541,19788,19998-20003,20005,20012-20014,20034,20046,20048-20049,20057,20167,20202,20222,20480,20670,20999-21000,21010,21212-21213,21221,21553-21554,21590,21800,21845-21849,22000-22005,22125,22128,22222,22273,22305,22335,22343,22347,22350-22351,22537,22555,22763,22800,22951,23000-23005,23053,23272,23294,23333,23400-23402,23456-23457,23546,24000-24006,24242,24249,24321-24323,24386,24465,24554,24577,24666,24676-24678,24680,24754,24850,24922,25000-25009,25576,25604,25793,25900-25903,25954-25955,26000,26133,26208,26257,26260-26263,26486-26487,26489,27010,27017,27345,27442,27504,27782,27876,27999-28001,28010,28119,28200,28240,28589,29118,29167-29168,29999-30004,30100,30260,30400,30832,30999,31016,31020,31029,31400,31416,31457,31620,31685,31765,31948-31949,32034,32249,32400,32483,32635-32636,32767-32777,32801,32811,32896,33000,33060,33123,33331,33333-33334,33434-33435,33656,34249,34378-34379,34567,34962-34964,34980,35000-35006,35100,35354-35357,36001,36411-36412,36422,36462,36524,36602,36700,36865,37475,37483,37601,37654,38000-38002,38201-38203,38412,38422,38462,38472,38800,38865,39681,40000,40023,40404,40841-40843,40853,41111,41121,41230,41794-41797,42508-42510,43000,43188-43191,43210,43438-43441,44123,44321-44323,44444-44445,44544,44553,44600,44818,44900,45000-45002,45045,45054,45514,45678,45824-45825,45966,46336,46998-47001,47100,47557,47624,47806,47808-47809,48000-48005,48048-48050,48128-48129,48556,48619,48653,49000-49001,49150,6000-6063,6665-6669",  # pylint: disable=C0301
     "ALL_TCP_AND_NMAP_5_51_TOP_100_UDP": "T:1-65535, U:7-7,9-9,17-17,19-19,49-49,53-53,67-69,80-80,88-88,111-111,120-120,123-123,135-139,158-158,161-162,177-177,427-427,443-443,445-445,497-497,500-500,514-515,518-518,520-520,593-593,623-623,626-626,631-631,996-999,1022-1023,1025-1030,1433-1434,1645-1646,1701-1701,1718-1719,1812-1813,1900-1900,2000-2000,2048-2049,2222-2223,3283-3283,3456-3456,3703-3703,4444-4444,4500-4500,5000-5000,5060-5060,5353-5353,5632-5632,9200-9200,10000-10000,17185-17185,20031-20031,30718-30718,31337-31337,32768-32769,32771-32771,32815-32815,33281-33281,49152-49154,49156-49156,49181-49182,49185-49186,49188-49188,49190-49194,49200-49201",  # pylint: disable=C0301
     "ALL_TCP_AND_NMAP_5_51_TOP_1000_UDP": "T:1-65535, U:2-3,7-7,9-9,13-13,17-17,19-23,37-38,42-42,49-49,53-53,67-69,80-80,88-88,111-113,120-120,123-123,135-139,158-158,161-162,177-177,192-192,199-199,207-207,217-217,363-363,389-389,402-402,407-407,427-427,434-434,443-443,445-445,464-464,497-497,500-500,502-502,512-515,517-518,520-520,539-539,559-559,593-593,623-623,626-626,631-631,639-639,643-643,657-657,664-664,682-689,764-764,767-767,772-776,780-782,786-786,789-789,800-800,814-814,826-826,829-829,838-838,902-903,944-944,959-959,965-965,983-983,989-990,996-1001,1007-1008,1012-1014,1019-1051,1053-1060,1064-1070,1072-1072,1080-1081,1087-1088,1090-1090,1100-1101,1105-1105,1124-1124,1200-1200,1214-1214,1234-1234,1346-1346,1419-1419,1433-1434,1455-1455,1457-1457,1484-1485,1524-1524,1645-1646,1701-1701,1718-1719,1761-1761,1782-1782,1804-1804,1812-1813,1885-1886,1900-1901,1993-1993,2000-2000,2002-2002,2048-2049,2051-2051,2148-2148,2160-2161,2222-2223,2343-2343,2345-2345,2362-2362,2967-2967,3052-3052,3130-3130,3283-3283,3296-3296,3343-3343,3389-3389,3401-3401,3456-3457,3659-3659,3664-3664,3702-3703,4000-4000,4008-4008,4045-4045,4444-4444,4500-4500,4666-4666,4672-4672,5000-5003,5010-5010,5050-5050,5060-5060,5093-5093,5351-5351,5353-5353,5355-5355,5500-5500,5555-5555,5632-5632,6000-6002,6004-6004,6050-6050,6346-6347,6970-6971,7000-7000,7938-7938,8000-8001,8010-8010,8181-8181,8193-8193,8900-8900,9000-9001,9020-9020,9103-9103,9199-9200,9370-9370,9876-9877,9950-9950,10000-10000,10080-10080,11487-11487,16086-16086,16402-16402,16420-16420,16430-16430,16433-16433,16449-16449,16498-16498,16503-16503,16545-16545,16548-16548,16573-16573,16674-16674,16680-16680,16697-16697,16700-16700,16708-16708,16711-16711,16739-16739,16766-16766,16779-16779,16786-16786,16816-16816,16829-16829,16832-16832,16838-16839,16862-16862,16896-16896,16912-16912,16918-16919,16938-16939,16947-16948,16970-16970,16972-16972,16974-16974,17006-17006,17018-17018,17077-17077,17091-17091,17101-17101,17146-17146,17184-17185,17205-17205,17207-17207,17219-17219,17236-17237,17282-17282,17302-17302,17321-17321,17331-17332,17338-17338,17359-17359,17417-17417,17423-17424,17455-17455,17459-17459,17468-17468,17487-17487,17490-17490,17494-17494,17505-17505,17533-17533,17549-17549,17573-17573,17580-17580,17585-17585,17592-17592,17605-17605,17615-17616,17629-17629,17638-17638,17663-17663,17673-17674,17683-17683,17726-17726,17754-17754,17762-17762,17787-17787,17814-17814,17823-17824,17836-17836,17845-17845,17888-17888,17939-17939,17946-17946,17989-17989,18004-18004,18081-18081,18113-18113,18134-18134,18156-18156,18228-18228,18234-18234,18250-18250,18255-18255,18258-18258,18319-18319,18331-18331,18360-18360,18373-18373,18449-18449,18485-18485,18543-18543,18582-18582,18605-18605,18617-18617,18666-18666,18669-18669,18676-18676,18683-18683,18807-18807,18818-18818,18821-18821,18830-18830,18832-18832,18835-18835,18869-18869,18883-18883,18888-18888,18958-18958,18980-18980,18985-18985,18987-18987,18991-18991,18994-18994,18996-18996,19017-19017,19022-19022,19039-19039,19047-19047,19075-19075,19096-19096,19120-19120,19130-19130,19140-19141,19154-19154,19161-19161,19165-19165,19181-19181,19193-19193,19197-19197,19222-19222,19227-19227,19273-19273,19283-19283,19294-19294,19315-19315,19322-19322,19332-19332,19374-19374,19415-19415,19482-19482,19489-19489,19500-19500,19503-19504,19541-19541,19600-19600,19605-19605,19616-19616,19624-19625,19632-19632,19639-19639,19647-19647,19650-19650,19660-19660,19662-19663,19682-19683,19687-19687,19695-19695,19707-19707,19717-19719,19722-19722,19728-19728,19789-19789,19792-19792,19933-19933,19935-19936,19956-19956,19995-19995,19998-19998,20003-20004,20019-20019,20031-20031,20082-20082,20117-20117,20120-20120,20126-20126,20129-20129,20146-20146,20154-20154,20164-20164,20206-20206,20217-20217,20249-20249,20262-20262,20279-20279,20288-20288,20309-20309,20313-20313,20326-20326,20359-20360,20366-20366,20380-20380,20389-20389,20409-20409,20411-20411,20423-20425,20445-20445,20449-20449,20464-20465,20518-20518,20522-20522,20525-20525,20540-20540,20560-20560,20665-20665,20678-20679,20710-20710,20717-20717,20742-20742,20752-20752,20762-20762,20791-20791,20817-20817,20842-20842,20848-20848,20851-20851,20865-20865,20872-20872,20876-20876,20884-20884,20919-20919,21000-21000,21016-21016,21060-21060,21083-21083,21104-21104,21111-21111,21131-21131,21167-21167,21186-21186,21206-21207,21212-21212,21247-21247,21261-21261,21282-21282,21298-21298,21303-21303,21318-21318,21320-21320,21333-21333,21344-21344,21354-21354,21358-21358,21360-21360,21364-21364,21366-21366,21383-21383,21405-21405,21454-21454,21468-21468,21476-21476,21514-21514,21524-21525,21556-21556,21566-21566,21568-21568,21576-21576,21609-21609,21621-21621,21625-21625,21644-21644,21649-21649,21655-21655,21663-21663,21674-21674,21698-21698,21702-21702,21710-21710,21742-21742,21780-21780,21784-21784,21800-21800,21803-21803,21834-21834,21842-21842,21847-21847,21868-21868,21898-21898,21902-21902,21923-21923,21948-21948,21967-21967,22029-22029,22043-22043,22045-22045,22053-22053,22055-22055,22105-22105,22109-22109,22123-22124,22341-22341,22692-22692,22695-22695,22739-22739,22799-22799,22846-22846,22914-22914,22986-22986,22996-22996,23040-23040,23176-23176,23354-23354,23531-23531,23557-23557,23608-23608,23679-23679,23781-23781,23965-23965,23980-23980,24007-24007,24279-24279,24511-24511,24594-24594,24606-24606,24644-24644,24854-24854,24910-24910,25003-25003,25157-25157,25240-25240,25280-25280,25337-25337,25375-25375,25462-25462,25541-25541,25546-25546,25709-25709,25931-25931,26407-26407,26415-26415,26720-26720,26872-26872,26966-26966,27015-27015,27195-27195,27444-27444,27473-27473,27482-27482,27707-27707,27892-27892,27899-27899,28122-28122,28369-28369,28465-28465,28493-28493,28543-28543,28547-28547,28641-28641,28840-28840,28973-28973,29078-29078,29243-29243,29256-29256,29810-29810,29823-29823,29977-29977,30263-30263,30303-30303,30365-30365,30544-30544,30656-30656,30697-30697,30704-30704,30718-30718,30975-30975,31059-31059,31073-31073,31109-31109,31189-31189,31195-31195,31335-31335,31337-31337,31365-31365,31625-31625,31681-31681,31731-31731,31891-31891,32345-32345,32385-32385,32528-32528,32768-32780,32798-32798,32815-32815,32818-32818,32931-32931,33030-33030,33249-33249,33281-33281,33354-33355,33459-33459,33717-33717,33744-33744,33866-33866,33872-33872,34038-34038,34079-34079,34125-34125,34358-34358,34422-34422,34433-34433,34555-34555,34570-34570,34577-34580,34758-34758,34796-34796,34855-34855,34861-34862,34892-34892,35438-35438,35702-35702,35777-35777,35794-35794,36108-36108,36206-36206,36384-36384,36458-36458,36489-36489,36669-36669,36778-36778,36893-36893,36945-36945,37144-37144,37212-37212,37393-37393,37444-37444,37602-37602,37761-37761,37783-37783,37813-37813,37843-37843,38037-38037,38063-38063,38293-38293,38412-38412,38498-38498,38615-38615,39213-39213,39217-39217,39632-39632,39683-39683,39714-39714,39723-39723,39888-39888,40019-40019,40116-40116,40441-40441,40539-40539,40622-40622,40708-40708,40711-40711,40724-40724,40732-40732,40805-40805,40847-40847,40866-40866,40915-40915,41058-41058,41081-41081,41308-41308,41370-41370,41446-41446,41524-41524,41638-41638,41702-41702,41774-41774,41896-41896,41967-41967,41971-41971,42056-42056,42172-42172,42313-42313,42431-42431,42434-42434,42508-42508,42557-42557,42577-42577,42627-42627,42639-42639,43094-43094,43195-43195,43370-43370,43514-43514,43686-43686,43824-43824,43967-43967,44101-44101,44160-44160,44179-44179,44185-44185,44190-44190,44253-44253,44334-44334,44508-44508,44923-44923,44946-44946,44968-44968,45247-45247,45380-45380,45441-45441,45685-45685,45722-45722,45818-45818,45928-45928,46093-46093,46532-46532,46836-46836,47624-47624,47765-47765,47772-47772,47808-47808,47915-47915,47981-47981,48078-48078,48189-48189,48255-48255,48455-48455,48489-48489,48761-48761,49152-49163,49165-49182,49184-49202,49204-49205,49207-49216,49220-49220,49222-49222,49226-49226,49259-49259,49262-49262,49306-49306,49350-49350,49360-49360,49393-49393,49396-49396,49503-49503,49640-49640,49968-49968,50099-50099,50164-50164,50497-50497,50612-50612,50708-50708,50919-50919,51255-51255,51456-51456,51554-51554,51586-51586,51690-51690,51717-51717,51905-51905,51972-51972,52144-52144,52225-52225,52503-52503,53006-53006,53037-53037,53571-53571,53589-53589,53838-53838,54094-54094,54114-54114,54281-54281,54321-54321,54711-54711,54807-54807,54925-54925,55043-55043,55544-55544,55587-55587,56141-56141,57172-57172,57409-57410,57813-57813,57843-57843,57958-57958,57977-57977,58002-58002,58075-58075,58178-58178,58419-58419,58631-58631,58640-58640,58797-58797,59193-59193,59207-59207,59765-59765,59846-59846,60172-60172,60381-60381,60423-60423,61024-61024,61142-61142,61319-61319,61322-61322,61370-61370,61412-61412,61481-61481,61550-61550,61685-61685,61961-61961,62154-62154,62287-62287,62575-62575,62677-62677,62699-62699,62958-62958,63420-63420,63555-63555,64080-64080,64481-64481,64513-64513,64590-64590,64727-64727",  # pylint: disable=C0301
     "NMAP_5_51_TOP_2000_TCP_AND_TOP_100_UDP": "T:1-1,3-4,6-7,9-9,13-13,17-17,19-27,30-30,32-33,37-37,42-43,49-49,53-53,55-55,57-57,59-59,70-70,77-77,79-90,98-100,102-102,106-106,109-111,113-113,119-119,123-123,125-125,127-127,135-135,139-139,143-144,146-146,157-157,161-161,163-163,179-179,199-199,210-212,220-220,222-223,225-225,250-252,254-257,259-259,264-264,280-280,301-301,306-306,311-311,333-333,340-340,366-366,388-389,406-407,411-411,416-417,419-419,425-425,427-427,441-445,447-447,458-458,464-465,475-475,481-481,497-497,500-500,502-502,512-515,523-524,540-541,543-545,548-548,554-557,563-563,587-587,593-593,600-600,602-602,606-606,610-610,616-617,621-621,623-623,625-625,631-631,636-636,639-639,641-641,646-646,648-648,655-655,657-657,659-660,666-669,674-674,683-684,687-687,690-691,700-701,705-705,709-711,713-715,720-720,722-722,725-726,728-732,740-740,748-749,754-754,757-758,765-765,777-778,780-780,782-783,786-787,790-790,792-792,795-795,800-803,805-806,808-808,822-823,825-825,829-829,839-840,843-843,846-846,856-856,859-859,862-862,864-864,873-874,878-878,880-880,888-888,898-898,900-905,911-913,918-918,921-922,924-924,928-928,930-931,943-943,953-953,969-969,971-971,980-981,987-987,990-990,992-993,995-996,998-1002,1004-1015,1020-1114,1116-1119,1121-1128,1130-1132,1134-1138,1141-1141,1143-1145,1147-1154,1156-1159,1162-1169,1173-1176,1179-1180,1182-1188,1190-1192,1194-1196,1198-1201,1204-1204,1207-1213,1215-1218,1220-1223,1228-1229,1233-1234,1236-1236,1239-1241,1243-1244,1247-1251,1259-1259,1261-1262,1264-1264,1268-1268,1270-1272,1276-1277,1279-1279,1282-1282,1287-1287,1290-1291,1296-1297,1299-1303,1305-1311,1314-1319,1321-1322,1324-1324,1327-1328,1330-1331,1334-1334,1336-1337,1339-1340,1347-1347,1350-1353,1357-1357,1413-1414,1417-1417,1433-1434,1443-1443,1455-1455,1461-1461,1494-1494,1500-1501,1503-1503,1516-1516,1521-1522,1524-1526,1533-1533,1547-1547,1550-1550,1556-1556,1558-1560,1565-1566,1569-1569,1580-1580,1583-1584,1592-1592,1594-1594,1598-1598,1600-1600,1605-1605,1607-1607,1615-1615,1620-1620,1622-1622,1632-1632,1635-1635,1638-1638,1641-1641,1645-1645,1658-1658,1666-1666,1677-1677,1683-1683,1687-1688,1691-1691,1694-1694,1699-1701,1703-1703,1707-1709,1711-1713,1715-1715,1717-1723,1730-1730,1735-1736,1745-1745,1750-1750,1752-1753,1755-1755,1761-1761,1782-1783,1791-1792,1799-1801,1805-1808,1811-1812,1823-1823,1825-1825,1835-1835,1839-1840,1858-1858,1861-1864,1871-1871,1875-1875,1900-1901,1911-1912,1914-1914,1918-1918,1924-1924,1927-1927,1935-1935,1947-1947,1954-1954,1958-1958,1971-1976,1981-1981,1984-1984,1998-2013,2020-2022,2025-2025,2030-2031,2033-2035,2038-2038,2040-2049,2062-2062,2065-2065,2067-2070,2080-2083,2086-2087,2095-2096,2099-2101,2103-2107,2111-2112,2115-2115,2119-2119,2121-2121,2124-2124,2126-2126,2134-2135,2142-2142,2144-2144,2148-2148,2150-2150,2160-2161,2170-2170,2179-2179,2187-2187,2190-2191,2196-2197,2200-2201,2203-2203,2222-2222,2224-2224,2232-2232,2241-2241,2250-2251,2253-2253,2260-2262,2265-2265,2269-2271,2280-2280,2288-2288,2291-2292,2300-2302,2304-2304,2312-2313,2323-2323,2325-2326,2330-2330,2335-2335,2340-2340,2366-2366,2371-2372,2381-2383,2391-2391,2393-2394,2399-2399,2401-2401,2418-2418,2425-2425,2433-2433,2435-2436,2438-2439,2449-2449,2456-2456,2463-2463,2472-2472,2492-2492,2500-2501,2505-2505,2522-2522,2525-2525,2531-2532,2550-2551,2557-2558,2567-2567,2580-2580,2583-2584,2598-2598,2600-2602,2604-2608,2622-2623,2628-2628,2631-2631,2638-2638,2644-2644,2691-2691,2700-2702,2706-2706,2710-2712,2717-2718,2723-2723,2725-2725,2728-2728,2734-2734,2800-2800,2804-2804,2806-2806,2809-2809,2811-2812,2847-2847,2850-2850,2869-2869,2875-2875,2882-2882,2888-2889,2898-2898,2901-2903,2908-2910,2920-2920,2930-2930,2957-2958,2967-2968,2973-2973,2984-2984,2987-2988,2991-2991,2997-2998,3000-3003,3005-3007,3011-3011,3013-3014,3017-3017,3023-3023,3025-3025,3030-3031,3050-3050,3052-3052,3057-3057,3062-3063,3071-3071,3077-3077,3080-3080,3089-3089,3102-3103,3118-3119,3121-3121,3128-3128,3146-3146,3162-3162,3167-3168,3190-3190,3200-3200,3210-3211,3220-3221,3240-3240,3260-3261,3263-3263,3268-3269,3280-3281,3283-3283,3291-3291,3299-3301,3304-3304,3306-3307,3310-3311,3319-3319,3322-3325,3333-3334,3351-3351,3362-3363,3365-3365,3367-3372,3374-3374,3376-3376,3388-3390,3396-3396,3399-3400,3404-3404,3410-3410,3414-3415,3419-3419,3425-3425,3430-3430,3439-3439,3443-3443,3456-3456,3476-3476,3479-3479,3483-3483,3485-3486,3493-3493,3497-3497,3503-3503,3505-3506,3511-3511,3513-3515,3517-3517,3519-3520,3526-3527,3530-3530,3532-3532,3546-3546,3551-3551,3577-3577,3580-3580,3586-3586,3599-3600,3602-3603,3621-3622,3632-3632,3636-3637,3652-3653,3656-3656,3658-3659,3663-3663,3669-3670,3672-3672,3680-3681,3683-3684,3689-3690,3697-3697,3700-3700,3703-3703,3712-3712,3728-3728,3731-3731,3737-3737,3742-3742,3749-3749,3765-3766,3784-3784,3787-3788,3790-3790,3792-3793,3795-3796,3798-3801,3803-3803,3806-3806,3808-3814,3817-3817,3820-3820,3823-3828,3830-3831,3837-3837,3839-3839,3842-3842,3846-3853,3856-3856,3859-3860,3863-3863,3868-3872,3876-3876,3878-3880,3882-3882,3888-3890,3897-3897,3899-3899,3901-3902,3904-3909,3911-3911,3913-3916,3918-3920,3922-3923,3928-3931,3935-3937,3940-3941,3943-3946,3948-3949,3952-3952,3956-3957,3961-3964,3967-3969,3971-3972,3975-3975,3979-3983,3986-3986,3989-4007,4009-4010,4016-4016,4020-4020,4022-4022,4024-4025,4029-4029,4035-4036,4039-4040,4045-4045,4056-4056,4058-4058,4065-4065,4080-4080,4087-4087,4090-4090,4096-4096,4100-4101,4111-4113,4118-4121,4125-4126,4129-4129,4135-4135,4141-4141,4143-4143,4147-4147,4158-4158,4161-4161,4164-4164,4174-4174,4190-4190,4192-4192,4200-4200,4206-4206,4220-4220,4224-4224,4234-4234,4242-4242,4252-4252,4262-4262,4279-4279,4294-4294,4297-4298,4300-4300,4302-4302,4321-4321,4325-4325,4328-4328,4333-4333,4342-4343,4355-4358,4369-4369,4374-4376,4384-4384,4388-4388,4401-4401,4407-4407,4414-4415,4418-4418,4430-4430,4433-4433,4442-4447,4449-4449,4454-4454,4464-4464,4471-4471,4476-4476,4516-4517,4530-4530,4534-4534,4545-4545,4550-4550,4555-4555,4558-4559,4567-4567,4570-4570,4599-4602,4606-4606,4609-4609,4644-4644,4649-4649,4658-4658,4662-4662,4665-4665,4687-4687,4689-4689,4700-4700,4712-4712,4745-4745,4760-4760,4767-4767,4770-4771,4778-4778,4793-4793,4800-4800,4819-4819,4848-4848,4859-4860,4875-4877,4881-4881,4899-4900,4903-4903,4912-4912,4931-4931,4949-4949,4998-5005,5009-5017,5020-5021,5023-5023,5030-5030,5033-5033,5040-5040,5050-5055,5060-5061,5063-5063,5066-5066,5070-5070,5074-5074,5080-5081,5087-5088,5090-5090,5095-5096,5098-5098,5100-5102,5111-5111,5114-5114,5120-5122,5125-5125,5133-5133,5137-5137,5147-5147,5151-5152,5190-5190,5200-5202,5212-5212,5214-5214,5219-5219,5221-5223,5225-5226,5233-5235,5242-5242,5250-5250,5252-5252,5259-5259,5261-5261,5269-5269,5279-5280,5291-5291,5298-5298,5339-5339,5347-5347,5353-5353,5357-5357,5370-5370,5377-5377,5405-5405,5414-5414,5423-5423,5431-5433,5440-5442,5444-5444,5457-5458,5473-5473,5475-5475,5500-5502,5510-5510,5520-5520,5544-5544,5550-5550,5552-5555,5557-5557,5560-5560,5566-5566,5631-5631,5633-5633,5666-5666,5678-5680,5718-5718,5730-5730,5800-5803,5807-5807,5810-5812,5815-5815,5818-5818,5822-5823,5825-5825,5850-5850,5859-5859,5862-5862,5868-5869,5877-5877,5899-5907,5909-5911,5914-5915,5918-5918,5922-5922,5925-5925,5938-5938,5940-5940,5950-5950,5952-5952,5959-5963,5968-5968,5981-5981,5987-5989,5998-6009,6017-6017,6025-6025,6050-6051,6059-6060,6068-6068,6100-6101,6103-6103,6106-6106,6112-6112,6123-6123,6129-6129,6156-6156,6203-6203,6222-6222,6247-6247,6346-6346,6389-6389,6481-6481,6500-6500,6502-6502,6504-6504,6510-6510,6520-6520,6543-6543,6547-6547,6550-6550,6565-6567,6580-6580,6600-6600,6646-6646,6662-6662,6666-6670,6689-6689,6692-6692,6699-6699,6711-6711,6732-6732,6779-6779,6788-6789,6792-6792,6839-6839,6881-6881,6896-6896,6901-6901,6969-6969,7000-7004,7007-7007,7010-7010,7019-7019,7024-7025,7050-7051,7070-7070,7080-7080,7100-7100,7103-7103,7106-7106,7123-7123,7200-7201,7241-7241,7272-7272,7278-7278,7281-7281,7402-7402,7435-7435,7438-7438,7443-7443,7496-7496,7512-7512,7625-7625,7627-7627,7676-7676,7725-7725,7741-7741,7744-7744,7749-7749,7770-7770,7777-7778,7800-7800,7878-7878,7900-7900,7911-7911,7913-7913,7920-7921,7929-7929,7937-7938,7999-8002,8007-8011,8015-8016,8019-8019,8021-8022,8031-8031,8042-8042,8045-8045,8050-8050,8080-8090,8093-8093,8095-8095,8097-8100,8118-8118,8180-8181,8189-8189,8192-8194,8200-8200,8222-8222,8254-8254,8290-8294,8300-8300,8333-8333,8383-8383,8385-8385,8400-8400,8402-8402,8443-8443,8481-8481,8500-8500,8540-8540,8600-8600,8648-8649,8651-8652,8654-8654,8675-8676,8686-8686,8701-8701,8765-8766,8800-8800,8873-8873,8877-8877,8888-8889,8899-8899,8987-8987,8994-8994,8996-8996,9000-9003,9009-9011,9040-9040,9050-9050,9071-9071,9080-9081,9090-9091,9098-9103,9110-9111,9152-9152,9191-9191,9197-9198,9200-9200,9207-9207,9220-9220,9290-9290,9409-9409,9415-9415,9418-9418,9443-9444,9485-9485,9500-9503,9535-9535,9575-9575,9593-9595,9600-9600,9618-9618,9621-9621,9643-9643,9666-9666,9673-9673,9815-9815,9876-9878,9898-9898,9900-9900,9914-9914,9917-9917,9929-9929,9941-9941,9943-9944,9968-9968,9988-9988,9992-9992,9998-10005,10008-10012,10022-10025,10034-10034,10058-10058,10082-10083,10160-10160,10180-10180,10215-10215,10243-10243,10566-10566,10616-10617,10621-10621,10626-10626,10628-10629,10778-10778,10873-10873,11110-11111,11967-11967,12000-12000,12006-12006,12021-12021,12059-12059,12174-12174,12215-12215,12262-12262,12265-12265,12345-12346,12380-12380,12452-12452,13456-13456,13722-13722,13724-13724,13782-13783,14000-14000,14238-14238,14441-14442,15000-15004,15402-15402,15660-15660,15742-15742,16000-16001,16012-16012,16016-16016,16018-16018,16080-16080,16113-16113,16705-16705,16800-16800,16851-16851,16992-16993,17595-17595,17877-17877,17988-17988,18000-18000,18018-18018,18040-18040,18101-18101,18264-18264,18988-18988,19101-19101,19283-19283,19315-19315,19350-19350,19780-19780,19801-19801,19842-19842,19900-19900,20000-20000,20002-20002,20005-20005,20031-20031,20221-20222,20828-20828,21571-21571,21792-21792,22222-22222,22939-22939,23052-23052,23502-23502,23796-23796,24444-24444,24800-24800,25734-25735,26000-26000,26214-26214,26470-26470,27000-27000,27352-27353,27355-27357,27715-27715,28201-28201,28211-28211,29672-29672,29831-29831,30000-30000,30005-30005,30704-30704,30718-30718,30951-30951,31038-31038,31337-31337,31727-31727,32768-32785,32791-32792,32803-32803,32816-32816,32822-32822,32835-32835,33354-33354,33453-33453,33554-33554,33899-33899,34571-34573,35500-35500,35513-35513,37839-37839,38037-38037,38185-38185,38188-38188,38292-38292,39136-39136,39376-39376,39659-39659,40000-40000,40193-40193,40811-40811,40911-40911,41064-41064,41511-41511,41523-41523,42510-42510,44176-44176,44334-44334,44442-44443,44501-44501,44709-44709,45100-45100,46200-46200,46996-46996,47544-47544,48080-48080,49152-49161,49163-49165,49167-49168,49171-49171,49175-49176,49186-49186,49195-49195,49236-49236,49400-49401,49999-50003,50006-50006,50050-50050,50300-50300,50389-50389,50500-50500,50636-50636,50800-50800,51103-51103,51191-51191,51413-51413,51493-51493,52660-52660,52673-52673,52710-52710,52735-52735,52822-52822,52847-52851,52853-52853,52869-52869,53211-53211,53313-53314,53535-53535,54045-54045,54328-54328,55020-55020,55055-55056,55555-55555,55576-55576,55600-55600,56737-56738,57294-57294,57665-57665,57797-57797,58001-58002,58080-58080,58630-58630,58632-58632,58838-58838,59110-59110,59200-59202,60020-60020,60123-60123,60146-60146,60443-60443,60642-60642,61532-61532,61613-61613,61900-61900,62078-62078,63331-63331,64623-64623,64680-64680,65000-65000,65129-65129,65310-65310, U:7-7,9-9,17-17,19-19,49-49,53-53,67-69,80-80,88-88,111-111,120-120,123-123,135-139,158-158,161-162,177-177,427-427,443-443,445-445,497-497,500-500,514-515,518-518,520-520,593-593,623-623,626-626,631-631,996-999,1022-1023,1025-1030,1433-1434,1645-1646,1701-1701,1718-1719,1812-1813,1900-1900,2000-2000,2048-2049,2222-2223,3283-3283,3456-3456,3703-3703,4444-4444,4500-4500,5000-5000,5060-5060,5353-5353,5632-5632,9200-9200,10000-10000,17185-17185,20031-20031,30718-30718,31337-31337,32768-32769,32771-32771,32815-32815,33281-33281,49152-49154,49156-49156,49181-49182,49185-49186,49188-49188,49190-49194,49200-49201",  # pylint: disable=C0301
     "WEB_SERVICES": "T:80-80,443-443",
 }
 
-logging.disable()
+logging.disable(logging.CRITICAL)
 
 
 class ValidatePortList(unittest.TestCase):
     def test_valid_port_list_no_range(self):
         """Test no port list provided"""
         self.assertFalse(valid_port_list(None))
         self.assertFalse(valid_port_list(""))
```

### Comparing `ospd_openvas-22.5.0/tests/test_preferencehandler.py` & `ospd_openvas-22.5.1/tests/test_preferencehandler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_protocol.py` & `ospd_openvas-22.5.1/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_scan_and_result.py` & `ospd_openvas-22.5.1/tests/test_scan_and_result.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_target_convert.py` & `ospd_openvas-22.5.1/tests/test_target_convert.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_vthelper.py` & `ospd_openvas-22.5.1/tests/test_vthelper.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_vts.py` & `ospd_openvas-22.5.1/tests/test_vts.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/tests/test_xml.py` & `ospd_openvas-22.5.1/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.0/PKG-INFO` & `ospd_openvas-22.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospd-openvas
-Version: 22.5.0
+Version: 22.5.1
 Summary: ospd based scanner for openvas
 Home-page: https://github.com/greenbone/ospd-openvas
 License: AGPL-3.0-or-later
 Keywords: openvas,Greenbone Vulnerability Management,Vulnerability Scanning,OSP,Open Scanner Protocol
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
```

