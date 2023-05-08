# Comparing `tmp/m-abac-anhnt-1.0.5.tar.gz` & `tmp/m-abac-anhnt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-anhnt-1.0.5.tar", last modified: Mon May  8 04:15:54 2023, max compression
+gzip compressed data, was "m-abac-anhnt-1.0.6.tar", last modified: Mon May  8 04:57:45 2023, max compression
```

## Comparing `m-abac-anhnt-1.0.5.tar` & `m-abac-anhnt-1.0.6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1855 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/PKG-INFO
--rw-r--r--   0 mobio     (1000) mobio     (1000)      958 2023-05-08 04:11:43.000000 m-abac-anhnt-1.0.5/README.md
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1855 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/PKG-INFO
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     3586 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/SOURCES.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/dependency_links.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/requires.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        6 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/top_level.txt
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/abac/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       70 2023-04-20 10:26:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/__init__.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      267 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      435 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)    15511 2023-04-20 08:11:29.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     8187 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/call_api.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)    13654 2023-05-08 04:09:42.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/pdp.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       44 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/__init__.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 mobio     (1000) mobio     (1000)        0 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      662 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/base.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       39 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1127 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1107 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      323 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      629 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      654 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      638 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      664 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1341 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      754 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      602 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      774 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      728 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      243 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     2520 2023-03-28 05:00:01.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1345 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1367 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1389 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1358 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1380 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1363 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      197 2023-03-28 07:06:43.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1839 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/base.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1004 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      975 2023-03-28 06:54:31.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      974 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 07:02:53.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      978 2023-03-28 07:03:16.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       82 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1691 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      737 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      746 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      188 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1450 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      853 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      871 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      895 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      863 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      886 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      869 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)       73 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      963 2023-05-04 10:46:10.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/base.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      689 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      701 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     2026 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/schema.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      307 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1497 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1213 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1245 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1203 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1227 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1214 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1498 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1264 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1601 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     5812 2023-03-23 03:58:21.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     3259 2023-04-10 10:55:45.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     2762 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/result_access.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.5/pyproject.toml
--rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/setup.cfg
--rw-r--r--   0 mobio     (1000) mobio     (1000)     9780 2023-05-08 04:14:26.000000 m-abac-anhnt-1.0.5/setup.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1855 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/PKG-INFO
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      958 2023-05-08 04:11:43.000000 m-abac-anhnt-1.0.6/README.md
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1855 2023-05-08 04:57:45.000000 m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/PKG-INFO
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     3586 2023-05-08 04:57:45.000000 m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/SOURCES.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-05-08 04:57:45.000000 m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/dependency_links.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-05-08 04:57:45.000000 m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/requires.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        6 2023-05-08 04:57:45.000000 m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/top_level.txt
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.828728 m-abac-anhnt-1.0.6/mobio/
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.828728 m-abac-anhnt-1.0.6/mobio/libs/
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       70 2023-04-20 10:26:41.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/__init__.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/adapter/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      267 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      435 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)    15511 2023-04-20 08:11:29.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     8187 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/call_api.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)    10511 2023-05-08 04:57:39.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/pdp.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       44 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/__init__.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)        0 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      662 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/base.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       39 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1127 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1107 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      323 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      629 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      654 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      638 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      664 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1341 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      754 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      602 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      774 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      728 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      243 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2520 2023-03-28 05:00:01.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1345 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1367 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1389 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1358 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1380 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1363 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      197 2023-03-28 07:06:43.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1839 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/base.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1004 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      975 2023-03-28 06:54:31.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      974 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 07:02:53.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      978 2023-03-28 07:03:16.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       82 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1691 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      737 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      746 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      188 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1450 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      853 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      871 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      895 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      863 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      886 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      869 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)       73 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      963 2023-05-04 10:46:10.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/base.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      689 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      701 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2026 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/schema.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      307 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1497 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1213 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1245 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1203 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1227 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1214 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1498 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1264 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1601 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     5812 2023-03-23 03:58:21.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     3259 2023-04-10 10:55:45.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2762 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.6/mobio/libs/abac/result_access.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.6/pyproject.toml
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-05-08 04:57:45.832728 m-abac-anhnt-1.0.6/setup.cfg
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     9780 2023-05-08 04:57:39.000000 m-abac-anhnt-1.0.6/setup.py
```

### Comparing `m-abac-anhnt-1.0.5/PKG-INFO` & `m-abac-anhnt-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.5
+Version: 1.0.6
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-anhnt-1.0.5/README.md` & `m-abac-anhnt-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/PKG-INFO` & `m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.5
+Version: 1.0.6
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/SOURCES.txt` & `m-abac-anhnt-1.0.6/m_abac_anhnt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/call_api.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/call_api.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/pdp.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/pdp.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         ADD = "add"
         EDIT = "edit"
         DELETE = "delete"
         OTHER = "other"
 
     def __init__(self,
                  merchant_id: str, resource: str, action: str, account_id: str = None, user_info: dict = None,
-                 data_before: dict = None, data_after: dict = None, environment: dict = None, account_type=AccountType.NORMAL):
+                 data_before: dict = None, data_after: dict = None, environment: dict = None,
+                 account_type=AccountType.NORMAL):
         if not merchant_id:
             raise ValueError("merchant_id required")
         if not resource:
             raise ValueError("resource required")
         if not action:
             raise ValueError("action required")
 
