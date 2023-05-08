# Comparing `tmp/dataplicity-0.5.9a4.tar.gz` & `tmp/dataplicity-0.5.9a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataplicity-0.5.9a4.tar", last modified: Tue Jun 14 15:41:24 2022, max compression
+gzip compressed data, was "dataplicity-0.5.9a5.tar", last modified: Tue Jul 26 08:54:13 2022, max compression
```

## Comparing `dataplicity-0.5.9a4.tar` & `dataplicity-0.5.9a5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 15:41:24.390267 dataplicity-0.5.9a4/
--rw-rw-r--   0 root         (0) root         (0)     2028 2022-05-09 07:15:21.000000 dataplicity-0.5.9a4/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)       18 2022-05-09 07:15:21.000000 dataplicity-0.5.9a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1860 2022-06-14 15:41:24.386266 dataplicity-0.5.9a4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1346 2022-05-09 07:15:21.000000 dataplicity-0.5.9a4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 15:41:24.378266 dataplicity-0.5.9a4/dataplicity/
--rw-rw-r--   0 root         (0) root         (0)       34 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       30 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/__main__.py
--rw-rw-r--   0 root         (0) root         (0)      139 2022-06-14 15:41:18.000000 dataplicity-0.5.9a4/dataplicity/_version.py
--rw-rw-r--   0 root         (0) root         (0)     6242 2022-06-14 13:23:22.000000 dataplicity-0.5.9a4/dataplicity/app.py
--rw-rw-r--   0 root         (0) root         (0)    11746 2022-06-13 11:59:34.000000 dataplicity-0.5.9a4/dataplicity/client.py
--rw-rw-r--   0 root         (0) root         (0)     1166 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/clockcheck.py
--rw-rw-r--   0 root         (0) root         (0)     3061 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/compat.py
--rw-rw-r--   0 root         (0) root         (0)     1726 2022-05-05 10:48:04.000000 dataplicity-0.5.9a4/dataplicity/constants.py
--rw-rw-r--   0 root         (0) root         (0)     1547 2022-06-14 12:41:12.000000 dataplicity-0.5.9a4/dataplicity/device_meta.py
--rw-rw-r--   0 root         (0) root         (0)     2740 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/directory_scanner.py
--rw-rw-r--   0 root         (0) root         (0)     2527 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/disk_tools.py
--rw-rw-r--   0 root         (0) root         (0)     1747 2022-06-14 12:41:12.000000 dataplicity-0.5.9a4/dataplicity/iptool.py
--rw-rw-r--   0 root         (0) root         (0)     7719 2022-06-06 06:53:41.000000 dataplicity-0.5.9a4/dataplicity/jsonrpc.py
--rw-rw-r--   0 root         (0) root         (0)     2273 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/limiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 15:41:24.382266 dataplicity-0.5.9a4/dataplicity/m2m/
--rw-rw-r--   0 root         (0) root         (0)       68 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3753 2022-06-14 12:41:12.000000 dataplicity-0.5.9a4/dataplicity/m2m/bencode.py
--rw-rw-r--   0 root         (0) root         (0)     4496 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/commandservice.py
--rw-rw-r--   0 root         (0) root         (0)     3164 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/dispatcher.py
--rw-rw-r--   0 root         (0) root         (0)      631 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/echoservice.py
--rw-rw-r--   0 root         (0) root         (0)     3326 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/fileservice.py
--rw-rw-r--   0 root         (0) root         (0)     5855 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/packetbase.py
--rw-rw-r--   0 root         (0) root         (0)    11960 2022-06-13 11:59:34.000000 dataplicity-0.5.9a4/dataplicity/m2m/packets.py
--rw-rw-r--   0 root         (0) root         (0)     6517 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/proxy.py
--rw-rw-r--   0 root         (0) root         (0)     4559 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/m2m/remoteprocess.py
--rw-rw-r--   0 root         (0) root         (0)    16713 2022-05-25 11:41:01.000000 dataplicity-0.5.9a4/dataplicity/m2m/wsclient.py
--rw-rw-r--   0 root         (0) root         (0)     8587 2022-06-14 12:41:12.000000 dataplicity-0.5.9a4/dataplicity/m2mmanager.py
--rw-rw-r--   0 root         (0) root         (0)    12203 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/portforward.py
--rw-rw-r--   0 root         (0) root         (0)    14398 2022-06-14 15:37:14.000000 dataplicity-0.5.9a4/dataplicity/remote_directory.py
--rw-rw-r--   0 root         (0) root         (0)      903 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/rpi.py
--rw-rw-r--   0 root         (0) root         (0)     5662 2022-06-14 12:41:12.000000 dataplicity-0.5.9a4/dataplicity/scan_directory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 15:41:24.382266 dataplicity-0.5.9a4/dataplicity/security_extensions/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-23 10:33:10.000000 dataplicity-0.5.9a4/dataplicity/security_extensions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4476 2022-06-01 15:45:49.000000 dataplicity-0.5.9a4/dataplicity/security_extensions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 15:41:24.386266 dataplicity-0.5.9a4/dataplicity/security_extensions/commands/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-23 12:49:52.000000 dataplicity-0.5.9a4/dataplicity/security_extensions/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1218 2022-05-31 06:49:23.000000 dataplicity-0.5.9a4/dataplicity/security_extensions/commands/base.py
--rw-rw-r--   0 root         (0) root         (0)      134 2022-06-01 06:45:55.000000 dataplicity-0.5.9a4/dataplicity/security_extensions/commands/example.py
--rw-rw-r--   0 root         (0) root         (0)     2265 2022-06-01 16:01:10.000000 dataplicity-0.5.9a4/dataplicity/security_extensions/commands/netstat.py
--rw-rw-r--   0 root         (0) root         (0)     1549 2022-06-01 16:00:49.000000 dataplicity-0.5.9a4/dataplicity/security_extensions/commands/proc.py
--rw-rw-r--   0 root         (0) root         (0)      772 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/subcommand.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 15:41:24.386266 dataplicity-0.5.9a4/dataplicity/subcommands/
--rw-rw-r--   0 root         (0) root         (0)       40 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/subcommands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      325 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/subcommands/run.py
--rw-rw-r--   0 root         (0) root         (0)      319 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/subcommands/version.py
--rw-rw-r--   0 root         (0) root         (0)     1244 2022-03-29 14:15:54.000000 dataplicity-0.5.9a4/dataplicity/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-14 15:41:24.378266 dataplicity-0.5.9a4/dataplicity.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     1860 2022-06-14 15:41:24.000000 dataplicity-0.5.9a4/dataplicity.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1569 2022-06-14 15:41:24.000000 dataplicity-0.5.9a4/dataplicity.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-06-14 15:41:24.000000 dataplicity-0.5.9a4/dataplicity.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       54 2022-06-14 15:41:24.000000 dataplicity-0.5.9a4/dataplicity.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       40 2022-06-14 15:41:24.000000 dataplicity-0.5.9a4/dataplicity.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       12 2022-06-14 15:41:24.000000 dataplicity-0.5.9a4/dataplicity.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-06-13 09:21:45.000000 dataplicity-0.5.9a4/dataplicity.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-14 15:41:24.390267 dataplicity-0.5.9a4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      845 2022-05-09 07:15:21.000000 dataplicity-0.5.9a4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-26 08:54:13.314612 dataplicity-0.5.9a5/
+-rw-rw-r--   0 root         (0) root         (0)     2028 2022-05-09 07:15:21.000000 dataplicity-0.5.9a5/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       18 2022-05-09 07:15:21.000000 dataplicity-0.5.9a5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1860 2022-07-26 08:54:13.314612 dataplicity-0.5.9a5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1346 2022-05-09 07:15:21.000000 dataplicity-0.5.9a5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-26 08:54:13.310612 dataplicity-0.5.9a5/dataplicity/
+-rw-rw-r--   0 root         (0) root         (0)       34 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       30 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)      139 2022-07-26 08:49:49.000000 dataplicity-0.5.9a5/dataplicity/_version.py
+-rw-rw-r--   0 root         (0) root         (0)     6242 2022-06-14 13:23:22.000000 dataplicity-0.5.9a5/dataplicity/app.py
+-rw-rw-r--   0 root         (0) root         (0)    11746 2022-06-13 11:59:34.000000 dataplicity-0.5.9a5/dataplicity/client.py
+-rw-rw-r--   0 root         (0) root         (0)     1166 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/clockcheck.py
+-rw-rw-r--   0 root         (0) root         (0)     3061 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/compat.py
+-rw-rw-r--   0 root         (0) root         (0)     1726 2022-05-05 10:48:04.000000 dataplicity-0.5.9a5/dataplicity/constants.py
+-rw-rw-r--   0 root         (0) root         (0)     1547 2022-06-14 12:41:12.000000 dataplicity-0.5.9a5/dataplicity/device_meta.py
+-rw-rw-r--   0 root         (0) root         (0)     2740 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/directory_scanner.py
+-rw-rw-r--   0 root         (0) root         (0)     2527 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/disk_tools.py
+-rw-rw-r--   0 root         (0) root         (0)     1747 2022-06-14 12:41:12.000000 dataplicity-0.5.9a5/dataplicity/iptool.py
+-rw-rw-r--   0 root         (0) root         (0)     7719 2022-06-06 06:53:41.000000 dataplicity-0.5.9a5/dataplicity/jsonrpc.py
+-rw-rw-r--   0 root         (0) root         (0)     2273 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/limiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-26 08:54:13.314612 dataplicity-0.5.9a5/dataplicity/m2m/
+-rw-rw-r--   0 root         (0) root         (0)       68 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/m2m/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3753 2022-06-14 12:41:12.000000 dataplicity-0.5.9a5/dataplicity/m2m/bencode.py
+-rw-rw-r--   0 root         (0) root         (0)     4496 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/m2m/commandservice.py
+-rw-rw-r--   0 root         (0) root         (0)     3164 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/m2m/dispatcher.py
+-rw-rw-r--   0 root         (0) root         (0)      631 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/m2m/echoservice.py
+-rw-rw-r--   0 root         (0) root         (0)     3326 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/m2m/fileservice.py
+-rw-rw-r--   0 root         (0) root         (0)     5855 2022-07-19 08:23:14.000000 dataplicity-0.5.9a5/dataplicity/m2m/packetbase.py
+-rw-rw-r--   0 root         (0) root         (0)    11989 2022-07-18 10:15:31.000000 dataplicity-0.5.9a5/dataplicity/m2m/packets.py
+-rw-rw-r--   0 root         (0) root         (0)     6517 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/m2m/proxy.py
+-rw-rw-r--   0 root         (0) root         (0)     4559 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/m2m/remoteprocess.py
+-rw-rw-r--   0 root         (0) root         (0)    16763 2022-07-20 07:26:53.000000 dataplicity-0.5.9a5/dataplicity/m2m/wsclient.py
+-rw-rw-r--   0 root         (0) root         (0)     8587 2022-06-14 12:41:12.000000 dataplicity-0.5.9a5/dataplicity/m2mmanager.py
+-rw-rw-r--   0 root         (0) root         (0)    12203 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/portforward.py
+-rw-rw-r--   0 root         (0) root         (0)    14528 2022-07-26 08:45:58.000000 dataplicity-0.5.9a5/dataplicity/remote_directory.py
+-rw-rw-r--   0 root         (0) root         (0)      903 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/rpi.py
+-rw-rw-r--   0 root         (0) root         (0)     5662 2022-06-14 12:41:12.000000 dataplicity-0.5.9a5/dataplicity/scan_directory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-26 08:54:13.314612 dataplicity-0.5.9a5/dataplicity/security_extensions/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-05-23 10:33:10.000000 dataplicity-0.5.9a5/dataplicity/security_extensions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4476 2022-06-01 15:45:49.000000 dataplicity-0.5.9a5/dataplicity/security_extensions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-26 08:54:13.314612 dataplicity-0.5.9a5/dataplicity/security_extensions/commands/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-05-23 12:49:52.000000 dataplicity-0.5.9a5/dataplicity/security_extensions/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1218 2022-05-31 06:49:23.000000 dataplicity-0.5.9a5/dataplicity/security_extensions/commands/base.py
+-rw-rw-r--   0 root         (0) root         (0)      134 2022-06-01 06:45:55.000000 dataplicity-0.5.9a5/dataplicity/security_extensions/commands/example.py
+-rw-rw-r--   0 root         (0) root         (0)     2265 2022-06-01 16:01:10.000000 dataplicity-0.5.9a5/dataplicity/security_extensions/commands/netstat.py
+-rw-rw-r--   0 root         (0) root         (0)     1549 2022-06-01 16:00:49.000000 dataplicity-0.5.9a5/dataplicity/security_extensions/commands/proc.py
+-rw-rw-r--   0 root         (0) root         (0)      772 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/subcommand.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-26 08:54:13.314612 dataplicity-0.5.9a5/dataplicity/subcommands/
+-rw-rw-r--   0 root         (0) root         (0)       40 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/subcommands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      325 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/subcommands/run.py
+-rw-rw-r--   0 root         (0) root         (0)      319 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/subcommands/version.py
+-rw-rw-r--   0 root         (0) root         (0)     1244 2022-03-29 14:15:54.000000 dataplicity-0.5.9a5/dataplicity/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-26 08:54:13.310612 dataplicity-0.5.9a5/dataplicity.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     1860 2022-07-26 08:54:13.000000 dataplicity-0.5.9a5/dataplicity.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1569 2022-07-26 08:54:13.000000 dataplicity-0.5.9a5/dataplicity.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-07-26 08:54:13.000000 dataplicity-0.5.9a5/dataplicity.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       54 2022-07-26 08:54:13.000000 dataplicity-0.5.9a5/dataplicity.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)       40 2022-07-26 08:54:13.000000 dataplicity-0.5.9a5/dataplicity.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       12 2022-07-26 08:54:13.000000 dataplicity-0.5.9a5/dataplicity.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-06-13 09:21:45.000000 dataplicity-0.5.9a5/dataplicity.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2022-07-26 08:54:13.314612 dataplicity-0.5.9a5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      845 2022-05-09 07:15:21.000000 dataplicity-0.5.9a5/setup.py
```

### Comparing `dataplicity-0.5.9a4/LICENSE.txt` & `dataplicity-0.5.9a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/PKG-INFO` & `dataplicity-0.5.9a5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dataplicity
-Version: 0.5.9a4
+Version: 0.5.9a5
 Summary: Platform for connected devices
 Home-page: https://www.dataplicity.com
 Author: WildFoundry
 Author-email: support@dataplicity.com
 License: UNKNOWN
 Description: ## About 
         Dataplicity agent is a Python based script which allows remote connection to your device via dataplicity.com.
