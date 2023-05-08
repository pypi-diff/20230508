# Comparing `tmp/csaf-2023.5.6.tar.gz` & `tmp/csaf-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csaf-2023.5.6.tar", last modified: Sat May  6 14:40:24 2023, max compression
+gzip compressed data, was "csaf-2023.5.8.tar", last modified: Mon May  8 19:17:40 2023, max compression
```

## Comparing `csaf-2023.5.6.tar` & `csaf-2023.5.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.128668 csaf-2023.5.6/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 csaf-2023.5.6/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 csaf-2023.5.6/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-06 14:40:24.128510 csaf-2023.5.6/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2576 2023-05-06 13:23:15.000000 csaf-2023.5.6/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.109374 csaf-2023.5.6/csaf/
--rw-r--r--   0 ruth       (501) staff       (20)     1984 2023-05-06 14:37:47.000000 csaf-2023.5.6/csaf/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2023.5.6/csaf/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2023.5.6/csaf/category.py
--rw-r--r--   0 ruth       (501) staff       (20)     4112 2023-01-02 18:40:21.000000 csaf-2023.5.6/csaf/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      647 2022-12-21 15:07:30.000000 csaf-2023.5.6/csaf/config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2023.5.6/csaf/cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)    16866 2022-12-21 15:35:09.000000 csaf-2023.5.6/csaf/csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2023.5.6/csaf/cve.py
--rw-r--r--   0 ruth       (501) staff       (20)    11239 2023-05-06 14:07:29.000000 csaf-2023.5.6/csaf/cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2023.5.6/csaf/cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)    12425 2023-05-06 13:11:03.000000 csaf-2023.5.6/csaf/definitions.py
--rw-r--r--   0 ruth       (501) staff       (20)    14924 2022-07-31 13:30:33.000000 csaf-2023.5.6/csaf/document.py
--rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2023.5.6/csaf/env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2023.5.6/csaf/hash.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.118487 csaf-2023.5.6/csaf/mandatory/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2023.5.6/csaf/mandatory/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2023.5.6/csaf/mandatory/acyclic_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2023.5.6/csaf/mandatory/consistent_product_status.py
--rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2023.5.6/csaf/mandatory/defined_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2023.5.6/csaf/mandatory/defined_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     5288 2022-06-19 10:04:43.000000 csaf-2023.5.6/csaf/mandatory/rules.py
--rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2023.5.6/csaf/mandatory/translator_and_source_lang.py
--rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2023.5.6/csaf/mandatory/unique_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2023.5.6/csaf/mandatory/unique_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2023.5.6/csaf/mandatory/valid_category_name.py
--rw-r--r--   0 ruth       (501) staff       (20)    16500 2022-07-31 13:32:20.000000 csaf-2023.5.6/csaf/product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2023.5.6/csaf/purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2023.5.6/csaf/terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2023.5.6/csaf/tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2023.5.6/csaf/version.py
--rw-r--r--   0 ruth       (501) staff       (20)     3354 2022-03-13 16:02:22.000000 csaf-2023.5.6/csaf/vuln_types.py
--rw-r--r--   0 ruth       (501) staff       (20)    13432 2022-07-31 13:30:55.000000 csaf-2023.5.6/csaf/vulnerability.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.111520 csaf-2023.5.6/csaf.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1204 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      222 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        5 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     3004 2023-05-06 14:31:45.000000 csaf-2023.5.6/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-06 14:40:24.128708 csaf-2023.5.6/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.128279 csaf-2023.5.6/test/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2023.5.6/test/test_category.py
--rw-r--r--   0 ruth       (501) staff       (20)      544 2023-05-06 14:12:39.000000 csaf-2023.5.6/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2023.5.6/test/test_config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2023.5.6/test/test_cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:53.000000 csaf-2023.5.6/test/test_csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2023.5.6/test/test_cve.py
--rw-r--r--   0 ruth       (501) staff       (20)     8576 2023-05-06 14:28:48.000000 csaf-2023.5.6/test/test_cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2023.5.6/test/test_cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2023.5.6/test/test_document.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2023.5.6/test/test_env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2023.5.6/test/test_product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2023.5.6/test/test_purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2023.5.6/test/test_terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2023.5.6/test/test_tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2023.5.6/test/test_version.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:59.000000 csaf-2023.5.6/test/test_vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.427214 csaf-2023.5.8/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 csaf-2023.5.8/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 csaf-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-08 19:17:40.426897 csaf-2023.5.8/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2576 2023-05-06 13:23:15.000000 csaf-2023.5.8/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.306978 csaf-2023.5.8/csaf/
+-rw-r--r--   0 ruth       (501) staff       (20)     1984 2023-05-08 19:14:20.000000 csaf-2023.5.8/csaf/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2023.5.8/csaf/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2023.5.8/csaf/category.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4112 2023-01-02 18:40:21.000000 csaf-2023.5.8/csaf/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      647 2022-12-21 15:07:30.000000 csaf-2023.5.8/csaf/config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2023.5.8/csaf/cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16866 2022-12-21 15:35:09.000000 csaf-2023.5.8/csaf/csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2023.5.8/csaf/cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11239 2023-05-06 14:07:29.000000 csaf-2023.5.8/csaf/cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2023.5.8/csaf/cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12425 2023-05-06 13:11:03.000000 csaf-2023.5.8/csaf/definitions.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14924 2022-07-31 13:30:33.000000 csaf-2023.5.8/csaf/document.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2023.5.8/csaf/env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2023.5.8/csaf/hash.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.417227 csaf-2023.5.8/csaf/mandatory/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2023.5.8/csaf/mandatory/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2023.5.8/csaf/mandatory/acyclic_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2023.5.8/csaf/mandatory/consistent_product_status.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2023.5.8/csaf/mandatory/defined_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2023.5.8/csaf/mandatory/defined_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5288 2022-06-19 10:04:43.000000 csaf-2023.5.8/csaf/mandatory/rules.py
+-rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2023.5.8/csaf/mandatory/translator_and_source_lang.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2023.5.8/csaf/mandatory/unique_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2023.5.8/csaf/mandatory/unique_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2023.5.8/csaf/mandatory/valid_category_name.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16500 2022-07-31 13:32:20.000000 csaf-2023.5.8/csaf/product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2023.5.8/csaf/purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2023.5.8/csaf/terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2023.5.8/csaf/tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2023.5.8/csaf/version.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3354 2022-03-13 16:02:22.000000 csaf-2023.5.8/csaf/vuln_types.py
+-rw-r--r--   0 ruth       (501) staff       (20)    13724 2023-05-08 18:30:19.000000 csaf-2023.5.8/csaf/vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.309314 csaf-2023.5.8/csaf.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1204 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      222 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        5 2023-05-08 19:17:40.000000 csaf-2023.5.8/csaf.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     3004 2023-05-08 18:38:37.000000 csaf-2023.5.8/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-08 19:17:40.427296 csaf-2023.5.8/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-08 19:17:40.426241 csaf-2023.5.8/test/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2023.5.8/test/test_category.py
+-rw-r--r--   0 ruth       (501) staff       (20)      544 2023-05-06 14:12:39.000000 csaf-2023.5.8/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2023.5.8/test/test_config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2023.5.8/test/test_cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:53.000000 csaf-2023.5.8/test/test_csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2023.5.8/test/test_cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8920 2023-05-08 15:23:14.000000 csaf-2023.5.8/test/test_cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2023.5.8/test/test_cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2023.5.8/test/test_document.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2023.5.8/test/test_env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2023.5.8/test/test_product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2023.5.8/test/test_purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2023.5.8/test/test_terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2023.5.8/test/test_tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2023.5.8/test/test_version.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2259 2023-05-08 18:29:00.000000 csaf-2023.5.8/test/test_vulnerability.py
```

### Comparing `csaf-2023.5.6/LICENSE` & `csaf-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/PKG-INFO` & `csaf-2023.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csaf
-Version: 2023.5.6
+Version: 2023.5.8
 Summary: Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/csaf
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/csaf
 Project-URL: Documentation, https://codes.dilettant.life/docs/csaf
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/csaf
```

### Comparing `csaf-2023.5.6/README.md` & `csaf-2023.5.8/README.md`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/__init__.py` & `csaf-2023.5.8/csaf/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
 
 init_logger(name=APP_ENV, level=logging.DEBUG if DEBUG else None)
 
 from csaf.csaf import is_valid  # noqa
 
 # [[[fill git_describe()]]]
-__version__ = '2023.5.6+parent.75eb2ed8'
-# [[[end]]] (checksum: 68f0baf39732daf74a5084a1979c2fad)
+__version__ = '2023.5.8+parent.aa36605a'
+# [[[end]]] (checksum: 99e36df585743bf57b7cbd29fd80ca8c)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 __all__ = ['is_valid', 'log']
```

