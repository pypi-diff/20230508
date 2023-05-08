# Comparing `tmp/pythonsdk-0.5.0.tar.gz` & `tmp/pythonsdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsdk-0.5.0.tar", last modified: Sat Apr 29 21:37:37 2023, max compression
+gzip compressed data, was "pythonsdk-0.6.0.tar", last modified: Mon May  8 09:45:08 2023, max compression
```

## Comparing `pythonsdk-0.5.0.tar` & `pythonsdk-0.6.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.114232 pythonsdk-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/_fmt.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/bin/_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_value_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_config_value_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_optional_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/config/_string_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/encoding/_base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/log/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.118232 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_rotating_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/sentinel/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/sentinel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/sentinel/_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/testing/_prepackaged_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/utils/_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 21:37:31.000000 pythonsdk-0.5.0/src/python_sdk/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/python_sdk/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/src/python_sdk/versioning/_version_file_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:37:37.122232 pythonsdk-0.5.0/src/pythonsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 21:37:37.000000 pythonsdk-0.5.0/src/pythonsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 21:37:08.000000 pythonsdk-0.5.0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.424361 pythonsdk-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.424361 pythonsdk-0.6.0/src/python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.424361 pythonsdk-0.6.0/src/python_sdk/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/bin/_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_value_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_config_value_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_optional_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/config/_string_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/encoding/_base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_rotating_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.428362 pythonsdk-0.6.0/src/python_sdk/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/sentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/sentinel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/sentinel/_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/testing/_prepackaged_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/utils/_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 09:45:02.000000 pythonsdk-0.6.0/src/python_sdk/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/python_sdk/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/src/python_sdk/versioning/_version_file_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:45:08.432361 pythonsdk-0.6.0/src/pythonsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 09:45:08.000000 pythonsdk-0.6.0/src/pythonsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 09:44:38.000000 pythonsdk-0.6.0/version
```

### Comparing `pythonsdk-0.5.0/LICENSE` & `pythonsdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/PKG-INFO` & `pythonsdk-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pythonsdk-0.5.0/pyproject.toml` & `pythonsdk-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/_cli/_cli.py` & `pythonsdk-0.6.0/src/python_sdk/_cli/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 _CLI_DEPENDENCIES_INSTALLED: bool = all([shutil.which("black"), shutil.which("isort")])
 
 
 def app() -> None:
     if not _CLI_DEPENDENCIES_INSTALLED:
         print(
             "CLI dependencies are not installed. "
-            "Please run `pip install pythonsdk[cli]` to unlock this functionality."
+            "Please run `pip install pythonsdk[cli]` to unlock this functionality.",
+            file=sys.stderr,
         )
         sys.exit(1)
 
     args = _parser().parse_args()
 
     if args.command == "fmt":
         _fmt.fmt(target=args.target, check=args.check)
     elif args.command == "version":
         _version.version()
     else:
-        print(f"Unknown command: {args.command}")
+        print(f"Unknown command: {args.command}", file=sys.stderr)
         sys.exit(1)
 
 
 def _parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(prog="python-sdk", description="Python SDK CLI.")
     subparsers = parser.add_subparsers(title="Commands", dest="command")
     _fmt_parser(subparsers=subparsers)
```

### Comparing `pythonsdk-0.5.0/src/python_sdk/_cli/_fmt.py` & `pythonsdk-0.6.0/src/python_sdk/_cli/_fmt.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/bin/_call.py` & `pythonsdk-0.6.0/src/python_sdk/bin/_call.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/config/__init__.py` & `pythonsdk-0.6.0/src/python_sdk/config/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,7 +18,9 @@
 from python_sdk.config._config_value_validators import ConfigValueValidator as ConfigValueValidator
 from python_sdk.config._config_value_validators import ValidateDirectoryExists as ValidateDirectoryExists
 from python_sdk.config._config_value_validators import ValidateFileExists as ValidateFileExists
 from python_sdk.config._config_value_validators import ValidateFileType as ValidateFileType
 from python_sdk.config._config_value_validators import ValidatePathIsExecutable as ValidatePathIsExecutable
 from python_sdk.config._config_value_validators import ValidatePathIsReadable as ValidatePathIsReadable
 from python_sdk.config._config_value_validators import ValidatePathIsWritable as ValidatePathIsWritable
+from python_sdk.config._flags import disable_on_access_config_reloading as disable_on_access_config_reloading
+from python_sdk.config._flags import enable_on_access_config_reloading as enable_on_access_config_reloading
```

### Comparing `pythonsdk-0.5.0/src/python_sdk/config/_config.py` & `pythonsdk-0.6.0/src/python_sdk/config/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import python_sdk
 from python_sdk import sentinel
 from python_sdk.config import _config_option
 from python_sdk.config import _config_sources
 from python_sdk.config import _config_value_types
 from python_sdk.config import _config_value_validators
+from python_sdk.config import _flags
 
 if typing.TYPE_CHECKING:
     from python_sdk.config import _config_validators
 
 Unset: sentinel.Sentinel = sentinel.Sentinel("Unset")
 
 
@@ -37,14 +38,18 @@
         if not isinstance(attribute, _config_option.ConfigOption):
             return attribute
 
         if cls.meta.lazy_load_config and not cls.meta.loaded:
             cls._load_config()
             attribute = super().__getattribute__(item)
 
+        if _flags.ENABLE_ON_ACCESS_CONFIG_RELOADING:
+            cls.reload_config()
+            attribute = super().__getattribute__(item)
+
         return attribute.value
 
 
 @dataclasses.dataclass
 class _ConfigMeta:
     name: str
     description: str