```

### Comparing `dataplicity-0.5.9a4/README.md` & `dataplicity-0.5.9a5/README.md`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/app.py` & `dataplicity-0.5.9a5/dataplicity/app.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/client.py` & `dataplicity-0.5.9a5/dataplicity/client.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/clockcheck.py` & `dataplicity-0.5.9a5/dataplicity/clockcheck.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/compat.py` & `dataplicity-0.5.9a5/dataplicity/compat.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/constants.py` & `dataplicity-0.5.9a5/dataplicity/constants.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/device_meta.py` & `dataplicity-0.5.9a5/dataplicity/device_meta.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/directory_scanner.py` & `dataplicity-0.5.9a5/dataplicity/directory_scanner.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/disk_tools.py` & `dataplicity-0.5.9a5/dataplicity/disk_tools.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/iptool.py` & `dataplicity-0.5.9a5/dataplicity/iptool.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/jsonrpc.py` & `dataplicity-0.5.9a5/dataplicity/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/limiter.py` & `dataplicity-0.5.9a5/dataplicity/limiter.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/bencode.py` & `dataplicity-0.5.9a5/dataplicity/m2m/bencode.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/commandservice.py` & `dataplicity-0.5.9a5/dataplicity/m2m/commandservice.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/dispatcher.py` & `dataplicity-0.5.9a5/dataplicity/m2m/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/echoservice.py` & `dataplicity-0.5.9a5/dataplicity/m2m/echoservice.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/fileservice.py` & `dataplicity-0.5.9a5/dataplicity/m2m/fileservice.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/packetbase.py` & `dataplicity-0.5.9a5/dataplicity/m2m/packetbase.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/packets.py` & `dataplicity-0.5.9a5/dataplicity/m2m/packets.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,12 +508,13 @@
 
 
 class WriteRemoteFileResult(M2MPacket):
     type = PacketType.write_remote_file_result
     attributes = [
         ("id", bytes),
         ("position", int),
+        ("chunk_size", int),
         ("device_path", bytes),
         ("fail", int),
         ("fail_reason", bytes),
     ]
```

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/proxy.py` & `dataplicity-0.5.9a5/dataplicity/m2m/proxy.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/remoteprocess.py` & `dataplicity-0.5.9a5/dataplicity/m2m/remoteprocess.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/m2m/wsclient.py` & `dataplicity-0.5.9a5/dataplicity/m2m/wsclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,17 @@
         self.url = url
         self.remote_directory = remote_directory
         _user_agent = "Agent/{} {}".format(__version__, LOMOND_USER_AGENT)
         self.websocket = WebSocket(url, agent=_user_agent, compress=True)
         self.channel_callback = channel_callback
         self.control_callback = control_callback
 