@@ -52,14 +53,15 @@
         self.result_access = ResultAccess()
         self.request_access.update({
             "user": user_info if user_info else {},
             "env": self.get_info_environment(environment),
             self.resource: data_before if data_before else {}
         })
         self.data_after = data_after if data_after else {}
+        self.data_before = data_before if data_before else {}
 
     def get_policy_statement_for_target(self):
         return CallAPI.admin_get_list_statement(self.merchant_id, self.account_id, self.resource, self.action)
 
     def is_allowed(self):
         """
             Check if authorization request is allowed
@@ -103,77 +105,14 @@
             if environment:
                 if environment.get("env:user_agent"):
                     environment.update(Utils.parse_user_agent(environment.get("env:user_agent")))
         environment = environment if environment else {}
         environment.update({"env:current_time": Utils.get_date_utcnow()})
         return environment
 
-    def check_access_level_action(self, statement, access_level):
-        """
-                # list_statement_level = self.get_statement_by_level(list_statement)
-                # for statement_level in list_statement_level:
-                #     next_statement = True
-                #     for statement in statement_level:
-                #         next_statement = self.check_access_level_action(statement=statement, access_level=access_level)
-                #         if not next_statement:
-                #             break
-                #     if not next_statement:
-                #         break
-            kiểm tra các từng statement, condition thỏa mãn thì lấy thông tin bộ lọc hoặc hiển thị field nếu có
-        :param statement:
-        :return:
-        """
-        next_statement = True
-
-        statement_copy = deepcopy(statement)
-        condition_check = []
-        condition_filter = []
-        display_field = {}
-        if access_level == "list":
-            for item_cond in statement_copy.get("condition"):
-                if item_cond.get("field").startswith("user") or item_cond.get("field").startswith("env"):
-                    condition_check.append(item_cond)
-                else:
-                    values = [self.get_value_from_variable(i) for i in item_cond.get("values")]
-                    item_cond["values"] = values
-                    condition_filter.append(item_cond)
-        else:
-            condition_filter = statement_copy.get("condition")
-        if access_level in ["list", "read"]:
-            if statement_copy.get("fields"):
-                display_field.update({
-                    "effect": statement_copy.get("effect"),
-                    "fields": statement_copy.get("fields"),
-                })
-        statement_allow = False
-        if condition_check:
-            statement_check = {**statement_copy}
-            statement_check["condition"] = condition_check
-            statement_check["request_access"] = self.request_access
-            policy_schema = PolicySchema().load(statement_check)
-            if policy_schema.is_allowed():
-                statement_allow = True
-                if policy_schema.get("effect") == AccessType.ALLOW_ACCESS:
-                    next_statement = True
-                    self.result_access.set_allow_access(True)
-                else:
-                    next_statement = False
-                    self.result_access.set_allow_access(False)
-        else:
-            next_statement = True
-            statement_allow = True
-            self.result_access.set_allow_access(True)
-        if statement_allow:
-            if condition_filter:
-                statement_filter = {"effect": statement_copy.get("effect"), "condition": condition_filter}
-                self.result_access.add_filter_config(statement_filter)
-            if display_field:
-                self.result_access.add_display_config(display_field)
-        return next_statement
-
     def get_value_from_variable(self, str_variable):
         variables = Utils.get_field_key_from_variable(str_variable)
         if variables:
             if len(variables) == 1 and Utils.check_field_is_variable(variables[0]):
                 field_value = self.get_value_from_field(variables[0])
                 return field_value
             for field_key in variables:
@@ -188,24 +127,14 @@
         if resource_name and resource_key:
             if self.request_access.get(resource_name) and isinstance(self.request_access.get(resource_name), dict):
                 data_resource = self.request_access.get(resource_name)
                 value = Utils.get_nested_value(data_resource, resource_key)
                 return value
         return None
 
-    def get_statement_by_level(self, list_statement: list):
-        statement_deny = []
-        statement_allow = []
-        for item in list_statement:
-            if item.get("effect") == AccessType.DENY_ACCESS:
-                statement_deny.append(item)
-            else:
-                statement_allow.append(item)
-        return [statement_deny, statement_allow]
-
     def get_statement_by_type(self, list_statement: list, access_level: str):
         statement_check_allow, statement_check_deny = [], []
         for statement in list_statement:
             statement_copy = deepcopy(statement)
             fields = []
             if statement_copy.get("resource_field") and statement_copy.get("resource_field").get(self.resource):
                 fields = statement_copy.get("resource_field").get(self.resource)
@@ -241,14 +170,16 @@
                     statement_check_deny.append(statement_copy)
                 if fields:
                     self.result_access.add_display_config({
                         "effect": statement_copy.get("effect"),
                         "fields": fields,
                     })
             else:
+                if access_level == PolicyDecisionPoint.AccessLevel.ADD:
+                    self.data_after.update(self.data_before)
                 if fields:
                     statement_copy["check_field"] = 1
                 if statement_copy.get("effect") == AccessType.ALLOW_ACCESS:
                     statement_check_allow.append(statement_copy)
                 else:
                     statement_check_deny.append(statement_copy)
         return statement_check_allow, statement_check_deny
```

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/exceptions.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/policy.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/utils.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/mobio/libs/abac/result_access.py` & `m-abac-anhnt-1.0.6/mobio/libs/abac/result_access.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.5/setup.py` & `m-abac-anhnt-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.5',  # Required
+    version='1.0.6',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