```

### Comparing `pythonsdk-0.5.0/src/python_sdk/config/_config_option.py` & `pythonsdk-0.6.0/src/python_sdk/config/_config_option.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     prefix: str
     description: str
     datatype: type["_config_value_types.ConfigValueType"]
     default: typing.Union["_config_value_types.ConfigValueType", sentinel.Sentinel, None]
     validators: list["_config_value_validators.ConfigValueValidator"]
     hardcoded: bool
     is_sensitive: bool
+    reload_compatible: bool
     _value: typing.Union["_config_value_types.ConfigValueType", sentinel.Sentinel, None]
     _encoded_value: str | sentinel.Sentinel
 
     SECRET_REFERENCE_TOKEN: str = "secret:"
 
     def __init__(
         self,
@@ -37,23 +38,25 @@
         default: typing.Union[
             "_config_value_types.ConfigValueType",
             typing.Callable[[], "_config_value_types.ConfigValueType"],
             sentinel.Sentinel,
         ] = Unset,
         validators: list["_config_value_validators.ConfigValueValidator"] | None = None,
         is_sensitive: bool = False,
+        reload_compatible: bool = False,
     ) -> None:
         self.name = name
         self.prefix = prefix
         self.description = description
         self.datatype = datatype
         self.default = default() if callable(default) else default
         self.validators = validators or []
         self.hardcoded = False
         self.is_sensitive = is_sensitive
+        self.reload_compatbile = reload_compatible
         self._value = Unset
         self._encoded_value = Unset
 
         if not _string_decoder.type_is_supported(data_type=self._real_datatype):
             raise ValueError(f"{self.datatype} not supported.")
 
         if self.has_default and self.default is not None:
@@ -140,11 +143,17 @@
         "_config_value_types.ConfigValueType",
         typing.Callable[[], typing.Union["_config_value_types.ConfigValueType"]],
         sentinel.Sentinel,
     ] = Unset,
     description: str = "",
     is_sensitive: bool = False,
     validators: list["_config_value_validators.ConfigValueValidator"] | None = None,
+    reload_compatible: bool = True,
 ) -> typing.Any:
     return PartialConfigOption(
-        ConfigOption, default=default, description=description, is_sensitive=is_sensitive, validators=validators
+        ConfigOption,
+        default=default,
+        description=description,
+        is_sensitive=is_sensitive,
+        validators=validators,
+        reload_compatible=reload_compatible,
     )
```

### Comparing `pythonsdk-0.5.0/src/python_sdk/config/_config_sources.py` & `pythonsdk-0.6.0/src/python_sdk/config/_config_sources.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/config/_config_value_types.py` & `pythonsdk-0.6.0/src/python_sdk/config/_config_value_types.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/config/_config_value_validators.py` & `pythonsdk-0.6.0/src/python_sdk/config/_config_value_validators.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/config/_string_decoder.py` & `pythonsdk-0.6.0/src/python_sdk/config/_string_decoder.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/encoding/_base64url.py` & `pythonsdk-0.6.0/src/python_sdk/encoding/_base64url.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/__init__.py` & `pythonsdk-0.6.0/src/python_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_base.py` & `pythonsdk-0.6.0/src/python_sdk/log/_base.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_config.py` & `pythonsdk-0.6.0/src/python_sdk/log/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_context.py` & `pythonsdk-0.6.0/src/python_sdk/log/_context.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_log.py` & `pythonsdk-0.6.0/src/python_sdk/log/_log.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_logger.py` & `pythonsdk-0.6.0/src/python_sdk/log/_logger.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_factory.py` & `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_protocol.py` & `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_protocol.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py` & `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py` & `pythonsdk-0.6.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_factory.py` & `pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/log/_logging_handler/_rotating_file.py` & `pythonsdk-0.6.0/src/python_sdk/log/_logging_handler/_rotating_file.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/secrets/__init__.py` & `pythonsdk-0.6.0/src/python_sdk/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/secrets/_config.py` & `pythonsdk-0.6.0/src/python_sdk/secrets/_config.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py` & `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py` & `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py` & `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_factory.py` & `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/secrets/_secrets_engine/_protocol.py` & `pythonsdk-0.6.0/src/python_sdk/secrets/_secrets_engine/_protocol.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/sentinel/_sentinel.py` & `pythonsdk-0.6.0/src/python_sdk/sentinel/_sentinel.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/testing/_prepackaged_tests.py` & `pythonsdk-0.6.0/src/python_sdk/testing/_prepackaged_tests.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/utils/__init__.py` & `pythonsdk-0.6.0/src/python_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/utils/_file_watcher.py` & `pythonsdk-0.6.0/src/python_sdk/utils/_file_watcher.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/utils/_zipfile.py` & `pythonsdk-0.6.0/src/python_sdk/utils/_zipfile.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/python_sdk/versioning/_version_file_based.py` & `pythonsdk-0.6.0/src/python_sdk/versioning/_version_file_based.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.5.0/src/pythonsdk.egg-info/PKG-INFO` & `pythonsdk-0.6.0/src/pythonsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
         Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pythonsdk-0.5.0/src/pythonsdk.egg-info/SOURCES.txt` & `pythonsdk-0.6.0/src/pythonsdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/python_sdk/config/_config.py
 src/python_sdk/config/_config_documentation.py
 src/python_sdk/config/_config_option.py
 src/python_sdk/config/_config_sources.py
 src/python_sdk/config/_config_validators.py
 src/python_sdk/config/_config_value_types.py
 src/python_sdk/config/_config_value_validators.py
+src/python_sdk/config/_flags.py
 src/python_sdk/config/_optional_type.py
 src/python_sdk/config/_string_decoder.py
 src/python_sdk/encoding/__init__.py
 src/python_sdk/encoding/_base64url.py
 src/python_sdk/log/__init__.py
 src/python_sdk/log/_base.py
 src/python_sdk/log/_config.py
```