+
+        self._write_disk_lock = threading.Lock()
+
         self._closed = False
         self.identity = uuid
         self.channels = {}
         self.last_packet_time = time.time()
 
         self.callback_lock = threading.RLock()
         self.write_lock = threading.Lock()
@@ -487,12 +490,11 @@
 
     @expose(PacketType.write_remote_file)
     def on_write_remote_file(
         self, packet_type, id, path, device_path, offset, data, final
     ):
         # type: (PacketType, bytes, bytes, bytes, int, bytes, int) -> None
         """Server wants us to write to the filesystem."""
-
         self.remote_directory.on_write_remote_file(
             self, id, path, device_path, offset, data, final
         )
```

### Comparing `dataplicity-0.5.9a4/dataplicity/m2mmanager.py` & `dataplicity-0.5.9a5/dataplicity/m2mmanager.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/portforward.py` & `dataplicity-0.5.9a5/dataplicity/portforward.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/remote_directory.py` & `dataplicity-0.5.9a5/dataplicity/remote_directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import logging
 import shutil
 import os
 import os.path
 import shutil
 import tempfile
 import typing
@@ -11,14 +12,17 @@
 
 from . import disk_tools
 from .compat import PY2
 from .directory_scanner import DirectoryScanner
 from .m2m.packets import PacketType
 from .m2m.wsclient import WSClient
 
