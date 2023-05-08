# Comparing `tmp/rpcclient-3.15.4.tar.gz` & `tmp/rpcclient-3.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-3.15.4.tar", last modified: Mon Apr 24 06:57:29 2023, max compression
+gzip compressed data, was "rpcclient-3.15.5.tar", last modified: Mon May  8 10:55:33 2023, max compression
```

## Comparing `rpcclient-3.15.4.tar` & `rpcclient-3.15.5.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 06:57:20.000000 rpcclient-3.15.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-24 06:57:29.719548 rpcclient-3.15.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 06:57:20.000000 rpcclient-3.15.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.715548 rpcclient-3.15.4/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    37668 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.715548 rpcclient-3.15.4/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:57:29.719548 rpcclient-3.15.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-24 06:57:20.000000 rpcclient-3.15.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-08 10:55:23.000000 rpcclient-3.15.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-08 10:55:33.732786 rpcclient-3.15.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 10:55:23.000000 rpcclient-3.15.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.728786 rpcclient-3.15.5/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.728786 rpcclient-3.15.5/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37668 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.732786 rpcclient-3.15.5/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-08 10:55:23.000000 rpcclient-3.15.5/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:33.728786 rpcclient-3.15.5/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 10:55:33.000000 rpcclient-3.15.5/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 10:55:33.732786 rpcclient-3.15.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-08 10:55:23.000000 rpcclient-3.15.5/setup.py
```

### Comparing `rpcclient-3.15.4/LICENSE` & `rpcclient-3.15.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/PKG-INFO` & `rpcclient-3.15.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.15.4
+Version: 3.15.5
 Summary: rpcclient for connecting with the rpcserver
 Home-page: https://github.com/doronz88/rpc-project
 Author: DoronZ
 Author-email: doron88@gmail.com
 License: GNU GENERAL PUBLIC LICENSE - Version 3, 29 June 2007
 Project-URL: rpc-project, https://github.com/doronz88/rpc-project
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `rpcclient-3.15.4/rpcclient/__main__.py` & `rpcclient-3.15.5/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/client.py` & `rpcclient-3.15.5/rpcclient/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/client_factory.py` & `rpcclient-3.15.5/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/bluetooth.py` & `rpcclient-3.15.5/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/cfpreferences.py` & `rpcclient-3.15.5/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/client.py` & `rpcclient-3.15.5/rpcclient/darwin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from rpcclient.darwin.hid import Hid
 from rpcclient.darwin.ioregistry import IORegistry
 from rpcclient.darwin.keychain import Keychain
 from rpcclient.darwin.location import Location
 from rpcclient.darwin.media import DarwinMedia
 from rpcclient.darwin.network import DarwinNetwork
 from rpcclient.darwin.objective_c_symbol import ObjectiveCSymbol
+from rpcclient.darwin.power import Power
 from rpcclient.darwin.preferences import Preferences
 from rpcclient.darwin.processes import DarwinProcesses
 from rpcclient.darwin.structs import utsname
 from rpcclient.darwin.symbol import DarwinSymbol
 from rpcclient.darwin.syslog import Syslog
 from rpcclient.darwin.time import Time
 from rpcclient.darwin.xpc import Xpc
@@ -86,14 +87,15 @@
         self.time = Time(self)
         self.hid = Hid(self)
         self.lief = DarwinLief(self)
         self.bluetooth = Bluetooth(self)
         self.core_graphics = CoreGraphics(self)
         self.keychain = Keychain(self)
         self.network = DarwinNetwork(self)
+        self.power = Power(self)
         self.loaded_objc_classes = []
         self._NSPropertyListSerialization = self.objc_get_class('NSPropertyListSerialization')
         self._CFNullTypeID = self.symbols.CFNullGetTypeID()
 
     @property
     def modules(self) -> typing.List[str]:
         m = []
```

### Comparing `rpcclient-3.15.4/rpcclient/darwin/consts.py` & `rpcclient-3.15.5/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/core_graphics.py` & `rpcclient-3.15.5/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/crash_reports.py` & `rpcclient-3.15.5/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/darwin_lief.py` & `rpcclient-3.15.5/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/fs.py` & `rpcclient-3.15.5/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/hid.py` & `rpcclient-3.15.5/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/ioregistry.py` & `rpcclient-3.15.5/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/keychain.py` & `rpcclient-3.15.5/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/location.py` & `rpcclient-3.15.5/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/media.py` & `rpcclient-3.15.5/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/network.py` & `rpcclient-3.15.5/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/objc.py` & `rpcclient-3.15.5/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/objective_c_class.py` & `rpcclient-3.15.5/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-3.15.5/rpcclient/darwin/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/processes.py` & `rpcclient-3.15.5/rpcclient/darwin/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/reports.py` & `rpcclient-3.15.5/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/scpreferences.py` & `rpcclient-3.15.5/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/structs.py` & `rpcclient-3.15.5/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/symbol.py` & `rpcclient-3.15.5/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/syslog.py` & `rpcclient-3.15.5/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/time.py` & `rpcclient-3.15.5/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/darwin/xpc.py` & `rpcclient-3.15.5/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/exceptions.py` & `rpcclient-3.15.5/rpcclient/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,7 +166,12 @@
     """ XPC-related error """
     pass
 
 
 class RpcXpcSerializationError(RpcXpcError):
     """ Failed to serialize/deserialize XPC message """
     pass
