# Comparing `tmp/django-pfx-1.2.dev6.tar.gz` & `tmp/django-pfx-1.2.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pfx-1.2.dev6.tar", last modified: Thu Mar  2 15:31:57 2023, max compression
+gzip compressed data, was "django-pfx-1.2.dev8.tar", last modified: Thu Mar 30 14:30:10 2023, max compression
```

## Comparing `django-pfx-1.2.dev6.tar` & `django-pfx-1.2.dev8.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.260315 django-pfx-1.2.dev6/
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1691 2023-03-02 15:31:57.261315 django-pfx-1.2.dev6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.239313 django-pfx-1.2.dev6/django_pfx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1691 2023-03-02 15:31:57.000000 django-pfx-1.2.dev6/django_pfx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2259 2023-03-02 15:31:57.000000 django-pfx-1.2.dev6/django_pfx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 15:31:57.000000 django-pfx-1.2.dev6/django_pfx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-02 15:31:57.000000 django-pfx-1.2.dev6/django_pfx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-02 15:31:57.000000 django-pfx-1.2.dev6/django_pfx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.239313 django-pfx-1.2.dev6/img/
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/img/pfx.png
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/img/pfx.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.240313 django-pfx-1.2.dev6/pfx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.242313 django-pfx-1.2.dev6/pfx/pfxcore/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.243313 django-pfx-1.2.dev6/pfx/pfxcore/decorator/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1824 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/decorator/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.243313 django-pfx-1.2.dev6/pfx/pfxcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/http/json_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.230312 django-pfx-1.2.dev6/pfx/pfxcore/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.230312 django-pfx-1.2.dev6/pfx/pfxcore/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.244313 django-pfx-1.2.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3331 2023-03-02 15:31:51.000000 django-pfx-1.2.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     5332 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.245313 django-pfx-1.2.dev6/pfx/pfxcore/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2995 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/middleware/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/middleware/locale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.247313 django-pfx-1.2.dev6/pfx/pfxcore/models/
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/models/cache_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/models/not_null_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2793 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/models/pfx_models.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/models/user_filtered_queryset_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.248314 django-pfx-1.2.dev6/pfx/pfxcore/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/serializers/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2761 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.248314 django-pfx-1.2.dev6/pfx/pfxcore/storage/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/storage/s3_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.232312 django-pfx-1.2.dev6/pfx/pfxcore/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.250314 django-pfx-1.2.dev6/pfx/pfxcore/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/templates/registration/welcome_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/templates/registration/welcome_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)     9373 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/test.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.252314 django-pfx-1.2.dev6/pfx/pfxcore/views/
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10536 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/views/authentication_views.py
--rw-rw-rw-   0 root         (0) root         (0)     9169 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/views/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/views/filters_views.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/views/locale_views.py
--rw-rw-rw-   0 root         (0) root         (0)    16585 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pfx/pfxcore/views/rest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      440 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/runtest.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-03-02 15:31:57.261315 django-pfx-1.2.dev6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.253314 django-pfx-1.2.dev6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6123 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.255314 django-pfx-1.2.dev6/tests/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/settings/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/settings/dev.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/settings/dev_custom_example.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/settings/dev_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 15:31:57.260315 django-pfx-1.2.dev6/tests/tests/
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/basic_api_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    40170 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/basic_api_test.py
--rw-rw-rw-   0 root         (0) root         (0)    24088 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     9813 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_locale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_perm_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_perms_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_timezone_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     2990 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_user_queryset.py
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/tests/test_view_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6443 2023-03-02 15:31:02.000000 django-pfx-1.2.dev6/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.246585 django-pfx-1.2.dev8/
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-03-30 14:30:10.246585 django-pfx-1.2.dev8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.223583 django-pfx-1.2.dev8/django_pfx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-03-30 14:30:10.000000 django-pfx-1.2.dev8/django_pfx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.224583 django-pfx-1.2.dev8/img/
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/img/pfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/img/pfx.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.224583 django-pfx-1.2.dev8/pfx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.227583 django-pfx-1.2.dev8/pfx/pfxcore/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.228583 django-pfx-1.2.dev8/pfx/pfxcore/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/decorator/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.228583 django-pfx-1.2.dev8/pfx/pfxcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/http/json_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.214582 django-pfx-1.2.dev8/pfx/pfxcore/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.214582 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.229583 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-03-30 14:30:03.000000 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5332 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.230583 django-pfx-1.2.dev8/pfx/pfxcore/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/middleware/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/middleware/locale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.232584 django-pfx-1.2.dev8/pfx/pfxcore/models/
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/cache_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/not_null_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2793 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/pfx_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/models/user_filtered_queryset_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.233584 django-pfx-1.2.dev8/pfx/pfxcore/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/serializers/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2761 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.233584 django-pfx-1.2.dev8/pfx/pfxcore/storage/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/storage/s3_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.216582 django-pfx-1.2.dev8/pfx/pfxcore/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.235584 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/welcome_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/templates/registration/welcome_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)     9419 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.237584 django-pfx-1.2.dev8/pfx/pfxcore/views/
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10536 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/authentication_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     9169 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/filters_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/locale_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    16585 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pfx/pfxcore/views/rest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      440 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/runtest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-03-30 14:30:10.247585 django-pfx-1.2.dev8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.238584 django-pfx-1.2.dev8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6123 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.241585 django-pfx-1.2.dev8/tests/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/dev_custom_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/settings/dev_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:30:10.246585 django-pfx-1.2.dev8/tests/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/basic_api_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    40170 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/basic_api_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    26641 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9813 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_locale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_perm_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_perms_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_timezone_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_user_queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/tests/test_view_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6443 2023-03-30 14:29:14.000000 django-pfx-1.2.dev8/tests/views.py
```

### Comparing `django-pfx-1.2.dev6/.gitlab-ci.yml` & `django-pfx-1.2.dev8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/LICENSE` & `django-pfx-1.2.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/PKG-INFO` & `django-pfx-1.2.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev6
+Version: 1.2.dev8
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev6/README.md` & `django-pfx-1.2.dev8/README.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/django_pfx.egg-info/PKG-INFO` & `django-pfx-1.2.dev8/django_pfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev6
+Version: 1.2.dev8
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev6/django_pfx.egg-info/SOURCES.txt` & `django-pfx-1.2.dev8/django_pfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/img/pfx.png` & `django-pfx-1.2.dev8/img/pfx.png`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/img/pfx.svg` & `django-pfx-1.2.dev8/img/pfx.svg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/decorator/rest.py` & `django-pfx-1.2.dev8/pfx/pfxcore/decorator/rest.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/exceptions.py` & `django-pfx-1.2.dev8/pfx/pfxcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/fields.py` & `django-pfx-1.2.dev8/pfx/pfxcore/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo` & `django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.2.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/middleware/authentication.py` & `django-pfx-1.2.dev8/pfx/pfxcore/middleware/authentication.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AnonymousUser
 from django.utils.deprecation import MiddlewareMixin
-from django.utils.translation import gettext_lazy as _
 
 import jwt
 from jwt import DecodeError
 
-from pfx.pfxcore.exceptions import APIError, AuthenticationError
 from pfx.pfxcore.models import CacheableMixin
+from pfx.pfxcore.shortcuts import delete_token_cookie
 
 logger = logging.getLogger(__name__)
 
 
 class JWTTokenDecodeMixin:
 
     @classmethod
@@ -37,40 +36,38 @@
                     else {})
             decoded = jwt.decode(
                 token, settings.PFX_SECRET_KEY,
                 options=opts,
                 algorithms="HS256")
             return cls.get_cached_user(decoded['pfx_user_pk'])
         except get_user_model().DoesNotExist:
-            raise AuthenticationError(
-                message=_('Authentication error'), delete_cookie=True)
+            raise
         except DecodeError as e:
             logger.exception(e)
-            raise AuthenticationError(message=_('Authentication error'))
+            raise
         except jwt.ExpiredSignatureError:
-            raise AuthenticationError(message=_('Token has expired'))
+            raise
         except Exception as e:  # pragma: no cover
             logger.exception(e)
-            raise AuthenticationError(message=_('Authentication error'),
-                                      status=500)
+            raise
 
 
 class AuthenticationMiddleware(JWTTokenDecodeMixin, MiddlewareMixin):
 
     def process_request(self, request):
         authorization = request.headers.get('Authorization')
         if authorization:
             try:
                 _, key = authorization.split("Bearer ")
             except ValueError:
                 key = None
             try:
                 request.user = self.decode_jwt(key)
-            except APIError as e:
-                return e.response
+            except Exception:
+                request.user = AnonymousUser()
         else:
             if not hasattr(request, 'user'):
                 request.user = AnonymousUser()
 
     def process_response(self, request, response):
         return response
 
@@ -78,15 +75,18 @@
 class CookieAuthenticationMiddleware(JWTTokenDecodeMixin, MiddlewareMixin):
 
     def process_request(self, request):
         key = request.COOKIES.get('token')
         if key:
             try:
                 request.user = self.decode_jwt(key)
-            except APIError as e:
-                return e.response
+            except Exception:
+                request.user = AnonymousUser()
+                request.delete_cookie = True
         else:
             if not hasattr(request, 'user'):
                 request.user = AnonymousUser()
 
     def process_response(self, request, response):
+        if getattr(request, 'delete_cookie', False):
+            return delete_token_cookie(response)
         return response
```

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/middleware/locale.py` & `django-pfx-1.2.dev8/pfx/pfxcore/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/models/cache_mixins.py` & `django-pfx-1.2.dev8/pfx/pfxcore/models/cache_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/models/pfx_models.py` & `django-pfx-1.2.dev8/pfx/pfxcore/models/pfx_models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/shortcuts.py` & `django-pfx-1.2.dev8/pfx/pfxcore/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/storage/s3_storage.py` & `django-pfx-1.2.dev8/pfx/pfxcore/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/test.py` & `django-pfx-1.2.dev8/pfx/pfxcore/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,20 @@
         res.append("Streaming content")
     else:
         res.append("Response is empty")
     res.append("*******************************************************")
     return '\n'.join(res)
 
 