+import threading, time, random
+
+
 # Amount of free space (bytes) to leave on disk
 FREE_SPACE_MARGIN = 50 * 1000 * 1000
 
 
 log = logging.getLogger("agent")
 
 
@@ -121,15 +125,15 @@
             log.debug("%r created %s", self, dir_path)
 
         device_path = os.path.join(dir_path, id)
 
         # Create the file
         # This could fail for a variety of reasons
         # Exceptions must be caught by the caller
-        with open(device_path, "wb"):
+        with open(device_path, "a+"):
             pass
 
         return device_path
 
     def add_upload(self, path, upload_id):
         # type: (Text, Text) -> int
         """Add a new upload.
@@ -301,25 +305,31 @@
                 fail=0,
                 fail_reason="",
             )
 
     def on_write_remote_file(self, client, id, path, device_path, offset, data, final):
         # type: (WSClient, bytes, bytes, bytes, int, bytes, int) -> None
         """Write data from server to temporary file."""
+        print("Received ",
+              id, path, "offset", offset, "len", len(data), "final", final, datetime.datetime.now()
+        
+        )
         write_device_path = device_path.decode("utf-8")
         try:
             # If we haven't set a device_path allocate a temp location
             if not write_device_path:
                 write_device_path = self.add_download(id.decode("utf-8"))
         except Exception as error:
             log.exception("error adding download")
             # Couldn't create temporary location, tell server
             client.send(
                 PacketType.write_remote_file_result,
                 id,
+                0,
+                0,
                 device_path,
                 1,
                 str(error).encode("utf-8", "replace"),
             )
             return
 
         device_path = write_device_path.encode("utf-8")
@@ -328,68 +338,66 @@
             try:
                 # Write the data at the given offset
                 log.debug("writing %i bytes to %s offset=%i", len(data), write_device_path, offset)
                 with open(write_device_path, "r+b") as download_file:
                     download_file.seek(offset)
                     download_file.write(data)
             except Exception as error:
-                # Error writing chunk, tell server
-                log.exception("error writing download")
+                # Maybe file has been already deleted as there are multiple downloads.
+                log.debug("error writing download")
                 client.send(
                     PacketType.write_remote_file_result,
                     id,
                     offset,
+                    len(data),
                     device_path,
                     2,
                     str(error).encode("utf-8", "replace"),
                 )
                 try:
                     log.debug("removing %s", write_device_path)
                     os.remove(write_device_path)
                 except:
-                    log.exception("failed to remove %r", write_device_path)
+                    # Maybe file has been already deleted as there are multiple downloads.
+                    log.debug("failed to remove %r", write_device_path)
                 return
 
         if final:
             try:
-                print("FINAL1 ", type(write_device_path), type(path))
                 write_device_path = write_device_path.encode("utf-8")
-                print("FINAL2 ", type(write_device_path), type(path))
                 client.remote_directory.copy_download(write_device_path, path)
             except Exception as error:
                 log.exception("failed to copy download %s %s", write_device_path, path)
                 client.send(
                     PacketType.write_remote_file_result,
                     id,
                     offset,
+                    len(data),
                     device_path,
                     3,
                     str(error).encode("utf-8", "replace"),
                 )
                 return
 
         # Return a success response
         client.send(
             PacketType.write_remote_file_result,
             id,
             offset + len(data),
+            len(data),
             device_path,
             0,
             b"",
         )
 
     def copy_download(self, device_path, path):
         # type (Text, Text) -> None
         """Copy a download in to the remote directory"""
-        print("COPY self.path", self.path)
-        print("COPY path", path)
         if isinstance(path, bytes):
             path = path.decode("utf-8")
-        #if isinstance(self.path, str):
-        #    self.path = self.path.encode("utf-8")
         destination_path = os.path.join(self.path, path.lstrip("/"))
         dirname, filename = os.path.split(destination_path)
         if not os.path.isdir(dirname):
             dirname = self.path
 
         basename, ext = os.path.splitext(filename)
```

### Comparing `dataplicity-0.5.9a4/dataplicity/rpi.py` & `dataplicity-0.5.9a5/dataplicity/rpi.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/scan_directory.py` & `dataplicity-0.5.9a5/dataplicity/scan_directory.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/security_extensions/base.py` & `dataplicity-0.5.9a5/dataplicity/security_extensions/base.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/security_extensions/commands/base.py` & `dataplicity-0.5.9a5/dataplicity/security_extensions/commands/base.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/security_extensions/commands/netstat.py` & `dataplicity-0.5.9a5/dataplicity/security_extensions/commands/netstat.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/security_extensions/commands/proc.py` & `dataplicity-0.5.9a5/dataplicity/security_extensions/commands/proc.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/subcommand.py` & `dataplicity-0.5.9a5/dataplicity/subcommand.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity/tags.py` & `dataplicity-0.5.9a5/dataplicity/tags.py`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/dataplicity.egg-info/PKG-INFO` & `dataplicity-0.5.9a5/dataplicity.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dataplicity
-Version: 0.5.9a4
+Version: 0.5.9a5
 Summary: Platform for connected devices
 Home-page: https://www.dataplicity.com
 Author: WildFoundry
 Author-email: support@dataplicity.com
 License: UNKNOWN
 Description: ## About 
         Dataplicity agent is a Python based script which allows remote connection to your device via dataplicity.com.
```

### Comparing `dataplicity-0.5.9a4/dataplicity.egg-info/SOURCES.txt` & `dataplicity-0.5.9a5/dataplicity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataplicity-0.5.9a4/setup.py` & `dataplicity-0.5.9a5/setup.py`

 * *Files identical despite different names*