### Comparing `csaf-2023.5.6/csaf/cli.py` & `csaf-2023.5.8/csaf/cli.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/config.py` & `csaf-2023.5.8/csaf/config.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/csaf.py` & `csaf-2023.5.8/csaf/csaf.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/cvss.py` & `csaf-2023.5.8/csaf/cvss.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/definitions.py` & `csaf-2023.5.8/csaf/definitions.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/document.py` & `csaf-2023.5.8/csaf/document.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/env.py` & `csaf-2023.5.8/csaf/env.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/acyclic_product_ids.py` & `csaf-2023.5.8/csaf/mandatory/acyclic_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/consistent_product_status.py` & `csaf-2023.5.8/csaf/mandatory/consistent_product_status.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/defined_group_ids.py` & `csaf-2023.5.8/csaf/mandatory/defined_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/defined_product_ids.py` & `csaf-2023.5.8/csaf/mandatory/defined_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/rules.py` & `csaf-2023.5.8/csaf/mandatory/rules.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/translator_and_source_lang.py` & `csaf-2023.5.8/csaf/mandatory/translator_and_source_lang.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/unique_group_ids.py` & `csaf-2023.5.8/csaf/mandatory/unique_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/unique_product_ids.py` & `csaf-2023.5.8/csaf/mandatory/unique_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/mandatory/valid_category_name.py` & `csaf-2023.5.8/csaf/mandatory/valid_category_name.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/product.py` & `csaf-2023.5.8/csaf/product.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/vuln_types.py` & `csaf-2023.5.8/csaf/vuln_types.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/csaf/vulnerability.py` & `csaf-2023.5.8/csaf/vulnerability.py`

 * *Files 8% similar despite different names*