+def get_auth_cookie(response):
+    return [
+        v for k, v in response.client.cookies.items()
+        if k == 'token'][0]
+
+
 class APIClient(DjangoClient):
 
     token = None
     default_locale = None
     auth_cookie = None
 
     def __init__(self, enforce_csrf_checks=False, raise_request_exception=True,
@@ -49,17 +55,15 @@
         self.token = None
         response = self.post(
             f"{path}{self.with_cookie and '?mode=cookie' or ''}", {
                 'username': username,
                 'password': password}, locale=locale)
         if response.status_code == 200:
             if self.with_cookie:
-                self.auth_cookie = [
-                    v for k, v in response.client.cookies.items()
-                    if k == 'token'][0]
+                self.auth_cookie = get_auth_cookie(response)
                 regex = r".*token=([\w\._-]*);.*"
                 self.token = re.findall(regex, str(self.auth_cookie))[0]
             else:
                 self.token = response.json_content['token']
             return True
         return False
```

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/views/__init__.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/views/authentication_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/authentication_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/views/fields.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/views/filters_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/filters_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/views/locale_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/locale_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/pfx/pfxcore/views/rest_views.py` & `django-pfx-1.2.dev8/pfx/pfxcore/views/rest_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/setup.cfg` & `django-pfx-1.2.dev8/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/models.py` & `django-pfx-1.2.dev8/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/settings/common.py` & `django-pfx-1.2.dev8/tests/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/settings/dev_custom_example.py` & `django-pfx-1.2.dev8/tests/settings/dev_custom_example.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/__init__.py` & `django-pfx-1.2.dev8/tests/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/basic_api_errors.py` & `django-pfx-1.2.dev8/tests/tests/basic_api_errors.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/basic_api_test.py` & `django-pfx-1.2.dev8/tests/tests/basic_api_test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_auth_api.py` & `django-pfx-1.2.dev8/tests/tests/test_auth_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.core import mail
 from django.test import TransactionTestCase, modify_settings, override_settings
 from django.utils.encoding import force_bytes
 from django.utils.http import urlsafe_base64_encode
 
 import jwt
 
-from pfx.pfxcore.test import APIClient, TestAssertMixin
+from pfx.pfxcore.test import APIClient, TestAssertMixin, get_auth_cookie
 from tests.models import User
 
 logger = logging.getLogger(__name__)
 
 
 class AuthAPITest(TestAssertMixin, TransactionTestCase):
 
@@ -209,15 +209,15 @@
 
     @override_settings(PFX_TOKEN_VALIDITY={'minutes': 30})
     def test_valid_token_with_expiration(self):
         self.client.login(
             username='jrr.tolkien',
             password='RIGHT PASSWORD')
         response = self.client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 200)
 
     @override_settings(PFX_TOKEN_VALIDITY={'minutes': 30})
     def test_valid_cookie_token_with_expiration(self):
         self.cookie_client.login(
             username='jrr.tolkien',
             password='RIGHT PASSWORD')
@@ -232,15 +232,15 @@
         # cookie expires in 30 minutes +/- 5 minutes.
         self.assertTrue(
             datetime.utcnow() + timedelta(minutes=25) <
             d < datetime.utcnow() + timedelta(minutes=35))
         self.assertEqual(int(max_age), 1800)
 
         response = self.cookie_client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 200)
 
     @override_settings(
         PFX_TOKEN_VALIDITY={'minutes': 30}, PFX_COOKIE_DOMAIN='example.com')
     def test_valid_cookie_token_with_domain(self):
         self.cookie_client.login(
             username='jrr.tolkien',
@@ -255,15 +255,15 @@
         self.assertEqual(secure, "Secure")  # default value
 
         regex = r".*SameSite=([^;]*).*"
         samesite = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
         self.assertEqual(samesite, "None")  # default value
 
         response = self.cookie_client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 200)
 
     @override_settings(
         PFX_COOKIE_DOMAIN='example.com', PFX_COOKIE_SECURE=False,
         PFX_COOKIE_SAMESITE='Lax')
     def test_valid_cookie_token_with_domain_same_site_insecure(self):
         self.cookie_client.login(
@@ -279,25 +279,25 @@
             len(re.findall(regex, str(self.cookie_client.auth_cookie))), 0)
 
         regex = r".*SameSite=([^;]*).*"
         samesite = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
         self.assertEqual(samesite, "Lax")
 
         response = self.cookie_client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 200)
 
     @override_settings(PFX_TOKEN_VALIDITY={'minutes': -30})
     def test_expired_token(self):
         self.client.login(
             username='jrr.tolkien',
             password='RIGHT PASSWORD')
 
         response = self.client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 401)
 
     @override_settings(PFX_TOKEN_VALIDITY={'minutes': -30})
     def test_expired_cookie_token(self):
         self.cookie_client.login(
             username='jrr.tolkien',
             password='RIGHT PASSWORD')
@@ -310,23 +310,26 @@
         max_age = re.findall(regex, str(self.cookie_client.auth_cookie))[0]
 
         # cookie expires now +/- 5 minutes.
         self.assertTrue(
             datetime.utcnow() - timedelta(minutes=5) <
             d < datetime.utcnow() + timedelta(minutes=5))
         self.assertEqual(int(max_age), 0)
-
         response = self.cookie_client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 401)
+        self.assertEqual(
+            str(get_auth_cookie(response)),
+            'Set-Cookie: token=""; expires=Thu, 01 Jan 1970 00:00:00 GMT; '
+            'Max-Age=0; Path=/; SameSite=None; Secure')
 
     def test_invalid_auth_header(self):
         logging.disable(logging.CRITICAL)
         response = self.client.get(
-            '/api/books',
+            '/api/private/authors',
             HTTP_AUTHORIZATION='Beer here',
             content_type='application/json')
         logging.disable(logging.NOTSET)
         self.assertRC(response, 401)
 
     def test_valid_token_with_invalid_user(self):
         user = User.objects.create_user(
@@ -337,15 +340,15 @@
             last_name='Invisible',
         )
         self.client.login(
             username='invisible.man',
             password='RIGHT PASSWORD')
         user.delete()
         response = self.client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 401)
 
     def test_valid_cookie_with_invalid_user(self):
         user = User.objects.create_user(
             username='invisible.man',
             email="iv@invisible.com",
             password='RIGHT PASSWORD',
@@ -353,38 +356,92 @@
             last_name='Invisible',
         )
         self.cookie_client.login(
             username='invisible.man',
             password='RIGHT PASSWORD')
         user.delete()
         response = self.cookie_client.get(
-            '/api/books')
+            '/api/private/authors')
         self.assertRC(response, 401)
+        self.assertEqual(
+            str(get_auth_cookie(response)),
+            'Set-Cookie: token=""; expires=Thu, 01 Jan 1970 00:00:00 GMT; '
+            'Max-Age=0; Path=/; SameSite=None; Secure')
+
+    def test_valid_cookie_with_invalid_user_and_public_service(self):
+        user = User.objects.create_user(
+            username='invisible.man',
+            email="iv@invisible.com",
+            password='RIGHT PASSWORD',
+            first_name='Peter',
+            last_name='Invisible',
+        )
+        self.cookie_client.login(
+            username='invisible.man',
+            password='RIGHT PASSWORD')
+        user.delete()
+        response = self.cookie_client.get(
+            '/api/books')
+        self.assertRC(response, 200)
+        self.assertEqual(
+            str(get_auth_cookie(response)),
+            'Set-Cookie: token=""; expires=Thu, 01 Jan 1970 00:00:00 GMT; '
+            'Max-Age=0; Path=/; SameSite=None; Secure')
 
     def test_invalid_token(self):
         token = jwt.encode(
             {'pfx_user_pk': 1}, "A WRONG SECRET", algorithm="HS256")
         logging.disable(logging.CRITICAL)
         response = self.client.get(
-            '/api/books',
+            '/api/private/authors',
             HTTP_AUTHORIZATION='Bearer ' + token,
             content_type='application/json')
         logging.disable(logging.NOTSET)
         self.assertRC(response, 401)
 
+    def test_invalid_token_with_public_service(self):
+        token = jwt.encode(
+            {'pfx_user_pk': 1}, "A WRONG SECRET", algorithm="HS256")
+        logging.disable(logging.CRITICAL)
+        response = self.client.get(
+            '/api/books',
+            HTTP_AUTHORIZATION='Bearer ' + token,
+            content_type='application/json')
+        logging.disable(logging.NOTSET)
+        self.assertRC(response, 200)
+
     def test_invalid_cookie_token(self):
         token = jwt.encode(
             {'pfx_user_pk': 1}, "A WRONG SECRET", algorithm="HS256")
         logging.disable(logging.CRITICAL)
         self.client.cookies = SimpleCookie({'token': token})
         response = self.client.get(
-            '/api/books',
+            '/api/private/authors',
             content_type='application/json')
         logging.disable(logging.NOTSET)
         self.assertRC(response, 401)
+        self.assertEqual(
+            str(get_auth_cookie(response)),
+            'Set-Cookie: token=""; expires=Thu, 01 Jan 1970 00:00:00 GMT; '
+            'Max-Age=0; Path=/; SameSite=None; Secure')
+
+    def test_invalid_cookie_token_with_public_service(self):
+        token = jwt.encode(
+            {'pfx_user_pk': 1}, "A WRONG SECRET", algorithm="HS256")
+        logging.disable(logging.CRITICAL)
+        self.client.cookies = SimpleCookie({'token': token})
+        response = self.client.get(
+            '/api/books',
+            content_type='application/json')
+        logging.disable(logging.NOTSET)
+        self.assertRC(response, 200)
+        self.assertEqual(
+            str(get_auth_cookie(response)),
+            'Set-Cookie: token=""; expires=Thu, 01 Jan 1970 00:00:00 GMT; '
+            'Max-Age=0; Path=/; SameSite=None; Secure')
 
     def test_signup(self):
         # Try to create with an existing username
         response = self.client.post(
             '/api/auth/signup', {
                 'username': 'jrr.tolkien',
                 'email': "jrr.tolkien@oxford.com",
```

### Comparing `django-pfx-1.2.dev6/tests/tests/test_cache.py` & `django-pfx-1.2.dev8/tests/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_fields.py` & `django-pfx-1.2.dev8/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_filters.py` & `django-pfx-1.2.dev8/tests/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_locale_api.py` & `django-pfx-1.2.dev8/tests/tests/test_locale_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_perm_tests.py` & `django-pfx-1.2.dev8/tests/tests/test_perm_tests.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_perms_api.py` & `django-pfx-1.2.dev8/tests/tests/test_perms_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_shortcuts.py` & `django-pfx-1.2.dev8/tests/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_timezone_middleware.py` & `django-pfx-1.2.dev8/tests/tests/test_timezone_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_tools.py` & `django-pfx-1.2.dev8/tests/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_user_queryset.py` & `django-pfx-1.2.dev8/tests/tests/test_user_queryset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/tests/test_view_fields.py` & `django-pfx-1.2.dev8/tests/tests/test_view_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/urls.py` & `django-pfx-1.2.dev8/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev6/tests/views.py` & `django-pfx-1.2.dev8/tests/views.py`

 * *Files identical despite different names*

