# Comparing `tmp/netbox-secrets-1.7.6.tar.gz` & `tmp/netbox-secrets-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-secrets-1.7.6.tar", last modified: Wed Apr 12 16:45:23 2023, max compression
+gzip compressed data, was "netbox-secrets-1.8.0.tar", last modified: Sun May  7 20:43:16 2023, max compression
```

## Comparing `netbox-secrets-1.7.6.tar` & `netbox-secrets-1.8.0.tar`

### file list

```diff
@@ -1,82 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.437818 netbox-secrets-1.7.6/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/forms/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/graphql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/hashers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0002_populate_userkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0003_populate_secretroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0004_populate_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/models/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14959 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/querysets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.429818 netbox-secrets-1.7.6/netbox_secrets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js
--rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.433818 netbox-secrets-1.7.6/netbox_secrets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.441818 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/activate_keys.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret.html
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secretrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey.html
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/netbox_secrets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/netbox_secrets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/hashers.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/netbox_secrets/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:45:23.437818 netbox-secrets-1.7.6/netbox_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 16:45:23.000000 netbox-secrets-1.7.6/netbox_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:45:23.445818 netbox-secrets-1.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-12 16:45:12.000000 netbox-secrets-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.388205 netbox-secrets-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-07 20:43:16.388205 netbox-secrets-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.380205 netbox-secrets-1.8.0/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.384204 netbox-secrets-1.8.0/netbox_secrets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.384204 netbox-secrets-1.8.0/netbox_secrets/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/forms/bulk_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/forms/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/forms/model_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.384204 netbox-secrets-1.8.0/netbox_secrets/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/graphql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/hashers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.384204 netbox-secrets-1.8.0/netbox_secrets/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/0002_populate_userkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/0003_populate_secretroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/0004_populate_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.384204 netbox-secrets-1.8.0/netbox_secrets/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/querysets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.380205 netbox-secrets-1.8.0/netbox_secrets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.384204 netbox-secrets-1.8.0/netbox_secrets/static/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/static/netbox_secrets/secrets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/static/netbox_secrets/secrets.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.380205 netbox-secrets-1.8.0/netbox_secrets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.384204 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/activate_keys.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.388205 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/secret.html
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/secret_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/secretrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/userkey.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/userkey_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.388205 netbox-secrets-1.8.0/netbox_secrets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.388205 netbox-secrets-1.8.0/netbox_secrets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/utils/hashers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/netbox_secrets/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:43:16.380205 netbox-secrets-1.8.0/netbox_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-07 20:43:16.000000 netbox-secrets-1.8.0/netbox_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-07 20:43:16.000000 netbox-secrets-1.8.0/netbox_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:43:16.000000 netbox-secrets-1.8.0/netbox_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:43:16.000000 netbox-secrets-1.8.0/netbox_secrets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 20:43:16.000000 netbox-secrets-1.8.0/netbox_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 20:43:16.000000 netbox-secrets-1.8.0/netbox_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:43:16.388205 netbox-secrets-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-07 20:43:04.000000 netbox-secrets-1.8.0/setup.py
```

### Comparing `netbox-secrets-1.7.6/LICENSE.md` & `netbox-secrets-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/README.md` & `netbox-secrets-1.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 # Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 | 3.3.x          | 1.4.x, 1.5.x   |
 | 3.4.x          | 1.6.x, 1.7.x   |
+| 3.5.x          | 1.8.x          |
 
 # Installation
 
 * Install NetBox as per NetBox documentation
 * Add to local_requirements.txt:
   * `netbox-secrets`
 * Install requirements: `./venv/bin/pip install -r local_requirements.txt`
@@ -41,15 +42,15 @@
   - __Type__: `List`
   - __Description__: List of apps to enable
   - __Default__: `['dcim.device', 'virtualization.virtualmachine']`
 - `display_default`
   - __Type__: `String`
   - __Description__: Where to display the secret on the detail page of the defined apps
   - __Default__: `left_page`
-  - __Options__: `left_page`, `right_page`, `full_width_page`
+  - __Options__: `left_page`, `right_page`, `full_width_page`, `tab_view`
 - `display_setting`
   - __Type__: `Dict`
   - __Description__: Set display setting for concrete model
   - __Default__: `{}`
   - __Options__: `{'app.model': 'display_default'}`
   - __Example__: `{'dcim.device': 'full_width_page', 'virtualization.virtualmachine': 'right_page'}`
 - `enable_contacts`
@@ -58,14 +59,28 @@
   - __Default__: `False`
 - `public_key_size`
   - __Type__: `Integer`
   - __Description__: Size of the public key
   - __Default__: `2048`
   - __Options__: `2048`, `4096`, `8192`
 