```diff
@@ -377,14 +377,19 @@
     which products the given value applies.
     """
 
     cvss_v2: Optional[CVSS2] = None
     cvss_v3: Optional[Union[CVSS30, CVSS31]] = None
     products: Products
 
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
+
 
 class Vulnerability(BaseModel):
     """
     Is a container for the aggregation of all fields that are related to a single vulnerability in the document.
     """
 
     acknowledgments: Annotated[
@@ -493,13 +498,18 @@
             ' the vulnerability.',
             min_length=1,
             title='Title',
         ),
     ]
 
     @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
+
+    @no_type_check
     @validator('involvements', 'remediations', 'scores', 'threats')
     @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
```

### Comparing `csaf-2023.5.6/csaf.egg-info/PKG-INFO` & `csaf-2023.5.8/csaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csaf
-Version: 2023.5.6
+Version: 2023.5.8
 Summary: Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/csaf
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/csaf
 Project-URL: Documentation, https://codes.dilettant.life/docs/csaf
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/csaf
```

### Comparing `csaf-2023.5.6/csaf.egg-info/SOURCES.txt` & `csaf-2023.5.8/csaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/pyproject.toml` & `csaf-2023.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "csaf"
-version = "2023.5.6"
+version = "2023.5.8"
 description = "Common Security Advisory Framework (CSAF) Verification, Validation, and Application Programming Interface (API)."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `csaf-2023.5.6/test/test_cli.py` & `csaf-2023.5.8/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `csaf-2023.5.6/test/test_cvss.py` & `csaf-2023.5.8/test/test_cvss.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,35 @@
     'vectorString': 'CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H',
     'version': '3.1',
 }
 JSON = json.dumps(DATA)
 
 
 def test_cvss31_minimal():
+    vector_string = 'CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H'
     expected_value = (
-        '{"version": "3.1", "vectorString": "CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H", "attackVector": null,'
+        f'{{"version": "3.1", "vectorString": "{vector_string}", "attackVector": null,'
         ' "attackComplexity": null, "privilegesRequired": null, "userInteraction": null, "scope": null,'
         ' "confidentialityImpact": null, "integrityImpact": null, "availabilityImpact": null, "baseScore": 10.0,'
         ' "baseSeverity": "CRITICAL", "exploitCodeMaturity": null, "remediationLevel": null, "reportConfidence": null,'
         ' "temporalScore": null, "temporalSeverity": null, "confidentialityRequirement": null,'
         ' "integrityRequirement": null, "availabilityRequirement": null, "modifiedAttackVector": null,'
         ' "modifiedAttackComplexity": null, "modifiedPrivilegesRequired": null, "modifiedUserInteraction": null,'
         ' "modifiedScope": null, "modifiedConfidentialityImpact": null, "modifiedIntegrityImpact": null,'
         ' "modifiedAvailabilityImpact": null, "environmentalScore": null, "environmentalSeverity": null}'
     )
     c31 = cvss.CVSS31.parse_raw(JSON)
     assert c31.json() == expected_value
+    assert c31.vector_string == vector_string
+
+    json_lines = c31.json(indent=2).split('\n')
+    json_rep_of_vs = [line for line in json_lines if 'vectorString' in line]
+    assert len(json_rep_of_vs) == 1
+    assert vector_string in json_rep_of_vs[0]
+    assert '"vectorString":' in json_rep_of_vs[0]
 
     expected_schema = {
         'title': 'CVSS31',
         'type': 'object',
         'properties': {
             'version': {
                 'description': 'CVSS Version',
```

