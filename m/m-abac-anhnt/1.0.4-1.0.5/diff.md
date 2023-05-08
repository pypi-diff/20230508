# Comparing `tmp/m-abac-anhnt-1.0.4.tar.gz` & `tmp/m-abac-anhnt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-anhnt-1.0.4.tar", last modified: Thu Apr 20 10:27:00 2023, max compression
+gzip compressed data, was "m-abac-anhnt-1.0.5.tar", last modified: Mon May  8 04:15:54 2023, max compression
```

## Comparing `m-abac-anhnt-1.0.4.tar` & `m-abac-anhnt-1.0.5.tar`

### file list

```diff
@@ -1,89 +1,94 @@
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/PKG-INFO
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1115 2023-04-13 06:35:19.000000 m-abac-anhnt-1.0.4/README.md
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2012 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/PKG-INFO
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     3378 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/SOURCES.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/dependency_links.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/requires.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        6 2023-04-20 10:27:00.000000 m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/top_level.txt
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       70 2023-04-20 10:26:41.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/__init__.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      267 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      435 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)    15511 2023-04-20 08:11:29.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     8187 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/call_api.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)    13365 2023-04-12 06:41:17.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/pdp.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       44 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/__init__.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 mobio     (1000) mobio     (1000)        0 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      662 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/base.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       39 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1127 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1107 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.127152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      323 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      629 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      654 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      638 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      664 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1341 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      754 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      602 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      774 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      728 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      243 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     2520 2023-03-28 05:00:01.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1345 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1367 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1389 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1358 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1380 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1363 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      197 2023-03-28 07:06:43.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1839 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/base.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1004 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      975 2023-03-28 06:54:31.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      974 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 07:02:53.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      978 2023-03-28 07:03:16.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       82 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1691 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      737 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      746 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      188 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1450 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      853 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      871 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      895 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      863 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      886 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      869 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1934 2023-03-28 07:06:43.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/schema.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      307 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1497 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1213 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1245 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1203 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1227 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1214 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1498 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1264 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1601 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     5812 2023-03-23 03:58:21.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     3259 2023-04-10 10:55:45.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     2762 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.4/mobio/libs/abac/result_access.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.4/pyproject.toml
--rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-04-20 10:27:00.131152 m-abac-anhnt-1.0.4/setup.cfg
--rw-r--r--   0 mobio     (1000) mobio     (1000)     9780 2023-04-20 10:23:54.000000 m-abac-anhnt-1.0.4/setup.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1855 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/PKG-INFO
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      958 2023-05-08 04:11:43.000000 m-abac-anhnt-1.0.5/README.md
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1855 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/PKG-INFO
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     3586 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/SOURCES.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/dependency_links.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/requires.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        6 2023-05-08 04:15:54.000000 m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/top_level.txt
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/abac/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       70 2023-04-20 10:26:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/__init__.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      267 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      435 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)    15511 2023-04-20 08:11:29.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     8187 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/call_api.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)    13654 2023-05-08 04:09:42.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/pdp.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.502842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       44 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/__init__.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)        0 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      662 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/base.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       39 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1127 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1107 2023-03-22 08:58:07.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      323 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      629 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      654 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      638 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      664 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1341 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      754 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      602 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      774 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      728 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.506842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      243 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2520 2023-03-28 05:00:01.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1345 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1367 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1389 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1358 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1380 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1363 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      197 2023-03-28 07:06:43.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1839 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/base.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1004 2023-03-28 05:06:28.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      975 2023-03-28 06:54:31.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      974 2023-03-28 06:59:38.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 07:02:53.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      978 2023-03-28 07:03:16.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       82 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1691 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      737 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      746 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      188 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1450 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      853 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      871 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      895 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      863 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      886 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      869 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.510842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)       73 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      963 2023-05-04 10:46:10.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/base.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      689 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      701 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2026 2023-05-04 11:03:41.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/schema.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      307 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1497 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1213 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1245 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1203 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1227 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1214 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1498 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1264 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1601 2023-03-21 07:52:15.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     5812 2023-03-23 03:58:21.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     3259 2023-04-10 10:55:45.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2762 2023-04-20 09:49:59.000000 m-abac-anhnt-1.0.5/mobio/libs/abac/result_access.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abac-anhnt-1.0.5/pyproject.toml
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-05-08 04:15:54.514842 m-abac-anhnt-1.0.5/setup.cfg
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     9780 2023-05-08 04:14:26.000000 m-abac-anhnt-1.0.5/setup.py
```

### Comparing `m-abac-anhnt-1.0.4/PKG-INFO` & `m-abac-anhnt-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
@@ -30,34 +30,28 @@
  $ pip3 install m-abac
  ```
 
 ### Sử dụng:
 
 ##### Kiểm tra user có quyền thao tác hay không:
    ```python
