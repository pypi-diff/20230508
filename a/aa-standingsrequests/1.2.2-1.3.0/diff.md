# Comparing `tmp/aa-standingsrequests-1.2.2.tar.gz` & `tmp/aa_standingsrequests-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-standingsrequests-1.2.2.tar", last modified: Tue Jul 19 15:38:01 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa-standingsrequests-1.2.2.tar` & `aa_standingsrequests-1.3.0.tar`

### file list

```diff
@@ -1,119 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.886756 aa-standingsrequests-1.2.2/
--rw-rw-rw-   0 root         (0) root         (0)    35141 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-06-18 17:05:17.000000 aa-standingsrequests-1.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12363 2022-07-19 15:38:01.886756 aa-standingsrequests-1.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11393 2022-05-27 19:25:17.000000 aa-standingsrequests-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.866756 aa-standingsrequests-1.2.2/aa_standingsrequests.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12363 2022-07-19 15:38:01.000000 aa-standingsrequests-1.2.2/aa_standingsrequests.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4615 2022-07-19 15:38:01.000000 aa-standingsrequests-1.2.2/aa_standingsrequests.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 15:38:01.000000 aa-standingsrequests-1.2.2/aa_standingsrequests.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 15:38:01.000000 aa-standingsrequests-1.2.2/aa_standingsrequests.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       75 2022-07-19 15:38:01.000000 aa-standingsrequests-1.2.2/aa_standingsrequests.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-07-19 15:38:01.000000 aa-standingsrequests-1.2.2/aa_standingsrequests.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-19 15:38:01.886756 aa-standingsrequests-1.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1692 2022-07-19 15:24:00.000000 aa-standingsrequests-1.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.870756 aa-standingsrequests-1.2.2/standingsrequests/
--rw-rw-rw-   0 root         (0) root         (0)      126 2022-07-19 15:24:00.000000 aa-standingsrequests-1.2.2/standingsrequests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2022-02-11 22:44:52.000000 aa-standingsrequests-1.2.2/standingsrequests/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2211 2022-05-25 20:50:46.000000 aa-standingsrequests-1.2.2/standingsrequests/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2099 2022-02-11 22:44:52.000000 aa-standingsrequests-1.2.2/standingsrequests/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2022-05-26 14:58:46.000000 aa-standingsrequests-1.2.2/standingsrequests/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4540 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/core.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.870756 aa-standingsrequests-1.2.2/standingsrequests/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/helpers/evecharacter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/helpers/evecorporation.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/helpers/writers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.874755 aa-standingsrequests-1.2.2/standingsrequests/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     1125 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/management/commands/standingsrequests_sync_blue_alts.py
--rw-rw-rw-   0 root         (0) root         (0)    32649 2022-05-14 15:15:45.000000 aa-standingsrequests-1.2.2/standingsrequests/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.874755 aa-standingsrequests-1.2.2/standingsrequests/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     8896 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0002_contactlabel_labelid_bigintegerfield.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0003_rename_non_pep.py
--rw-rw-rw-   0 root         (0) root         (0)     5654 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0004_fix_types_and_indices.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0005_refactor_model_names.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0006_add_user_to_revocations.py
--rw-rw-rw-   0 root         (0) root         (0)     6950 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0007_big_performance_overhaul.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0008_add_revocation_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0009_make_ceo_optional.py
--rw-rw-rw-   0 root         (0) root         (0)     9280 2022-02-11 22:44:52.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/0010_add_request_log.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29570 2022-05-24 20:32:45.000000 aa-standingsrequests-1.2.2/standingsrequests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-06-18 17:05:17.000000 aa-standingsrequests-1.2.2/standingsrequests/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.874755 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/css/
--rw-rw-rw-   0 root         (0) root         (0)      171 2022-05-26 20:49:29.000000 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/css/create_requests.css
--rw-rw-rw-   0 root         (0) root         (0)      175 2022-05-24 14:44:27.000000 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)       50 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/css/manage.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.878755 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/img/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-light.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/js/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.878755 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/js/vendor/htmx/
--rw-rw-rw-   0 root         (0) root         (0)    37374 2022-05-12 22:21:52.000000 aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/js/vendor/htmx/htmx.min.js
--rw-rw-rw-   0 root         (0) root         (0)   887006 2022-06-18 17:05:17.000000 aa-standingsrequests-1.2.2/standingsrequests/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     6073 2022-02-11 22:44:52.000000 aa-standingsrequests-1.2.2/standingsrequests/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.862755 aa-standingsrequests-1.2.2/standingsrequests/templates/admin/standingsrequests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.878755 aa-standingsrequests-1.2.2/standingsrequests/templates/admin/standingsrequests/contactset/
--rw-rw-rw-   0 root         (0) root         (0)      245 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/admin/standingsrequests/contactset/change_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.878755 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/
--rw-rw-rw-   0 root         (0) root         (0)      438 2022-05-25 14:17:31.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.878755 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/bundles/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2022-05-27 19:02:38.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/bundles/helper-js.html
--rw-rw-rw-   0 root         (0) root         (0)      961 2022-05-25 20:50:46.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/bundles/htmx.html
--rw-rw-rw-   0 root         (0) root         (0)     4811 2022-05-27 19:02:38.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/create_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3433 2022-07-19 15:06:10.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/effective_requests.html
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-05-25 15:19:54.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/error.html
--rw-rw-rw-   0 root         (0) root         (0)     6175 2022-07-19 15:06:10.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/manage_requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.882755 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/
--rw-rw-rw-   0 root         (0) root         (0)      166 2022-05-13 20:03:01.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/manage_empty_row.html
--rw-rw-rw-   0 root         (0) root         (0)     3599 2022-05-26 15:26:31.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/manage_requests_list.html
--rw-rw-rw-   0 root         (0) root         (0)     3856 2022-05-26 15:26:31.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/manage_revocations_list.html
--rw-rw-rw-   0 root         (0) root         (0)     2460 2022-05-26 20:49:29.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/menu.html
--rw-rw-rw-   0 root         (0) root         (0)     5207 2022-05-26 20:49:29.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/request_characters.html
--rw-rw-rw-   0 root         (0) root         (0)     4363 2022-05-26 20:49:29.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/request_corporations.html
--rw-rw-rw-   0 root         (0) root         (0)      260 2022-05-24 20:32:45.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/spinner.html
--rw-rw-rw-   0 root         (0) root         (0)      665 2022-05-26 20:49:29.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/standing_symbol.html
--rw-rw-rw-   0 root         (0) root         (0)      571 2022-05-25 15:19:54.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tab_alliance_standings.html
--rw-rw-rw-   0 root         (0) root         (0)      894 2022-05-26 15:26:31.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tab_character_standings.html
--rw-rw-rw-   0 root         (0) root         (0)      951 2022-05-25 21:19:05.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tab_corporation_standings.html
--rw-rw-rw-   0 root         (0) root         (0)      655 2022-05-26 20:49:29.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tbl_effective_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     9253 2022-07-19 15:06:10.000000 aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/standings.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.886756 aa-standingsrequests-1.2.2/standingsrequests/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/entity_type_ids.py
--rw-rw-rw-   0 root         (0) root         (0)     9905 2022-05-14 15:15:45.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/my_test_data.json
--rw-rw-rw-   0 root         (0) root         (0)    19412 2022-07-19 15:24:00.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/my_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2757 2022-05-14 15:15:45.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     5132 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     6527 2022-03-02 15:01:48.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2021-12-02 10:37:43.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_helpers_evecharacter.py
--rw-rw-rw-   0 root         (0) root         (0)     4068 2022-05-14 15:15:45.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_helpers_evecorporation.py
--rw-rw-rw-   0 root         (0) root         (0)    38575 2022-05-14 15:15:45.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    34931 2022-07-19 15:24:00.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    25873 2022-02-11 22:44:52.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2022-05-14 15:15:45.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2022-05-26 19:17:30.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.886756 aa-standingsrequests-1.2.2/standingsrequests/tests/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-13 20:03:01.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26491 2022-05-14 15:15:45.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_create_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     3326 2022-05-26 19:17:30.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_effective_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    13017 2022-05-26 14:58:46.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_manage_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10324 2022-05-26 19:17:30.000000 aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_standings.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2022-05-25 20:50:46.000000 aa-standingsrequests-1.2.2/standingsrequests/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 15:38:01.886756 aa-standingsrequests-1.2.2/standingsrequests/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-13 20:03:01.000000 aa-standingsrequests-1.2.2/standingsrequests/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8744 2022-05-26 15:26:31.000000 aa-standingsrequests-1.2.2/standingsrequests/views/_common.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2022-05-13 20:03:01.000000 aa-standingsrequests-1.2.2/standingsrequests/views/admin.py
--rw-rw-rw-   0 root         (0) root         (0)    15569 2022-05-24 20:32:45.000000 aa-standingsrequests-1.2.2/standingsrequests/views/create_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     3179 2022-05-26 19:17:30.000000 aa-standingsrequests-1.2.2/standingsrequests/views/effective_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     5463 2022-05-13 20:03:01.000000 aa-standingsrequests-1.2.2/standingsrequests/views/manage_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    13191 2022-05-26 19:17:30.000000 aa-standingsrequests-1.2.2/standingsrequests/views/standings.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/__init__.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/admin.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/app_settings.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/apps.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/auth_hooks.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/constants.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/core.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/decorators.py
+-rw-r--r--   0        0        0    32714 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/managers.py
+-rw-r--r--   0        0        0    29814 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/models.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/providers.py
+-rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/swagger.json
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tasks.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/helpers/__init__.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/helpers/evecharacter.py
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/helpers/evecorporation.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/helpers/writers.py
+-rw-r--r--   0        0        0    17178 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/django.pot
+-rw-r--r--   0        0        0    17225 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17225 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17225 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17178 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17178 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17178 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17369 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17456 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/management/commands/standingsrequests_sync_blue_alts.py
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0001_initial.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0002_contactlabel_labelid_bigintegerfield.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0003_rename_non_pep.py
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0004_fix_types_and_indices.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0005_refactor_model_names.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0006_add_user_to_revocations.py
+-rw-r--r--   0        0        0     6949 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0007_big_performance_overhaul.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0008_add_revocation_reason.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0009_make_ceo_optional.py
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/0010_add_request_log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/migrations/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/css/create_requests.css
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/css/global.css
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/css/manage.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    37374 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/js/vendor/htmx/htmx.min.js
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/admin/standingsrequests/contactset/change_list.html
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/_base.html
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/create_requests.html
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/effective_requests.html
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/error.html
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/manage_requests.html
+-rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/standings.html
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/bundles/helper-js.html
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/bundles/htmx.html
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/manage_empty_row.html
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/manage_requests_list.html
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/manage_revocations_list.html
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/menu.html
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/request_characters.html
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/request_corporations.html
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/spinner.html
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/standing_symbol.html
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tab_alliance_standings.html
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tab_character_standings.html
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tab_corporation_standings.html
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tbl_effective_requests.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/__init__.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/entity_type_ids.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/my_test_data.json
+-rw-r--r--   0        0        0    19411 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/my_test_data.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_commands.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_core.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_decorators.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_helpers_evecharacter.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_helpers_evecorporation.py
+-rw-r--r--   0        0        0    38574 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_integration.py
+-rw-r--r--   0        0        0    34931 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_managers.py
+-rw-r--r--   0        0        0    25873 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_models.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/test_tasks.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/views/__init__.py
+-rw-r--r--   0        0        0    26519 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_create_requests.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_effective_requests.py
+-rw-r--r--   0        0        0    13017 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_manage_requests.py
+-rw-r--r--   0        0        0    11286 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_standings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/views/__init__.py
+-rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/views/_common.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/views/admin.py
+-rw-r--r--   0        0        0    15817 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/views/create_requests.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/views/effective_requests.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/views/manage_requests.py
+-rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/standingsrequests/views/standings.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/.gitignore
+-rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/LICENSE
+-rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/README.md
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13442 2020-02-02 00:00:00.000000 aa_standingsrequests-1.3.0/PKG-INFO
```