+
+
+class RpcSetDeveloperModeError(BadReturnValueError):
+    """ Failed to set Developer Mode """
+    pass
```

### Comparing `rpcclient-3.15.4/rpcclient/fs.py` & `rpcclient-3.15.5/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/accessibility.py` & `rpcclient-3.15.5/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/backlight.py` & `rpcclient-3.15.5/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/client.py` & `rpcclient-3.15.5/rpcclient/ios/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 
 from rpcclient.darwin.client import DarwinClient
 from rpcclient.darwin.reports import Reports
 from rpcclient.ios.accessibility import Accessibility
+from rpcclient.ios.amfi import Amfi
 from rpcclient.ios.backlight import Backlight
 from rpcclient.ios.lockdown import Lockdown
 from rpcclient.ios.mobile_gestalt import MobileGestalt
 from rpcclient.ios.screen_capture import ScreenCapture
 from rpcclient.ios.sprinboard import SpringBoard
 from rpcclient.ios.telephony import Telephony
 from rpcclient.ios.wifi import IosWifi
@@ -23,14 +24,15 @@
         self.mobile_gestalt = MobileGestalt(self)
         self.lockdown = Lockdown(self)
         self.telephony = Telephony(self)
         self.screen_capture = ScreenCapture(self)
         self.accessibility = Accessibility(self)
         self.wifi = IosWifi(self)
         self.springboard = SpringBoard(self)
+        self.amfi = Amfi(self)
         self._radio_preferences = self.symbols.objc_getClass('RadiosPreferences').objc_call('new')
 
     @property
     def roots(self) -> typing.List[str]:
         """ get a list of all accessible darwin roots when used for lookup of files/preferences/... """
         return super().roots + ['/var/mobile']
```

### Comparing `rpcclient-3.15.4/rpcclient/ios/lockdown.py` & `rpcclient-3.15.5/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/mobile_gestalt.py` & `rpcclient-3.15.5/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/screen_capture.py` & `rpcclient-3.15.5/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/sprinboard.py` & `rpcclient-3.15.5/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/telephony.py` & `rpcclient-3.15.5/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/ios/wifi.py` & `rpcclient-3.15.5/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/lief.py` & `rpcclient-3.15.5/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/linux/client.py` & `rpcclient-3.15.5/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/linux/structs.py` & `rpcclient-3.15.5/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/macos/apple_script.py` & `rpcclient-3.15.5/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/macos/client.py` & `rpcclient-3.15.5/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/network.py` & `rpcclient-3.15.5/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/processes.py` & `rpcclient-3.15.5/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/protocol.py` & `rpcclient-3.15.5/rpcclient/protocol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/structs/consts.py` & `rpcclient-3.15.5/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/structs/generic.py` & `rpcclient-3.15.5/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/symbol.py` & `rpcclient-3.15.5/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/symbols_jar.py` & `rpcclient-3.15.5/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/sysctl.py` & `rpcclient-3.15.5/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient/xonshrc.py` & `rpcclient-3.15.5/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.4/rpcclient.egg-info/PKG-INFO` & `rpcclient-3.15.5/rpcclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.15.4
+Version: 3.15.5
 Summary: rpcclient for connecting with the rpcserver
 Home-page: https://github.com/doronz88/rpc-project
 Author: DoronZ
 Author-email: doron88@gmail.com
 License: GNU GENERAL PUBLIC LICENSE - Version 3, 29 June 2007
 Project-URL: rpc-project, https://github.com/doronz88/rpc-project
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `rpcclient-3.15.4/rpcclient.egg-info/SOURCES.txt` & `rpcclient-3.15.5/rpcclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,25 +37,27 @@
 rpcclient/darwin/keychain.py
 rpcclient/darwin/location.py
 rpcclient/darwin/media.py
 rpcclient/darwin/network.py
 rpcclient/darwin/objc.py
 rpcclient/darwin/objective_c_class.py
 rpcclient/darwin/objective_c_symbol.py
+rpcclient/darwin/power.py
 rpcclient/darwin/preferences.py
 rpcclient/darwin/processes.py
 rpcclient/darwin/reports.py
 rpcclient/darwin/scpreferences.py
 rpcclient/darwin/structs.py
 rpcclient/darwin/symbol.py
 rpcclient/darwin/syslog.py
 rpcclient/darwin/time.py
 rpcclient/darwin/xpc.py
 rpcclient/ios/__init__.py
 rpcclient/ios/accessibility.py
+rpcclient/ios/amfi.py
 rpcclient/ios/backlight.py
 rpcclient/ios/client.py
 rpcclient/ios/lockdown.py
 rpcclient/ios/mobile_gestalt.py
 rpcclient/ios/screen_capture.py
 rpcclient/ios/sprinboard.py
 rpcclient/ios/telephony.py
```

### Comparing `rpcclient-3.15.4/setup.py` & `rpcclient-3.15.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 BASE_DIR = Path(__file__).parent.resolve(strict=True)
-VERSION = '3.15.4'
+VERSION = '3.15.5'
 PACKAGE_NAME = 'rpcclient'
 PACKAGES = [p for p in find_packages() if not p.startswith('tests')]
 
 
 def parse_requirements():
     reqs = []
     with open(BASE_DIR / 'requirements.txt', 'r') as fd:
```