-    from m_abac import PolicyDecisionPoint
+    from mobio.libs.abac import PolicyDecisionPoint
     merchant_id = "1b99bdcf-d582-4f49-9715-1b61dfff3924"
     resource = "deal"
     # action = "UpdateFromSale"
     action = "ListFromSale"
     account_id = "704eac91-7416-497f-a17d-d81cfa2d3211"
     # thông tin user ko có thì để None 
     user_info = {
         "block": "KHDN",
         "scope_code": "MB##HN"
     }
-    request_access = {
-        "deal": {
-            # "block": "KHCN",
-            # "scope_code": "MB##HN##CAU_GIAY"
-        }
-    }
 
     pdb = PolicyDecisionPoint(merchant_id=merchant_id, resource=resource, action=action, account_id=account_id,
-                              user_info=user_info, request_access=request_access)
+                              user_info=user_info)
     result = pdb.is_allowed()
     if not result.get_allow_access():
         # trả về lỗi không có quyền truy cập 
    ```
 #### Log - 1.0.0
     - release sdk
```

### Comparing `m-abac-anhnt-1.0.4/README.md` & `m-abac-anhnt-1.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,34 +7,28 @@
  $ pip3 install m-abac
  ```
 
 ### Sử dụng:
 
 ##### Kiểm tra user có quyền thao tác hay không:
    ```python
-    from m_abac import PolicyDecisionPoint
+    from mobio.libs.abac import PolicyDecisionPoint
     merchant_id = "1b99bdcf-d582-4f49-9715-1b61dfff3924"
     resource = "deal"
     # action = "UpdateFromSale"
     action = "ListFromSale"
     account_id = "704eac91-7416-497f-a17d-d81cfa2d3211"
     # thông tin user ko có thì để None 
     user_info = {
         "block": "KHDN",
         "scope_code": "MB##HN"
     }
-    request_access = {
-        "deal": {
-            # "block": "KHCN",
-            # "scope_code": "MB##HN##CAU_GIAY"
-        }
-    }
 
     pdb = PolicyDecisionPoint(merchant_id=merchant_id, resource=resource, action=action, account_id=account_id,
-                              user_info=user_info, request_access=request_access)
+                              user_info=user_info)
     result = pdb.is_allowed()
     if not result.get_allow_access():
         # trả về lỗi không có quyền truy cập 
    ```
 #### Log - 1.0.0
     - release sdk
```

### Comparing `m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/PKG-INFO` & `m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-anhnt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
@@ -30,34 +30,28 @@
  $ pip3 install m-abac
  ```
 
 ### Sử dụng:
 
 ##### Kiểm tra user có quyền thao tác hay không:
    ```python
-    from m_abac import PolicyDecisionPoint
+    from mobio.libs.abac import PolicyDecisionPoint
     merchant_id = "1b99bdcf-d582-4f49-9715-1b61dfff3924"
     resource = "deal"
     # action = "UpdateFromSale"
     action = "ListFromSale"
     account_id = "704eac91-7416-497f-a17d-d81cfa2d3211"
     # thông tin user ko có thì để None 
     user_info = {
         "block": "KHDN",
         "scope_code": "MB##HN"
     }
-    request_access = {
-        "deal": {
-            # "block": "KHCN",
-            # "scope_code": "MB##HN##CAU_GIAY"
-        }
-    }
 
     pdb = PolicyDecisionPoint(merchant_id=merchant_id, resource=resource, action=action, account_id=account_id,
-                              user_info=user_info, request_access=request_access)
+                              user_info=user_info)
     result = pdb.is_allowed()
     if not result.get_allow_access():
         # trả về lỗi không có quyền truy cập 
    ```
 #### Log - 1.0.0
     - release sdk
```