### Comparing `aa-standingsrequests-1.2.2/LICENSE` & `aa_standingsrequests-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/PKG-INFO` & `aa_standingsrequests-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 Metadata-Version: 2.1
 Name: aa-standingsrequests
-Version: 1.2.2
+Version: 1.3.0
 Summary: App for managing character standing requests, made for Alliance Auth
-Home-page: https://gitlab.com/ErikKalkoken/aa-standingsrequests
-Author: Erik Kalkoken
-Author-email: kaloken87@gmail.com
-License: GPL-3.0
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-standingsrequests
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-standingsrequests
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-standingsrequests/-/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-standingsrequests/-/issues
+Author-email: Erik Kalkoken <kaloken87@gmail.com>
+License-Expression: GPL-3.0
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
+Requires-Python: >=3.8
+Requires-Dist: allianceauth-app-utils>=1.18
+Requires-Dist: allianceauth>=3
+Requires-Dist: django-eveuniverse>=0.19.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Standings Requests
 
 App for managing character standing requests, made for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth).
 
-![release](https://img.shields.io/pypi/v/aa-standingsrequests?label=release) ![python](https://img.shields.io/pypi/pyversions/aa-standingsrequests) ![django](https://img.shields.io/pypi/djversions/aa-standingsrequests?label=django) ![pipeline](https://gitlab.com/ErikKalkoken/aa-standingsrequests/badges/master/pipeline.svg) ![coverage](https://gitlab.com/ErikKalkoken/aa-standingsrequests/badges/master/coverage.svg) ![license](https://img.shields.io/badge/license-GPLv3-green) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+[![release](https://img.shields.io/pypi/v/aa-standingsrequests?label=release)](https://pypi.org/project/aa-standingsrequests/)
+[![python](https://img.shields.io/pypi/pyversions/aa-standingsrequests)](https://pypi.org/project/aa-standingsrequests/)
+[![django](https://img.shields.io/pypi/djversions/aa-standingsrequests?label=django)](https://pypi.org/project/aa-standingsrequests/)
+[![pipeline](https://gitlab.com/ErikKalkoken/aa-standingsrequests/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/aa-standingsrequests/-/pipelines)
+[![codecov](https://codecov.io/gl/ErikKalkoken/aa-standingsrequests/branch/master/graph/badge.svg?token=gf23N35S3S)](https://codecov.io/gl/ErikKalkoken/aa-standingsrequests)
+[![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/aa-standingsrequests/-/blob/master/LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Contents
 
 - [Features](#features)
 - [Screenshots](#screenshots)
 - [Installation](#installation)
 - [Settings](#settings)
@@ -248,9 +261,7 @@
 
 Standings created by this command will not have an actioner name set.
 
 ## History
 
 This is a fork of [Basraah's standingrequests](https://gitlab.com/ErikKalkoken/aa-standingsrequests).
 Big thanks to Basraah for all his effort in developing the initial version.
-
-
```

### Comparing `aa-standingsrequests-1.2.2/README.md` & `aa_standingsrequests-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Standings Requests
 
 App for managing character standing requests, made for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth).
 
-![release](https://img.shields.io/pypi/v/aa-standingsrequests?label=release) ![python](https://img.shields.io/pypi/pyversions/aa-standingsrequests) ![django](https://img.shields.io/pypi/djversions/aa-standingsrequests?label=django) ![pipeline](https://gitlab.com/ErikKalkoken/aa-standingsrequests/badges/master/pipeline.svg) ![coverage](https://gitlab.com/ErikKalkoken/aa-standingsrequests/badges/master/coverage.svg) ![license](https://img.shields.io/badge/license-GPLv3-green) ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+[![release](https://img.shields.io/pypi/v/aa-standingsrequests?label=release)](https://pypi.org/project/aa-standingsrequests/)
+[![python](https://img.shields.io/pypi/pyversions/aa-standingsrequests)](https://pypi.org/project/aa-standingsrequests/)
+[![django](https://img.shields.io/pypi/djversions/aa-standingsrequests?label=django)](https://pypi.org/project/aa-standingsrequests/)
+[![pipeline](https://gitlab.com/ErikKalkoken/aa-standingsrequests/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/aa-standingsrequests/-/pipelines)
+[![codecov](https://codecov.io/gl/ErikKalkoken/aa-standingsrequests/branch/master/graph/badge.svg?token=gf23N35S3S)](https://codecov.io/gl/ErikKalkoken/aa-standingsrequests)
+[![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/aa-standingsrequests/-/blob/master/LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Contents
 
 - [Features](#features)
 - [Screenshots](#screenshots)
 - [Installation](#installation)
 - [Settings](#settings)
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/admin.py` & `aa_standingsrequests-1.3.0/standingsrequests/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,10 +131,9 @@
 
     def has_change_permission(self, *args, **kwargs):
         return False
 
     def has_add_permission(self, *args, **kwargs):
         return False
 
-    # TODO: enable for production
-    # def has_delete_permission(self, *args, **kwargs) -> bool:
-    #     return False
+    def has_delete_permission(self, *args, **kwargs) -> bool:
+        return False
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/app_settings.py` & `aa_standingsrequests-1.3.0/standingsrequests/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/auth_hooks.py` & `aa_standingsrequests-1.3.0/standingsrequests/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/core.py` & `aa_standingsrequests-1.3.0/standingsrequests/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if cls.operation_mode is OperationMode.ALLIANCE:
             if character.alliance_id:
                 entity, _ = EveEntity.objects.get_or_create_esi(
                     id=character.alliance_id
                 )
             else:
                 entity = None
-        elif cls.operation_mode is OperationMode.CORPORATON:
+        elif cls.operation_mode is OperationMode.CORPORATION:
             entity, _ = EveEntity.objects.get_or_create_esi(id=character.corporation_id)
         else:
             raise NotImplementedError()
 
         return entity
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/decorators.py` & `aa_standingsrequests-1.3.0/standingsrequests/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/helpers/evecharacter.py` & `aa_standingsrequests-1.3.0/standingsrequests/helpers/evecharacter.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/helpers/evecorporation.py` & `aa_standingsrequests-1.3.0/standingsrequests/helpers/evecorporation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from concurrent.futures import ThreadPoolExecutor
+from typing import List
 
 from bravado.exception import HTTPError
 
 from django.contrib.auth.models import User
 from django.core.cache import cache
 from eveuniverse.models import EveEntity
 
 from allianceauth.eveonline.evelinks import eveimageserver
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
-from .. import __title__
-from ..providers import esi
+from standingsrequests import __title__
+from standingsrequests.providers import esi
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 MAX_WORKERS = 10
 
 
 class EveCorporation:
     CACHE_PREFIX = "STANDINGS_REQUESTS_EVECORPORATION_"
     CACHE_TIME = 60 * 60  # 60 minutes
 
     def __init__(self, **kwargs):
-        self.corporation_id = int(kwargs.get("corporation_id"))
+        self.corporation_id = int(kwargs.get("corporation_id", 0))
         self.corporation_name = kwargs.get("corporation_name")
         self.ticker = kwargs.get("ticker")
         self.member_count = kwargs.get("member_count")
         self.ceo_id = kwargs.get("ceo_id")
         self.alliance_id = kwargs.get("alliance_id")
         self.alliance_name = kwargs.get("alliance_name")
 
@@ -160,33 +161,35 @@
 
     @classmethod
     def thread_fetch_corporation(cls, corporation_id: int) -> object:
         """Gets one corporation by ID and returns it - used for threads"""
         return EveCorporation.get_by_id(corporation_id)
 
     @classmethod
-    def get_many_by_id(cls, corporation_ids: list) -> list:
+    def get_many_by_id(cls, corporation_ids: List[int]) -> list:
         """Returns multiple corporations by ID
 
         Fetches requested corporations from cache or API as needed.
         Uses threads to fetch them in parallel.
         """
-        corporation_ids = set(corporation_ids)
-        if not corporation_ids:
+        corporation_ids2 = set(corporation_ids)
+        if not corporation_ids2:
             return []
 
         # make sure client is loaded before starting threads
-        esi.client
+        esi.client.Status.get_status().results()
         logger.info(
             "Starting to fetch the %d corporations from ESI with up to %d workers",
-            len(corporation_ids),
+            len(corporation_ids2),
             MAX_WORKERS,
         )
         with ThreadPoolExecutor(max_workers=MAX_WORKERS) as executor:
             futures = [
                 executor.submit(cls.thread_fetch_corporation, corporation_id)
-                for corporation_id in corporation_ids
+                for corporation_id in corporation_ids2
             ]
             logger.info("Waiting for all threads fetching corporations to complete...")
 
-        logger.info("Completed fetching %d corporations from ESI", len(corporation_ids))
+        logger.info(
+            "Completed fetching %d corporations from ESI", len(corporation_ids2)
+        )
         return [f.result() for f in futures]
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/helpers/writers.py` & `aa_standingsrequests-1.3.0/standingsrequests/helpers/writers.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/management/commands/standingsrequests_sync_blue_alts.py` & `aa_standingsrequests-1.3.0/standingsrequests/management/commands/standingsrequests_sync_blue_alts.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/managers.py` & `aa_standingsrequests-1.3.0/standingsrequests/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             ).results()
             self.labels = [self.Label(label) for label in labels]
             contacts = esi.client.Contacts.get_alliances_alliance_id_contacts(
                 alliance_id=owner_character.alliance_id,
                 token=token.valid_access_token(),
             ).results()
 
-        elif BaseConfig.operation_mode is OperationMode.CORPORATON:
+        elif BaseConfig.operation_mode is OperationMode.CORPORATION:
             labels = (
                 esi.client.Contacts.get_corporations_corporation_id_contacts_labels(
                     corporation_id=owner_character.corporation_id,
                     token=token.valid_access_token(),
                 ).results()
             )
             self.labels = [self.Label(label) for label in labels]
@@ -232,18 +232,16 @@
             is_satisfied_standing = standing_request.evaluate_effective_standing()
             if is_satisfied_standing and not is_currently_effective:
                 if SR_NOTIFICATIONS_ENABLED:
                     # send notification to user about standing change if enabled
                     if standing_request.is_standing_request:
                         notify(
                             user=standing_request.user,
-                            title=_(
-                                "%s: Standing with %s now in effect"
-                                % (__title__, contact.name)
-                            ),
+                            title=_("%s: Standing with %s now in effect")
+                            % (__title__, contact.name),
                             message=_(
                                 "'%(organization_name)s' now has blue standing with "
                                 "your alt %(contact_category)s '%(contact_name)s'. "
                                 "Please also update the standing of "
                                 "your %(contact_category)s accordingly."
                             )
                             % {
@@ -303,26 +301,29 @@
                 actioned_timeout = standing_request.check_actioned_timeout()
                 if actioned_timeout is not None and actioned_timeout:
                     logger.info(
                         "Standing request for contact ID %d has timedout "
                         "and will be reset" % standing_request.contact_id
                     )
                     if SR_NOTIFICATIONS_ENABLED:
-                        title = _("Standing Request for %s reset" % contact.name)
-                        message = _(
-                            "The standing request for %(contact_category)s "
-                            "'%(contact_name)s' from %(user_name)s "
-                            "has been reset as it did not appear in "
-                            "game before the timeout period expired."
+                        title = _("Standing Request for %s reset") % contact.name
+                        message = (
+                            _(
+                                "The standing request for %(contact_category)s "
+                                "'%(contact_name)s' from %(user_name)s "
+                                "has been reset as it did not appear in "
+                                "game before the timeout period expired."
+                            )
                             % {
                                 "contact_category": contact.category,
                                 "contact_name": contact.name,
                                 "user_name": standing_request.user.username,
                             },
                         )
+
                         # Notify standing manager
                         notify(user=actioned_timeout, title=title, message=message)
                         # Notify the user
                         notify(user=standing_request.user, title=title, message=message)
 
     def has_pending_request(self, contact_id: int) -> bool:
         """Checks if a request is pending for the given contact_id
@@ -477,15 +478,19 @@
             defaults={"user": user},
         )
         return instance
 
 
 class StandingRevocationManager(AbstractStandingsRequestManager):
     def add_revocation(
-        self, contact_id: int, contact_type: str, user: User = None, reason: str = None
+        self,
+        contact_id: int,
+        contact_type: str,
+        user: Optional[User] = None,
+        reason: Optional[str] = None,
     ) -> object:
         """Add a new standings revocation
 
         Params:
         - contact_id: contact_id to request standings on
         - contact_type_id: contact_type_id from AbstractContact concrete implementation
         - user: user making the request
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0001_initial.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0003_rename_non_pep.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0003_rename_non_pep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.13 on 2020-06-18 16:21
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("standingsrequests", "0002_contactlabel_labelid_bigintegerfield"),
     ]
 
     operations = [
         migrations.RenameField(
             model_name="abstractstandingsrequest",
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0004_fix_types_and_indices.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0004_fix_types_and_indices.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("standingsrequests", "0003_rename_non_pep"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="evenamecache",
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0005_refactor_model_names.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0005_refactor_model_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.13 on 2020-07-07 19:43
 
 from django.conf import settings
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     atomic = False
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("standingsrequests", "0004_fix_types_and_indices"),
     ]
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0006_add_user_to_revocations.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0006_add_user_to_revocations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("standingsrequests", "0005_refactor_model_names"),
     ]
 
     operations = [
         migrations.AddField(
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0007_big_performance_overhaul.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0007_big_performance_overhaul.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.10 on 2021-05-12 19:51
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveuniverse", "0005_type_materials_and_sections"),
         ("eveonline", "0014_auto_20210105_1413"),
         ("standingsrequests", "0006_add_user_to_revocations"),
     ]
 
     operations = [
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0008_add_revocation_reason.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0008_add_revocation_reason.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.10 on 2021-05-13 19:49
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("standingsrequests", "0007_big_performance_overhaul"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="standingrevocation",
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0009_make_ceo_optional.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0009_make_ceo_optional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.9 on 2021-12-01 18:58
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveuniverse", "0005_type_materials_and_sections"),
         ("standingsrequests", "0008_add_revocation_reason"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/migrations/0010_add_request_log.py` & `aa_standingsrequests-1.3.0/standingsrequests/migrations/0010_add_request_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django.conf import settings
 from django.db import migrations, models
 
 import standingsrequests.models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("authentication", "0019_merge_20211026_0919"),
         ("eveuniverse", "0005_type_materials_and_sections"),
         ("standingsrequests", "0009_make_ceo_optional"),
     ]
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/models.py` & `aa_standingsrequests-1.3.0/standingsrequests/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import timedelta
-from typing import List
+from typing import List, Optional
 
 from django.contrib.auth.models import User
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.utils.functional import cached_property
 from django.utils.html import format_html
 from django.utils.timezone import now
@@ -122,15 +122,15 @@
         return created_counter
 
     @staticmethod
     def required_esi_scope() -> str:
         """returns the required ESI scopes for syncing"""
         if BaseConfig.operation_mode is OperationMode.ALLIANCE:
             return "esi-alliances.read_contacts.v1"
-        elif BaseConfig.operation_mode is OperationMode.CORPORATON:
+        elif BaseConfig.operation_mode is OperationMode.CORPORATION:
             return "esi-corporations.read_contacts.v1"
         else:
             raise NotImplementedError()
 
 
 class ContactLabel(models.Model):
     """A contact label"""
@@ -177,15 +177,15 @@
         )
 
     @property
     def name(self) -> str:
         return self.eve_entity.name
 
     @property
-    def is_standing_satisfied(self) -> str:
+    def is_standing_satisfied(self) -> bool:
         return StandingRequest.is_standing_satisfied(self.standing)
 
     @cached_property
     def labels_sorted(self) -> List[str]:
         return sorted([label.name for label in self.labels.all()])
 
 
@@ -250,14 +250,18 @@
 
     class Meta:
         permissions = (
             ("affect_standings", "User can process standings requests."),
             ("request_standings", "User can request standings."),
         )
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # self.reason = ""
+
     def __repr__(self) -> str:
         try:
             user_str = f", user='{self.user}'"
         except AttributeError:
             user_str = ""
 
         return (
@@ -394,15 +398,19 @@
         try:
             latest = ContactSet.objects.latest()
         except ContactSet.DoesNotExist:
             logger.debug("Cannot check standing timeout, no standings available")
             return None
 
         # Reset request that has not become effective after timeout expired
-        if self.action_date + timedelta(hours=SR_STANDING_TIMEOUT_HOURS) < latest.date:
+        if (
+            self.action_date
+            and self.action_date + timedelta(hours=SR_STANDING_TIMEOUT_HOURS)
+            < latest.date
+        ):
             logger.info(
                 "Standing actioned timed out, resetting actioned for contact_id %d",
                 self.contact_id,
             )
             actioner = self.action_by
             self.action_by = None
             self.action_date = None
@@ -506,15 +514,17 @@
             contact_id=self.contact_id,
             contact_type=StandingRevocation.ContactType.CORPORATION,
             user=self.user,
             reason=StandingRevocation.Reason.OWNER_REQUEST,
         )
         return True
 
-    def delete(self, using=None, keep_parents=False, reason=None):
+    def delete(
+        self, using=None, keep_parents: bool = False, reason: Optional[str] = None
+    ):
         """
         Add a revocation before deleting if the standing has been
         actioned (pending) or is effective and
         doesn't already have a pending revocation request.
         """
         if self.action_by is not None or self.is_effective:
             # Check if theres not already a revocation pending
@@ -664,15 +674,15 @@
 
     objects = CharacterAffiliationManager()
 
     def __str__(self) -> str:
         return self.character.name
 
     @cached_property
-    def character_name(self) -> str:
+    def character_name(self) -> Optional[str]:
         """Return character name for main."""
         return self.character.name if self.character.name else None
 
     def entity_ids(self) -> set:
         """Ids of all entities."""
         return set(
             filter(
@@ -818,15 +828,15 @@
                 default_if_none(self.character, "-"),
                 default_if_none(self.corporation, "-"),
             )
         return str(self.user)
 
 
 class FrozenAlt(FrozenModelMixin, models.Model):
-    """Alt with alignmants. Objects are frozen at creation and can not be changed."""
+    """Alt with alignments. Objects are frozen at creation and can not be changed."""
 
     class Category(models.TextChoices):
         CHARACTER = "CH", "character"
         CORPORATION = "CP", "corporation"
 
     alliance = models.ForeignKey(
         EveEntity, on_delete=models.SET_NULL, null=True, related_name="+"
@@ -841,15 +851,15 @@
     faction = models.ForeignKey(
         EveEntity, on_delete=models.SET_NULL, null=True, related_name="+"
     )
 
     objects = FrozenAltManager()
 
     def __str__(self) -> str:
-        return str(self.character) if self.character else (self.corporation)
+        return str(self.character) if self.character else str(self.corporation)
 
     @property
     def is_character(self) -> bool:
         return self.category == self.Category.CHARACTER
 
     @property
     def is_corporation(self) -> bool:
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-dark.gif` & `aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-light.gif` & `aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/static/standingsrequests/js/vendor/htmx/htmx.min.js` & `aa_standingsrequests-1.3.0/standingsrequests/static/standingsrequests/js/vendor/htmx/htmx.min.js`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/swagger.json` & `aa_standingsrequests-1.3.0/standingsrequests/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tasks.py` & `aa_standingsrequests-1.3.0/standingsrequests/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,30 +48,28 @@
         except User.DoesNotExist:
             logger.warning("Can not find a user with pk %d", user_pk)
             return
         else:
             source_entity = BaseConfig.standings_source_entity()
             notify(
                 user,
-                _("%s: Standings loaded" % __title__),
-                _(
-                    "Standings have been successfully loaded for %s"
-                    % source_entity.name
-                ),
+                _("%s: Standings loaded") % __title__,
+                _("Standings have been successfully loaded for %s")
+                % source_entity.name,
                 level="success",
             )
 
 
 @shared_task(name="standings_requests.standings_update")
 def standings_update():
     """Updates standings from ESI"""
     logger.info("Standings API update started")
     contact_set = ContactSet.objects.create_new_from_api()
     if not contact_set:
-        logger.warn(
+        logger.warning(
             "Standings API update returned None (API error probably),"
             "aborting standings update"
         )
     else:
         if SR_SYNC_BLUE_ALTS_ENABLED:
             contact_set.generate_standing_requests_for_blue_alts()
         StandingRequest.objects.process_requests()
@@ -150,15 +148,15 @@
                 ContactLabel.objects.filter(contact_set=contact_set).delete()
 
             stale_contacts_qs.delete()
         else:
             logger.debug("No ContactSets to delete")
 
     except ContactSet.DoesNotExist:
-        logger.warn("No ContactSets available, nothing to delete")
+        logger.warning("No ContactSets available, nothing to delete")
 
 
 @shared_task
 def update_all_corporation_details():
     existing_corporation_ids = (
         CorporationDetails.objects.corporation_ids_from_contacts()
     )
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/bundles/helper-js.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/bundles/helper-js.html`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/bundles/htmx.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/bundles/htmx.html`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/create_requests.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/create_requests.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 {% extends "standingsrequests/_base.html" %}
 {% load static %}
 {% load i18n %}
 
 {% block details %}
     <h2>{% translate "My Requests" %}</h2>
     <p class="text-muted">
-        On this page you can create requests to <strong>get standing</strong> or <strong>revoke standing</strong> with <strong>{{ organization.name }}</strong> for your alts. If you are missing an alt, please add it first on the dashboard.
+        {% blocktranslate with organization_name=organization.name %}
+            On this page you can create requests to get standing or revoke standing with {{ organization_name }} for your alts.
+            If you are missing an alt, please add it first on the dashboard.
+        {% endblocktranslate %}
     </p>
 
     <ul id="myTabs" class="nav nav-tabs" role="tablist">
         <li role="presentation" class="active">
             <a href="#tab-characters" aria-controls="tab-characters" role="tab" data-toggle="tab">
-                My Characters
+                {% translate "My Characters" %}
             </a>
         </li>
         {% if corporations_enabled %}
             <li role="presentation">
                 <a href="#tab-corporations" aria-controls="tab-corporations" role="tab" data-toggle="tab">
-                    My Corporations
+                    {% translate "My Corporations" %}
                 </a>
             </li>
         {% endif %}
     </ul>
 
     <div class="panel panel-default panel-tabs">
         <div class="panel-body">
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/effective_requests.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/effective_requests.html`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 {% load bootstrap %}
 {% load static %}
 {% load i18n %}
 
 {% block details %}
     <h2>{% translate "Effective Requests" %}</h2>
     {% include "standingsrequests/partials/tbl_effective_requests.html" %}
-    <p class="text-muted">All effective standing requests for <strong>{{organization.name}}</strong> • This data is cached</p>
+    <p class="text-muted">
+        {% blocktranslate with organization_name=organization.name %}
+            All effective standing requests for {{organization_name}} • This data is cached
+        {% endblocktranslate %}
+    </p>
 {% endblock details %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
     {% include 'bundles/filterdropdown-js.html' %}
     <script type="application/javascript">
         $(document).ready(function () {
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/manage_requests.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/manage_requests.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 
 {% block details %}
     <h2>{% translate "Manage Requests" %}</h2>
 
     <ul id="myTabs" class="nav nav-tabs" role="tablist">
         <li role="presentation">
             <a href="#tab-requests" aria-controls="tab-requests" role="tab" data-toggle="tab">
-                Open Requests
+                {% translate "Open Requests" %}
                 {% if requests_count > 0 %}
                     &nbsp;<span class="badge badge-nav alert-info">
                         {{ requests_count }}
                     </span>
                 {% endif %}
             </a>
         </li>
         <li role="presentation">
             <a href="#tab-revocations" aria-controls="tab-revocations" role="tab" data-toggle="tab">
-                Open Revocations
+                {% translate "Open Revocations" %}
                 {% if revocations_count > 0 %}
                     &nbsp;<span class="badge badge-nav alert-info">
                         {{ revocations_count }}
                     </span>
                 {% endif %}
             </a>
         </li>
         <li role="presentation">
             <a href="#tab-effective-requests" aria-controls="tab-effective-requests" role="tab" data-toggle="tab">
-                Effective Requests
+                {% translate "Effective Requests" %}
             </a>
         </li>
     </ul>
 
     <div class="panel panel-default panel-tabs">
         <div class="panel-body">
             <div class="tab-content">
@@ -41,32 +41,40 @@
                 <div role="tabpanel" class="tab-pane" id="tab-requests">
                     <div
                         hx-get="{% url 'manage_requests_list' %}"
                         hx-trigger="load">
                         {% include "standingsrequests/partials/spinner.html" %}
                     </div>
                     <p class="text-muted">
-                        Standing requests with pending action for <strong>{{organization.name}}</strong>
+                        {% blocktranslate with organization_name=organization.name %}
+                            Standing requests with pending action for {{ organization_name }}
+                        {% endblocktranslate %}
                     </p>
                 </div>
 
                 <div role="tabpanel" class="tab-pane" id="tab-revocations">
                     <div
                         hx-get="{% url 'manage_revocations_list' %}"
                         hx-trigger="load">
                         {% include "standingsrequests/partials/spinner.html" %}
                     </div>
                     <p class="text-muted">
-                        Standing revocations with pending action for <strong>{{organization.name}}</strong>
+                        {% blocktranslate with organization_name=organization.name %}
+                            Standing revocations with pending action for {{ organization_name }}
+                        {% endblocktranslate %}
                     </p>
                 </div>
 
                 <div role="tabpanel" class="tab-pane" id="tab-effective-requests">
                     {% include "standingsrequests/partials/tbl_effective_requests.html" %}
-                    <p class="text-muted">Currently effective standing requests for <strong>{{organization.name}}</strong> • This data is cached</p>
+                    <p class="text-muted">
+                        {% blocktranslate with organization_name=organization.name %}
+                            Currently effective standing requests for {{ organization_name }} • This data is cached
+                        {% endblocktranslate %}
+                    </p>
                 </div>
 
 
             </div>
         </div>
     </div>
 {% endblock details %}
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/manage_requests_list.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/manage_requests_list.html`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,22 @@
                         {% endif %}
                         {{contact.state}}
                     </td>
                     <td>
                         <button class="btn btn-success"
                                 hx-put="{% url 'manage_requests_write' contact.contact_id %}"
                                 title="{% translate 'Confirm the standing was ADDED in game' %}">
-                            Confirm
+                            {% translate "Confirm" %}
                         </button>
                         &nbsp;&nbsp;&nbsp;&nbsp;
                         <button class="btn btn-danger"
                                 hx-confirm="{% translate 'Are you sure?' %}"
                                 hx-delete="{% url 'manage_requests_write' contact.contact_id %}"
                                 title="{% translate 'Reject this standing request' %}">
-                            Reject
+                            {% translate "Reject" %}
                         </button>
                     </td>
                 </tr>
             {% empty %}
                 {% include "standingsrequests/partials/manage_empty_row.html" %}
             {% endfor %}
         </tbody>
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/manage_revocations_list.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/manage_revocations_list.html`

 * *Files 3% similar despite different names*

```diff
@@ -47,22 +47,22 @@
                         {{ contact.reason }}<br>
                         {{ contact.labels|join:", " }}
                     </td>
                     <td>
                         <button class="btn btn-success"
                                 hx-put="{% url 'manage_revocations_write' contact.contact_id %}"
                                 title="{% translate 'Confirm the standing was REMOVED in game' %}">
-                            Confirm
+                            {% translate "Confirm" %}
                         </button>
                         &nbsp;&nbsp;&nbsp;&nbsp;
                         <button class="btn btn-danger"
                                 hx-confirm="{% translate 'Are you sure?' %}"
                                 hx-delete="{% url 'manage_revocations_write' contact.contact_id %}"
                                 title="{% translate 'Reject this revocation request' %}">
-                            Reject
+                            {% translate "Reject" %}
                         </button>
                     </td>
                 </tr>
             {% empty %}
                 {% include "standingsrequests/partials/manage_empty_row.html" %}
             {% endfor %}
         </tbody>
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/menu.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/menu.html`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         <div class="navbar-header">
             <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
                 <span class="sr-only">{% translate "Toggle navigation" %}</span>
                 <span class="icon-bar"></span>
                 <span class="icon-bar"></span>
                 <span class="icon-bar"></span>
             </button>
-            <a class="navbar-brand" href="{% url 'standingsrequests:index' %}">{% translate app_title %}</a>
+            <a class="navbar-brand" href="{% url 'standingsrequests:index' %}">{{ app_title }}</a>
         </div>
         <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
             <ul class="nav navbar-nav">
                 <li class="{% navactive request 'standingsrequests:create_requests' %}">
                     <a href="{% url 'standingsrequests:create_requests' %}">{% translate "My Requests" %}</a>
                 </li>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load i18n %} {% load navactive %}
- {% translate "Toggle navigation" %}     {%_translate_app_title_%}
+ {% translate "Toggle navigation" %}     {{_app_title_}}
     * {%_translate_"My_Requests"_%}
     * {% if perms.standingsrequests.affect_standings %}
     * {%_translate_"Manage_Requests"_%}_{%_if_pending_total_count_>_0_%}_ {
       {_pending_total_count_}}_{%_endif_%}
     * {% endif %}
     * {{_operation_mode|capfirst_}}_{%_translate_"Standings"_%}
     * {% if perms.standingsrequests.affect_standings %} {%_if_operation_mode_==
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/request_characters.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/request_characters.html`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,17 @@
                     <td>
                         {{ std.character.alliance_name|default_if_none:"" }}
                     </td>
                     <td>
                         {% if std.hasRequiredScopes %}
                             <i class="fas fa-check fa-fw fa-lg text-success" title="Has required scopes"></i>
                         {% else %}
-                            <a title="{% translate 'Add required scopes' %}" class="btn btn-danger btn-sm" href="{% url 'standingsrequests:view_requester_add_scopes' %}">
+                            <a  title="{% translate 'Add required scopes' %}"
+                                class="btn btn-danger btn-sm"
+                                href="{% url 'standingsrequests:view_requester_add_scopes' %}">
                                 <i class="fas fa-plus fa-fw fa-lg"></i> {% translate "Required" %}
                             </a>
                         {% endif %}
                     </td>
                     <td>
                         {% if std.inOrganisation == True %}
                             <i class="fas fa-star fa-fw fa-lg text-primary" title="{% translate 'In Organisation' %}"></i>
@@ -53,41 +55,44 @@
                         {% if std.inOrganisation == True %}
                             <!-- Already in organisation, No actions -->
                         {% elif std.pendingRequest == True or std.requestActioned == True %}
                             <a
                                 class="btn btn-warning"
                                 role="button"
                                 href="{% url 'standingsrequests:remove_character_standing' character_id=std.character.character_id %}"
-                                title="Cancel Request">
-                                Cancel
+                                title="{% translate 'Cancel Request' %}">
+                                {% translate "Cancel" %}
                             </a>
                         {% elif std.pendingRevocation == True %}
                             <!-- Revoked, No actions -->
                         {% elif not std.hasStanding %}
                             {% if std.hasRequiredScopes %}
                                 <a
                                     class="btn btn-primary"
                                     role="button"
                                     href="{% url 'standingsrequests:request_character_standing' character_id=std.character.character_id %}"
-                                    title="Request to get standing for this character"
+                                    title="{% translate 'Request to get standing for this character' %}"
                                     >
-                                    &nbsp;Apply&nbsp;
+                                    {% translate "Apply" %}
                                 </a>
                             {% else %}
-                                <button class="btn btn-primary" role="button" title="Missing scopes" disabled>
-                                    &nbsp;Apply&nbsp;
+                                <button
+                                    class="btn btn-primary"
+                                    role="button"
+                                    title="{% translate 'Missing scopes' %}" disabled>
+                                    {% translate "Apply" %}
                                 </button>
                             {% endif %}
                         {% else %}
                             <a
                                 class="btn btn-danger"
                                 role="button"
                                 href="{% url 'standingsrequests:remove_character_standing' character_id=std.character.character_id %}"
-                                title="Request to revoke standing for this character">
-                                Revoke
+                                title="{% translate 'Request to revoke standing for this character' %}">
+                                {% translate "Revoke" %}
                             </a>
                         {% endif %}
                     </td>
                 </tr>
             {% endfor %}
         </tbody>
     </table>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 {% load i18n %} {% load evelinks %}
-{% translate "Character" %}                            {% translate "Corporation" %}    {% translate "Alliance" %}                   {% translate "Scopes" {% translate          {% translate "Actions" %}
-                                                                                                                                     %}                    "Standing" %}
-                                                                                                                                                           {% if
-                                                                                                                                                           std.inOrganisation ==
-                                                                                                                                                           True %}  {% elif
-                                                                                                                                                           std.requestActioned
-                                                                                                                                                           == True %}  {% elif
-                                                                                                                                                           std.pendingRequest ==
-                                                                                                                                                           True %}  {% elif
-                                                       [{                                                                            {% if                 std.pendingRevocation
-                                                       {                                {                                            std.hasRequiredScopes == True %}  {% elif   {% if std.inOrganisation == True %}  {% elif std.pendingRequest == True or
-[{{ std.character|character_portrait_url:32 }}]   { std.character.corporation_ticker {                                            %}  {% else %}        std.standing == None  std.requestActioned == True %} Cancel {% elif std.pendingRevocation ==
-{ std.character.character_name }}                      }}] {                            std.character.alliance_name|default_if_none:  {%_translate         and                   True %}  {% elif not std.hasStanding %} {% if std.hasRequiredScopes %}
-                                                       { std.character.corporation_name "" }}                                        "Required"_%}         std.pendingRequest ==  Apply  {% else %}   Apply   {% endif %} {% else %} Revoke {% endif %}
-                                                       }}                                                                             {% endif %}          False %}  {% else %}
-                                                                                                                                                           {% include
-                                                                                                                                                           'standingsrequests/
-                                                                                                                                                           partials/
-                                                                                                                                                           standing_symbol.html'
-                                                                                                                                                           with
-                                                                                                                                                           standing=std.standing
-                                                                                                                                                           %} {% endif %}
+{% translate "Character" %}                            {% translate "Corporation" %}    {% translate "Alliance" %}                   {% translate "Scopes" {% translate          {% translate
+                                                                                                                                     %}                    "Standing" %}         "Actions" %}
+                                                                                                                                                           {% if                 {% if
+                                                                                                                                                           std.inOrganisation == std.inOrganisation ==
+                                                                                                                                                           True %}  {% elif      True %}  {% elif
+                                                                                                                                                           std.requestActioned   std.pendingRequest ==
+                                                                                                                                                           == True %}  {% elif   True or
+                                                                                                                                                           std.pendingRequest == std.requestActioned
+                                                                                                                                                           True %}  {% elif      == True %} {%
+                                                       [{                                                                            {% if                 std.pendingRevocation translate_"Cancel"_%}
+                                                       {                                {                                            std.hasRequiredScopes == True %}  {% elif   {% elif
+[{{ std.character|character_portrait_url:32 }}]   { std.character.corporation_ticker {                                            %}  {% else %}        std.standing == None  std.pendingRevocation
+{ std.character.character_name }}                      }}] {                            std.character.alliance_name|default_if_none:  {%_translate         and                   == True %}  {% elif
+                                                       { std.character.corporation_name "" }}                                        "Required"_%}         std.pendingRequest == not std.hasStanding
+                                                       }}                                                                             {% endif %}          False %}  {% else %}  %} {% if
+                                                                                                                                                           {% include            std.hasRequiredScopes
+                                                                                                                                                           'standingsrequests/   %} {%_translate
+                                                                                                                                                           partials/             "Apply"_%} {% else %}
+                                                                                                                                                           standing_symbol.html' {% translate "Apply"
+                                                                                                                                                           with                  %}  {% endif %} {%
+                                                                                                                                                           standing=std.standing else %} {%_translate
+                                                                                                                                                           %} {% endif %}        "Revoke"_%} {% endif
+                                                                                                                                                                                 %}
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/request_corporations.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/request_corporations.html`

 * *Files 12% similar despite different names*

```diff
@@ -45,38 +45,38 @@
                     </td>
                     <td>
                         {% if st.pendingRequest == True or st.requestActioned == True %}
                             <a
                                 class="btn btn-warning"
                                 role="button"
                                 href="{% url 'standingsrequests:remove_corp_standing' corporation_id=st.corp.corporation_id %}"
-                                title="Cancel Request">
-                                Cancel
+                                title="{% translate 'Cancel Request' %}">
+                                {% translate "Cancel" %}
                             </a>
                         {% elif st.pendingRevocation == True %}
                             <!-- Revoked, No actions -->
                         {% elif not st.hasStanding %}
                             {% if st.token_count >= st.corp.member_count %}
                                 <a
                                     class="btn btn-primary"
                                     role="button"
                                     href="{% url 'standingsrequests:request_corp_standing' corporation_id=st.corp.corporation_id %}"
-                                    title="Request to get standing for this corporation">
-                                    &nbsp;Apply&nbsp;
+                                    title="{% translate 'Request to get standing for this corporation' %}">
+                                    {% translate "Apply" %}
                                 </a>
                             {% else %}
                                 <i class="fas fa-info-circle fa-lg fa-fw text-info" title="{% translate 'More keys required to request standings' %}"></i>
                             {% endif %}
                         {% else %}
                             <a
                                 class="btn btn-danger"
                                 role="button"
                                 href="{% url 'standingsrequests:remove_corp_standing' corporation_id=st.corp.corporation_id %}"
-                                title="Request to revoke standing for this corporation">
-                                Revoke
+                                title="{% translate 'Request to revoke standing for this corporation' %}">
+                                {% translate "Revoke" %}
                             </a>
                         {% endif %}
                     </td>
                 </tr>
             {% endfor %}
         </tbody>
     </table>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 {% load static %} {% load i18n %} {% load evelinks %}
-{% translate "Corporation" %}                                   {% translate "Alliance" %}             {% translate "Keys/  {% translate          {% translate "Actions" %}
-                                                                                                       Req" %}              "Standing" %}
-                                                                                                                            {% if
-                                                                                                                            st.inOrganisation ==
-                                                                                                                            True %}  {% elif
-                                                                                                                            st.requestActioned ==
-                                                                                                                            True %}  {% elif
-                                                                                                                            st.pendingRequest ==
-                                                                                                                            True %}  {% elif
-                                                                {                                      {{ st.token_count    st.pendingRevocation  {% if st.pendingRequest == True or st.requestActioned == True %} Cancel {%
-[{{ st.corp.corporation_id|corporation_logo_url:32 }}]     { {                                      }}/{                 == True %}  {% elif   elif st.pendingRevocation == True %}  {% elif not st.hasStanding %} {% if
-{ st.corp.corporation_name }}                                   st.corp.alliance_name|default_if_none: {                    st.standing == None   st.token_count >= st.corp.member_count %}  Apply  {% else %}  {% endif %} {%
-                                                                "" }}                                  st.corp.member_count and st.pendingRequest else %} Revoke {% endif %}
-                                                                                                       }}                   == False %}  {% else
-                                                                                                                            %} {% include
-                                                                                                                            'standingsrequests/
-                                                                                                                            partials/
-                                                                                                                            standing_symbol.html'
-                                                                                                                            with
-                                                                                                                            standing=st.standing
-                                                                                                                            %} {% endif %}
+{% translate "Corporation" %}                                   {% translate "Alliance" %}             {% translate "Keys/  {% translate          {% translate
+                                                                                                       Req" %}              "Standing" %}         "Actions" %}
+                                                                                                                            {% if                 {% if
+                                                                                                                            st.inOrganisation ==  st.pendingRequest ==
+                                                                                                                            True %}  {% elif      True or
+                                                                                                                            st.requestActioned == st.requestActioned
+                                                                                                                            True %}  {% elif      == True %} {%
+                                                                                                                            st.pendingRequest ==  translate_"Cancel"
+                                                                                                                            True %}  {% elif      %} {% elif
+                                                                {                                      {{ st.token_count    st.pendingRevocation  st.pendingRevocation
+[{{ st.corp.corporation_id|corporation_logo_url:32 }}]     { {                                      }}/{                 == True %}  {% elif   == True %}  {% elif
+{ st.corp.corporation_name }}                                   st.corp.alliance_name|default_if_none: {                    st.standing == None   not st.hasStanding
+                                                                "" }}                                  st.corp.member_count and st.pendingRequest %} {% if
+                                                                                                       }}                   == False %}  {% else  st.token_count >=
+                                                                                                                            %} {% include         st.corp.member_count
+                                                                                                                            'standingsrequests/   %} {%_translate
+                                                                                                                            partials/             "Apply"_%} {% else
+                                                                                                                            standing_symbol.html' %}  {% endif %} {%
+                                                                                                                            with                  else %} {%_translate
+                                                                                                                            standing=st.standing  "Revoke"_%} {% endif
+                                                                                                                            %} {% endif %}        %}
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/standing_symbol.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/standing_symbol.html`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tab_alliance_standings.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tab_alliance_standings.html`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tab_character_standings.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tab_character_standings.html`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tab_corporation_standings.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tab_corporation_standings.html`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/partials/tbl_effective_requests.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/partials/tbl_effective_requests.html`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/templates/standingsrequests/standings.html` & `aa_standingsrequests-1.3.0/standingsrequests/templates/standingsrequests/standings.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,44 @@
 
 {% block details %}
 
     <h2>{{ operation_mode|capfirst }} {% translate "Standings" %}</h2>
 
     <ul id="myTabs" class="nav nav-tabs" role="tablist">
         <li role="presentation" class="active">
-            <a href="#tab-characters" aria-controls="tab-characters" role="tab" data-toggle="tab">Characters</a>
+            <a href="#tab-characters" aria-controls="tab-characters" role="tab" data-toggle="tab">
+                {% translate "Characters" %}
+            </a>
         </li>
         <li role="presentation">
-            <a href="#tab-corporations" aria-controls="tab-corporations" role="tab" data-toggle="tab">Corporations</a>
+            <a href="#tab-corporations" aria-controls="tab-corporations" role="tab" data-toggle="tab">
+                {% translate "Corporations" %}
+            </a>
         </li>
         <li role="presentation">
-            <a href="#tab-alliances" aria-controls="tab-alliances" role="tab" data-toggle="tab">Alliances</a>
+            <a href="#tab-alliances" aria-controls="tab-alliances" role="tab" data-toggle="tab">
+                {% translate "Alliances" %}
+            </a>
         </li>
     </ul>
 
     <div class="panel panel-default panel-tabs">
         <div class="panel-body">
             <div class="tab-content">
                 {% include "standingsrequests/partials/tab_character_standings.html" %}
                 {% include "standingsrequests/partials/tab_corporation_standings.html" %}
                 {% include "standingsrequests/partials/tab_alliance_standings.html" %}
             </div>
         </div>
     </div>
     <p class="text-muted">
-        Current in-game contacts with standings for <strong>{{ organization.name }}</strong> •
-        This data was last updated {{ lastUpdate|timesince }} ago and is cached
+        {% blocktranslate with organization_name=organization.name last_update=lastUpdate|timesince %}
+            Current in-game contacts with standings for {{ organization_name }} •
+            This data was last updated {{ last_update }} ago and is cached
+        {% endblocktranslate %}
     </p>
     <!-- transfer data to javascript -->
     {{ show_mains|json_script:"show-mains-data" }}
 {% endblock details %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/entity_type_ids.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/entity_type_ids.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/my_test_data.json` & `aa_standingsrequests-1.3.0/standingsrequests/tests/my_test_data.json`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/my_test_data.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/my_test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,14 @@
     for contact_data in get_my_test_data()["alliance_contacts"]:
         contacts.append(_ContactsWrapper.Contact(contact_data, labels, names_info))
 
     return contacts
 
 
 def create_contacts_set(my_set: ContactSet = None, include_assoc=True) -> ContactSet:
-
     if not my_set:
         my_set = ContactSet.objects.create(name="Dummy Set")
 
     # add labels
     ContactSet.objects._add_labels_from_api(my_set, get_test_labels())
 
     # create contacts for ContactSet
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_commands.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_core.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_decorators.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_helpers_evecharacter.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_helpers_evecharacter.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_helpers_evecorporation.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_helpers_evecorporation.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_integration.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     MODELS_PATH + ".SR_REQUIRED_SCOPES",
     {"Member": [TEST_REQUIRED_SCOPE], "Blue": [], "": []},
 )
 @patch(CORE_PATH + ".STANDINGS_API_CHARID", TEST_STANDINGS_API_CHARID)
 @patch(MANAGERS_PATH + ".SR_NOTIFICATIONS_ENABLED", True)
 @patch(CORE_PATH + ".STR_ALLIANCE_IDS", [TEST_STANDINGS_ALLIANCE_ID])
 class TestMainUseCases(WebTest):
-
     csrf_checks = False
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         create_standings_char()
         create_eve_objects()
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_managers.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_models.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/test_tasks.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/utils.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_create_requests.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_create_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,22 +312,23 @@
             user=self.user,
         )
         # when
         result = self._view_request_pilot_standing(alt_character.character_id)
         # then
         self.assertFalse(result)
 
-    def test_should_not_create_new_request_if_character_is_missing_scopes(self):
-        # given
-        alt_character = create_entity(EveCharacter, 1009)
-        add_character_to_user(self.user, alt_character)
-        # when
-        result = self._view_request_pilot_standing(alt_character.character_id)
-        # then
-        self.assertFalse(result)
+    # FIXME
+    # def test_should_not_create_new_request_if_character_is_missing_scopes(self):
+    #     # given
+    #     alt_character = create_entity(EveCharacter, 1009)
+    #     add_character_to_user(self.user, alt_character)
+    #     # when
+    #     result = self._view_request_pilot_standing(alt_character.character_id)
+    #     # then
+    #     self.assertFalse(result)
 
     def test_should_not_create_new_request_if_character_is_not_owned_by_anyone(self):
         # given
         random_character = create_entity(EveCharacter, 1007)
         # when
         result = self._view_request_pilot_standing(random_character.character_id)
         # then
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_effective_requests.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_effective_requests.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_manage_requests.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_manage_requests.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/tests/views/test_standings.py` & `aa_standingsrequests-1.3.0/standingsrequests/tests/views/test_standings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime as dt
+from unittest.mock import patch
 
 from django.test import RequestFactory
 from django.urls import reverse
 from django.utils.timezone import now
 
 from allianceauth.eveonline.models import EveAllianceInfo, EveCharacter
 from allianceauth.tests.auth_utils import AuthUtils
@@ -16,14 +17,41 @@
     create_eve_objects,
     load_corporation_details,
     load_eve_entities,
 )
 from ..utils import NoSocketsTestCasePlus, json_response_to_dict_2
 
 TEST_SCOPE = "publicData"
+MODULE_PATH = "standingsrequests.views.standings"
+
+
+@patch("standingsrequests.core.STANDINGS_API_CHARID", 1001)
+class TestStandingsView(NoSocketsTestCasePlus):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        cls.factory = RequestFactory()
+        load_eve_entities()
+        create_eve_objects()
+        cls.contact_set = create_contacts_set()
+        CharacterAffiliation.objects.update_evecharacter_relations()
+
+        cls.user = AuthUtils.create_member("John Doe")
+        cls.user = AuthUtils.add_permission_to_user_by_name(
+            "standingsrequests.request_standings", cls.user
+        )
+
+    def test_can_open_standings_page(self):
+        # given
+        request = self.factory.get(reverse("standingsrequests:standings"))
+        request.user = self.user
+        # when
+        response = standings.standings(request)
+        # then
+        self.assertEqual(response.status_code, 200)
 
 
 class TestCharacterStandingsData(NoSocketsTestCasePlus):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.factory = RequestFactory()
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/urls.py` & `aa_standingsrequests-1.3.0/standingsrequests/urls.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/views/_common.py` & `aa_standingsrequests-1.3.0/standingsrequests/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/views/admin.py` & `aa_standingsrequests-1.3.0/standingsrequests/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/views/create_requests.py` & `aa_standingsrequests-1.3.0/standingsrequests/views/create_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,28 +247,30 @@
         character_id=character_id,
     )
     error = StandingRequest.objects.create_character_request(request.user, character)
     if error is not CreateCharacterRequestError.NO_ERROR:
         if error is CreateCharacterRequestError.CHARACTER_IS_MISSING_SCOPES:
             messages.error(
                 request,
-                "You character %s is missing scopes."
+                _("You character %s is missing scopes.")
                 % EveEntity.objects.resolve_name(character_id),
             )
         elif error is CreateCharacterRequestError.USER_IS_NOT_OWNER:
             messages.error(
                 request,
-                "You are not the owner of character %s."
+                _("You are not the owner of character %s.")
                 % EveEntity.objects.resolve_name(character_id),
             )
         else:
             messages.error(
                 request,
-                "An unexpected error occurred when trying to process "
-                "your standing request for %s. Please try again."
+                _(
+                    "An unexpected error occurred when trying to process "
+                    "your standing request for %s. Please try again."
+                )
                 % EveEntity.objects.resolve_name(character_id),
             )
     else:
         update_associations_api.delay()
     return redirect("standingsrequests:create_requests")
 
 
@@ -284,16 +286,18 @@
         character_id,
     )
     req = get_object_or_404(StandingRequest, user=request.user, contact_id=character_id)
     success = req.remove()
     if not success:
         messages.warning(
             request,
-            "An unexpected error occurred when trying to process "
-            "your request to revoke standing for %s. Please try again."
+            _(
+                "An unexpected error occurred when trying to process "
+                "your request to revoke standing for %s. Please try again."
+            )
             % EveEntity.objects.resolve_name(character_id),
         )
     return redirect("standingsrequests:create_requests")
 
 
 @login_required
 @permission_required(StandingRequest.REQUEST_PERMISSION_NAME)
@@ -306,16 +310,18 @@
         "Standings request from user %s for corpID %d", request.user, corporation_id
     )
     if not StandingRequest.objects.create_corporation_request(
         request.user, corporation_id
     ):
         messages.warning(
             request,
-            "An unexpected error occurred when trying to process "
-            "your standing request for %s. Please try again."
+            _(
+                "An unexpected error occurred when trying to process "
+                "your standing request for %s. Please try again."
+            )
             % EveEntity.objects.resolve_name(corporation_id),
         )
     else:
         update_associations_api.delay()
     return redirect("standingsrequests:create_requests")
 
 
@@ -333,16 +339,18 @@
     except StandingRequest.DoesNotExist:
         success = False
     else:
         success = req.remove()
     if not success:
         messages.warning(
             request,
-            "An unexpected error occurred when trying to process "
-            "your request to revoke standing for %s. Please try again."
+            _(
+                "An unexpected error occurred when trying to process "
+                "your request to revoke standing for %s. Please try again."
+            )
             % EveEntity.objects.resolve_name(corporation_id),
         )
     return redirect("standingsrequests:create_requests")
 
 
 @login_required
 @permission_required("standingsrequests.affect_standings")
@@ -351,33 +359,36 @@
     source_entity = BaseConfig.standings_source_entity()
     char_name = EveEntity.objects.resolve_name(BaseConfig.owner_character_id)
     if not source_entity:
         messages.error(
             request,
             format_html(
                 _(
-                    "The configured character <strong>%s</strong> does not belong "
+                    "The configured character %s does not belong "
                     "to an alliance and can therefore not be used "
                     "to setup alliance standings. "
                     "Please configure a character that has an alliance."
                 )
                 % char_name,
             ),
         )
     elif token.character_id == BaseConfig.owner_character_id:
         update_all.delay(user_pk=request.user.pk)
         messages.success(
             request,
             format_html(
                 _(
-                    "Token for character <strong>%s</strong> has been setup "
+                    "Token for character %(user_character)s has been setup "
                     "successfully and the app has started pulling standings "
-                    "from <strong>%s</strong>."
+                    "from %(standings_character)s."
                 )
-                % (char_name, source_entity.name),
+                % {
+                    "user_character": char_name,
+                    "standings_character": source_entity.name,
+                },
             ),
         )
     else:
         messages.error(
             request,
             _(
                 "Failed to setup token for configured character "
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/views/effective_requests.py` & `aa_standingsrequests-1.3.0/standingsrequests/views/effective_requests.py`

 * *Files identical despite different names*

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/views/manage_requests.py` & `aa_standingsrequests-1.3.0/standingsrequests/views/manage_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,19 +83,22 @@
         standing_request = get_object_or_404(StandingRequest, contact_id=contact_id)
         RequestLogEntry.objects.create_from_standing_request(
             standing_request, RequestLogEntry.Action.REJECTED, request.user
         )
         standing_request.delete()
         if SR_NOTIFICATIONS_ENABLED:
             entity_name = EveEntity.objects.resolve_name(contact_id)
-            title = _("Standing request for %s rejected" % entity_name)
+            title = _("Standing request for %s rejected") % entity_name
             message = _(
-                "Your standing request for '%s' has been rejected by %s."
-                % (entity_name, request.user)
-            )
+                "Your standing request for %(character)s has been rejected by %(user)s."
+            ) % {
+                "character": entity_name,
+                "user": request.user,
+            }
+
             notify(user=standing_request.user, title=title, message=message)
         return HttpResponse("")
     return HttpResponseNotFound()
 
 
 @login_required
 @permission_required("standingsrequests.affect_standings")
@@ -126,15 +129,16 @@
         standing_revocation = standing_revocations_qs.first()
         RequestLogEntry.objects.create_from_standing_request(
             standing_revocation, RequestLogEntry.Action.REJECTED, request.user
         )
         standing_revocations_qs.delete()
         if SR_NOTIFICATIONS_ENABLED and standing_revocation.user:
             entity_name = EveEntity.objects.resolve_name(contact_id)
-            title = _("Standing revocation for %s rejected" % entity_name)
+            title = _("Standing revocation for %s rejected") % entity_name
             message = _(
-                "Your standing revocation for '%s' "
-                "has been rejected by %s." % (entity_name, request.user)
-            )
+                "Your standing revocation for %(character)s "
+                "has been rejected by %(user)s."
+            ) % {"character": entity_name, "user": request.user}
+
             notify(user=standing_revocation.user, title=title, message=message)
         return HttpResponse("")
     return HttpResponseNotFound()
```

### Comparing `aa-standingsrequests-1.2.2/standingsrequests/views/standings.py` & `aa_standingsrequests-1.3.0/standingsrequests/views/standings.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,16 @@
 @login_required
 @permission_required("standingsrequests.request_standings")
 def standings(request):
     try:
         contact_set = ContactSet.objects.latest()
     except ContactSet.DoesNotExist:
         contact_set = None
-    finally:
-        organization = BaseConfig.standings_source_entity()
-        last_update = contact_set.date if contact_set else None
+    organization = BaseConfig.standings_source_entity()
+    last_update = contact_set.date if contact_set else None
     context = {
         "lastUpdate": last_update,
         "organization": organization,
         "show_mains": request.user.has_perm("standingsrequests.view"),
     }
     return render(
         request,
```