+## Extra Configuration
+
+The following options are inherited from NetBox to configure the cookies:
+
+- `SESSION_COOKIE_SECURE`
+  - __Type__: `Boolean`
+  - __Description__: [Session Cookie Secure](https://docs.netbox.dev/en/stable/configuration/security/#session_cookie_secure)
+- `LOGIN_TIMEOUT`
+  - __Type__: `Integer`
+  - __Description__: [Login Timeout](https://docs.netbox.dev/en/stable/configuration/security/#login_timeout)
+
+__Note: These options should be set in the NetBox configuration file.__
+
+
 ## Screenshots
 
 ### User key (Without Session)
 
 ![user-key.png](./assets/user-key.png)
 
 ### User key (With Session)
@@ -84,23 +99,25 @@
 
 ![role.png](./assets/role.png)
 
 ## FAQ
 
 1. How can I migrate the data from `netbox-secretstore`?
 
-_Note: This is a one-way migration. You can't migrate back to `netbox-secretstore`. Ensure you do not have any data for netbox-secrets already in the database_
+_Note: This is a one-way migration. You can't migrate back to `netbox-secretstore`. Ensure you do not have any data including tables for netbox-secrets already in the database_
 
-These instructions assume that you are running Netbox v3.4.x and the plugin version 1.6.x. Install a new version
+These instructions assume that you are running Netbox v3.4.x and the plugin version 1.7.x. Install a new version
 of `netbox_secretstore` as:
 
 ```shell
 pip install git+https://github.com/Onemind-Services-LLC/netbox-secretstore@migration/nb34
 ```
 
+_Note: You should have netbox-secretstore v1.4.4 installed now._
+
 Make sure to add both plugins to the `configuration.py` before the migration.
 
 Run the migration:
 
 ```shell
 python manage.py migrate
 ```
@@ -109,8 +126,8 @@
 
 ```shell
 python manage.py sqlsequencereset netbox_secrets
 ```
 
 Run the output of the previous command in the database.
 
-You can now remove `netbox-secretstore` from the application.
+You can now remove `netbox-secretstore` from the application. You may have clean up your database of the old tables manually.
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/admin.py` & `netbox-secrets-1.8.0/netbox_secrets/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/api/serializers.py` & `netbox-secrets-1.8.0/netbox_secrets/api/serializers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,121 @@
 from django.contrib.contenttypes.models import ContentType
-from drf_yasg.utils import swagger_serializer_method
+from drf_spectacular.utils import extend_schema_field
 from netbox.api.fields import ContentTypeField
 from netbox.api.serializers import NetBoxModelSerializer
 from netbox.constants import NESTED_SERIALIZER_PREFIX
 from rest_framework import serializers
 from utilities.api import get_serializer_for_model
 
 from ..constants import SECRET_ASSIGNABLE_MODELS
-from ..models import Secret, SecretRole, UserKey
+from ..models import *
 from .nested_serializers import *
 
+__all__ = [
+    'SecretRoleSerializer',
+    'SecretSerializer',
+    'SessionKeySerializer',
+    'SessionKeyCreateSerializer',
+    'UserKeySerializer',
+    'RSAKeyPairSerializer',
+]
+
+
 #
 # User Key
 #
 
 
 class UserKeySerializer(serializers.ModelSerializer):
+    url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_secrets-api:userkey-detail')
     public_key = serializers.CharField()
     private_key = serializers.CharField(
         write_only=True,
     )
 
     display = serializers.SerializerMethodField(read_only=True)
 
+    is_active = serializers.BooleanField(read_only=True)
+
+    is_filled = serializers.BooleanField(read_only=True)
+
     class Meta:
         model = UserKey
         fields = [
             'pk',
             'id',
+            'url',
             'display',
             'public_key',
             'private_key',
             'created',
             'last_updated',
             'is_active',
             'is_filled',
         ]
 
+    @extend_schema_field(serializers.CharField())
+    def get_display(self, obj):
+        return str(obj)
+
+
+#
+# Session Keys
+#
+
+
+class SessionKeySerializer(serializers.ModelSerializer):
+    url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_secrets-api:sessionkey-detail')
+
+    display = serializers.SerializerMethodField(read_only=True)
+
+    userkey = NestedUserKeySerializer()
+
+    session_key = serializers.SerializerMethodField(
+        read_only=True,
+    )
+
+    class Meta:
+        model = SessionKey
+        fields = [
+            'pk',
+            'id',
+            'url',
+            'display',
+            'userkey',
+            'session_key',
+            'created',
+        ]
+
+    @extend_schema_field(serializers.CharField())
     def get_display(self, obj):
         return str(obj)
 
+    @extend_schema_field(serializers.CharField())
+    def get_session_key(self, obj):
+        return self.context.get('session_key', None)
+
+
+class SessionKeyCreateSerializer(serializers.ModelSerializer):
+    private_key = serializers.CharField(
+        write_only=True,
+    )
+
+    preserve_key = serializers.BooleanField(
+        default=False,
+        write_only=True,
+    )
+
+    class Meta:
+        model = SessionKey
+        fields = [
+            'private_key',
+            'preserve_key',
+        ]
+
 
 #
 # Secret Roles
 #
 
 
 class SecretRoleSerializer(NetBoxModelSerializer):
@@ -55,14 +127,15 @@
         fields = [
             'id',
             'url',
             'display',
             'name',
             'slug',
             'description',
+            'comments',
             'custom_fields',
             'created',
             'last_updated',
             'secret_count',
         ]
 
 
@@ -87,22 +160,24 @@
             'assigned_object_type',
             'assigned_object_id',
             'assigned_object',
             'role',
             'name',
             'plaintext',
             'hash',
+            'description',
+            'comments',
             'tags',
             'custom_fields',
             'created',
             'last_updated',
         ]
         validators = []
 
-    @swagger_serializer_method(serializer_or_field=serializers.DictField)
+    @extend_schema_field(serializers.DictField())
     def get_assigned_object(self, obj):
         serializer = get_serializer_for_model(obj.assigned_object, prefix=NESTED_SERIALIZER_PREFIX)
         context = {'request': self.context['request']}
         return serializer(obj.assigned_object, context=context).data
 
     def validate(self, data):
         # Encrypt plaintext data using the master key provided from the view context
@@ -111,7 +186,12 @@
             s.encrypt(self.context['master_key'])
             data['ciphertext'] = s.ciphertext
             data['hash'] = s.hash
 
         super().validate(data)
 
         return data
+
+
+class RSAKeyPairSerializer(serializers.Serializer):
+    public_key = serializers.CharField()
+    private_key = serializers.CharField()
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/api/urls.py` & `netbox-secrets-1.8.0/netbox_secrets/api/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from netbox.api.routers import NetBoxRouter
 
 from . import views
 
 router = NetBoxRouter()
 router.APIRootView = views.SecretsRootView
 
-# User Key
 router.register('user-keys', views.UserKeyViewSet)
-
-# Secrets
+router.register('session-keys', views.SessionKeyViewSet)
 router.register('secret-roles', views.SecretRoleViewSet)
 router.register('secrets', views.SecretViewSet)
 
 # Miscellaneous
 router.register('get-session-key', views.GetSessionKeyViewSet, basename='get-session-key')
 router.register('generate-rsa-key-pair', views.GenerateRSAKeyPairViewSet, basename='generate-rsa-key-pair')
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/api/views.py` & `netbox-secrets-1.8.0/netbox_secrets/api/views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import base64
 
 from Crypto.PublicKey import RSA
 from django.conf import settings
 from django.http import HttpResponseBadRequest
-from drf_yasg import openapi
-from drf_yasg.utils import swagger_auto_schema
-from netbox.api.viewsets import NetBoxModelViewSet
+from drf_spectacular import utils as drf_utils
+from netbox.api.viewsets import BaseViewSet, NetBoxModelViewSet, mixins
+from rest_framework import mixins as drf_mixins
 from rest_framework.exceptions import ValidationError
+from rest_framework.parsers import FormParser, JSONParser, MultiPartParser
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.routers import APIRootView
 from rest_framework.viewsets import ModelViewSet, ViewSet
 from utilities.utils import count_related
 
-from netbox_secrets import filtersets
-from netbox_secrets.exceptions import InvalidKey
-from netbox_secrets.models import Secret, SecretRole, SessionKey, UserKey
-
+from .. import constants, exceptions, filtersets, models
 from . import serializers
 
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_secrets', {})
 public_key_size = plugin_settings.get('public_key_size')
 
 ERR_USERKEY_MISSING = "No UserKey found for the current user."
 ERR_USERKEY_INACTIVE = "UserKey has not been activated for decryption."
@@ -37,39 +35,41 @@
         return 'Secrets'
 
 
 #
 # User Key
 #
 class UserKeyViewSet(ModelViewSet):
-    queryset = UserKey.objects.all()
+    queryset = models.UserKey.objects.all()
     serializer_class = serializers.UserKeySerializer
 
     def get_queryset(self):
-        return UserKey.objects.filter(user=self.request.user)
+        return models.UserKey.objects.filter(user=self.request.user)
 
 
 #
 # Secret Roles
 #
 
 
 class SecretRoleViewSet(NetBoxModelViewSet):
-    queryset = SecretRole.objects.annotate(secret_count=count_related(Secret, 'role')).prefetch_related('tags')
+    queryset = models.SecretRole.objects.annotate(secret_count=count_related(models.Secret, 'role')).prefetch_related(
+        'tags',
+    )
     serializer_class = serializers.SecretRoleSerializer
     filterset_class = filtersets.SecretRoleFilterSet
 
 
 #
 # Secrets
 #
 
 
 class SecretViewSet(NetBoxModelViewSet):
-    queryset = Secret.objects.prefetch_related('role', 'tags')
+    queryset = models.Secret.objects.prefetch_related('role', 'tags')
     serializer_class = serializers.SecretSerializer
     filterset_class = filtersets.SecretFilterSet
 
     master_key = None
 
     def get_serializer_context(self):
 
@@ -83,31 +83,31 @@
 
         super().initial(request, *args, **kwargs)
 
         if request.user.is_authenticated:
 
             # Read session key from HTTP cookie or header if it has been provided. The session key must be provided in
             # order to encrypt/decrypt secrets.
-            if 'session_key' in request.COOKIES:
-                session_key = base64.b64decode(request.COOKIES['session_key'])
+            if constants.SESSION_COOKIE_NAME in request.COOKIES:
+                session_key = base64.b64decode(request.COOKIES[constants.SESSION_COOKIE_NAME])
             elif 'HTTP_X_SESSION_KEY' in request.META:
                 session_key = base64.b64decode(request.META['HTTP_X_SESSION_KEY'])
             else:
                 session_key = None
 
             # We can't encrypt secret plaintext without a session key.
             if self.action in ['create', 'update'] and session_key is None:
                 raise ValidationError("A session key must be provided when creating or updating secrets.")
 
             # Attempt to retrieve the master key for encryption/decryption if a session key has been provided.
             if session_key is not None:
                 try:
-                    sk = SessionKey.objects.get(userkey__user=request.user)
+                    sk = models.SessionKey.objects.get(userkey__user=request.user)
                     self.master_key = sk.get_master_key(session_key)
-                except (SessionKey.DoesNotExist, InvalidKey):
+                except (models.SessionKey.DoesNotExist, exceptions.InvalidKey):
                     raise ValidationError("Invalid session key.")
 
     def retrieve(self, request, *args, **kwargs):
 
         secret = self.get_object()
 
         # Attempt to decrypt the secret if the master key is known
@@ -136,136 +136,135 @@
 
             return self.get_paginated_response(serializer.data)
 
         serializer = self.get_serializer(queryset, many=True)
         return Response(serializer.data)
 
 
-class GetSessionKeyViewSet(ViewSet):
-    """
-    Retrieve a temporary session key to use for encrypting and decrypting secrets via the API. The user's private RSA
-    key is POSTed with the name `private_key`.
-
-    This endpoint accepts one optional parameter: `preserve_key`. If True and a session key exists, the existing session
-    key will be returned instead of a new one.
-    """
+#
+# Session Keys
+#
+class SessionKeyViewSet(
+    drf_mixins.ListModelMixin,
+    drf_mixins.RetrieveModelMixin,
+    drf_mixins.DestroyModelMixin,
+    mixins.BriefModeMixin,
+    mixins.BulkDestroyModelMixin,
+    BaseViewSet,
+):
+    queryset = models.SessionKey.objects.prefetch_related('userkey__user')
+    serializer_class = serializers.SessionKeySerializer
 
-    permission_classes = [IsAuthenticated]
+    def get_queryset(self):
+        return models.SessionKey.objects.filter(userkey__user=self.request.user)
 
-    @swagger_auto_schema(
-        request_body=openapi.Schema(
-            type=openapi.TYPE_OBJECT,
-            required=['private_key'],
-            properties={
-                'private_key': openapi.Schema(
-                    type=openapi.TYPE_STRING,
-                    description='Private RSA key used to decrypt the session key',
-                ),
-                'preserve_key': openapi.Schema(
-                    type=openapi.TYPE_BOOLEAN,
-                    description='Preserve existing session key',
-                    default=False,
-                ),
-            },
-        ),
+    @drf_utils.extend_schema(
+        request=serializers.SessionKeyCreateSerializer,
+        responses={
+            201: drf_utils.OpenApiResponse(
+                description="Session key created successfully.",
+                response=serializers.SessionKeySerializer,
+            ),
+            400: drf_utils.OpenApiResponse(
+                description="Session key creation failed.",
+                response={
+                    'type': 'string',
+                },
+                examples=[
+                    drf_utils.OpenApiExample(name=ERR_PRIVKEY_MISSING, value=ERR_PRIVKEY_MISSING),
+                    drf_utils.OpenApiExample(name=ERR_USERKEY_MISSING, value=ERR_USERKEY_MISSING),
+                    drf_utils.OpenApiExample(name=ERR_USERKEY_INACTIVE, value=ERR_USERKEY_INACTIVE),
+                    drf_utils.OpenApiExample(name=ERR_PRIVKEY_INVALID, value=ERR_PRIVKEY_INVALID),
+                ],
+            ),
+        },
     )
     def create(self, request):
+        """
+        Creates a new session key for the current user.
+        """
 
-        # Read private key
         private_key = request.data.get('private_key', None)
+        preserve_key = str(request.data.get('preserve_key', False)).lower() in ['true', 'yes', '1']
+
         if private_key is None:
             return HttpResponseBadRequest(ERR_PRIVKEY_MISSING)
 
         # Validate user key
         try:
-            user_key = UserKey.objects.get(user=request.user)
-        except UserKey.DoesNotExist:
+            user_key = models.UserKey.objects.get(user=request.user)
+        except models.UserKey.DoesNotExist:
             return HttpResponseBadRequest(ERR_USERKEY_MISSING)
         if not user_key.is_active():
             return HttpResponseBadRequest(ERR_USERKEY_INACTIVE)
 
         # Validate private key
         master_key = user_key.get_master_key(private_key)
         if master_key is None:
             return HttpResponseBadRequest(ERR_PRIVKEY_INVALID)
 
-        try:
-            current_session_key = SessionKey.objects.get(userkey__user_id=request.user.pk)
-        except SessionKey.DoesNotExist:
-            current_session_key = None
+        current_session_key = self.queryset.first()
 
-        if current_session_key and request.data.get('preserve_key', False):
+        if current_session_key and preserve_key:
 
             # Retrieve the existing session key
             key = current_session_key.get_session_key(master_key)
+            self.queryset = current_session_key
 
         else:
 
             # Create a new SessionKey
-            SessionKey.objects.filter(userkey__user=request.user).delete()
-            sk = SessionKey(userkey=user_key)
+            self.queryset.delete()
+            sk = models.SessionKey(userkey=user_key)
             sk.save(master_key=master_key)
             key = sk.key
+            self.queryset = sk
 
         # Encode the key using base64. (b64decode() returns a bytestring under Python 3.)
         encoded_key = base64.b64encode(key).decode()
 
         # Craft the response
         response = Response(
-            {
-                'session_key': encoded_key,
-            },
+            self.serializer_class(
+                self.queryset,
+                context={'request': request, 'session_key': encoded_key},
+            ).data,
+            status=200 if preserve_key else 201,
         )
 
         # If token authentication is not in use, assign the session key as a cookie
         if request.auth is None:
-            response.set_cookie('session_key', value=encoded_key)
+            response.set_cookie(
+                constants.SESSION_COOKIE_NAME,
+                value=encoded_key,
+                secure=settings.SESSION_COOKIE_SECURE,
+                samesite='Strict',
+                max_age=settings.LOGIN_TIMEOUT,
+            )
 
         return response
 
 
 class GenerateRSAKeyPairViewSet(ViewSet):
     """
     This endpoint can be used to generate a new RSA key pair. The keys are returned in PEM format.
 
         {
             "public_key": "<public key>",
             "private_key": "<private key>"
         }
     """
 
+    serializer_class = serializers.RSAKeyPairSerializer
     permission_classes = [IsAuthenticated]
 
-    @swagger_auto_schema(
-        manual_parameters=[
-            openapi.Parameter(
-                name='key_size',
-                in_=openapi.IN_QUERY,
-                type=openapi.TYPE_INTEGER,
-                description='Number of bits in the key',
-                default=public_key_size,
-            ),
-        ],
-        responses={
-            200: openapi.Schema(
-                type=openapi.TYPE_OBJECT,
-                required=['public_key', 'private_key'],
-                properties={
-                    'public_key': openapi.Schema(
-                        type=openapi.TYPE_STRING,
-                        description='Public RSA key',
-                    ),
-                    'private_key': openapi.Schema(
-                        type=openapi.TYPE_STRING,
-                        description='Private RSA key',
-                    ),
-                },
-            ),
-        },
-    )
+    def get_queryset(self):
+        # This is only used to generate the schema
+        return models.UserKey.objects.filter(user=self.request.user)
+
     def list(self, request):
 
         # Determine what size key to generate
         try:
             key_size = request.GET.get('key_size', public_key_size)
             key_size = int(key_size)
         except ValueError:
@@ -281,7 +280,75 @@
 
         return Response(
             {
                 'private_key': private_key,
                 'public_key': public_key,
             },
         )
+
+
+class GetSessionKeyViewSet(ViewSet):
+    """
+    Retrieve a temporary session key to use for encrypting and decrypting secrets via the API. The user's private RSA
+    key is POSTed with the name `private_key`.
+    This endpoint accepts one optional parameter: `preserve_key`. If True and a session key exists, the existing session
+    key will be returned instead of a new one.
+
+    Deprecation notice: This endpoint is deprecated and will be removed in a future release. Use the `SessionKeyViewSet`.
+    """
+
+    permission_classes = [IsAuthenticated]
+    parser_classes = [JSONParser, FormParser, MultiPartParser]
+
+    def create(self, request):
+
+        # Read private key
+        private_key = request.data.get('private_key', None)
+        if private_key is None:
+            return HttpResponseBadRequest(ERR_PRIVKEY_MISSING)
+
+        # Validate user key
+        try:
+            user_key = models.UserKey.objects.get(user=request.user)
+        except models.UserKey.DoesNotExist:
+            return HttpResponseBadRequest(ERR_USERKEY_MISSING)
+        if not user_key.is_active():
+            return HttpResponseBadRequest(ERR_USERKEY_INACTIVE)
+
+        # Validate private key
+        master_key = user_key.get_master_key(private_key)
+        if master_key is None:
+            return HttpResponseBadRequest(ERR_PRIVKEY_INVALID)
+
+        try:
+            current_session_key = models.SessionKey.objects.get(userkey__user_id=request.user.pk)
+        except models.SessionKey.DoesNotExist:
+            current_session_key = None
+
+        if current_session_key and request.data.get('preserve_key', False):
+
+            # Retrieve the existing session key
+            key = current_session_key.get_session_key(master_key)
+
+        else:
+
+            # Create a new SessionKey
+            models.SessionKey.objects.filter(userkey__user=request.user).delete()
+            sk = models.SessionKey(userkey=user_key)
+            sk.save(master_key=master_key)
+            key = sk.key
+
+        # Encode the key using base64. (b64decode() returns a bytestring under Python 3.)
+        encoded_key = base64.b64encode(key).decode()
+
+        # Craft the response
+        response = Response(
+            {
+                'session_key': encoded_key,
+            },
+        )
+
+        # If token authentication is not in use, assign the session key as a cookie
+        if request.auth is None:
+            response.set_cookie('session_key', value=encoded_key)
+
+        return response
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/filtersets.py` & `netbox-secrets-1.8.0/netbox_secrets/filtersets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import django_filters
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q
 from django.utils.translation import gettext as _
 from netbox.filtersets import NetBoxModelFilterSet
 from tenancy.models import Contact
+from utilities.filters import MultiValueCharFilter
 
 from .constants import SECRET_ASSIGNABLE_MODELS
 from .models import Secret, SecretRole
 
 __all__ = [
     'SecretFilterSet',
     'SecretRoleFilterSet',
@@ -22,35 +23,36 @@
         method='search',
         label='Search',
     )
     name = django_filters.ModelMultipleChoiceFilter(queryset=SecretRole.objects.all(), field_name='name')
 
     class Meta:
         model = SecretRole
-        fields = ['id', 'name', 'slug']
+        fields = ['id', 'name', 'slug', 'description', 'comments']
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
-        return queryset.filter(Q(name__icontains=value) | Q(slug__icontains=value))
+        return queryset.filter(
+            Q(name__icontains=value)
+            | Q(slug__icontains=value)
+            | Q(description__icontains=value)
+            | Q(comments__icontains=value),
+        )
 
 
 if plugin_settings.get('enable_contacts', False):
 
     class SecretFilterSet(NetBoxModelFilterSet):
         q = django_filters.CharFilter(
             method='search',
             label='Search',
         )
 
-        name = django_filters.ModelMultipleChoiceFilter(
-            queryset=Secret.objects.all(),
-            field_name='name',
-            label='Name',
-        )
+        name = MultiValueCharFilter(lookup_expr='iexact')
 
         role_id = django_filters.ModelMultipleChoiceFilter(
             queryset=SecretRole.objects.all(),
             label='Role (ID)',
         )
         role = django_filters.ModelMultipleChoiceFilter(
             field_name='role__slug',
@@ -69,34 +71,46 @@
             field_name='contacts__contact',
             queryset=Contact.objects.all(),
             label=_('Contact'),
         )
 
         class Meta:
             model = Secret
-            fields = ['id', 'assigned_object_type_id', 'assigned_object_id', 'role_id', 'role', 'name', 'contact']
+            fields = [
+                'id',
+                'assigned_object_type_id',
+                'assigned_object_id',
+                'role_id',
+                'role',
+                'name',
+                'contact',
+                'description',
+                'comments',
+                '_object_repr',
+            ]
 
         def search(self, queryset, name, value):
             if not value.strip():
                 return queryset
-            return queryset.filter(Q(name__icontains=value))
+            return queryset.filter(
+                Q(name__icontains=value)
+                | Q(_object_repr__icontains=value)
+                | Q(description__icontains=value)
+                | Q(comments__icontains=value),
+            )
 
 else:
 
     class SecretFilterSet(NetBoxModelFilterSet):
         q = django_filters.CharFilter(
             method='search',
             label='Search',
         )
 
-        name = django_filters.ModelMultipleChoiceFilter(
-            queryset=Secret.objects.all(),
-            field_name='name',
-            label='Name',
-        )
+        name = MultiValueCharFilter(lookup_expr='iexact')
 
         role_id = django_filters.ModelMultipleChoiceFilter(
             queryset=SecretRole.objects.all(),
             label='Role (ID)',
         )
         role = django_filters.ModelMultipleChoiceFilter(
             field_name='role__slug',
@@ -109,13 +123,28 @@
             field_name='assigned_object_type',
             queryset=ContentType.objects.filter(SECRET_ASSIGNABLE_MODELS),
             label='Object type (ID)',
         )
 
         class Meta:
             model = Secret
-            fields = ['id', 'assigned_object_type_id', 'assigned_object_id', 'role_id', 'role', 'name']
+            fields = [
+                'id',
+                'assigned_object_type_id',
+                'assigned_object_id',
+                'role_id',
+                'role',
+                'name',
+                '_object_repr',
+                'description',
+                'comments',
+            ]
 
         def search(self, queryset, name, value):
             if not value.strip():
                 return queryset
-            return queryset.filter(Q(name__icontains=value))
+            return queryset.filter(
+                Q(name__icontains=value)
+                | Q(_object_repr__icontains=value)
+                | Q(description__icontains=value)
+                | Q(comments__icontains=value),
+            )
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/migrations/0001_initial.py` & `netbox-secrets-1.8.0/netbox_secrets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/migrations/0002_populate_userkeys.py` & `netbox-secrets-1.8.0/netbox_secrets/migrations/0002_populate_userkeys.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     UserKey = apps.get_model('netbox_secrets', 'UserKey')
 
     # Retrieve the necessary data from SecretStore objects
     userkeys = UserKeyOld.objects.values('id', 'created', 'last_updated', 'user', 'public_key', 'master_key_cipher')
 
     # Queue UserKeys to be created
     userkeys_to_create = []
-    userkey_count = userkeys.count()
     for i, userkey in enumerate(userkeys, start=1):
         userkeys_to_create.append(
             UserKey(
                 id=userkey['id'],
                 created=userkey['created'],
                 last_updated=userkey['last_updated'],
                 user_id=userkey['user'],
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/migrations/0003_populate_secretroles.py` & `netbox-secrets-1.8.0/netbox_secrets/migrations/0003_populate_secretroles.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         'created',
         'last_updated',
         'custom_field_data',
     )
 
     # Queue SecretRoles to be created
     roles_to_create = []
-    role_count = roles.count()
     for i, role in enumerate(roles, start=1):
         roles_to_create.append(
             SecretRole(
                 id=role['id'],
                 name=role['name'],
                 slug=role['slug'],
                 description=role['description'],
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/migrations/0004_populate_secrets.py` & `netbox-secrets-1.8.0/netbox_secrets/migrations/0004_populate_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         'hash',
         'assigned_object_type_id',
         'role_id',
     )
 
     # Queue Secrets to be created
     secrets_to_create = []
-    secret_count = secrets.count()
     for i, secret in enumerate(secrets, start=1):
         secrets_to_create.append(
             Secret(
                 created=secret['created'],
                 last_updated=secret['last_updated'],
                 custom_field_data=secret['custom_field_data'],
                 id=secret['id'],
@@ -42,14 +41,15 @@
                 hash=secret['hash'],
             ),
         )
 
     # Bulk create the secret objects
     Secret.objects.bulk_create(secrets_to_create, batch_size=100)
 
+
 def update_objectchanges(apps, schema_editor):
     """
     Update the ObjectChange records to reflect the new model name.
     """
     ObjectChange = apps.get_model('extras', 'ObjectChange')
     ContentType = apps.get_model('contenttypes', 'ContentType')
 
@@ -62,17 +62,19 @@
         ctnbsecret = ContentType.objects.get(app_label='netbox_secretstore', model='secret')
         ctnbsecretrole = ContentType.objects.get(app_label='netbox_secretstore', model='secretrole')
         ctnbuserkey = ContentType.objects.get(app_label='netbox_secretstore', model='userkey')
         ctnbsessionkey = ContentType.objects.get(app_label='netbox_secretstore', model='sessionkey')
 
         ObjectChange.objects.filter(changed_object_type_id=ctnbsecret.id).update(changed_object_type_id=ctsecret.id)
         ObjectChange.objects.filter(changed_object_type_id=ctnbsecretrole.id).update(
-            changed_object_type_id=ctsecretrole.id)
+            changed_object_type_id=ctsecretrole.id,
+        )
         ObjectChange.objects.filter(changed_object_type_id=ctnbsessionkey.id).update(
-            changed_object_type_id=ctsessionkey.id)
+            changed_object_type_id=ctsessionkey.id,
+        )
         ObjectChange.objects.filter(changed_object_type_id=ctnbuserkey.id).update(changed_object_type_id=ctuserkey.id)
     except (ContentType.DoesNotExist, LookupError):
         pass
 
 
 class Migration(migrations.Migration):
     dependencies = [
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py` & `netbox-secrets-1.8.0/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py` & `netbox-secrets-1.8.0/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/models/secrets.py` & `netbox-secrets-1.8.0/netbox_secrets/models/secrets.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,22 @@
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.urls import reverse
 from django.utils.encoding import force_bytes
-from netbox.models import NetBoxModel
+from netbox.models import PrimaryModel
 from netbox.models.features import ChangeLoggingMixin, WebhooksMixin
 from utilities.querysets import RestrictedQuerySet
 
-from netbox_secrets.exceptions import InvalidKey
-from netbox_secrets.hashers import SecretValidationHasher
-from netbox_secrets.querysets import UserKeyQuerySet
-from netbox_secrets.utils import (
-    decrypt_master_key,
-    encrypt_master_key,
-    generate_random_key,
-)
+from ..exceptions import InvalidKey
+from ..hashers import SecretValidationHasher
+from ..querysets import UserKeyQuerySet
+from ..utils import decrypt_master_key, encrypt_master_key, generate_random_key
 
 __all__ = [
     'Secret',
     'SecretRole',
     'SessionKey',
     'UserKey',
 ]
@@ -219,47 +215,36 @@
         # Validate the recovered session key
         if not check_password(session_key, self.hash):
             raise InvalidKey("Invalid master key")
 
         return session_key
 
 
-class SecretRole(NetBoxModel):
+class SecretRole(PrimaryModel):
     """
     A SecretRole represents an arbitrary functional classification of Secrets. For example, a user might define roles
     such as "Login Credentials" or "SNMP Communities."
     """
 
     name = models.CharField(max_length=100, unique=True)
     slug = models.SlugField(max_length=100, unique=True)
-    description = models.CharField(
-        max_length=200,
-        blank=True,
-    )
 
-    csv_headers = ['name', 'slug', 'description']
+    clone_fields = ['tags']
 
     class Meta:
         ordering = ['name']
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_secrets:secretrole', args=[self.pk])
 
-    def to_csv(self):
-        return (
-            self.name,
-            self.slug,
-            self.description,
-        )
-
 
-class Secret(NetBoxModel):
+class Secret(PrimaryModel):
     """
     A Secret stores an AES256-encrypted copy of sensitive data, such as passwords or secret keys. An irreversible
     SHA-256 hash is stored along with the ciphertext for validation upon decryption. Each Secret is assigned to exactly
     one NetBox object, and objects may have multiple Secrets associated with them. A name can optionally be defined
     along with the ciphertext; this string is stored as plain text in the database.
 
     A Secret can be up to 65,535 bytes (64KB - 1B) in length. Each secret string will be padded with random data to
@@ -268,27 +253,32 @@
 
     assigned_object_type = models.ForeignKey(
         to=ContentType,
         on_delete=models.PROTECT,
         related_name='secrets',
     )
     assigned_object_id = models.PositiveIntegerField()
+    # Internal field for searching the assinged object
+    _object_repr = models.CharField(max_length=200, editable=False, blank=True, null=True)
     assigned_object = GenericForeignKey(ct_field='assigned_object_type', fk_field='assigned_object_id')
     role = models.ForeignKey(to='SecretRole', on_delete=models.PROTECT, related_name='secrets')
     name = models.CharField(max_length=100, blank=True)
     ciphertext = models.BinaryField(
         max_length=65568,
         editable=False,  # 128-bit IV + 16-bit pad length + 65535B secret + 15B padding
     )
     hash = models.CharField(max_length=128, editable=False)
 
     objects = RestrictedQuerySet.as_manager()
 
     plaintext = None
-    csv_headers = ['assigned_object_type', 'assigned_object_id', 'role', 'name', 'plaintext']
+
+    clone_fields = ('role', 'assigned_object_id', 'assigned_object_type', 'tags')
+
+    prerequisite_models = ('netbox_secrets.SecretRole', *plugin_settings.get('apps'))
 
     class Meta:
         ordering = ('role', 'name', 'pk')
         unique_together = ('assigned_object_type', 'assigned_object_id', 'role', 'name')
 
     def __init__(self, *args, **kwargs):
         self.plaintext = kwargs.pop('plaintext', None)
@@ -296,26 +286,18 @@
 
     def __str__(self):
         return self.name or 'Secret'
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_secrets:secret', args=[self.pk])
 
-    @classmethod
-    def get_prerequisite_models(cls):
-        return [SecretRole]
-
-    def to_csv(self):
-        return (
-            f'{self.assigned_object_type.app_label}.{self.assigned_object_type.model}',
-            self.assigned_object_id,
-            self.role,
-            self.name,
-            self.plaintext or '',
-        )
+    def save(self, *args, **kwargs):
+        self._object_repr = str(self.assigned_object)
+
+        return super().save(*args, **kwargs)
 
     def _pad(self, s):
         """
         Prepend the length of the plaintext (2B) and pad with garbage to a multiple of 16B (minimum of 64B).
         +--+--------+-------------------------------------------+
         |LL|MySecret|xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx|
         +--+--------+-------------------------------------------+
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/navigation.py` & `netbox-secrets-1.8.0/netbox_secrets/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js` & `netbox-secrets-1.8.0/netbox_secrets/static/netbox_secrets/secrets.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,104 +1,121 @@
+"use strict";
 (() => {
-    var R = Object.create;
-    var E = Object.defineProperty;
-    var I = Object.getOwnPropertyDescriptor;
-    var M = Object.getOwnPropertyNames;
-    var P = Object.getPrototypeOf,
-        C = Object.prototype.hasOwnProperty;
-    var B = e => E(e, "__esModule", {
-        value: !0
-    });
-    var D = (e, r) => () => (r || e((r = {
+    var P = Object.create;
+    var b = Object.defineProperty;
+    var M = Object.getOwnPropertyDescriptor;
+    var R = Object.getOwnPropertyNames;
+    var C = Object.getPrototypeOf,
+        D = Object.prototype.hasOwnProperty;
+    var _ = (e, r) => () => (r || e((r = {
         exports: {}
     }).exports, r), r.exports);
-    var H = (e, r, o) => {
-            if (r && typeof r == "object" || typeof r == "function")
-                for (let t of M(r)) !C.call(e, t) && t !== "default" && E(e, t, {
-                    get: () => r[t],
-                    enumerable: !(o = I(r, t)) || o.enumerable
-                });
-            return e
-        },
-        _ = e => H(B(E(e != null ? R(P(e)) : {}, "default", e && e.__esModule && "default" in e ? {
-            get: () => e.default,
-            enumerable: !0
-        } : {
-            value: e,
-            enumerable: !0
-        })), e);
+    var H = (e, r, o, t) => {
+        if (r && typeof r == "object" || typeof r == "function")
+            for (let i of R(r)) !D.call(e, i) && i !== o && b(e, i, {
+                get: () => r[i],
+                enumerable: !(t = M(r, i)) || t.enumerable
+            });
+        return e
+    };
+    var B = (e, r, o) => (o = e != null ? P(C(e)) : {}, H(r || !e || !e.__esModule ? b(o, "default", {
+        value: e,
+        enumerable: !0
+    }) : o, e));
     var p = (e, r, o) => new Promise((t, i) => {
-        var c = a => {
+        var s = c => {
                 try {
-                    s(o.next(a))
+                    a(o.next(c))
                 } catch (l) {
                     i(l)
                 }
             },
-            n = a => {
+            n = c => {
                 try {
-                    s(o.throw(a))
+                    a(o.throw(c))
                 } catch (l) {
                     i(l)
                 }
             },
-            s = a => a.done ? t(a.value) : Promise.resolve(a.value).then(c, n);
-        s((o = o.apply(e, r)).next())
+            a = c => c.done ? t(c.value) : Promise.resolve(c.value).then(s, n);
+        a((o = o.apply(e, r)).next())
     });
-    var T = D(v => {
+    var h = _(E => {
         "use strict";
-        v.parse = O;
-        v.serialize = F;
-        var q = decodeURIComponent,
-            $ = encodeURIComponent,
-            K = /; */,
+        E.parse = O;
+        E.serialize = q;
+        var I = Object.prototype.toString,
             m = /^[\u0009\u0020-\u007e\u0080-\u00ff]+$/;
 
         function O(e, r) {
             if (typeof e != "string") throw new TypeError("argument str must be a string");
-            for (var o = {}, t = r || {}, i = e.split(K), c = t.decode || q, n = 0; n < i.length; n++) {
-                var s = i[n],
-                    a = s.indexOf("=");
-                if (!(a < 0)) {
-                    var l = s.substr(0, a).trim(),
-                        u = s.substr(++a, s.length).trim();
-                    u[0] == '"' && (u = u.slice(1, -1)), o[l] == null && (o[l] = U(u, c))
+            for (var o = {}, t = r || {}, i = t.decode || $, s = 0; s < e.length;) {
+                var n = e.indexOf("=", s);
+                if (n === -1) break;
+                var a = e.indexOf(";", s);
+                if (a === -1) a = e.length;
+                else if (a < n) {
+                    s = e.lastIndexOf(";", n - 1) + 1;
+                    continue
+                }
+                var c = e.slice(s, n).trim();
+                if (o[c] === void 0) {
+                    var l = e.slice(n + 1, a).trim();
+                    l.charCodeAt(0) === 34 && (l = l.slice(1, -1)), o[c] = F(l, i)
                 }
+                s = a + 1
             }
             return o
         }
 
-        function F(e, r, o) {
+        function q(e, r, o) {
             var t = o || {},
-                i = t.encode || $;
+                i = t.encode || K;
             if (typeof i != "function") throw new TypeError("option encode is invalid");
             if (!m.test(e)) throw new TypeError("argument name is invalid");
-            var c = i(r);
-            if (c && !m.test(c)) throw new TypeError("argument val is invalid");
-            var n = e + "=" + c;
+            var s = i(r);
+            if (s && !m.test(s)) throw new TypeError("argument val is invalid");
+            var n = e + "=" + s;
             if (t.maxAge != null) {
-                var s = t.maxAge - 0;
-                if (isNaN(s) || !isFinite(s)) throw new TypeError("option maxAge is invalid");
-                n += "; Max-Age=" + Math.floor(s)
+                var a = t.maxAge - 0;
+                if (isNaN(a) || !isFinite(a)) throw new TypeError("option maxAge is invalid");
+                n += "; Max-Age=" + Math.floor(a)
             }
             if (t.domain) {
                 if (!m.test(t.domain)) throw new TypeError("option domain is invalid");
                 n += "; Domain=" + t.domain
             }
             if (t.path) {
                 if (!m.test(t.path)) throw new TypeError("option path is invalid");
                 n += "; Path=" + t.path
             }
             if (t.expires) {
-                if (typeof t.expires.toUTCString != "function") throw new TypeError("option expires is invalid");
-                n += "; Expires=" + t.expires.toUTCString()
+                var c = t.expires;
+                if (!j(c) || isNaN(c.valueOf())) throw new TypeError("option expires is invalid");
+                n += "; Expires=" + c.toUTCString()
             }
-            if (t.httpOnly && (n += "; HttpOnly"), t.secure && (n += "; Secure"), t.sameSite) {
-                var a = typeof t.sameSite == "string" ? t.sameSite.toLowerCase() : t.sameSite;
-                switch (a) {
+            if (t.httpOnly && (n += "; HttpOnly"), t.secure && (n += "; Secure"), t.priority) {
+                var l = typeof t.priority == "string" ? t.priority.toLowerCase() : t.priority;
+                switch (l) {
+                    case "low":
+                        n += "; Priority=Low";
+                        break;
+                    case "medium":
+                        n += "; Priority=Medium";
+                        break;
+                    case "high":
+                        n += "; Priority=High";
+                        break;
+                    default:
+                        throw new TypeError("option priority is invalid")
+                }
+            }
+            if (t.sameSite) {
+                var u = typeof t.sameSite == "string" ? t.sameSite.toLowerCase() : t.sameSite;
+                switch (u) {
                     case !0:
                         n += "; SameSite=Strict";
                         break;
                     case "lax":
                         n += "; SameSite=Lax";
                         break;
                     case "strict":
@@ -110,15 +127,27 @@
                     default:
                         throw new TypeError("option sameSite is invalid")
                 }
             }
             return n
         }
 
-        function U(e, r) {
+        function $(e) {
+            return e.indexOf("%") !== -1 ? decodeURIComponent(e) : e
+        }
+
+        function K(e) {
+            return encodeURIComponent(e)
+        }
+
+        function j(e) {
+            return I.call(e) === "[object Date]" || e instanceof Date
+        }
+
+        function F(e, r) {
             try {
                 return r(e)
             } catch (o) {
                 return e
             }
         }
     });
@@ -135,195 +164,200 @@
             case "info":
                 i = "mdi-information";
                 break;
             case "danger":
                 i = "mdi-alert";
                 break
         }
-        let c = document.createElement("div");
-        c.setAttribute("class", "toast-container position-fixed bottom-0 end-0 m-3");
+        let s = document.createElement("div");
+        s.setAttribute("class", "toast-container position-fixed bottom-0 end-0 m-3");
         let n = document.createElement("div");
         n.setAttribute("class", `toast bg-${e}`), n.setAttribute("role", "alert"), n.setAttribute("aria-live", "assertive"), n.setAttribute("aria-atomic", "true");
-        let s = document.createElement("div");
-        s.setAttribute("class", `toast-header bg-${e} text-body`);
-        let a = document.createElement("i");
-        a.setAttribute("class", `mdi ${i}`);
+        let a = document.createElement("div");
+        a.setAttribute("class", `toast-header bg-${e} text-body`);
+        let c = document.createElement("i");
+        c.setAttribute("class", `mdi ${i}`);
         let l = document.createElement("strong");
         l.setAttribute("class", "me-auto ms-1"), l.innerText = r;
         let u = document.createElement("button");
         u.setAttribute("type", "button"), u.setAttribute("class", "btn-close"), u.setAttribute("data-bs-dismiss", "toast"), u.setAttribute("aria-label", "Close");
         let y = document.createElement("div");
-        if (y.setAttribute("class", "toast-body"), s.appendChild(a), s.appendChild(l), typeof t != "undefined") {
-            let b = document.createElement("small");
-            b.setAttribute("class", "text-muted"), s.appendChild(b)
+        if (y.setAttribute("class", "toast-body"), a.appendChild(c), a.appendChild(l), typeof t != "undefined") {
+            let g = document.createElement("small");
+            g.setAttribute("class", "text-muted"), a.appendChild(g)
         }
-        return s.appendChild(u), y.innerText = o.trim(), n.appendChild(s), n.appendChild(y), c.appendChild(n), document.body.appendChild(c), new window.Toast(n)
+        return a.appendChild(u), y.innerText = o.trim(), n.appendChild(a), n.appendChild(y), s.appendChild(n), document.body.appendChild(s), new window.Toast(n)
     }
-    var h = _(T());
+    var T = B(h());
 
-    function S(e) {
+    function A(e) {
         return "error" in e && "exception" in e
     }
 
     function f(e) {
         return "error" in e
     }
 
-    function k(e) {
+    function v(e) {
         return "value" in e && "required" in e
     }
 
-    function j() {
+    function N() {
         let {
             csrftoken: e
-        } = h.default.parse(document.cookie);
+        } = T.default.parse(document.cookie);
         if (typeof e == "undefined") throw new Error("Invalid or missing CSRF token");
         return e
     }
 
-    function A(e, r, o) {
+    function S(e, r, o) {
         return p(this, null, function*() {
-            let t = j(),
+            let t = N(),
                 i = new Headers({
                     "X-CSRFToken": t
                 }),
-                c;
-            typeof o != "undefined" && (c = JSON.stringify(o), i.set("content-type", "application/json"), i.set("Accept", "application/json"));
+                s;
+            typeof o != "undefined" && (s = JSON.stringify(o), i.set("content-type", "application/json"), i.set("Accept", "application/json"));
             let n = yield fetch(e, {
                 method: r,
-                body: c,
+                body: s,
                 headers: i,
                 credentials: "same-origin"
-            }), s = n.headers.get("Content-Type");
-            if (typeof s == "string" && s.includes("text")) return {
+            }), a = n.headers.get("Content-Type");
+            if (typeof a == "string" && a.includes("text")) return {
                 error: yield n.text()
             };
-            let a = yield n.json();
-            return !n.ok && Array.isArray(a) ? {
-                error: a.join(`
+            let c = yield n.json();
+            return !n.ok && Array.isArray(c) ? {
+                error: c.join(`
 `)
-            } : !n.ok && "detail" in a ? {
-                error: a.detail
-            } : a
+            } : !n.ok && "detail" in c ? {
+                error: c.detail
+            } : c
         })
     }
 
     function x(e, r) {
         return p(this, null, function*() {
-            return yield A(e, "POST", r)
+            return yield S(e, "POST", r)
         })
     }
 
-    function g(e) {
+    function k(e) {
         return p(this, null, function*() {
-            return yield A(e, "GET")
+            return yield S(e, "GET")
         })
     }
 
     function G() {
         let e = document.getElementById("new_keypair_modal"),
             r = document.getElementById("use_new_pubkey");
         if (e === null || r === null) return;
         let o = e.querySelector("textarea#new_pubkey"),
             t = e.querySelector("textarea#new_privkey");
 
         function i() {
             for (let n of [o, t]) n !== null && n.setAttribute("readonly", "");
-            g("/api/plugins/secrets/generate-rsa-key-pair/").then(n => {
+            k("/api/plugins/secrets/generate-rsa-key-pair/").then(n => {
                 if (f(n)) d("danger", "Error", n.error).show();
                 else {
                     let {
-                        private_key: s,
-                        public_key: a
+                        private_key: a,
+                        public_key: c
                     } = n;
-                    o !== null && t !== null && (o.value = a, t.value = s)
+                    o !== null && t !== null && (o.value = c, t.value = a)
                 }
             })
         }
 
-        function c() {
+        function s() {
             let n = document.getElementById("id_public_key");
             o !== null && (n.value = o.value, n.innerText = o.value)
         }
-        e.addEventListener("shown.bs.modal", () => i()), r.addEventListener("click", () => c())
+        e.addEventListener("shown.bs.modal", () => i()), r.addEventListener("click", () => s())
     }
 
     function L(e, r) {
         let o = document.querySelector(`button.unlock-secret[secret-id='${e}']`),
             t = document.querySelector(`button.lock-secret[secret-id='${e}']`),
             i = document.querySelector(`button.copy-secret[secret-id='${e}']`);
         o !== null && (r === "unlock" && o.classList.add("d-none"), r === "lock" && o.classList.remove("d-none")), t !== null && (r === "unlock" && t.classList.remove("d-none"), r === "lock" && t.classList.add("d-none")), i !== null && (r === "unlock" && i.classList.remove("d-none"), r === "lock" && i.classList.add("d-none"))
     }
 
-    function N() {
+    function U() {
         let e = new window.Modal("#privkey_modal");
 
         function r(t) {
             let i = document.getElementById(`secret_${t}`);
-            typeof t == "string" && t !== "" && g(`/api/plugins/secrets/secrets/${t}/`).then(c => {
-                if (f(c)) c.error.toLowerCase().includes("invalid session key") ? e.show() : d("danger", "Error", c.error).show();
+            typeof t == "string" && t !== "" && k(`/api/plugins/secrets/secrets/${t}/`).then(s => {
+                if (f(s)) s.error.toLowerCase().includes("invalid session key") ? e.show() : d("danger", "Error", s.error).show();
                 else {
                     let {
                         plaintext: n
-                    } = c;
-                    i !== null && n !== null ? (k(i) ? i.value = n : i.innerText = n, L(t, "unlock")) : e.show()
+                    } = s;
+                    i !== null && n !== null ? (v(i) ? i.value = n : i.innerText = n, L(t, "unlock")) : e.show()
                 }
             })
         }
 
         function o(t) {
             if (typeof t == "string" && t !== "") {
                 let i = document.getElementById(`secret_${t}`);
-                k(i) ? i.value = "********" : i.innerText = "********", L(t, "lock")
+                v(i) ? i.value = "********" : i.innerText = "********", L(t, "lock")
             }
         }
         for (let t of document.querySelectorAll("button.unlock-secret")) t.addEventListener("click", () => r(t.getAttribute("secret-id")));
         for (let t of document.querySelectorAll("button.lock-secret")) t.addEventListener("click", () => o(t.getAttribute("secret-id")))
     }
 
     function z(e) {
-        x("/api/plugins/secrets/get-session-key/", {
+        x("/api/plugins/secrets/session-keys/", {
             private_key: e,
-            preserve: !0
+            preserve_key: !0
         }).then(r => {
             if (!f(r)) window.location.pathname === "/plugins/secrets/user-key/" ? window.location.reload() : d("success", "Session Key Received", "You may now unlock secrets.").show();
             else {
                 let o = r.error;
-                S(r) && (o += `
+                A(r) && (o += `
 ${r.exception}`), d("danger", "Failed to Retrieve Session Key", o).show()
             }
         })
     }
 
     function J() {
-        for (let e of document.querySelectorAll("#request_session_key")) {
-            let r = function() {
-                for (let o of document.querySelectorAll("#user_privkey")) z(o.value), o.value = ""
+        for (let r of document.querySelectorAll("#request_session_key")) {
+            let o = function() {
+                for (let t of document.querySelectorAll("#user_privkey")) z(t.value), t.value = ""
             };
-            e.addEventListener("click", r)
+            var e = o;
+            r.addEventListener("click", o)
         }
     }
 
     function X() {
         let e = new window.Modal("#privkey_modal");
 
         function r(o) {
-            document.cookie.indexOf("session_key") === -1 && (o.preventDefault(), e.show())
+            document.cookie.indexOf("netbox_secrets_sessionid") === -1 && (o.preventDefault(), e.show())
         }
         for (let o of document.querySelectorAll(".requires-session-key")) {
             let t = o.closest("form");
             t !== null && t.addEventListener("submit", r)
         }
     }
 
     function w() {
-        for (let e of [G, N, J, X]) e()
+        for (let e of [G, U, J, X]) e()
     }
     document.readyState !== "loading" ? w() : document.addEventListener("DOMContentLoaded", w);
 })();
-/*!
- * cookie
- * Copyright(c) 2012-2014 Roman Shtylman
- * Copyright(c) 2015 Douglas Christopher Wilson
- * MIT Licensed
- */
+/*! Bundled license information:
+
+cookie/index.js:
+  (*!
+   * cookie
+   * Copyright(c) 2012-2014 Roman Shtylman
+   * Copyright(c) 2015 Douglas Christopher Wilson
+   * MIT Licensed
+   *)
+*/
 //# sourceMappingURL=/static/netbox_secrets/secrets.js.map
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/static/netbox_secrets/secrets.js.map` & `netbox-secrets-1.8.0/netbox_secrets/static/netbox_secrets/secrets.js.map`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7428571428571429%*

 * *Differences: {"'mappings'": "'yuBAAA,IAAAA,EAAAC,EAAAC,GAAA,cAcAA,EAAQ,MAAQC,EAChBD,EAAQ,UAAYE,EAOpB,IAAIC,EAAa,OAAO,UAAU,SAU9BC,EAAqB,wCAczB,SAASH,EAAMI,EAAKC,EAAS,CAC3B,GAAI,OAAOD,GAAQ,SACjB,MAAM,IAAI,UAAU,+BAA+B,EAQrD,QALIE,EAAM,CAAC,EACPC,EAAMF,GAAW,CAAC,EAClBG,EAAMD,EAAI,QAAUE,EAEpBC,EAAQ,EACLA,EAAQN,EAAI,QAAQ,CACzB,IAAIO,EAAQP,EAAI,QAAQ,IAAKM,CAAK,EAGlC,GAAIC,IAAU,GACZ,MAGF,IAAIC,EAASR,EAAI,QAAQ,IAAKM,CAAK,EAEnC,GAAIE,IAAW,GACbA,EAASR,EAAI,eACJQ,EAASD,EAAO,CAEzBD,EAAQN,EAAI,YAAY,IAAKO,EAAQ,CAAC,EAAI,EAC1C,SAGF,IAA […]*

```diff
@@ -1,19 +1,128 @@
 {
-    "mappings": "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",
-    "names": [],
+    "mappings": "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",
+    "names": [
+        "require_cookie",
+        "__commonJSMin",
+        "exports",
+        "parse",
+        "serialize",
+        "__toString",
+        "fieldContentRegExp",
+        "str",
+        "options",
+        "obj",
+        "opt",
+        "dec",
+        "decode",
+        "index",
+        "eqIdx",
+        "endIdx",
+        "key",
+        "val",
+        "tryDecode",
+        "name",
+        "enc",
+        "encode",
+        "value",
+        "maxAge",
+        "expires",
+        "isDate",
+        "priority",
+        "sameSite",
+        "e",
+        "createToast",
+        "level",
+        "title",
+        "message",
+        "extra",
+        "iconName",
+        "container",
+        "main",
+        "header",
+        "icon",
+        "titleElement",
+        "button",
+        "body",
+        "extraElement",
+        "import_cookie",
+        "isApiError",
+        "data",
+        "hasError",
+        "isInputElement",
+        "element",
+        "getCsrfToken",
+        "csrfToken",
+        "Cookie",
+        "apiRequest",
+        "url",
+        "method",
+        "__async",
+        "token",
+        "headers",
+        "body",
+        "res",
+        "contentType",
+        "json",
+        "apiPostForm",
+        "apiGetBase",
+        "initGenerateKeyPair",
+        "element",
+        "accept",
+        "publicElem",
+        "privateElem",
+        "handleOpen",
+        "elem",
+        "apiGetBase",
+        "data",
+        "hasError",
+        "createToast",
+        "priv",
+        "pub",
+        "handleAccept",
+        "publicKeyField",
+        "toggleSecretButtons",
+        "id",
+        "action",
+        "unlockButton",
+        "lockButton",
+        "copyButton",
+        "initLockUnlock",
+        "privateKeyModal",
+        "unlock",
+        "target",
+        "plaintext",
+        "isInputElement",
+        "lock",
+        "requestSessionKey",
+        "privateKey",
+        "apiPostForm",
+        "res",
+        "message",
+        "isApiError",
+        "initGetSessionKey",
+        "handleClick",
+        "pk",
+        "initSecretsEdit",
+        "handleSubmit",
+        "event",
+        "form",
+        "initSecrets",
+        "func",
+        "initSecrets"
+    ],
     "sources": [
         "../node_modules/cookie/index.js",
         "../src/bs.ts",
         "../src/util.ts",
         "../src/secrets.ts",
         "../src/index.ts"
     ],
     "sourcesContent": [
-        "/*!\n * cookie\n * Copyright(c) 2012-2014 Roman Shtylman\n * Copyright(c) 2015 Douglas Christopher Wilson\n * MIT Licensed\n */\n\n'use strict';\n\n/**\n * Module exports.\n * @public\n */\n\nexports.parse = parse;\nexports.serialize = serialize;\n\n/**\n * Module variables.\n * @private\n */\n\nvar decode = decodeURIComponent;\nvar encode = encodeURIComponent;\nvar pairSplitRegExp = /; */;\n\n/**\n * RegExp to match field-content in RFC 7230 sec 3.2\n *\n * field-content = field-vchar [ 1*( SP / HTAB ) field-vchar ]\n * field-vchar   = VCHAR / obs-text\n * obs-text      = %x80-FF\n */\n\nvar fieldContentRegExp = /^[\\u0009\\u0020-\\u007e\\u0080-\\u00ff]+$/;\n\n/**\n * Parse a cookie header.\n *\n * Parse the given cookie header string into an object\n * The object has the various cookies as keys(names) => values\n *\n * @param {string} str\n * @param {object} [options]\n * @return {object}\n * @public\n */\n\nfunction parse(str, options) {\n  if (typeof str !== 'string') {\n    throw new TypeError('argument str must be a string');\n  }\n\n  var obj = {}\n  var opt = options || {};\n  var pairs = str.split(pairSplitRegExp);\n  var dec = opt.decode || decode;\n\n  for (var i = 0; i < pairs.length; i++) {\n    var pair = pairs[i];\n    var eq_idx = pair.indexOf('=');\n\n    // skip things that don't look like key=value\n    if (eq_idx < 0) {\n      continue;\n    }\n\n    var key = pair.substr(0, eq_idx).trim()\n    var val = pair.substr(++eq_idx, pair.length).trim();\n\n    // quoted values\n    if ('\"' == val[0]) {\n      val = val.slice(1, -1);\n    }\n\n    // only assign once\n    if (undefined == obj[key]) {\n      obj[key] = tryDecode(val, dec);\n    }\n  }\n\n  return obj;\n}\n\n/**\n * Serialize data into a cookie header.\n *\n * Serialize the a name value pair into a cookie string suitable for\n * http headers. An optional options object specified cookie parameters.\n *\n * serialize('foo', 'bar', { httpOnly: true })\n *   => \"foo=bar; httpOnly\"\n *\n * @param {string} name\n * @param {string} val\n * @param {object} [options]\n * @return {string}\n * @public\n */\n\nfunction serialize(name, val, options) {\n  var opt = options || {};\n  var enc = opt.encode || encode;\n\n  if (typeof enc !== 'function') {\n    throw new TypeError('option encode is invalid');\n  }\n\n  if (!fieldContentRegExp.test(name)) {\n    throw new TypeError('argument name is invalid');\n  }\n\n  var value = enc(val);\n\n  if (value && !fieldContentRegExp.test(value)) {\n    throw new TypeError('argument val is invalid');\n  }\n\n  var str = name + '=' + value;\n\n  if (null != opt.maxAge) {\n    var maxAge = opt.maxAge - 0;\n\n    if (isNaN(maxAge) || !isFinite(maxAge)) {\n      throw new TypeError('option maxAge is invalid')\n    }\n\n    str += '; Max-Age=' + Math.floor(maxAge);\n  }\n\n  if (opt.domain) {\n    if (!fieldContentRegExp.test(opt.domain)) {\n      throw new TypeError('option domain is invalid');\n    }\n\n    str += '; Domain=' + opt.domain;\n  }\n\n  if (opt.path) {\n    if (!fieldContentRegExp.test(opt.path)) {\n      throw new TypeError('option path is invalid');\n    }\n\n    str += '; Path=' + opt.path;\n  }\n\n  if (opt.expires) {\n    if (typeof opt.expires.toUTCString !== 'function') {\n      throw new TypeError('option expires is invalid');\n    }\n\n    str += '; Expires=' + opt.expires.toUTCString();\n  }\n\n  if (opt.httpOnly) {\n    str += '; HttpOnly';\n  }\n\n  if (opt.secure) {\n    str += '; Secure';\n  }\n\n  if (opt.sameSite) {\n    var sameSite = typeof opt.sameSite === 'string'\n      ? opt.sameSite.toLowerCase() : opt.sameSite;\n\n    switch (sameSite) {\n      case true:\n        str += '; SameSite=Strict';\n        break;\n      case 'lax':\n        str += '; SameSite=Lax';\n        break;\n      case 'strict':\n        str += '; SameSite=Strict';\n        break;\n      case 'none':\n        str += '; SameSite=None';\n        break;\n      default:\n        throw new TypeError('option sameSite is invalid');\n    }\n  }\n\n  return str;\n}\n\n/**\n * Try decoding a string using a decoding function.\n *\n * @param {string} str\n * @param {function} decode\n * @private\n */\n\nfunction tryDecode(str, decode) {\n  try {\n    return decode(str);\n  } catch (e) {\n    return str;\n  }\n}\n",
+        "/*!\n * cookie\n * Copyright(c) 2012-2014 Roman Shtylman\n * Copyright(c) 2015 Douglas Christopher Wilson\n * MIT Licensed\n */\n\n'use strict';\n\n/**\n * Module exports.\n * @public\n */\n\nexports.parse = parse;\nexports.serialize = serialize;\n\n/**\n * Module variables.\n * @private\n */\n\nvar __toString = Object.prototype.toString\n\n/**\n * RegExp to match field-content in RFC 7230 sec 3.2\n *\n * field-content = field-vchar [ 1*( SP / HTAB ) field-vchar ]\n * field-vchar   = VCHAR / obs-text\n * obs-text      = %x80-FF\n */\n\nvar fieldContentRegExp = /^[\\u0009\\u0020-\\u007e\\u0080-\\u00ff]+$/;\n\n/**\n * Parse a cookie header.\n *\n * Parse the given cookie header string into an object\n * The object has the various cookies as keys(names) => values\n *\n * @param {string} str\n * @param {object} [options]\n * @return {object}\n * @public\n */\n\nfunction parse(str, options) {\n  if (typeof str !== 'string') {\n    throw new TypeError('argument str must be a string');\n  }\n\n  var obj = {}\n  var opt = options || {};\n  var dec = opt.decode || decode;\n\n  var index = 0\n  while (index < str.length) {\n    var eqIdx = str.indexOf('=', index)\n\n    // no more cookie pairs\n    if (eqIdx === -1) {\n      break\n    }\n\n    var endIdx = str.indexOf(';', index)\n\n    if (endIdx === -1) {\n      endIdx = str.length\n    } else if (endIdx < eqIdx) {\n      // backtrack on prior semicolon\n      index = str.lastIndexOf(';', eqIdx - 1) + 1\n      continue\n    }\n\n    var key = str.slice(index, eqIdx).trim()\n\n    // only assign once\n    if (undefined === obj[key]) {\n      var val = str.slice(eqIdx + 1, endIdx).trim()\n\n      // quoted values\n      if (val.charCodeAt(0) === 0x22) {\n        val = val.slice(1, -1)\n      }\n\n      obj[key] = tryDecode(val, dec);\n    }\n\n    index = endIdx + 1\n  }\n\n  return obj;\n}\n\n/**\n * Serialize data into a cookie header.\n *\n * Serialize the a name value pair into a cookie string suitable for\n * http headers. An optional options object specified cookie parameters.\n *\n * serialize('foo', 'bar', { httpOnly: true })\n *   => \"foo=bar; httpOnly\"\n *\n * @param {string} name\n * @param {string} val\n * @param {object} [options]\n * @return {string}\n * @public\n */\n\nfunction serialize(name, val, options) {\n  var opt = options || {};\n  var enc = opt.encode || encode;\n\n  if (typeof enc !== 'function') {\n    throw new TypeError('option encode is invalid');\n  }\n\n  if (!fieldContentRegExp.test(name)) {\n    throw new TypeError('argument name is invalid');\n  }\n\n  var value = enc(val);\n\n  if (value && !fieldContentRegExp.test(value)) {\n    throw new TypeError('argument val is invalid');\n  }\n\n  var str = name + '=' + value;\n\n  if (null != opt.maxAge) {\n    var maxAge = opt.maxAge - 0;\n\n    if (isNaN(maxAge) || !isFinite(maxAge)) {\n      throw new TypeError('option maxAge is invalid')\n    }\n\n    str += '; Max-Age=' + Math.floor(maxAge);\n  }\n\n  if (opt.domain) {\n    if (!fieldContentRegExp.test(opt.domain)) {\n      throw new TypeError('option domain is invalid');\n    }\n\n    str += '; Domain=' + opt.domain;\n  }\n\n  if (opt.path) {\n    if (!fieldContentRegExp.test(opt.path)) {\n      throw new TypeError('option path is invalid');\n    }\n\n    str += '; Path=' + opt.path;\n  }\n\n  if (opt.expires) {\n    var expires = opt.expires\n\n    if (!isDate(expires) || isNaN(expires.valueOf())) {\n      throw new TypeError('option expires is invalid');\n    }\n\n    str += '; Expires=' + expires.toUTCString()\n  }\n\n  if (opt.httpOnly) {\n    str += '; HttpOnly';\n  }\n\n  if (opt.secure) {\n    str += '; Secure';\n  }\n\n  if (opt.priority) {\n    var priority = typeof opt.priority === 'string'\n      ? opt.priority.toLowerCase()\n      : opt.priority\n\n    switch (priority) {\n      case 'low':\n        str += '; Priority=Low'\n        break\n      case 'medium':\n        str += '; Priority=Medium'\n        break\n      case 'high':\n        str += '; Priority=High'\n        break\n      default:\n        throw new TypeError('option priority is invalid')\n    }\n  }\n\n  if (opt.sameSite) {\n    var sameSite = typeof opt.sameSite === 'string'\n      ? opt.sameSite.toLowerCase() : opt.sameSite;\n\n    switch (sameSite) {\n      case true:\n        str += '; SameSite=Strict';\n        break;\n      case 'lax':\n        str += '; SameSite=Lax';\n        break;\n      case 'strict':\n        str += '; SameSite=Strict';\n        break;\n      case 'none':\n        str += '; SameSite=None';\n        break;\n      default:\n        throw new TypeError('option sameSite is invalid');\n    }\n  }\n\n  return str;\n}\n\n/**\n * URL-decode string value. Optimized to skip native call when no %.\n *\n * @param {string} str\n * @returns {string}\n */\n\nfunction decode (str) {\n  return str.indexOf('%') !== -1\n    ? decodeURIComponent(str)\n    : str\n}\n\n/**\n * URL-encode value.\n *\n * @param {string} str\n * @returns {string}\n */\n\nfunction encode (val) {\n  return encodeURIComponent(val)\n}\n\n/**\n * Determine if value is a Date.\n *\n * @param {*} val\n * @private\n */\n\nfunction isDate (val) {\n  return __toString.call(val) === '[object Date]' ||\n    val instanceof Date\n}\n\n/**\n * Try decoding a string using a decoding function.\n *\n * @param {string} str\n * @param {function} decode\n * @private\n */\n\nfunction tryDecode(str, decode) {\n  try {\n    return decode(str);\n  } catch (e) {\n    return str;\n  }\n}\n",
         "type ToastLevel = 'danger' | 'warning' | 'success' | 'info';\n\nexport function createToast(\n  level: ToastLevel,\n  title: string,\n  message: string,\n  extra?: string,\n): InstanceType<typeof window.Toast> {\n  let iconName = 'mdi-alert';\n  switch (level) {\n    case 'warning':\n      iconName = 'mdi-alert';\n      break;\n    case 'success':\n      iconName = 'mdi-check-circle';\n      break;\n    case 'info':\n      iconName = 'mdi-information';\n      break;\n    case 'danger':\n      iconName = 'mdi-alert';\n      break;\n  }\n\n  const container = document.createElement('div');\n  container.setAttribute('class', 'toast-container position-fixed bottom-0 end-0 m-3');\n\n  const main = document.createElement('div');\n  main.setAttribute('class', `toast bg-${level}`);\n  main.setAttribute('role', 'alert');\n  main.setAttribute('aria-live', 'assertive');\n  main.setAttribute('aria-atomic', 'true');\n\n  const header = document.createElement('div');\n  header.setAttribute('class', `toast-header bg-${level} text-body`);\n\n  const icon = document.createElement('i');\n  icon.setAttribute('class', `mdi ${iconName}`);\n\n  const titleElement = document.createElement('strong');\n  titleElement.setAttribute('class', 'me-auto ms-1');\n  titleElement.innerText = title;\n\n  const button = document.createElement('button');\n  button.setAttribute('type', 'button');\n  button.setAttribute('class', 'btn-close');\n  button.setAttribute('data-bs-dismiss', 'toast');\n  button.setAttribute('aria-label', 'Close');\n\n  const body = document.createElement('div');\n  body.setAttribute('class', 'toast-body');\n\n  header.appendChild(icon);\n  header.appendChild(titleElement);\n\n  if (typeof extra !== 'undefined') {\n    const extraElement = document.createElement('small');\n    extraElement.setAttribute('class', 'text-muted');\n    header.appendChild(extraElement);\n  }\n\n  header.appendChild(button);\n\n  body.innerText = message.trim();\n\n  main.appendChild(header);\n  main.appendChild(body);\n  container.appendChild(main);\n  document.body.appendChild(container);\n\n  const toast = new window.Toast(main);\n  return toast;\n}\n",
         "import Cookie from 'cookie';\n\ntype APIRes<T> = T | ErrorBase | APIError;\ntype Method = 'GET' | 'POST' | 'PATCH' | 'PUT' | 'DELETE';\ntype ReqData = URLSearchParams | Dict | undefined | unknown;\n\n/**\n * Type guard to determine if an API response is a detailed error.\n *\n * @param data API JSON Response\n * @returns Type guard for `data`.\n */\nexport function isApiError(data: Record<string, unknown>): data is APIError {\n  return 'error' in data && 'exception' in data;\n}\n\n/**\n * Type guard to determine if an API response is an error.\n *\n * @param data API JSON Response\n * @returns Type guard for `data`.\n */\nexport function hasError(data: Record<string, unknown>): data is ErrorBase {\n  return 'error' in data;\n}\n\n/**\n * Type guard to determine if an element is an `HTMLInputElement`.\n *\n * @param element HTML Element.\n */\nexport function isInputElement(element: HTMLElement): element is HTMLInputElement {\n  return 'value' in element && 'required' in element;\n}\n\n/**\n * Retrieve the CSRF token from cookie storage.\n */\nexport function getCsrfToken(): string {\n  const { csrftoken: csrfToken } = Cookie.parse(document.cookie);\n  if (typeof csrfToken === 'undefined') {\n    throw new Error('Invalid or missing CSRF token');\n  }\n  return csrfToken;\n}\n\n/**\n * Authenticate and interact with the NetBox API.\n *\n * @param url Request URL\n * @param method Request Method\n * @param data Data to `POST`, `PATCH`, or `PUT`, if applicable.\n * @returns JSON Response\n */\nexport async function apiRequest<R extends Dict, D extends ReqData = undefined>(\n  url: string,\n  method: Method,\n  data?: D,\n): Promise<APIRes<R>> {\n  const token = getCsrfToken();\n  const headers = new Headers({ 'X-CSRFToken': token });\n\n  let body;\n  if (typeof data !== 'undefined') {\n    body = JSON.stringify(data);\n    headers.set('content-type', 'application/json');\n    headers.set('Accept', 'application/json');\n  }\n\n  const res = await fetch(url, { method, body, headers, credentials: 'same-origin' });\n  const contentType = res.headers.get('Content-Type');\n  if (typeof contentType === 'string' && contentType.includes('text')) {\n    const error = await res.text();\n    return { error } as ErrorBase;\n  }\n  const json = (await res.json()) as R | APIError;\n  if (!res.ok && Array.isArray(json)) {\n    const error = json.join('\\n');\n    return { error } as ErrorBase;\n  } else if (!res.ok && 'detail' in json) {\n    return { error: json.detail } as ErrorBase;\n  }\n  return json;\n}\n\n/**\n * `POST` an object as form data to the NetBox API.\n *\n * @param url Request URL\n * @param data Object to convert to form data\n * @returns JSON Response\n */\nexport async function apiPostForm<R extends Dict, D extends Dict>(\n  url: string,\n  data: D,\n): Promise<APIRes<R>> {\n  return await apiRequest<R, D>(url, 'POST', data);\n}\n\n/**\n * `GET` data from the NetBox API.\n *\n * @param url Request URL\n * @returns JSON Response\n */\nexport async function apiGetBase<R extends Dict>(url: string): Promise<APIRes<R>> {\n  return await apiRequest<R>(url, 'GET');\n}\n",
-        "import { createToast } from './bs';\nimport { apiGetBase, apiPostForm, isApiError, isInputElement, hasError } from './util';\n\nimport type { APISecret, APIKeyPair } from './types';\n\n/**\n * Initialize Generate Private Key Pair Elements.\n */\nfunction initGenerateKeyPair() {\n  const element = document.getElementById('new_keypair_modal') as HTMLDivElement;\n  const accept = document.getElementById('use_new_pubkey') as HTMLButtonElement;\n  // If the elements are not loaded, stop.\n  if (element === null || accept === null) {\n    return;\n  }\n  const publicElem = element.querySelector<HTMLTextAreaElement>('textarea#new_pubkey');\n  const privateElem = element.querySelector<HTMLTextAreaElement>('textarea#new_privkey');\n\n  /**\n   * Handle Generate Private Key Pair Modal opening.\n   */\n  function handleOpen() {\n    // When the modal opens, set the `readonly` attribute on the textarea elements.\n    for (const elem of [publicElem, privateElem]) {\n      if (elem !== null) {\n        elem.setAttribute('readonly', '');\n      }\n    }\n    // Fetch the key pair from the API.\n    apiGetBase<APIKeyPair>('/api/plugins/secrets/generate-rsa-key-pair/').then(data => {\n      if (!hasError(data)) {\n        // If key pair generation was successful, set the textarea elements' value to the generated\n        // values.\n        const { private_key: priv, public_key: pub } = data;\n        if (publicElem !== null && privateElem !== null) {\n          publicElem.value = pub;\n          privateElem.value = priv;\n        }\n      } else {\n        // Otherwise, show an error.\n        const toast = createToast('danger', 'Error', data.error);\n        toast.show();\n      }\n    });\n  }\n\n  /**\n   * Set the public key form field's value to the generated public key.\n   */\n  function handleAccept() {\n    const publicKeyField = document.getElementById('id_public_key') as HTMLTextAreaElement;\n    if (publicElem !== null) {\n      publicKeyField.value = publicElem.value;\n      publicKeyField.innerText = publicElem.value;\n    }\n  }\n  element.addEventListener('shown.bs.modal', () => handleOpen());\n  accept.addEventListener('click', () => handleAccept());\n}\n\n/**\n * Toggle copy/lock/unlock button visibility based on the action occurring.\n * @param id Secret ID.\n * @param action Lock or Unlock, so we know which buttons to display.\n */\nfunction toggleSecretButtons(id: string, action: 'lock' | 'unlock') {\n  const unlockButton = document.querySelector(`button.unlock-secret[secret-id='${id}']`);\n  const lockButton = document.querySelector(`button.lock-secret[secret-id='${id}']`);\n  const copyButton = document.querySelector(`button.copy-secret[secret-id='${id}']`);\n  // If we're unlocking, hide the unlock button. Otherwise, show it.\n  if (unlockButton !== null) {\n    if (action === 'unlock') unlockButton.classList.add('d-none');\n    if (action === 'lock') unlockButton.classList.remove('d-none');\n  }\n  // If we're unlocking, show the lock button. Otherwise, hide it.\n  if (lockButton !== null) {\n    if (action === 'unlock') lockButton.classList.remove('d-none');\n    if (action === 'lock') lockButton.classList.add('d-none');\n  }\n  // If we're unlocking, show the copy button. Otherwise, hide it.\n  if (copyButton !== null) {\n    if (action === 'unlock') copyButton.classList.remove('d-none');\n    if (action === 'lock') copyButton.classList.add('d-none');\n  }\n}\n\n/**\n * Initialize Lock & Unlock button event listeners & callbacks.\n */\nfunction initLockUnlock() {\n  const privateKeyModal = new window.Modal('#privkey_modal');\n\n  /**\n   * Unlock a secret, or prompt the user for their private key, if a session key is not available.\n   *\n   * @param id Secret ID\n   */\n  function unlock(id: string | null) {\n    const target = document.getElementById(`secret_${id}`) as HTMLDivElement | HTMLInputElement;\n    if (typeof id === 'string' && id !== '') {\n      apiGetBase<APISecret>(`/api/plugins/secrets/secrets/${id}/`).then(data => {\n        if (!hasError(data)) {\n          const { plaintext } = data;\n          // `plaintext` is the plain text value of the secret. If it is null, it has not been\n          // decrypted, likely due to a mission session key.\n\n          if (target !== null && plaintext !== null) {\n            // If `plaintext` is not null, we have the decrypted value. Set the target element's\n            // inner text to the decrypted value and toggle copy/lock button visibility.\n            if (isInputElement(target)) {\n              target.value = plaintext;\n            } else {\n              target.innerText = plaintext;\n            }\n\n            toggleSecretButtons(id, 'unlock');\n          } else {\n            // Otherwise, we do _not_ have the decrypted value and need to prompt the user for\n            // their private RSA key, in order to get a session key. The session key is then sent\n            // as a cookie in future requests.\n            privateKeyModal.show();\n          }\n        } else {\n          if (data.error.toLowerCase().includes('invalid session key')) {\n            // If, for some reason, a request was made but resulted in an API error that complains\n            // of a missing session key, prompt the user for their session key.\n            privateKeyModal.show();\n          } else {\n            // If we received an API error but it doesn't contain 'invalid session key', show the\n            // user an error message.\n            const toast = createToast('danger', 'Error', data.error);\n            toast.show();\n          }\n        }\n      });\n    }\n  }\n\n  /**\n   * Lock a secret and toggle visibility of the unlock button.\n   * @param id Secret ID\n   */\n  function lock(id: string | null) {\n    if (typeof id === 'string' && id !== '') {\n      const target = document.getElementById(`secret_${id}`) as HTMLDivElement | HTMLInputElement;\n\n      // Obscure the inner text of the secret element.\n      if (isInputElement(target)) {\n        target.value = '********';\n      } else {\n        target.innerText = '********';\n      }\n\n      // Toggle visibility of the copy/lock/unlock buttons.\n      toggleSecretButtons(id, 'lock');\n    }\n  }\n\n  for (const element of document.querySelectorAll<HTMLButtonElement>('button.unlock-secret')) {\n    element.addEventListener('click', () => unlock(element.getAttribute('secret-id')));\n  }\n  for (const element of document.querySelectorAll<HTMLButtonElement>('button.lock-secret')) {\n    element.addEventListener('click', () => lock(element.getAttribute('secret-id')));\n  }\n}\n\n/**\n * Request a session key from the API.\n * @param privateKey RSA Private Key (valid JSON string)\n */\nfunction requestSessionKey(privateKey: string) {\n  apiPostForm('/api/plugins/secrets/get-session-key/', {\n    private_key: privateKey,\n    preserve: true,\n  }).then(res => {\n    if (!hasError(res)) {\n      // If the session key has been added from the user key page, reload the page.\n      if (window.location.pathname === '/plugins/secrets/user-key/') {\n        window.location.reload();\n      } else {\n        // If the response received was not an error, show the user a success message.\n        const toast = createToast('success', 'Session Key Received', 'You may now unlock secrets.');\n        toast.show();\n      }\n    } else {\n      // Otherwise, show the user an error message.\n      let message = res.error;\n      if (isApiError(res)) {\n        // If the error received was a standard API error containing a Python exception message,\n        // append it to the error.\n        message += `\\n${res.exception}`;\n      }\n      const toast = createToast('danger', 'Failed to Retrieve Session Key', message);\n      toast.show();\n    }\n  });\n}\n\n/**\n * Initialize Request Session Key Elements.\n */\nfunction initGetSessionKey() {\n  for (const element of document.querySelectorAll<HTMLButtonElement>('#request_session_key')) {\n    /**\n     * Send the user's input private key to the API to get a session key, which will be stored as\n     * a cookie for future requests.\n     */\n    function handleClick() {\n      for (const pk of document.querySelectorAll<HTMLTextAreaElement>('#user_privkey')) {\n        requestSessionKey(pk.value);\n        // Clear the private key form field value.\n        pk.value = '';\n      }\n    }\n    element.addEventListener('click', handleClick);\n  }\n}\n\n/**\n * Initialize Secret Edit Form Handler.\n */\nfunction initSecretsEdit() {\n  const privateKeyModal = new window.Modal('#privkey_modal');\n\n  /**\n   * Check the cookie store for a `session_key`. If not present, prompt the user to submit their\n   * private key.\n   */\n  function handleSubmit(event: Event): void {\n    if (document.cookie.indexOf('session_key') === -1) {\n      event.preventDefault();\n      privateKeyModal.show();\n    }\n  }\n\n  for (const element of document.querySelectorAll<HTMLInputElement>('.requires-session-key')) {\n    const form = element.closest<HTMLFormElement>('form');\n    if (form !== null) {\n      form.addEventListener('submit', handleSubmit);\n    }\n  }\n}\n\nexport function initSecrets() {\n  for (const func of [initGenerateKeyPair, initLockUnlock, initGetSessionKey, initSecretsEdit]) {\n    func();\n  }\n}\n",
+        "import { createToast } from './bs';\nimport { apiGetBase, apiPostForm, isApiError, isInputElement, hasError } from './util';\n\nimport type { APISecret, APIKeyPair } from './types';\n\n/**\n * Initialize Generate Private Key Pair Elements.\n */\nfunction initGenerateKeyPair() {\n  const element = document.getElementById('new_keypair_modal') as HTMLDivElement;\n  const accept = document.getElementById('use_new_pubkey') as HTMLButtonElement;\n  // If the elements are not loaded, stop.\n  if (element === null || accept === null) {\n    return;\n  }\n  const publicElem = element.querySelector<HTMLTextAreaElement>('textarea#new_pubkey');\n  const privateElem = element.querySelector<HTMLTextAreaElement>('textarea#new_privkey');\n\n  /**\n   * Handle Generate Private Key Pair Modal opening.\n   */\n  function handleOpen() {\n    // When the modal opens, set the `readonly` attribute on the textarea elements.\n    for (const elem of [publicElem, privateElem]) {\n      if (elem !== null) {\n        elem.setAttribute('readonly', '');\n      }\n    }\n    // Fetch the key pair from the API.\n    apiGetBase<APIKeyPair>('/api/plugins/secrets/generate-rsa-key-pair/').then(data => {\n      if (!hasError(data)) {\n        // If key pair generation was successful, set the textarea elements' value to the generated\n        // values.\n        const { private_key: priv, public_key: pub } = data;\n        if (publicElem !== null && privateElem !== null) {\n          publicElem.value = pub;\n          privateElem.value = priv;\n        }\n      } else {\n        // Otherwise, show an error.\n        const toast = createToast('danger', 'Error', data.error);\n        toast.show();\n      }\n    });\n  }\n\n  /**\n   * Set the public key form field's value to the generated public key.\n   */\n  function handleAccept() {\n    const publicKeyField = document.getElementById('id_public_key') as HTMLTextAreaElement;\n    if (publicElem !== null) {\n      publicKeyField.value = publicElem.value;\n      publicKeyField.innerText = publicElem.value;\n    }\n  }\n  element.addEventListener('shown.bs.modal', () => handleOpen());\n  accept.addEventListener('click', () => handleAccept());\n}\n\n/**\n * Toggle copy/lock/unlock button visibility based on the action occurring.\n * @param id Secret ID.\n * @param action Lock or Unlock, so we know which buttons to display.\n */\nfunction toggleSecretButtons(id: string, action: 'lock' | 'unlock') {\n  const unlockButton = document.querySelector(`button.unlock-secret[secret-id='${id}']`);\n  const lockButton = document.querySelector(`button.lock-secret[secret-id='${id}']`);\n  const copyButton = document.querySelector(`button.copy-secret[secret-id='${id}']`);\n  // If we're unlocking, hide the unlock button. Otherwise, show it.\n  if (unlockButton !== null) {\n    if (action === 'unlock') unlockButton.classList.add('d-none');\n    if (action === 'lock') unlockButton.classList.remove('d-none');\n  }\n  // If we're unlocking, show the lock button. Otherwise, hide it.\n  if (lockButton !== null) {\n    if (action === 'unlock') lockButton.classList.remove('d-none');\n    if (action === 'lock') lockButton.classList.add('d-none');\n  }\n  // If we're unlocking, show the copy button. Otherwise, hide it.\n  if (copyButton !== null) {\n    if (action === 'unlock') copyButton.classList.remove('d-none');\n    if (action === 'lock') copyButton.classList.add('d-none');\n  }\n}\n\n/**\n * Initialize Lock & Unlock button event listeners & callbacks.\n */\nfunction initLockUnlock() {\n  const privateKeyModal = new window.Modal('#privkey_modal');\n\n  /**\n   * Unlock a secret, or prompt the user for their private key, if a session key is not available.\n   *\n   * @param id Secret ID\n   */\n  function unlock(id: string | null) {\n    const target = document.getElementById(`secret_${id}`) as HTMLDivElement | HTMLInputElement;\n    if (typeof id === 'string' && id !== '') {\n      apiGetBase<APISecret>(`/api/plugins/secrets/secrets/${id}/`).then(data => {\n        if (!hasError(data)) {\n          const { plaintext } = data;\n          // `plaintext` is the plain text value of the secret. If it is null, it has not been\n          // decrypted, likely due to a mission session key.\n\n          if (target !== null && plaintext !== null) {\n            // If `plaintext` is not null, we have the decrypted value. Set the target element's\n            // inner text to the decrypted value and toggle copy/lock button visibility.\n            if (isInputElement(target)) {\n              target.value = plaintext;\n            } else {\n              target.innerText = plaintext;\n            }\n\n            toggleSecretButtons(id, 'unlock');\n          } else {\n            // Otherwise, we do _not_ have the decrypted value and need to prompt the user for\n            // their private RSA key, in order to get a session key. The session key is then sent\n            // as a cookie in future requests.\n            privateKeyModal.show();\n          }\n        } else {\n          if (data.error.toLowerCase().includes('invalid session key')) {\n            // If, for some reason, a request was made but resulted in an API error that complains\n            // of a missing session key, prompt the user for their session key.\n            privateKeyModal.show();\n          } else {\n            // If we received an API error but it doesn't contain 'invalid session key', show the\n            // user an error message.\n            const toast = createToast('danger', 'Error', data.error);\n            toast.show();\n          }\n        }\n      });\n    }\n  }\n\n  /**\n   * Lock a secret and toggle visibility of the unlock button.\n   * @param id Secret ID\n   */\n  function lock(id: string | null) {\n    if (typeof id === 'string' && id !== '') {\n      const target = document.getElementById(`secret_${id}`) as HTMLDivElement | HTMLInputElement;\n\n      // Obscure the inner text of the secret element.\n      if (isInputElement(target)) {\n        target.value = '********';\n      } else {\n        target.innerText = '********';\n      }\n\n      // Toggle visibility of the copy/lock/unlock buttons.\n      toggleSecretButtons(id, 'lock');\n    }\n  }\n\n  for (const element of document.querySelectorAll<HTMLButtonElement>('button.unlock-secret')) {\n    element.addEventListener('click', () => unlock(element.getAttribute('secret-id')));\n  }\n  for (const element of document.querySelectorAll<HTMLButtonElement>('button.lock-secret')) {\n    element.addEventListener('click', () => lock(element.getAttribute('secret-id')));\n  }\n}\n\n/**\n * Request a session key from the API.\n * @param privateKey RSA Private Key (valid JSON string)\n */\nfunction requestSessionKey(privateKey: string) {\n  apiPostForm('/api/plugins/secrets/session-keys/', {\n    private_key: privateKey,\n    preserve_key: true,\n  }).then(res => {\n    if (!hasError(res)) {\n      // If the session key has been added from the user key page, reload the page.\n      if (window.location.pathname === '/plugins/secrets/user-key/') {\n        window.location.reload();\n      } else {\n        // If the response received was not an error, show the user a success message.\n        const toast = createToast('success', 'Session Key Received', 'You may now unlock secrets.');\n        toast.show();\n      }\n    } else {\n      // Otherwise, show the user an error message.\n      let message = res.error;\n      if (isApiError(res)) {\n        // If the error received was a standard API error containing a Python exception message,\n        // append it to the error.\n        message += `\\n${res.exception}`;\n      }\n      const toast = createToast('danger', 'Failed to Retrieve Session Key', message);\n      toast.show();\n    }\n  });\n}\n\n/**\n * Initialize Request Session Key Elements.\n */\nfunction initGetSessionKey() {\n  for (const element of document.querySelectorAll<HTMLButtonElement>('#request_session_key')) {\n    /**\n     * Send the user's input private key to the API to get a session key, which will be stored as\n     * a cookie for future requests.\n     */\n    function handleClick() {\n      for (const pk of document.querySelectorAll<HTMLTextAreaElement>('#user_privkey')) {\n        requestSessionKey(pk.value);\n        // Clear the private key form field value.\n        pk.value = '';\n      }\n    }\n    element.addEventListener('click', handleClick);\n  }\n}\n\n/**\n * Initialize Secret Edit Form Handler.\n */\nfunction initSecretsEdit() {\n  const privateKeyModal = new window.Modal('#privkey_modal');\n\n  /**\n   * Check the cookie store for a `netbox_secrets_sessionid`. If not present, prompt the user to submit their\n   * private key.\n   */\n  function handleSubmit(event: Event): void {\n    if (document.cookie.indexOf('netbox_secrets_sessionid') === -1) {\n      event.preventDefault();\n      privateKeyModal.show();\n    }\n  }\n\n  for (const element of document.querySelectorAll<HTMLInputElement>('.requires-session-key')) {\n    const form = element.closest<HTMLFormElement>('form');\n    if (form !== null) {\n      form.addEventListener('submit', handleSubmit);\n    }\n  }\n}\n\nexport function initSecrets() {\n  for (const func of [initGenerateKeyPair, initLockUnlock, initGetSessionKey, initSecretsEdit]) {\n    func();\n  }\n}\n",
         "import { initSecrets } from './secrets';\n\nif (document.readyState !== 'loading') {\n  initSecrets();\n} else {\n  document.addEventListener('DOMContentLoaded', initSecrets);\n}\n"
     ],
     "version": 3
 }
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/template_content.py` & `netbox-secrets-1.8.0/netbox_secrets/template_content.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import logging
 
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db.utils import OperationalError
 from extras.plugins import PluginTemplateExtension
+from netbox.views import generic
+from utilities.views import ViewTab, register_model_view
 
+from .filtersets import SecretFilterSet
 from .models import Secret
+from .tables import SecretTable
 
 logger = logging.getLogger(__name__)
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_secrets')
 template_extensions = []
 
 
 def secrets_panel(self):
@@ -31,24 +35,65 @@
 
     if display_setting := plugin_settings.get('display_setting'):
         display_on = display_setting.get(app_model, display_on)
 
     return display_on
 
 
+def tab_view(_model):
+    class ModelTabView(generic.ObjectChildrenView):
+        queryset = _model.objects.all()
+        child_model = Secret
+        table = SecretTable
+        filterset = SecretFilterSet
+        template_name = 'netbox_secrets/inc/view_tab.html'
+        tab = ViewTab(
+            label='Secrets',
+            badge=lambda obj: obj.secrets.count(),
+            weight=500,
+        )
+
+        def get_children(self, request, parent):
+            return self.child_model.objects.restrict(request.user, 'view').filter(
+                assigned_object_type=ContentType.objects.get_for_model(parent),
+                assigned_object_id=parent.pk,
+            )
+
+    register_model_view(_model, name='secrets')(ModelTabView)
+
+
+def secret_add_button(_app_model):
+    class Button(PluginTemplateExtension):
+        model = _app_model
+
+        def buttons(self):
+            return self.render(
+                'netbox_secrets/inc/secret_add_button.html',
+            )
+
+    return Button
+
+
 # Generate plugin extensions for the defined classes
 try:
     for app_model in plugin_settings.get('apps'):
         app_label, model = app_model.split('.')
         klass_name = f'{app_label}_{model}_plugin_template_extension'
-        dynamic_klass = type(
-            klass_name,
-            (PluginTemplateExtension,),
-            {'model': app_model, get_display_on(app_model): secrets_panel},
-        )
-        template_extensions.append(dynamic_klass)
+
+        display = get_display_on(app_model)
+
+        if display == 'tab_view':
+            template_extensions.append(secret_add_button(app_model))
+            tab_view(ContentType.objects.get(app_label=app_label, model=model).model_class())
+        else:
+            dynamic_klass = type(
+                klass_name,
+                (PluginTemplateExtension,),
+                {'model': app_model, get_display_on(app_model): secrets_panel},
+            )
+            template_extensions.append(dynamic_klass)
 except OperationalError as e:
     # This happens when the database is not yet ready
     logger.warning(f'Database not ready, skipping plugin extensions: {e}')
 except Exception as e:
     # Unexpected error
     raise Exception(f'Unexpected error: {e}')
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html`

 * *Files 7% similar despite different names*

```diff
@@ -28,17 +28,13 @@
                         {% endfor %}
                     </table>
                 {% else %}
                     <div class="text-muted">None</div>
                 {% endif %}
             {% endwith %}
         </div>
-        {% if perms.netbox_secrets.add_secret %}
-            <div class="card-footer text-end noprint">
-                <a class="btn btn-primary btn-sm"
-                   href="{% url 'plugins:netbox_secrets:secret_add' %}?assigned_object_type={{ object|content_type_id }}&assigned_object_id={{ object.pk }}&return_url={{ request.path }}"><i
-                        class="mdi mdi-plus-thick"></i> Add Secret</a>
-            </div>
-        {% endif %}
+        <div class="card-footer text-end noprint">
+            {% include 'netbox_secrets/inc/secret_add_button.html' %}
+        </div>
     </div>
     {% include 'netbox_secrets/inc/private_key_modal.html' %}
 {% endif %}
```

#### html2text {}

```diff
@@ -6,11 +6,9 @@
 {%_if_secret.name_%}{                                 {% include
 {_secret.name_}}{%_else_%} {{_secret.role_}} ******** 'netbox_secrets/inc/
 (Not_Set){%_endif_%}                                  secret_actions.html' with
                                                       object=secret %}
 {% else %}
 None
 {% endif %} {% endwith %}
-{% if perms.netbox_secrets.add_secret %}
- Add_Secret
-{% endif %}
+{% include 'netbox_secrets/inc/secret_add_button.html' %}
 {% include 'netbox_secrets/inc/private_key_modal.html' %} {% endif %}
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/inc/view_tab.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/inc/view_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/secret.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 {% extends 'generic/object.html' %}
 {% load buttons %}
 {% load helpers %}
 {% load static %}
 {% load plugins %}
 
 {% block breadcrumbs %}
-  <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_secrets:secret_list' %}">Secrets</a></li>
-  <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_secrets:secret_list' %}?role_id={{ object.role.pk }}">{{ object.role }}</a></li>
-  <li class="breadcrumb-item"><a href="{{ object.assigned_object.get_absolute_url }}">{{ object.assigned_object }}</a></li>
+  <li class="breadcrumb-item">
+    <a href="{% url 'plugins:netbox_secrets:secret_list' %}">Secrets</a>
+  </li>
+  <li class="breadcrumb-item">
+    <a href="{% url 'plugins:netbox_secrets:secret_list' %}?role_id={{ object.role.pk }}">{{ object.role }}</a>
+  </li>
+  <li class="breadcrumb-item">
+    <a href="{{ object.assigned_object.get_absolute_url }}">{{ object.assigned_object }}</a>
+  </li>
   <li class="breadcrumb-item">{{ object }}</li>
 {% endblock %}
 
 {% block content %}
-<div class="row">
-	<div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">
-                Secret Attributes
-            </h5>
-            <div class="card-body">
-                <table class="table table-hover">
-                    <tr>
-                        <th scope="row">Assigned Object</th>
-                        <td>
-                            <a href="{{ object.assigned_object.get_absolute_url }}">{{ object.assigned_object }}</a>
-                        </td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Role</th>
-                        <td>
-                            <a href="{{ object.role.get_absolute_url }}">{{ object.role }}</a>
-                        </td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Name</th>
-                        <td>{{ object.name|placeholder }}</td>
-                    </tr>
-                </table>
-            </div>
+  <div class="row">
+    <div class="col col-md-6">
+      <div class="card">
+        <h5 class="card-header">
+          Secret Attributes
+        </h5>
+        <div class="card-body">
+          <table class="table table-hover attr-table">
+            <tr>
+              <th scope="row">Assigned Object</th>
+              <td>
+                <a href="{{ object.assigned_object.get_absolute_url }}">{{ object.assigned_object }}</a>
+              </td>
+            </tr>
+            <tr>
+              <th scope="row">Role</th>
+              <td>
+                <a href="{{ object.role.get_absolute_url }}">{{ object.role }}</a>
+              </td>
+            </tr>
+            <tr>
+              <th scope="row">Name</th>
+              <td>{{ object.name|placeholder }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Description</th>
+              <td>{{ object.description|placeholder }}</td>
+            </tr>
+          </table>
         </div>
-        {% include 'inc/panels/custom_fields.html' %}
-        {% plugin_left_page object %}
-	</div>
-	<div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">
-                Secret Data
-            </h5>
-            <div class="card-body">
-                <form id="secret_form">
-                    {% csrf_token %}
-                </form>
-                <div class="row">
-                    <div class="col col-md-2">Secret</div>
-                    <div class="col col-md-6"><code id="secret_{{ object.pk }}">********</code></div>
-                    <div class="col col-md-4 text-end noprint">
-                        {% include 'netbox_secrets/inc/secret_actions.html' %}
-                    </div>
-                </div>
+      </div>
+      {% include 'inc/panels/custom_fields.html' %}
+      {% plugin_left_page object %}
+    </div>
+    <div class="col col-md-6">
+      <div class="card">
+        <h5 class="card-header">
+          Secret Data
+        </h5>
+        <div class="card-body">
+          <form id="secret_form">
+            {% csrf_token %}
+          </form>
+          <div class="row">
+            <div class="col col-md-2">Secret</div>
+            <div class="col col-md-6"><code id="secret_{{ object.pk }}">********</code></div>
+            <div class="col col-md-4 text-end noprint">
+              {% include 'netbox_secrets/inc/secret_actions.html' %}
             </div>
+          </div>
         </div>
-        {% include 'inc/panels/tags.html' %}
-        {% if object.enable_contacts %}
-            {% include 'inc/panels/contacts.html' %}
-        {% endif %}
-        {% plugin_right_page object %}
+      </div>
+      {% include 'inc/panels/tags.html' %}
+      {% include 'inc/panels/comments.html' %}
+      {% if object.enable_contacts %}
+        {% include 'inc/panels/contacts.html' %}
+      {% endif %}
+      {% plugin_right_page object %}
     </div>
-</div>
-<div class="row">
+  </div>
+  <div class="row">
     <div class="col col-md-12">
-        {% plugin_full_width_page object %}
+      {% plugin_full_width_page object %}
     </div>
-</div>
+  </div>
 
-{% include 'netbox_secrets/inc/private_key_modal.html' %}
+  {% include 'netbox_secrets/inc/private_key_modal.html' %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,17 +5,19 @@
 {{_object.assigned_object_}}
 {{ object }}
 {% endblock %} {% block content %}
 ** Secret Attributes **
 Assigned Object {{_object.assigned_object_}}
 Role            {{_object.role_}}
 Name            {{ object.name|placeholder }}
+Description     {{ object.description|placeholder }}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 ** Secret Data **
 {% csrf_token %}
 Secret
 ********
 {% include 'netbox_secrets/inc/secret_actions.html' %}
-{% include 'inc/panels/tags.html' %} {% if object.enable_contacts %} {% include
-'inc/panels/contacts.html' %} {% endif %} {% plugin_right_page object %}
+{% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% if object.enable_contacts %} {% include 'inc/panels/contacts.html' %} {%
+endif %} {% plugin_right_page object %}
 {% plugin_full_width_page object %}
 {% include 'netbox_secrets/inc/private_key_modal.html' %} {% endblock %}
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secret_edit.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/secret_edit.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 {% extends 'generic/object_edit.html' %}
 {% load static %}
 {% load form_helpers %}
 {% load helpers %}
+
 {% block form %}
     <div class="field-group-mb-5">
         <div class="row mb-3">
             <label class="col-sm-3 col-form-label text-lg-end required">
                 {{ object.assigned_object|meta:"verbose_name"|bettertitle }}</label>
             <div class="col-sm-9">
                 <div class="form-control-plaintext">{{ object.assigned_object|linkify }}</div>
             </div>
         </div>
-        {% render_form form %}
+        {{ block.super }}
     </div>
     {% include 'netbox_secrets/inc/private_key_modal.html' %}
 {% endblock form %}
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/secretrole.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/secretrole.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load plugins %}
 
 {% block breadcrumbs %}
-  <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_secrets:secretrole_list' %}">Secret Roles</a></li>
-  <li class="breadcrumb-item">{{ object }}</li>
+    <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_secrets:secretrole_list' %}">Secret Roles</a></li>
+    <li class="breadcrumb-item">{{ object }}</li>
 {% endblock %}
 
 {% block content %}
-  <div class="row mb-3">
-      <div class="col col-md-6">
-      <div class="card">
-        <h5 class="card-header">
-          Secret Role
-        </h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Secrets</th>
-              <td>
-                <a href="{% url 'plugins:netbox_secrets:secret_list' %}?role_id={{ object.pk }}">{{ object.secrets.count }}</a>
-              </td>
-            </tr>
-          </table>
+    <div class="row mb-3">
+        <div class="col col-md-6">
+            <div class="card">
+                <h5 class="card-header">
+                    Secret Role
+                </h5>
+                <div class="card-body">
+                    <table class="table table-hover attr-table">
+                        <tr>
+                            <th scope="row">Name</th>
+                            <td>{{ object.name }}</td>
+                        </tr>
+                        <tr>
+                            <th scope="row">Description</th>
+                            <td>{{ object.description|placeholder }}</td>
+                        </tr>
+                        <tr>
+                            <th scope="row">Secrets</th>
+                            <td>
+                                <a href="{% url 'plugins:netbox_secrets:secret_list' %}?role_id={{ object.pk }}">{{ object.secrets.count }}</a>
+                            </td>
+                        </tr>
+                        <tr>
+                            <th scope="row">Description</th>
+                            <td>{{ object.description|placeholder }}</td>
+                        </tr>
+                    </table>
+                </div>
+            </div>
+            {% plugin_left_page object %}
+        </div>
+        <div class="col col-md-6">
+            {% include 'inc/panels/tags.html' %}
+            {% include 'inc/panels/custom_fields.html' %}
+            {% include 'inc/panels/comments.html' %}
+            {% plugin_right_page object %}
         </div>
-      </div>
-      {% plugin_left_page object %}
-      </div>
-      <div class="col col-md-6">
-      {% include 'inc/panels/custom_fields.html' %}
-      {% plugin_right_page object %}
     </div>
-  </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,10 +3,12 @@
 Secret_Roles
 {{ object }}
 {% endblock %} {% block content %}
 ** Secret Role **
 Name        {{ object.name }}
 Description {{ object.description|placeholder }}
 Secrets     {{_object.secrets.count_}}
+Description {{ object.description|placeholder }}
 {% plugin_left_page object %}
-{% include 'inc/panels/custom_fields.html' %} {% plugin_right_page object %}
+{% include 'inc/panels/tags.html' %} {% include 'inc/panels/custom_fields.html'
+%} {% include 'inc/panels/comments.html' %} {% plugin_right_page object %}
 {% endblock %}
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/userkey.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/templates/netbox_secrets/userkey_edit.html` & `netbox-secrets-1.8.0/netbox_secrets/templates/netbox_secrets/userkey_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/tests/constants.py` & `netbox-secrets-1.8.0/netbox_secrets/tests/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 d453d1eY95xYVbFrIHs7yJy8lcDR2criwGEI68VP1FwcOkkwhicjtQZQS5fkkBIb
 RjA2wmt2PVT26YbOX2qCMItV1+meo/Ogh+uI1oNePJ8VYuGXbGNggf1qMY8fGhhh
 GY2b4PKuSTcsYjbg8adOGzFL9RXLI1X4PHNCzD/Y1vdM3jJXv+luk3TU+JIbzJeN
 5ZEEz+sIdlMPCAACaZAY/t9Kd/LxHr0o4K/6gqkZIukxFCK6sN53gibAXfaKc4xl
 qQIDAQAB
 -----END PUBLIC KEY-----"""
 
-SSH_PUBLIC_KEY = """ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCy2yMGnuvmM5CnFG8CsohfUYobXU7+pz/RJtvUUnARAY11Ybc3cn0tvzn4aPxclX8+514n6R7jJCZuVGJXXapqZDq2l+PLmgLhyBJxE9qq7rbp4EAJiUP0inDyf8qFzSKT7Rm8cjHvY3v2GI32JUXuWACA23t5YPUqVglkjfdVX8VHJh6fMQrQ4O3CKKh2x0S82UHH7SaYH0HqOknPgyRQ+ZQorUU25IpzJPesk29nN3DYqfY+VQsKJOLglWvoapaZiu+wK/7ovXqYXNuhfAwlkjbCRKjwix1kZjtDS44US1//BCaT7AeuwMpFLI44v/VajoxTfE0h74Mxl48mNt7Qme4lbXxH8yMa6HNfDp4vjnxPE1CWuSrFo4G+HI1rc22qSmw9e67qIGRbcI7/cIFpeBvnfCCgWrqWZ6ZzdAZJCnu7/aWn00+VG+54GFmJ+3R2xhWcu+Uzn+o1aWROtUuzq0qR6zdXME3A0Oud2uQrQAiAGFdWpfvcOEbD+tlPNDk= test"""
+SSH_PUBLIC_KEY = """ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCy2yMGnuvmM5CnFG8CsohfUYobXU7+pz/RJtvUUnARAY11Ybc3cn0tvzn4aPxclX8+514n6R7jJCZuVGJXXapqZDq2l+PLmgLhyBJxE9qq7rbp4EAJiUP0inDyf8qFzSKT7Rm8cjHvY3v2GI32JUXuWACA23t5YPUqVglkjfdVX8VHJh6fMQrQ4O3CKKh2x0S82UHH7SaYH0HqOknPgyRQ+ZQorUU25IpzJPesk29nN3DYqfY+VQsKJOLglWvoapaZiu+wK/7ovXqYXNuhfAwlkjbCRKjwix1kZjtDS44US1//BCaT7AeuwMpFLI44v/VajoxTfE0h74Mxl48mNt7Qme4lbXxH8yMa6HNfDp4vjnxPE1CWuSrFo4G+HI1rc22qSmw9e67qIGRbcI7/cIFpeBvnfCCgWrqWZ6ZzdAZJCnu7/aWn00+VG+54GFmJ+3R2xhWcu+Uzn+o1aWROtUuzq0qR6zdXME3A0Oud2uQrQAiAGFdWpfvcOEbD+tlPNDk= test"""  # noqa
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/tests/test_filters.py` & `netbox-secrets-1.8.0/netbox_secrets/tests/test_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def test_id(self):
         params = {'id': self.queryset.values_list('pk', flat=True)[:2]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_name(self):
         name = Secret.objects.all()
-        params = {'name': [name[0].pk, name[1].pk, name[2].pk, name[3].pk, name[4].pk, name[5].pk]}
+        params = {'name': [name[0].name, name[1].name, name[2].name, name[3].name, name[4].name, name[5].name]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 6)
 
     def test_role(self):
         roles = SecretRole.objects.all()[:2]
         params = {'role_id': [roles[0].pk, roles[1].pk]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 4)
         params = {'role': [roles[0].slug, roles[1].slug]}
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/tests/test_form.py` & `netbox-secrets-1.8.0/netbox_secrets/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/tests/test_models.py` & `netbox-secrets-1.8.0/netbox_secrets/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def test_05_invalid_private_key(self):
         """
         Ensure that an exception is raised when attempting to retrieve a secret key using an invalid private key.
         """
         secret_key = generate_random_key()
         secret_key_cipher = encrypt_master_key(secret_key, self.TEST_KEYS['alice_public'])
         try:
-            decrypted_secret_key = decrypt_master_key(secret_key_cipher, self.TEST_KEYS['bob_private'])
+            decrypt_master_key(secret_key_cipher, self.TEST_KEYS['bob_private'])
             self.fail("Decrypting secret key from Alice's UserKey using Bob's private key did not fail")
         except ValueError:
             pass
 
 
 class SecretTestCase(TestCase):
     @classmethod
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/tests/test_views.py` & `netbox-secrets-1.8.0/netbox_secrets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/urls.py` & `netbox-secrets-1.8.0/netbox_secrets/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,14 @@
     path('secret-roles/edit/', views.SecretRoleBulkEditView.as_view(), name='secretrole_bulk_edit'),
     path('secret-roles/delete/', views.SecretRoleBulkDeleteView.as_view(), name='secretrole_bulk_delete'),
     path('secret-roles/<int:pk>/', include(get_model_urls('netbox_secrets', 'secretrole'))),
     # Secrets
     path('secrets/', views.SecretListView.as_view(), name='secret_list'),
     path('secrets/add/', views.SecretEditView.as_view(), name='secret_add'),
     path('secrets/delete/', views.SecretBulkDeleteView.as_view(), name='secret_bulk_delete'),
+    path('secrets/edit/', views.SecretBulkEditView.as_view(), name='secret_bulk_edit'),
     path('secrets/<int:pk>/', include(get_model_urls('netbox_secrets', 'secret'))),
     # User
     path('user-key/', views.UserKeyView.as_view(), name='userkey'),
     path('user-key/edit/', views.UserKeyEditView.as_view(), name='userkey_edit'),
     path('session-key/delete/', views.SessionKeyDeleteView.as_view(), name='sessionkey_delete'),
 ]
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets/utils/crypto.py` & `netbox-secrets-1.8.0/netbox_secrets/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.7.6/netbox_secrets/views.py` & `netbox-secrets-1.8.0/netbox_secrets/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 from django.views.generic.base import View
 from extras.signals import clear_webhooks
 from netbox.views import generic
 from utilities.exceptions import AbortRequest, PermissionsViolation
-from utilities.forms import ConfirmationForm, restrict_form_fields
+from utilities.forms import restrict_form_fields
 from utilities.utils import count_related, prepare_cloned_fields
 from utilities.views import GetReturnURLMixin, ViewTab, register_model_view
 
-from . import exceptions, filtersets, forms, models, tables, utils
+from . import constants, exceptions, filtersets, forms, models, tables, utils
 
 #
 # Mixins
 #
 
 
 class ObjectChildrenViewMixin(generic.ObjectChildrenView):
@@ -265,14 +265,21 @@
 
 
 @register_model_view(models.Secret, 'delete')
 class SecretDeleteView(generic.ObjectDeleteView):
     queryset = models.Secret.objects.prefetch_related('role', 'tags')
 
 
+class SecretBulkEditView(generic.BulkEditView):
+    queryset = models.Secret.objects.prefetch_related('role', 'tags')
+    filterset = filtersets.SecretFilterSet
+    table = tables.SecretTable
+    form = forms.SecretBulkEditForm
+
+
 class SecretBulkDeleteView(generic.BulkDeleteView):
     queryset = models.Secret.objects.prefetch_related('role', 'tags')
     filterset = filtersets.SecretFilterSet
     table = tables.SecretTable
 
 
 class UserKeyView(LoginRequiredMixin, View):
@@ -342,7 +349,13 @@
 
 @register_model_view(models.SessionKey, 'delete')
 class SessionKeyDeleteView(generic.ObjectDeleteView):
     queryset = models.SessionKey.objects.all()
 
     def get_queryset(self, request):
         return super().get_queryset(request).filter(userkey__user=request.user)
+
+    def post(self, request, *args, **kwargs):
+        response = super().post(request, *args, **kwargs)
+        # Delete the cookie
+        response.delete_cookie(constants.SESSION_COOKIE_NAME)
+        return response
```

### Comparing `netbox-secrets-1.7.6/netbox_secrets.egg-info/SOURCES.txt` & `netbox-secrets-1.8.0/netbox_secrets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,37 +23,42 @@
 netbox_secrets.egg-info/top_level.txt
 netbox_secrets/api/__init__.py
 netbox_secrets/api/nested_serializers.py
 netbox_secrets/api/serializers.py
 netbox_secrets/api/urls.py
 netbox_secrets/api/views.py
 netbox_secrets/forms/__init__.py
-netbox_secrets/forms/secrets.py
+netbox_secrets/forms/bulk_edit.py
+netbox_secrets/forms/bulk_import.py
+netbox_secrets/forms/filterset.py
+netbox_secrets/forms/model_forms.py
 netbox_secrets/graphql/__init__.py
 netbox_secrets/graphql/schema.py
 netbox_secrets/graphql/types.py
 netbox_secrets/migrations/0001_initial.py
 netbox_secrets/migrations/0002_populate_userkeys.py
 netbox_secrets/migrations/0003_populate_secretroles.py
 netbox_secrets/migrations/0004_populate_secrets.py
 netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
 netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
+netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
 netbox_secrets/migrations/__init__.py
 netbox_secrets/models/__init__.py
 netbox_secrets/models/secrets.py
 netbox_secrets/static/netbox_secrets/secrets.js
 netbox_secrets/static/netbox_secrets/secrets.js.map
 netbox_secrets/templates/netbox_secrets/activate_keys.html
 netbox_secrets/templates/netbox_secrets/secret.html
 netbox_secrets/templates/netbox_secrets/secret_edit.html
 netbox_secrets/templates/netbox_secrets/secretrole.html
 netbox_secrets/templates/netbox_secrets/userkey.html
 netbox_secrets/templates/netbox_secrets/userkey_edit.html
 netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
 netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
+netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
 netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
 netbox_secrets/templates/netbox_secrets/inc/view_tab.html
 netbox_secrets/tests/__init__.py
 netbox_secrets/tests/constants.py
 netbox_secrets/tests/test_api.py
 netbox_secrets/tests/test_filters.py
 netbox_secrets/tests/test_form.py
```

### Comparing `netbox-secrets-1.7.6/setup.py` & `netbox-secrets-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-secrets',
-    version='1.7.6',
+    version='1.8.0',
     description='Netbox Secrets',
     long_description='A Secret store for NetBox',
     url='https://github.com/Onemind-Services-LLC/netbox-secrets/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     license='Apache 2.0',
     install_requires=[
```