### Comparing `m-abac-anhnt-1.0.4/m_abac_anhnt.egg-info/SOURCES.txt` & `m-abac-anhnt-1.0.5/m_abac_anhnt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 mobio/libs/abac/policy/conditions/numeric/base.py
 mobio/libs/abac/policy/conditions/numeric/eq.py
 mobio/libs/abac/policy/conditions/numeric/gt.py
 mobio/libs/abac/policy/conditions/numeric/gte.py
 mobio/libs/abac/policy/conditions/numeric/lt.py
 mobio/libs/abac/policy/conditions/numeric/lte.py
 mobio/libs/abac/policy/conditions/numeric/neq.py
+mobio/libs/abac/policy/conditions/others/__init__.py
+mobio/libs/abac/policy/conditions/others/base.py
+mobio/libs/abac/policy/conditions/others/exists.py
+mobio/libs/abac/policy/conditions/others/not_exists.py
 mobio/libs/abac/policy/conditions/string/__init__.py
 mobio/libs/abac/policy/conditions/string/base.py
 mobio/libs/abac/policy/conditions/string/contains.py
 mobio/libs/abac/policy/conditions/string/ends_with.py
 mobio/libs/abac/policy/conditions/string/equals.py
 mobio/libs/abac/policy/conditions/string/not_contains.py
 mobio/libs/abac/policy/conditions/string/not_equals.py
