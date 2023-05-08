# Comparing `tmp/sqlmath-0.0.1.tar.gz` & `tmp/sqlmath-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmath-0.0.1.tar", last modified: Sat Apr 29 22:43:26 2023, max compression
+gzip compressed data, was "sqlmath-0.0.5.tar", last modified: Mon May  8 03:19:58 2023, max compression
```

## Comparing `sqlmath-0.0.1.tar` & `sqlmath-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:43:26.784573 sqlmath-0.0.1/
--rw-rw-rw-   0        0        0     1051 2022-05-14 23:09:18.000000 sqlmath-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      203 2023-04-29 22:43:26.784573 sqlmath-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4522 2023-04-28 07:29:01.000000 sqlmath-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 22:43:26.784573 sqlmath-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      285 2023-04-29 22:30:46.000000 sqlmath-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:43:26.783573 sqlmath-0.0.1/sqlmath.egg-info/
--rw-rw-rw-   0        0        0      203 2023-04-29 22:43:26.000000 sqlmath-0.0.1/sqlmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-04-29 22:43:26.000000 sqlmath-0.0.1/sqlmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:43:26.000000 sqlmath-0.0.1/sqlmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:43:26.000000 sqlmath-0.0.1/sqlmath.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 03:19:58.279513 sqlmath-0.0.5/
+-rw-rw-rw-   0        0        0    16089 2023-05-08 03:17:26.000000 sqlmath-0.0.5/.ci.sh
+-rw-rw-rw-   0        0        0      649 2023-05-08 01:15:03.000000 sqlmath-0.0.5/.gitconfig
+drwxrwxrwx   0        0        0        0 2023-05-08 03:19:58.217024 sqlmath-0.0.5/.github/
+drwxrwxrwx   0        0        0        0 2023-05-08 03:19:58.263889 sqlmath-0.0.5/.github/workflows/
+-rw-rw-rw-   0        0        0     2678 2023-05-08 01:15:04.000000 sqlmath-0.0.5/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0     1979 2023-05-08 01:15:04.000000 sqlmath-0.0.5/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      350 2023-05-08 01:15:04.000000 sqlmath-0.0.5/.gitignore
+-rw-rw-rw-   0        0        0      121 2022-07-01 08:39:09.000000 sqlmath-0.0.5/.npmignore
+-rw-rw-rw-   0        0        0    21637 2023-05-07 18:37:00.000000 sqlmath-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1051 2022-05-14 23:09:18.000000 sqlmath-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      942 2023-05-08 03:19:08.000000 sqlmath-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6911 2023-05-08 03:19:58.263889 sqlmath-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4522 2023-05-08 03:19:07.000000 sqlmath-0.0.5/README.md
+-rw-rw-rw-   0        0        0      564 2021-11-23 01:13:14.000000 sqlmath-0.0.5/asset_image_folder_open_solid.svg
+-rw-rw-rw-   0        0        0     1536 2022-07-01 09:15:31.000000 sqlmath-0.0.5/asset_image_github_brands.svg
+-rw-rw-rw-   0        0        0     1060 2023-01-30 03:31:22.000000 sqlmath-0.0.5/asset_image_logo_512.html
+-rw-rw-rw-   0        0        0     7087 2023-01-27 00:39:47.000000 sqlmath-0.0.5/asset_image_logo_512.png
+-rw-rw-rw-   0        0        0     2823 2023-01-27 00:41:57.000000 sqlmath-0.0.5/asset_image_logo_512.svg
+-rw-rw-rw-   0        0        0   472927 2023-05-08 01:15:05.000000 sqlmath-0.0.5/asset_sqlmath_external_rollup.js
+-rw-rw-rw-   0        0        0   262193 2022-03-12 08:38:29.000000 sqlmath-0.0.5/cpplint.py
+-rw-rw-rw-   0        0        0   385557 2023-05-07 18:36:21.000000 sqlmath-0.0.5/csslint.js
+-rwxrwxrwx   0        0        0    72704 2022-03-12 07:15:31.000000 sqlmath-0.0.5/indent.exe
+-rw-rw-rw-   0        0        0    23525 2023-05-08 01:15:06.000000 sqlmath-0.0.5/index.html
+-rw-rw-rw-   0        0        0   336202 2023-05-07 08:16:38.000000 sqlmath-0.0.5/jslint.mjs
+-rw-rw-rw-   0        0        0    98311 2023-05-07 18:31:32.000000 sqlmath-0.0.5/jslint_ci.sh
+-rw-rw-rw-   0        0        0  1008128 2023-04-26 05:21:52.000000 sqlmath-0.0.5/libiconv2.dll
+-rw-rw-rw-   0        0        0   103424 2023-04-26 05:21:52.000000 sqlmath-0.0.5/libintl3.dll
+-rw-rw-rw-   0        0        0      924 2023-05-07 18:19:11.000000 sqlmath-0.0.5/package.json
+-rw-rw-rw-   0        0        0     1426 2023-05-08 02:26:27.000000 sqlmath-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 03:19:58.279513 sqlmath-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-05-08 03:17:13.000000 sqlmath-0.0.5/setup.py
+-rw-rw-rw-   0        0        0 11480382 2023-05-08 01:15:09.000000 sqlmath-0.0.5/sqlite3_rollup.c
+drwxrwxrwx   0        0        0        0 2023-05-08 03:19:58.263889 sqlmath-0.0.5/sqlmath/
+-rw-rw-rw-   0        0        0      790 2023-05-08 03:12:40.000000 sqlmath-0.0.5/sqlmath/__init__.py
+-rw-rw-rw-   0        0        0   141019 2023-05-08 01:15:10.000000 sqlmath-0.0.5/sqlmath/sqlmath_dbapi2.py
+drwxrwxrwx   0        0        0        0 2023-05-08 03:19:58.263889 sqlmath-0.0.5/sqlmath.egg-info/
+-rw-rw-rw-   0        0        0     6911 2023-05-08 03:19:58.000000 sqlmath-0.0.5/sqlmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-05-08 03:19:58.000000 sqlmath-0.0.5/sqlmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 03:19:58.000000 sqlmath-0.0.5/sqlmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 03:19:58.000000 sqlmath-0.0.5/sqlmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    48961 2023-05-08 03:19:00.000000 sqlmath-0.0.5/sqlmath.mjs
+-rw-rw-rw-   0        0        0    73000 2023-05-05 23:31:29.000000 sqlmath-0.0.5/sqlmath_base.c
+-rw-rw-rw-   0        0        0   142223 2023-05-06 15:24:54.000000 sqlmath-0.0.5/sqlmath_browser.mjs
+-rw-rw-rw-   0        0        0     1514 2023-05-04 02:30:40.000000 sqlmath-0.0.5/sqlmath_custom.c
+-rw-rw-rw-   0        0        0      150 2022-06-07 06:43:45.000000 sqlmath-0.0.5/sqlmath_custom.mjs
+-rw-rw-rw-   0        0        0    32635 2023-05-05 23:31:29.000000 sqlmath-0.0.5/sqlmath_jenks.c
+-rw-rw-rw-   0        0        0     7931 2022-07-09 16:42:41.000000 sqlmath-0.0.5/sqlmath_wrapper_wasm.js
+-rw-rw-rw-   0        0        0    47352 2023-05-08 01:16:21.000000 sqlmath-0.0.5/test.mjs
```

### Comparing `sqlmath-0.0.1/LICENSE` & `sqlmath-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmath-0.0.1/README.md` & `sqlmath-0.0.5/README.md`

 * *Files identical despite different names*