```

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/call_api.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/call_api.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/pdp.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/pdp.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         READ = "read"
         ADD = "add"
         EDIT = "edit"
         DELETE = "delete"
         OTHER = "other"
 
     def __init__(self,
-                 merchant_id, resource: str, action: str, account_id: str = None, user_info: dict = None,
-                 request_access: dict = None, environment: dict = None, account_type=AccountType.NORMAL):
+                 merchant_id: str, resource: str, action: str, account_id: str = None, user_info: dict = None,
+                 data_before: dict = None, data_after: dict = None, environment: dict = None, account_type=AccountType.NORMAL):
         if not merchant_id:
             raise ValueError("merchant_id required")
         if not resource:
             raise ValueError("resource required")
         if not action:
             raise ValueError("action required")
 
@@ -44,20 +44,22 @@
                 user_info = CallAPI.admin_get_account_info(merchant_id, account_id)
 
         self.account_type = account_type
         self.merchant_id = merchant_id
         self.account_id = account_id
         self.resource = resource
         self.action = action
-        self.request_access = request_access if request_access else {}
+        self.request_access = {}
         self.result_access = ResultAccess()
         self.request_access.update({
             "user": user_info if user_info else {},
-            "env": self.get_info_environment(environment)
+            "env": self.get_info_environment(environment),
+            self.resource: data_before if data_before else {}
         })
+        self.data_after = data_after if data_after else {}
 
     def get_policy_statement_for_target(self):
         return CallAPI.admin_get_list_statement(self.merchant_id, self.account_id, self.resource, self.action)
 
     def is_allowed(self):
         """
             Check if authorization request is allowed
@@ -200,19 +202,17 @@
                 statement_allow.append(item)
         return [statement_deny, statement_allow]
 
     def get_statement_by_type(self, list_statement: list, access_level: str):
         statement_check_allow, statement_check_deny = [], []
         for statement in list_statement:
             statement_copy = deepcopy(statement)
-            fields = {}
-            for item_resource in statement_copy.get("resource"):
-                data_fields = Utils.get_fields_of_resource(item_resource)
-                if data_fields and self.resource in data_fields:
-                    fields.update(data_fields)
+            fields = []
+            if statement_copy.get("resource_field") and statement_copy.get("resource_field").get(self.resource):
+                fields = statement_copy.get("resource_field").get(self.resource)
             if fields:
                 statement_copy["fields"] = fields
             if access_level == PolicyDecisionPoint.AccessLevel.LIST:
                 condition_check = []
                 condition_filter = []
                 for item_cond in statement_copy.get("condition"):
                     if item_cond.get("field").startswith("user") or item_cond.get("field").startswith("env"):
@@ -235,57 +235,63 @@
                     self.result_access.add_filter_config(
                         {"effect": statement_copy.get("effect"), "condition": condition_filter})
             elif access_level == PolicyDecisionPoint.AccessLevel.READ:
                 if statement_copy.get("effect") == AccessType.ALLOW_ACCESS:
                     statement_check_allow.append(statement_copy)
                 else:
                     statement_check_deny.append(statement_copy)
-                if statement_copy.get("fields"):
+                if fields:
                     self.result_access.add_display_config({
                         "effect": statement_copy.get("effect"),
-                        "fields": statement_copy.get("fields"),
+                        "fields": fields,
                     })
             else:
                 if fields:
                     statement_copy["check_field"] = 1
                 if statement_copy.get("effect") == AccessType.ALLOW_ACCESS:
                     statement_check_allow.append(statement_copy)
                 else:
                     statement_check_deny.append(statement_copy)
         return statement_check_allow, statement_check_deny
 
     def check_list_statement_is_deny(self, list_statement: list):
         result_deny = False
         try:
             for statement in list_statement:
-                if statement.get("check_field") and statement.get("fields"):
-                    if not Utils.field_in_body_request(statement.get("fields").get(self.resource),
-                                                       self.request_access.get(self.resource)):
-                        continue
                 statement["request_access"] = self.request_access
                 policy_schema = PolicySchema().load(statement)
                 if policy_schema.is_allowed():
+                    if statement.get("check_field") and statement.get("fields"):
+                        if not Utils.field_in_body_request(statement.get("fields"), self.data_after):
+                            continue
                     result_deny = True
                     break
         except Exception as err:
             print("check_list_statement_is_deny err: {}".format(err))
             result_deny = False
         return result_deny
 
     def check_list_statement_is_allow(self, list_statement: list):
         result_allow = True
         try:
             for statement in list_statement:
-                # đối với action là edit create mà resource liên quan đến field thì kiểm tra field có trong body yêu cầu truy cập hay ko. nếu ko có thì bỏ qua statement
-                if statement.get("check_field") and statement.get("fields"):
-                    if not Utils.field_in_body_request(statement.get("fields").get(self.resource),
-                                                       self.request_access.get(self.resource)):
-                        continue
+                # đối với action là edit create mà resource liên quan đến field thì kiểm tra field có trong body
+                # yêu cầu truy cập hay ko
+                # case: policy cho sửa 3 field, dữ liệu gửi lên có 5 field trong đó có 1 field trong policy
+                # thì hiện tại chưa chặn dc do có policy * all, sau này bỏ policy * all thì
+                # sửa lại kiểm tra danh sách field gửi lên phải nằm trong policy
+                # hiện tại chỉ cần có 1 field trong dữ liệu gửi lên có trong policy là dc cho qua
+
                 statement["request_access"] = self.request_access
                 policy_schema = PolicySchema().load(statement)
                 if not policy_schema.is_allowed():
                     result_allow = False
                     break
+                if statement.get("check_field") and statement.get("fields"):
+                    if not Utils.field_in_body_request(statement.get("fields"), self.data_after):
+                        result_allow = False
+                        break
+
         except Exception as err:
             print("check_list_statement_is_allow err: {}".format(err))
             result_allow = False
         return result_allow
```

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .boolean import *
 from .collection import *
 from .date_time import *
 from .ip_address import *
 from .numeric import *
 from .string import *
 from .day import *
-
+from .others import *
 
 class ConditionSchema(OneOfSchema):
     """
         Polymorphic JSON schema for conditions
     """
     type_field = "operator"
     type_schemas = {
@@ -57,12 +57,15 @@
         "DayEquals": DayEqSchema,
         "DayNotEquals": DayNeqSchema,
         "DayLessThan": DayLtSchema,
         "DayLessThanEquals": DayLteSchema,
         "DayGreaterThan": DayGtSchema,
         "DayGreaterThanEquals": DayGteSchema,
 
+        "Exists": ExistsSchema,
+        "NotExists": NotExistsSchema,
+
     }
 
     class Meta:
         unknown = EXCLUDE
```

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/exceptions.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/policy.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/policy/utils.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/mobio/libs/abac/result_access.py` & `m-abac-anhnt-1.0.5/mobio/libs/abac/result_access.py`

 * *Files identical despite different names*

### Comparing `m-abac-anhnt-1.0.4/setup.py` & `m-abac-anhnt-1.0.5/setup.py`

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
-    version='1.0.4',  # Required
+    version='1.0.5',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

