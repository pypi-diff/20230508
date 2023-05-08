# Comparing `tmp/django-afip-8.0.4.tar.gz` & `tmp/django-afip-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-afip-8.0.4.tar", last modified: Wed Apr  7 10:12:34 2021, max compression
+gzip compressed data, was "django-afip-9.0.0.tar", last modified: Sat Oct 16 16:29:52 2021, max compression
```

## Comparing `django-afip-8.0.4.tar` & `django-afip-9.0.0.tar`

### file list

```diff
@@ -1,135 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (116)       81 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/.kodiak.toml
--rw-r--r--   0 runner    (1001) docker     (116)      655 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      631 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (116)      705 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/no-response.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      795 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/workflows/checks.yml
--rw-r--r--   0 runner    (1001) docker     (116)      309 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1145 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1558 2021-04-07 10:12:29.000000 django-afip-8.0.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)      196 2021-04-07 10:12:29.000000 django-afip-8.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      723 2021-04-07 10:12:29.000000 django-afip-8.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       87 2021-04-07 10:12:29.000000 django-afip-8.0.4/.pypirc
--rw-r--r--   0 runner    (1001) docker     (116)    13771 2021-04-07 10:12:29.000000 django-afip-8.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)      762 2021-04-07 10:12:29.000000 django-afip-8.0.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (116)     3657 2021-04-07 10:12:34.000000 django-afip-8.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2076 2021-04-07 10:12:29.000000 django-afip-8.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-04-07 10:12:29.000000 django-afip-8.0.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13263 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/admin.py
--rw-r--r--   0 runner    (1001) docker     (116)      297 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)     3103 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/clients.py
--rw-r--r--   0 runner    (1001) docker     (116)     2073 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/crypto.py
--rw-r--r--   0 runner    (1001) docker     (116)     1405 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5297 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/fixtures/
--rw-r--r--   0 runner    (1001) docker     (116)      380 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/fixtures/concepttype.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     6609 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/fixtures/currencytype.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     4549 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/fixtures/documenttype.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     5161 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/fixtures/receipttype.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1430 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/fixtures/taxtype.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      679 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/fixtures/vattype.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/locale/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)    12556 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)    12496 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/management/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/management/commands/
--rw-r--r--   0 runner    (1001) docker     (116)      330 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/management/commands/afipmetadata.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)    39213 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/migrations/0001_squashed_0036_receiptpdf__client_address__blank.py
--rw-r--r--   0 runner    (1001) docker     (116)     1554 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/migrations/0002_taxpayerextras.py
--rw-r--r--   0 runner    (1001) docker     (116)      566 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/migrations/0003_issuance_type_length.py
--rw-r--r--   0 runner    (1001) docker     (116)     2130 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/migrations/0004_storages_and_help_texts.py
--rw-r--r--   0 runner    (1001) docker     (116)      992 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/migrations/0005_flatten_taxpayer_extras.py
--rw-r--r--   0 runner    (1001) docker     (116)      256 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/migrations/0006_delete_taxpayerextras.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    45619 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/models.py
--rw-r--r--   0 runner    (1001) docker     (116)      705 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/pdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     3358 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/serializers.py
--rw-r--r--   0 runner    (1001) docker     (116)      590 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/static/receipts/
--rw-r--r--   0 runner    (1001) docker     (116)     2117 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/static/receipts/receipt.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/templates/receipts/
--rw-r--r--   0 runner    (1001) docker     (116)     4170 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/templates/receipts/code_11.html
--rw-r--r--   0 runner    (1001) docker     (116)     4170 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/templates/receipts/code_13.html
--rw-r--r--   0 runner    (1001) docker     (116)     4170 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/templates/receipts/code_3.html
--rw-r--r--   0 runner    (1001) docker     (116)     4170 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/templates/receipts/code_6.html
--rw-r--r--   0 runner    (1001) docker     (116)     4170 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/templates/receipts/code_8.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/templatetags/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      279 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/templatetags/django_afip.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/testing/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1201 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/test.crt
--rw-r--r--   0 runner    (1001) docker     (116)     1679 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/test.key
--rw-r--r--   0 runner    (1001) docker     (116)     1201 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/test2.crt
--rw-r--r--   0 runner    (1001) docker     (116)     1675 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/test2.key
--rw-r--r--   0 runner    (1001) docker     (116)     1549 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/test_expired.crt
--rw-r--r--   0 runner    (1001) docker     (116)     1679 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/test_expired.key
--rw-r--r--   0 runner    (1001) docker     (116)      156 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/testing/tiny.png
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     3248 2021-04-07 10:12:29.000000 django-afip-8.0.4/django_afip/views.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3657 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3301 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      333 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-04-07 10:12:34.000000 django-afip-8.0.4/django_afip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      634 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (116)     2202 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/_ext/django_models.py
--rw-r--r--   0 runner    (1001) docker     (116)     2061 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       30 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2690 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3770 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2668 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2816 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/printables.rst
--rw-r--r--   0 runner    (1001) docker     (116)       23 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6208 2021-04-07 10:12:29.000000 django-afip-8.0.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (116)      929 2021-04-07 10:12:29.000000 django-afip-8.0.4/scripts/dump_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)      522 2021-04-07 10:12:34.000000 django-afip-8.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1876 2021-04-07 10:12:29.000000 django-afip-8.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/
--rw-r--r--   0 runner    (1001) docker     (116)      333 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      250 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/manage.py
--rw-r--r--   0 runner    (1001) docker     (116)     1790 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/signed_data.bin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/testapp/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2495 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/testapp/testmain/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/testapp/testmain/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/testapp/testmain/templates/receipts/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/testapp/testmain/templates/receipts/20329642330/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/testapp/testmain/templates/receipts/20329642330/pos_9999/
--rw-r--r--   0 runner    (1001) docker     (116)       53 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/templates/receipts/20329642330/pos_9999/code_6.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:34.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10567 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (116)      574 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (116)      704 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (116)      424 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (116)     7881 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (116)     1198 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2862 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (116)      859 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (116)     3262 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_taxpayer.py
--rw-r--r--   0 runner    (1001) docker     (116)     9883 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (116)    12140 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/test_webservices.py
--rw-r--r--   0 runner    (1001) docker     (116)     1131 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/tests/testcases.py
--rw-r--r--   0 runner    (1001) docker     (116)      120 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/testmain/views.py
--rw-r--r--   0 runner    (1001) docker     (116)      639 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)      386 2021-04-07 10:12:29.000000 django-afip-8.0.4/testapp/testapp/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (116)      758 2021-04-07 10:12:29.000000 django-afip-8.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.061742 django-afip-9.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.045741 django-afip-9.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-10-16 16:29:41.000000 django-afip-9.0.0/.github/.kodiak.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2021-10-16 16:29:41.000000 django-afip-9.0.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.045741 django-afip-9.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-10-16 16:29:41.000000 django-afip-9.0.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-10-16 16:29:41.000000 django-afip-9.0.0/.github/no-response.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.045741 django-afip-9.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-10-16 16:29:41.000000 django-afip-9.0.0/.github/workflows/live.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2021-10-16 16:29:41.000000 django-afip-9.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2669 2021-10-16 16:29:41.000000 django-afip-9.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2021-10-16 16:29:41.000000 django-afip-9.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-10-16 16:29:41.000000 django-afip-9.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-10-16 16:29:41.000000 django-afip-9.0.0/.pypirc
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-10-16 16:29:41.000000 django-afip-9.0.0/.pyup.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-10-16 16:29:41.000000 django-afip-9.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    14985 2021-10-16 16:29:41.000000 django-afip-9.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2021-10-16 16:29:41.000000 django-afip-9.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (121)     3775 2021-10-16 16:29:52.061742 django-afip-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2021-10-16 16:29:41.000000 django-afip-9.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.049742 django-afip-9.0.0/django_afip/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12697 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3124 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/clients.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6535 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.049742 django-afip-9.0.0/django_afip/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/fixtures/concepttype.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6609 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/fixtures/currencytype.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4549 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/fixtures/documenttype.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5161 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/fixtures/receipttype.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/fixtures/taxtype.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/fixtures/vattype.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/django_afip/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/django_afip/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.049742 django-afip-9.0.0/django_afip/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    12556 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    12496 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/django_afip/management/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.049742 django-afip-9.0.0/django_afip/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/management/commands/afipmetadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.053742 django-afip-9.0.0/django_afip/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    39216 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0001_squashed_0036_receiptpdf__client_address__blank.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1554 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0002_taxpayerextras.py
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0003_issuance_type_length.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0004_storages_and_help_texts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0005_flatten_taxpayer_extras.py
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0006_delete_taxpayerextras.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7008 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0007_auto_20210409_1641.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3378 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/0008_move_taxpayerprofile_to_pos.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49104 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3549 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/django_afip/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.053742 django-afip-9.0.0/django_afip/static/receipts/
+-rw-r--r--   0 runner    (1001) docker     (121)     2117 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/static/receipts/receipt.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/django_afip/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.053742 django-afip-9.0.0/django_afip/templates/receipts/
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/templates/receipts/code_11.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/templates/receipts/code_13.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/templates/receipts/code_3.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/templates/receipts/code_6.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/templates/receipts/code_8.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.053742 django-afip-9.0.0/django_afip/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/templatetags/django_afip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.053742 django-afip-9.0.0/django_afip/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/test.crt
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/test.key
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/test2.crt
+-rw-r--r--   0 runner    (1001) docker     (121)     1675 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/test2.key
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/test_expired.crt
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/test_expired.key
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/testing/tiny.png
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-10-16 16:29:51.000000 django-afip-9.0.0/django_afip/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3247 2021-10-16 16:29:41.000000 django-afip-9.0.0/django_afip/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.049742 django-afip-9.0.0/django_afip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3775 2021-10-16 16:29:51.000000 django-afip-9.0.0/django_afip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3450 2021-10-16 16:29:51.000000 django-afip-9.0.0/django_afip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-16 16:29:51.000000 django-afip-9.0.0/django_afip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2021-10-16 16:29:51.000000 django-afip-9.0.0/django_afip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-16 16:29:51.000000 django-afip-9.0.0/django_afip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.057742 django-afip-9.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.057742 django-afip-9.0.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (121)     2172 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/_ext/django_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2156 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2962 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1882 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3732 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4173 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3109 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/printables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-10-16 16:29:41.000000 django-afip-9.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.057742 django-afip-9.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2021-10-16 16:29:41.000000 django-afip-9.0.0/scripts/dump_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-10-16 16:29:52.061742 django-afip-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-10-16 16:29:41.000000 django-afip-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.057742 django-afip-9.0.0/testapp/
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      250 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/signed_data.bin
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.057742 django-afip-9.0.0/testapp/testapp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.057742 django-afip-9.0.0/testapp/testapp/testmain/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/testapp/testapp/testmain/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/testapp/testapp/testmain/templates/receipts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.041741 django-afip-9.0.0/testapp/testapp/testmain/templates/receipts/20329642330/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.057742 django-afip-9.0.0/testapp/testapp/testmain/templates/receipts/20329642330/pos_9999/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/templates/receipts/20329642330/pos_9999/code_6.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:52.061742 django-afip-9.0.0/testapp/testapp/testmain/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10702 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9267 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2582 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3063 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_taxpayer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9823 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10354 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/tests/test_webservices.py
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/testmain/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2021-10-16 16:29:41.000000 django-afip-9.0.0/testapp/testapp/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-10-16 16:29:41.000000 django-afip-9.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-afip-8.0.4/.github/FUNDING.yml` & `django-afip-9.0.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/.github/ISSUE_TEMPLATE/question.md` & `django-afip-9.0.0/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/.github/no-response.yml` & `django-afip-9.0.0/.github/no-response.yml`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/.pre-commit-config.yaml` & `django-afip-9.0.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.2.0
+    rev: v4.0.1
     hooks:
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
       - id: end-of-file-fixer
       - id: check-toml
       - id: check-added-large-files
       - id: debug-statements
-  - repo: https://github.com/asottile/reorder_python_imports
-    rev: v2.3.5
+  - repo: https://github.com/pycqa/isort
+    rev: 5.9.3
     hooks:
-      - id: reorder-python-imports
+      - id: isort
   - repo: https://github.com/psf/black
-    rev: "20.8b1"
+    rev: "21.9b0"
     hooks:
       - id: black
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: "3.8.3" # pick a git hash / tag to point to
+  - repo: https://github.com/PyCQA/flake8
+    rev: "4.0.1" # pick a git hash / tag to point to
     hooks:
       - id: flake8
         additional_dependencies:
-          [flake8-comprehensions, flake8-import-order, flake8-bugbear]
+          - flake8-comprehensions
+          - flake8-bugbear
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "v0.910-1"
+    hooks:
+      - id: mypy
+        additional_dependencies:
+          - types-pytz
+          - types-freezegun
+          - types-pyOpenSSL
+          - types-requests
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v2.29.0
+    hooks:
+    -   id: pyupgrade
+        args: [--py37-plus]
```

### Comparing `django-afip-8.0.4/CHANGELOG.rst` & `django-afip-9.0.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,38 @@
 Changelog
 =========
 
-This file contains a brief summary of new features and dependency changes or
-releases, in reverse chronological order.
+Este archivo tiene un resúmen de nuevas funcionalidades o cambios de
+dependencia en cada versión, en orden cronológicamente inverso.
+
+Todos los cambios que necesites tener en cuenta al actualizar están listados
+acá.
+
+9.0.0
+-----
+
+* Django 2.2 y 3.0 ya no son soportados. Ambos tienen problemas de
+  compatibilidad con versiones nuevas de dependencias.
+  Ver https://code.djangoproject.com/ticket/32856
+* Python 3.6 ya no es soportado.
+* Soporte para Zeep ~4.0.0.
+* Soporte para Django 3.2.
+* La [mayoría de la] documentación ahora está traducida.
+* Se implementa :meth:`~.Receipt.revalidate`. Provee un mecanismo de revalidacion
+  de un comprobante para completar datos faltandes referentes a la validacion del mismo.
+* Se agrega :func:`~.get_server_status` para determinar el estado de los
+  servidores del AFIP.
+* The fields from the ``TaxPayerProfile`` have moved into the ``PointOfSales``
+  model. A migration will handle copying data from table to the other for you.
+  If you have any references to this model (e.g.: forms for your users, custom
+  admins, etc), make sure you update these to point to the
+  :class:`~PointOfSales` model.
+  This allow customising invoices for different points of sales differently.
+  Noticeably, different points of sales commonly have different address,
+  websites, and/or phone number.
 
 8.0.4
 -----
 
 * Fix mixup when sending validated receipts, introduced in v8.0.3.
 
 8.0.3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-afip-8.0.4/LICENCE` & `django-afip-9.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/PKG-INFO` & `django-afip-9.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,109 @@
 Metadata-Version: 2.1
 Name: django-afip
-Version: 8.0.4
+Version: 9.0.0
 Summary: AFIP integration for django
 Home-page: https://github.com/WhyNotHugo/django-afip
 Author: Hugo Osvaldo Barrera
 Author-email: hugo@barrera.io
 License: ISC
-Description: django-afip
-        ===========
-        
-        .. image:: https://travis-ci.com/WhyNotHugo/django-afip.svg?branch=main
-          :target: https://travis-ci.com/WhyNotHugo/django-afip
-          :alt: build status
-        
-        .. image:: https://codecov.io/gh/WhyNotHugo/django-afip/branch/main/graph/badge.svg
-          :target: https://codecov.io/gh/WhyNotHugo/django-afip
-          :alt: Build coverage
-        
-        .. image:: https://readthedocs.org/projects/django-afip/badge/?version=latest
-          :target: http://django-afip.readthedocs.io/en/latest/?badge=latest
-          :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/pypi/v/django-afip.svg
-          :target: https://pypi.python.org/pypi/django-afip
-          :alt: version on pypi
-        
-        .. image:: https://img.shields.io/pypi/dm/django-afip.svg
-          :target: https://pypi.python.org/pypi/django-afip
-          :alt: downloads
-        
-        .. image:: https://img.shields.io/pypi/l/django-afip.svg
-          :target: https://github.com/WhyNotHugo/django-afip/blob/main/LICENCE
-          :alt: licence
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-          :target: https://github.com/WhyNotHugo/django-afip/
-          :alt: code style: black
-        
-        What's this?
-        ------------
-        
-        AFIP is Argentina's tax collection agency. For emitting invoices, taxpayers are
-        required to inform AFIP of each invoice by using a dedicated SOAP-like web
-        service for that.
-        
-        **django-afip** is a Django application implementing the necessary bits for
-        Django-based applications to both store and comunícate invoicing information.
-        
-        Features
-        --------
-        
-        * Validate invoices and other receipt types with AFIP's WSFE service.
-        * Generate valid PDF files for those receipts to send to clients.
-        
-        Documentation
-        -------------
-        
-        The full documentation is available at https://django-afip.readthedocs.io/
-        
-        Donate
-        ------
-        
-        While some of the work done here is done for clients, much of it is done in my
-        free time. If you appreciate the work done here, please consider donating_.
-        
-        .. _donating: https://github.com/sponsors/WhyNotHugo
-        
-        Licence
-        -------
-        
-        This software is distributed under the ISC licence. See LICENCE for details.
-        
-        Copyright (c) 2015-2020 Hugo Osvaldo Barrera <hugo@barrera.io>
-        
+Project-URL: Documentation, https://django-afip.readthedocs.io/
+Project-URL: Issue Tracker, https://github.com/WhyNotHugo/django-afip/issues
+Project-URL: Donate, https://liberapay.com/WhyNotHugo/
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: postgres
 Provides-Extra: mysql
 Provides-Extra: factories
+License-File: LICENCE
+
+django-afip
+===========
+
+.. image:: https://github.com/WhyNotHugo/django-afip/actions/workflows/tests.yml/badge.svg
+  :target: https://github.com/WhyNotHugo/django-afip/actions/workflows/tests.yml
+  :alt: unit tests
+
+.. image:: https://github.com/WhyNotHugo/django-afip/actions/workflows/live.yml/badge.svg
+  :target: https://github.com/WhyNotHugo/django-afip/actions/workflows/live.yml
+  :alt: integrations tests
+
+.. image:: https://results.pre-commit.ci/badge/github/WhyNotHugo/django-afip/main.svg
+  :target: https://results.pre-commit.ci/latest/github/WhyNotHugo/django-afip/main
+  :alt: pre-commit.ci status
+
+.. image:: https://codecov.io/gh/WhyNotHugo/django-afip/branch/main/graph/badge.svg
+  :target: https://codecov.io/gh/WhyNotHugo/django-afip
+  :alt: Build coverage
+
+.. image:: https://readthedocs.org/projects/django-afip/badge/?version=latest
+  :target: http://django-afip.readthedocs.io/en/latest/?badge=latest
+  :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/django-afip.svg
+  :target: https://pypi.python.org/pypi/django-afip
+  :alt: version on pypi
+
+.. image:: https://img.shields.io/pypi/dm/django-afip.svg
+  :target: https://pypi.python.org/pypi/django-afip
+  :alt: downloads
+
+.. image:: https://img.shields.io/pypi/l/django-afip.svg
+  :target: https://github.com/WhyNotHugo/django-afip/blob/main/LICENCE
+  :alt: licence
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+  :target: https://github.com/WhyNotHugo/django-afip/
+  :alt: code style: black
+
+What's this?
+------------
+
+AFIP is Argentina's tax collection agency. For emitting invoices, taxpayers are
+required to inform AFIP of each invoice by using a dedicated SOAP-like web
+service for that.
+
+**django-afip** is a Django application implementing the necessary bits for
+Django-based applications to both store and comunícate invoicing information.
+
+Features
+--------
+
+* Validate invoices and other receipt types with AFIP's WSFE service.
+* Generate valid PDF files for those receipts to send to clients.
+
+Documentation
+-------------
+
+The full documentation is available at https://django-afip.readthedocs.io/
+
+Donate
+------
+
+While some of the work done here is done for clients, much of it is done in my
+free time. If you appreciate the work done here, please consider donating_.
+
+.. _donating: https://github.com/sponsors/WhyNotHugo
+
+Licence
+-------
+
+This software is distributed under the ISC licence. See LICENCE for details.
+
+Copyright (c) 2015-2020 Hugo Osvaldo Barrera <hugo@barrera.io>
+
+
```

### Comparing `django-afip-8.0.4/README.rst` & `django-afip-9.0.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 django-afip
 ===========
 
-.. image:: https://travis-ci.com/WhyNotHugo/django-afip.svg?branch=main
-  :target: https://travis-ci.com/WhyNotHugo/django-afip
-  :alt: build status
+.. image:: https://github.com/WhyNotHugo/django-afip/actions/workflows/tests.yml/badge.svg
+  :target: https://github.com/WhyNotHugo/django-afip/actions/workflows/tests.yml
+  :alt: unit tests
+
+.. image:: https://github.com/WhyNotHugo/django-afip/actions/workflows/live.yml/badge.svg
+  :target: https://github.com/WhyNotHugo/django-afip/actions/workflows/live.yml
+  :alt: integrations tests
+
+.. image:: https://results.pre-commit.ci/badge/github/WhyNotHugo/django-afip/main.svg
+  :target: https://results.pre-commit.ci/latest/github/WhyNotHugo/django-afip/main
+  :alt: pre-commit.ci status
 
 .. image:: https://codecov.io/gh/WhyNotHugo/django-afip/branch/main/graph/badge.svg
   :target: https://codecov.io/gh/WhyNotHugo/django-afip
   :alt: Build coverage
 
 .. image:: https://readthedocs.org/projects/django-afip/badge/?version=latest
   :target: http://django-afip.readthedocs.io/en/latest/?badge=latest
```

### Comparing `django-afip-8.0.4/django_afip/admin.py` & `django-afip-9.0.0/django_afip/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,61 @@
-import functools
+# Mypy doesn't play well with action-functions.
+#
+# type: ignore
 import logging
+from contextlib import contextmanager
 from datetime import datetime
 
-import django
 from django.contrib import admin
 from django.contrib import messages
 from django.db.models import F
 from django.http import HttpResponse
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 
 from django_afip import exceptions
 from django_afip import models
 
-
 logger = logging.getLogger(__name__)
 
 
 # TODO: Add an action to populate generic types.
 
 
-def catch_errors(f):
-    """
-    Catches specific errors in admin actions and shows a friendly error.
-    """
-
-    @functools.wraps(f)
-    def wrapper(self, request, *args, **kwargs):
-        try:
-            return f(self, request, *args, **kwargs)
-        except exceptions.CertificateExpired:
-            self.message_user(
-                request,
-                _("The AFIP Taxpayer certificate has expired."),
-                messages.ERROR,
-            )
-        except exceptions.UntrustedCertificate:
-            self.message_user(
-                request,
-                _("The AFIP Taxpayer certificate is untrusted."),
-                messages.ERROR,
-            )
-        except exceptions.CorruptCertificate:
-            self.message_user(
-                request,
-                _("The AFIP Taxpayer certificate is corrupt."),
-                messages.ERROR,
-            )
-        except exceptions.AuthenticationError as e:
-            logger.exception("AFIP auth failed")
-            self.message_user(
-                request,
-                _("An unknown authentication error has ocurred: %s") % e,
-                messages.ERROR,
-            )
-
-    return wrapper
+@contextmanager
+def catch_errors(self, request):
+    """Catches specific errors in admin actions and shows a friendly error."""
+    try:
+        yield
+    except exceptions.CertificateExpired:
+        self.message_user(
+            request,
+            _("The AFIP Taxpayer certificate has expired."),
+            messages.ERROR,
+        )
+    except exceptions.UntrustedCertificate:
+        self.message_user(
+            request,
+            _("The AFIP Taxpayer certificate is untrusted."),
+            messages.ERROR,
+        )
+    except exceptions.CorruptCertificate:
+        self.message_user(
+            request,
+            _("The AFIP Taxpayer certificate is corrupt."),
+            messages.ERROR,
+        )
+    except exceptions.AuthenticationError as e:
+        logger.exception("AFIP auth failed")
+        self.message_user(
+            request,
+            _("An unknown authentication error has ocurred: %s") % e,
+            messages.ERROR,
+        )
 
 
 class VatInline(admin.TabularInline):
     model = models.Vat
     fields = (
         "vat_type",
         "base_amount",
@@ -167,21 +162,14 @@
     autocomplete_fields = (
         "currency",
         "receipt_type",
         "related_receipts",
     )
     date_hierarchy = "issued_date"
 
-    def get_exclude(self, request, obj=None):
-        if django.VERSION < (2, 0):
-            # This field would load every single receipts for the widget which
-            # will always result in thousands of queries until an evetual OOM.
-            return ["related_receipts"]
-        return []
-
     __related_fields = [
         "validated",
         "cae",
     ]
 
     inlines = (
         VatInline,
@@ -252,17 +240,18 @@
 
     def cae(self, obj):
         return obj.validation.cae
 
     cae.short_description = _("cae")
     cae.admin_order_field = "validation__cae"
 
-    @catch_errors
     def validate(self, request, queryset):
-        errs = queryset.validate()
+        with catch_errors(self, request):
+            errs = queryset.validate()
+
         if errs:
             self.message_user(
                 request,
                 _("Receipt validation failed: %s.") % errs,
                 messages.ERROR,
             )
 
@@ -286,21 +275,21 @@
 class TaxPayerAdmin(admin.ModelAdmin):
     list_display = (
         "name",
         "cuit",
         "certificate_expiration",
     )
 
-    @catch_errors
     def fetch_points_of_sales(self, request, queryset):
-        poses = [
-            pos
-            for taxpayer in queryset.all()
-            for pos in taxpayer.fetch_points_of_sales()
-        ]
+        with catch_errors(self, request):
+            poses = [
+                pos
+                for taxpayer in queryset.all()
+                for pos in taxpayer.fetch_points_of_sales()
+            ]
 
         created = len([pos for pos in poses if pos[1]])
         skipped = len(poses) - created
 
         self.message_user(
             request,
             message=(_("%d points of sales created.") % created),
@@ -351,15 +340,15 @@
         csr = taxpayer.generate_csr()
         filename = "cuit-{}-{}.csr".format(
             taxpayer.cuit,
             int(datetime.now().timestamp()),
         )
 
         response = HttpResponse(content_type="application/pkcs10")
-        response["Content-Disposition"] = "attachment; filename={}".format(filename)
+        response["Content-Disposition"] = f"attachment; filename={filename}"
 
         response.write(csr.read())
         return response
 
     generate_csr.short_description = _("Generate CSR")
 
     actions = (
@@ -500,21 +489,12 @@
         return obj.result == models.ReceiptValidation.RESULT_APPROVED
 
     successful.short_description = _("result")
     successful.admin_order_field = "result"
     successful.boolean = True
 
 
-@admin.register(models.TaxPayerProfile)
-class TaxPayerProfileAdmin(admin.ModelAdmin):
-    list_display = (
-        "taxpayer",
-        "issuing_name",
-        "issuing_email",
-    )
-
-
 admin.site.register(models.ConceptType)
 admin.site.register(models.DocumentType)
 admin.site.register(models.VatType)
 admin.site.register(models.TaxType)
 admin.site.register(models.Observation)
```

### Comparing `django-afip-8.0.4/django_afip/clients.py` & `django-afip-9.0.0/django_afip/clients.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from urllib.parse import urlparse
 
 import pytz
 from django.utils.functional import LazyObject
 from requests import Session
 from requests.adapters import HTTPAdapter
-from urllib3.util.ssl_ import create_urllib3_context, DEFAULT_CIPHERS
+from urllib3.util.ssl_ import DEFAULT_CIPHERS
+from urllib3.util.ssl_ import create_urllib3_context
 from zeep import Client
 from zeep.cache import SqliteCache
 from zeep.transports import Transport
 
 TZ_AR = pytz.timezone(pytz.country_timezones["ar"][0])
 CIPHERS = DEFAULT_CIPHERS + "HIGH:!DH:!aNULL"
 WSDLS = {
@@ -82,8 +83,8 @@
 
     try:
         if key not in cached_clients:
             cached_clients[key] = Client(WSDLS[key], transport=transport)
 
         return cached_clients[key]
     except KeyError:
-        raise ValueError("Unknown service name, {}".format(service_name))
+        raise ValueError(f"Unknown service name, {service_name}")
```

### Comparing `django-afip-8.0.4/django_afip/crypto.py` & `django-afip-9.0.0/django_afip/crypto.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from cryptography.hazmat.primitives.serialization.pkcs7 import PKCS7SignatureBuilder
 from cryptography.x509 import load_pem_x509_certificate
 from OpenSSL import crypto
 
 from django_afip import exceptions
 
 
-def create_embeded_pkcs7_signature(data: bytes, cert: bytes, key: bytes):
+def create_embeded_pkcs7_signature(data: bytes, cert: bytes, key: bytes) -> bytes:
     """Creates an embedded ("nodetached") PKCS7 signature.
 
     This is equivalent to the output of::
 
         openssl smime -sign -signer cert -inkey key -outform DER -nodetach < data
     """
 
@@ -56,11 +56,7 @@
     subj.CN = common_name
     subj.serialNumber = serial_number
 
     req.set_pubkey(key)
     req.sign(key, "md5")
 
     file_.write(crypto.dump_certificate_request(crypto.FILETYPE_PEM, req))
-
-
-def parse_certificate(file_):
-    return crypto.load_certificate(crypto.FILETYPE_PEM, file_)
```

### Comparing `django-afip-8.0.4/django_afip/exceptions.py` & `django-afip-9.0.0/django_afip/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/factories.py` & `django-afip-9.0.0/django_afip/factories.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from datetime import datetime
 from pathlib import Path
 
 from django.contrib.auth.models import User
 from django.utils.timezone import make_aware
 from factory import LazyFunction
 from factory import PostGenerationMethodCall
+from factory import Sequence
 from factory import SubFactory
+from factory import post_generation
 from factory.django import DjangoModelFactory
 from factory.django import FileField
 from factory.django import ImageField
 
 from django_afip import models
 
 
@@ -71,14 +73,15 @@
     description = "Factura C"
     valid_from = date(2011, 3, 30)
 
 
 class TaxPayerFactory(DjangoModelFactory):
     class Meta:
         model = models.TaxPayer
+        django_get_or_create = ["cuit"]
 
     name = "John Smith"
     cuit = 20329642330
     is_sandboxed = True
     key = FileField(from_path=get_test_file("test.key"))
     certificate = FileField(from_path=get_test_file("test.crt"))
     active_since = datetime(2011, 10, 3)
@@ -95,35 +98,30 @@
     cuit = 20329642330
     is_sandboxed = True
     key = FileField(from_path=get_test_file("test2.key"))
     certificate = FileField(from_path=get_test_file("test2.crt"))
     active_since = datetime(2011, 10, 3)
 
 
-class TaxPayerProfileFactory(DjangoModelFactory):
-    class Meta:
-        model = models.TaxPayerProfile
-
-    taxpayer = SubFactory(TaxPayerFactory)
-    issuing_name = "Red Company Inc."
-    issuing_address = "100 Red Av\nRedsville\nUK"
-    issuing_email = "billing@example.com"
-    vat_condition = "Exempt"
-    gross_income_condition = "Exempt"
-    sales_terms = "Credit Card"
-
-
 class PointOfSalesFactory(DjangoModelFactory):
     class Meta:
         model = models.PointOfSales
+        django_get_or_create = ["owner", "number"]
 
     number = 1
     issuance_type = "CAE"
     blocked = False
     owner = SubFactory(TaxPayerFactory)
+    # TODO: Renamethis to something more regional:
+    issuing_name = "Red Company Inc."
+    issuing_address = "100 Red Av\nRedsville\nUK"
+    issuing_email = "billing@example.com"
+    vat_condition = "Exempt"
+    gross_income_condition = "Exempt"
+    sales_terms = "Credit Card"
 
 
 class ReceiptFactory(DjangoModelFactory):
     class Meta:
         model = models.Receipt
 
     concept = SubFactory(ConceptTypeFactory, code=1)
@@ -136,14 +134,46 @@
     exempt_amount = 0
     currency = SubFactory(CurrencyTypeFactory, code="PES")
     currency_quote = 1
     receipt_type = SubFactory(ReceiptTypeFactory, code=6)
     point_of_sales = SubFactory(PointOfSalesFactory)
 
 
+class ReceiptWithVatAndTaxFactory(ReceiptFactory):
+    """Receipt with a valid Vat and Tax, ready to validate."""
+
+    point_of_sales = LazyFunction(lambda: models.PointOfSales.objects.first())
+
+    @post_generation
+    def post(obj: models.Receipt, create, extracted, **kwargs):
+        VatFactory(vat_type__code=5, receipt=obj)
+        TaxFactory(tax_type__code=3, receipt=obj)
+
+
+class ReceiptWithInconsistentVatAndTaxFactory(ReceiptWithVatAndTaxFactory):
+    """Receipt with a valid Vat and Tax, ready to validate."""
+
+    document_type = SubFactory(DocumentTypeFactory, code=80)
+
+    @post_generation
+    def post(obj: models.Receipt, create, extracted, **kwargs):
+        VatFactory(vat_type__code=5, receipt=obj)
+        TaxFactory(tax_type__code=3, receipt=obj)
+
+
+class ReceiptWithApprovedValidation(ReceiptFactory):
+    """Receipt with fake (e.g.: not live) approved validation."""
+
+    receipt_number = Sequence(lambda n: n + 1)
+
+    @post_generation
+    def post(obj: models.Receipt, create, extracted, **kwargs):
+        ReceiptValidationFactory(receipt=obj)
+
+
 class ReceiptValidationFactory(DjangoModelFactory):
     class Meta:
         model = models.ReceiptValidation
 
     result = models.ReceiptValidation.RESULT_APPROVED
     processed_date = make_aware(datetime(2017, 7, 2, 21, 6, 4))
     cae = "67190616790549"
@@ -162,14 +192,18 @@
     issuing_address = "Happy Street 123, CABA"
     issuing_name = "Alice Doe"
     receipt = SubFactory(ReceiptFactory)
     sales_terms = "Contado"
     vat_condition = "Responsable Monotributo"
 
 
+class ReceiptPDFWithFileFactory(ReceiptPDFFactory):
+    receipt = SubFactory(ReceiptWithApprovedValidation)
+
+
 class GenericAfipTypeFactory(DjangoModelFactory):
     class Meta:
         model = models.GenericAfipType
 
     code = 80
     description = "CUIT"
     valid_from = datetime(2017, 8, 10)
```

### Comparing `django-afip-8.0.4/django_afip/fixtures/currencytype.yaml` & `django-afip-9.0.0/django_afip/fixtures/currencytype.yaml`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/fixtures/documenttype.yaml` & `django-afip-9.0.0/django_afip/fixtures/documenttype.yaml`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/fixtures/receipttype.yaml` & `django-afip-9.0.0/django_afip/fixtures/receipttype.yaml`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/fixtures/taxtype.yaml` & `django-afip-9.0.0/django_afip/fixtures/taxtype.yaml`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/fixtures/vattype.yaml` & `django-afip-9.0.0/django_afip/fixtures/vattype.yaml`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/locale/es/LC_MESSAGES/django.mo` & `django-afip-9.0.0/django_afip/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/locale/es/LC_MESSAGES/django.po` & `django-afip-9.0.0/django_afip/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/migrations/0001_squashed_0036_receiptpdf__client_address__blank.py` & `django-afip-9.0.0/django_afip/migrations/0001_squashed_0036_receiptpdf__client_address__blank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 import django.db.models.deletion
 from django.db import migrations
 from django.db import models
 
 import django_afip.models
 
 
@@ -44,15 +46,15 @@
         ("afip", "0034_vat_condition_choices"),
         ("afip", "0035_receiptentry__vat__blankable"),
         ("afip", "0036_receiptpdf__client_address__blank"),
     ]
 
     initial = True
 
-    dependencies = []
+    dependencies: List[str] = []
 
     operations = [
         migrations.CreateModel(
             name="AuthTicket",
             fields=[
                 (
                     "id",
@@ -62,29 +64,29 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "unique_id",
                     models.IntegerField(
-                        default=django_afip.models.AuthTicket.default_unique_id,
+                        default=django_afip.models.default_unique_id,
                         verbose_name="unique id",
                     ),
                 ),
                 (
                     "generated",
                     models.DateTimeField(
-                        default=django_afip.models.AuthTicket.default_generated,
+                        default=django_afip.models.default_generated,
                         verbose_name="generated",
                     ),
                 ),
                 (
                     "expires",
                     models.DateTimeField(
-                        default=django_afip.models.AuthTicket.default_expires,
+                        default=django_afip.models.default_expires,
                         verbose_name="expires",
                     ),
                 ),
                 (
                     "service",
                     models.CharField(
                         help_text="Service for which this ticket has been authorized",
```

### Comparing `django-afip-8.0.4/django_afip/migrations/0002_taxpayerextras.py` & `django-afip-9.0.0/django_afip/migrations/0002_taxpayerextras.py`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/migrations/0003_issuance_type_length.py` & `django-afip-9.0.0/django_afip/migrations/0003_issuance_type_length.py`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/migrations/0004_storages_and_help_texts.py` & `django-afip-9.0.0/django_afip/migrations/0004_storages_and_help_texts.py`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/migrations/0005_flatten_taxpayer_extras.py` & `django-afip-9.0.0/django_afip/migrations/0005_flatten_taxpayer_extras.py`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/models.py` & `django-afip-9.0.0/django_afip/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,48 @@
+from __future__ import annotations
+
 import base64
 import logging
 import os
 import random
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from io import BytesIO
 from tempfile import NamedTemporaryFile
-from typing import List
-from typing import Type
+from typing import BinaryIO
 from uuid import uuid4
 
 import pytz
 from django.conf import settings
 from django.core import management
 from django.core.files import File
+from django.core.files.storage import Storage
 from django.db import models
 from django.db.models import Count
 from django.db.models import Sum
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 from django_renderpdf.helpers import render_pdf
 from lxml import etree
 from lxml.builder import E
+from OpenSSL.crypto import FILETYPE_PEM
+from OpenSSL.crypto import X509
+from OpenSSL.crypto import load_certificate
 from zeep.exceptions import Fault
 
 from . import clients
 from . import crypto
 from . import exceptions
 from . import parsers
 from . import serializers
 
 logger = logging.getLogger(__name__)
 TZ_AR = pytz.timezone(pytz.country_timezones["ar"][0])
 
-
 # http://www.afip.gov.ar/afip/resol1415_anexo2.html
 VAT_CONDITIONS = (
     "IVA Responsable Inscripto",
     "IVA Responsable No Inscripto",
     "IVA Exento",
     "No Responsable IVA",
     "Responsable Monotributo",
@@ -56,80 +60,75 @@
     "IVA Liberado - Ley Nº 19.640",
     "IVA Responsable Inscripto - Agente de Percepción",
     "Monotributista Social",
     "IVA no alcanzado",
 )
 
 
-def load_metadata():
+def load_metadata() -> None:
     """Loads metadata from fixtures into the database."""
 
     for model in GenericAfipType.SUBCLASSES:
         label = model._meta.label.split(".")[1].lower()
         management.call_command("loaddata", label, app="afip")
 
 
-def check_response(response):
-    """
-    Check that a response is not an error.
+def check_response(response) -> None:
+    """Check that a response is not an error.
 
     AFIP allows us to create valid tickets with invalid key/CUIT pairs, so we
     can end up with tickets that fail on any service.
 
     Due to how zeep works, we can't quite catch these sort of errors on some
     middleware level (well, honestly, we need to do a large refactor).
 
     This method checks if responses have an error, and raise a readable
     message.
     """
     if response.Errors:
         raise exceptions.AfipException(response)
 
 
-def first_currency():
-    """
-    Returns the id for the first currency
+def first_currency() -> int | None:
+    """Returns the id for the first currency
 
     The `default` parameter of a foreign key *MUST* be a primary key (and not
     an instance), else migrations break. This helper method exists solely for
     that purpose.
     """
     ct = CurrencyType.objects.filter(code="PES").first()
     if ct:
         return ct.pk
 
 
-def _get_storage_from_settings(setting_name=None):
+def _get_storage_from_settings(setting_name: str) -> Storage:
     path = getattr(settings, setting_name, None)
     if not path:
         return import_string(settings.DEFAULT_FILE_STORAGE)()
     return import_string(path)
 
 
 class GenericAfipTypeManager(models.Manager):
     """Default Manager for GenericAfipType."""
 
-    def __init__(self, service_name, type_name):
-        """
-        Create a new Manager instance for a GenericAfipType.
+    def __init__(self, service_name: str, type_name: str):
+        """Create a new Manager instance for a GenericAfipType.
 
         This should generally only be required to manually populate a single
         type with upstream data.
         """
         super().__init__()
         self.__service_name = service_name
         self.__type_name = type_name
 
-    def populate(self, ticket=None):
+    def populate(self, ticket: AuthTicket = None) -> None:
         """Fetch and save data for this model from AFIP's WS.
 
         Direct usage of this method is discouraged, use
         :func:`~.models.load_metadata` instead.
-
-        If no ticket is provided, the most recent available one will be used.
         """
         ticket = ticket or AuthTicket.objects.get_any_active("wsfe")
         client = clients.get_client("wsfe", ticket.owner.is_sandboxed)
         service = getattr(client.service, self.__service_name)
         response_xml = service(serializers.serialize_ticket(ticket))
 
         check_response(response_xml)
@@ -138,29 +137,29 @@
             self.get_or_create(
                 code=result.Id,
                 description=result.Desc,
                 valid_from=parsers.parse_date(result.FchDesde),
                 valid_to=parsers.parse_date(result.FchHasta),
             )
 
-    def get_by_natural_key(self, code):
+    def get_by_natural_key(self, code: str) -> GenericAfipType:
         return self.get(code=code)
 
-    def exists_by_natural_key(self, code):
+    def exists_by_natural_key(self, code: str) -> bool:
         return self.filter(code=code).exists()
 
 
 class GenericAfipType(models.Model):
     """An abstract class for several of AFIP's metadata types.
 
     You should not use this class directly, only subclasses of it. You should
     not create subclasses of this model unless you really know what you're doing.
     """
 
-    SUBCLASSES: List[Type] = []
+    SUBCLASSES: list[type[models.Model]] = []
 
     def __init_subclass__(cls, **kwargs):
         """Keeps a registry of known subclasses."""
         super().__init_subclass__(**kwargs)
         GenericAfipType.SUBCLASSES.append(cls)
 
     code = models.CharField(
@@ -178,114 +177,107 @@
     )
     valid_to = models.DateField(
         _("valid until"),
         null=True,
         blank=True,
     )
 
-    def natural_key(self):
+    def natural_key(self) -> tuple[str]:
         return (self.code,)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.description
 
     class Meta:
         abstract = True
 
 
 class ReceiptType(GenericAfipType):
-    """
-    An AFIP receipt type.
+    """An AFIP receipt type.
 
     See the AFIP's documentation for details on each receipt type.
     """
 
     objects = GenericAfipTypeManager("FEParamGetTiposCbte", "CbteTipo")
 
     class Meta:
         verbose_name = _("receipt type")
         verbose_name_plural = _("receipt types")
 
 
 class ConceptType(GenericAfipType):
-    """
-    An AFIP concept type.
+    """An AFIP concept type.
 
     See the AFIP's documentation for details on each concept type.
     """
 
     objects = GenericAfipTypeManager("FEParamGetTiposConcepto", "ConceptoTipo")
 
     class Meta:
         verbose_name = _("concept type")
         verbose_name_plural = _("concept types")
 
 
 class DocumentType(GenericAfipType):
-    """
-    An AFIP document type.
+    """An AFIP document type.
 
     See the AFIP's documentation for details on each document type.
     """
 
     objects = GenericAfipTypeManager("FEParamGetTiposDoc", "DocTipo")
 
     class Meta:
         verbose_name = _("document type")
         verbose_name_plural = _("document types")
 
 
 class VatType(GenericAfipType):
-    """
-    An AFIP VAT type.
+    """An AFIP VAT type.
 
     See the AFIP's documentation for details on each VAT type.
     """
 
     objects = GenericAfipTypeManager("FEParamGetTiposIva", "IvaTipo")
 
     class Meta:
         verbose_name = _("vat type")
         verbose_name_plural = _("vat types")
 
 
 class TaxType(GenericAfipType):
-    """
-    An AFIP tax type.
+    """An AFIP tax type.
 
     See the AFIP's documentation for details on each tax type.
     """
 
     objects = GenericAfipTypeManager("FEParamGetTiposTributos", "TributoTipo")
 
     class Meta:
         verbose_name = _("tax type")
         verbose_name_plural = _("tax types")
 
 
 class CurrencyType(GenericAfipType):
-    """
-    An AFIP curreny type.
+    """An AFIP curreny type.
 
     See the AFIP's documentation for details on each currency type.
     """
 
     objects = GenericAfipTypeManager("FEParamGetTiposMonedas", "Moneda")
 
-    def __str__(self):
-        return "{} ({})".format(self.description, self.code)
+    def __str__(self) -> str:
+        return f"{self.description} ({self.code})"
 
     class Meta:
         verbose_name = _("currency type")
         verbose_name_plural = _("currency types")
 
 
 class TaxPayer(models.Model):
-    """
-    Represents an AFIP TaxPayer.
+    """Represents an AFIP TaxPayer.
 
     Note that multiple instances of this object can actually represent the same
     taxpayer, each using a different key.
 
     The following fields are only used for generating printables, and are never
     sent to AFIP, hence, are entirely optional:
 
@@ -294,22 +286,22 @@
 
     name = models.CharField(
         _("name"),
         max_length=32,
         help_text=_("A friendly name to recognize this taxpayer."),
     )
     key = models.FileField(
-        _("key"),
+        verbose_name=_("key"),
         upload_to="afip/taxpayers/keys/",
         storage=_get_storage_from_settings("AFIP_KEY_STORAGE"),
         blank=True,
         null=True,
     )
     certificate = models.FileField(
-        _("certificate"),
+        verbose_name=_("certificate"),
         upload_to="afip/taxpayers/certs/",
         storage=_get_storage_from_settings("AFIP_CERT_STORAGE"),
         blank=True,
         null=True,
     )
     cuit = models.BigIntegerField(
         _("cuit"),
@@ -340,47 +332,58 @@
         storage=_get_storage_from_settings("AFIP_LOGO_STORAGE"),
         blank=True,
         null=True,
         help_text=_("A logo to use when generating printable receipts."),
     )
 
     @property
-    def logo_as_data_uri(self):
+    def logo_as_data_uri(self) -> str:
         """This TaxPayer's logo as a data uri."""
         _, ext = os.path.splitext(self.logo.file.name)
         with self.logo.open() as f:
             data = base64.b64encode(f.read())
 
         return "data:image/{};base64,{}".format(
             ext[1:], data.decode()  # Remove the leading dot.
         )
 
     @property
-    def certificate_object(self):
-        """Return the certificate as an OpenSSL object."""
+    def certificate_object(self) -> X509 | None:
+        """Returns the certificate as an OpenSSL object
+
+        Returns the certificate as an OpenSSL object (rather than as a file
+        object).
+        """
+
         if not self.certificate:
             return None
         self.certificate.seek(0)
-        return crypto.parse_certificate(self.certificate.read())
+        return load_certificate(FILETYPE_PEM, self.certificate.read())
 
-    def get_certificate_expiration(self):
+    def get_certificate_expiration(self) -> datetime | None:
         """
         Gets the certificate expiration from the certificate
 
 
         Gets the certificate expiration from the certificate file. Note that
         this value is stored into ``certificate_expiration`` when an instance
         is saved, so you should generally prefer that method (since this one
         requires reading and parsing the entire certificate).
         """
-        datestring = self.certificate_object.get_notAfter().decode()
+        cert = self.certificate_object
+        if not cert:
+            return None
+        not_after = cert.get_notAfter()
+        if not not_after:
+            return None
+        datestring = not_after.decode()
         dt = datetime.strptime(datestring, "%Y%m%d%H%M%SZ")
         return dt.replace(tzinfo=timezone.utc)
 
-    def generate_key(self, force=False):
+    def generate_key(self, force=False) -> bool:
         """
         Creates a key file for this TaxPayer
 
         Creates a key file for this TaxPayer if it does not have one, and
         immediately saves it.
 
         A new key will not be generated if one is already set, unless the ``force``
@@ -390,62 +393,63 @@
         """
         if self.key and not force:
             logger.warning("Tried to generate key for a taxpayer that already had one")
             return False
 
         with NamedTemporaryFile(suffix=".key") as file_:
             crypto.create_key(file_)
-            self.key = File(file_, name="{}.key".format(uuid4().hex))
+            self.key = File(file_, name=f"{uuid4().hex}.key")
             self.save()
 
         return True
 
-    def generate_csr(self, basename="djangoafip"):
+    def generate_csr(self, basename="djangoafip") -> BinaryIO:
         """
         Creates a CSR for this TaxPayer's key
 
         Creates a file-like object that contains the CSR which can be used to
         request a new certificate from AFIP.
         """
         csr = BytesIO()
         crypto.create_csr(
             self.key.file,
             self.name,
-            "{}{}".format(basename, int(datetime.now().timestamp())),
-            "CUIT {}".format(self.cuit),
+            f"{basename}{int(datetime.now().timestamp())}",
+            f"CUIT {self.cuit}",
             csr,
         )
         csr.seek(0)
         return csr
 
-    def create_ticket(self, service):
+    def create_ticket(self, service: str) -> AuthTicket:
         """Create an AuthTicket for a given service."""
         ticket = AuthTicket(owner=self, service=service)
         ticket.authorize()
         return ticket
 
-    def get_ticket(self, service):
-        """Return an existing AuthTicket for a given service."""
+    def get_ticket(self, service: str) -> AuthTicket | None:
+        """Return an existing AuthTicket for a given service, if any."""
         return self.auth_tickets.filter(
-            expires__gt=datetime.now(timezone.utc), service=service
+            expires__gt=datetime.now(timezone.utc),
+            service=service,
         ).last()
 
-    def get_or_create_ticket(self, service):
+    def get_or_create_ticket(self, service: str) -> AuthTicket:
         """
         Return or create a new AuthTicket for a given serivce.
 
         Return an existing ticket for a service if one is available, otherwise,
         create a new one and return that.
 
         This is generally the preferred method of obtaining tickets for any
         service.
         """
         return self.get_ticket(service) or self.create_ticket(service)
 
-    def fetch_points_of_sales(self, ticket=None):
+    def fetch_points_of_sales(self, ticket: AuthTicket = None) -> list[PointOfSales]:
         """
         Fetch all point of sales objects.
 
         Fetch all point of sales from the WS and store (or update) them
         locally.
 
         Returns a list of tuples with the format (pos, created,).
@@ -470,53 +474,89 @@
                         "drop_date": parsers.parse_date(pos_data.FchBaja),
                     },
                 )
             )
 
         return results
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<TaxPayer {}: {}, CUIT {}>".format(
             self.pk,
             self.name,
             self.cuit,
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.name)
 
     class Meta:
         verbose_name = _("taxpayer")
         verbose_name_plural = _("taxpayers")
 
 
-class TaxPayerProfile(models.Model):
+class PointOfSales(models.Model):
     """
-    Metadata about a taxpayer used for printable receipts.
+    Represents an existing AFIP point of sale.
+
+    Points of sales need to be created via AFIP's web interface and it is
+    recommended that you use :meth:`~.TaxPayer.fetch_points_of_sales` to fetch
+    these programatically.
+
+    Note that deleting or altering these models will not affect upstream point
+    of sales.
 
-    None of this information is required or sent to the AFIP when notifying
-    about receipt generation. It is used *only* for PDF generation.
+    This model also contains a few fields that are not required or sent to the
+    AFIP when validating receipt. They are used *only* for PDF generation.
+    Those fields are:
+
+    - issuing_name
+    - issuing_address
+    - issuing_email
+    - vat_condition
+    - gross_income_condition
+    - sales_terms
 
-    Most of these can be overriden per-receipt as this class is a placeholder
-    for default values.
+    These fields may be ignored when using an external mechanism to generate
+    PDF or printable receipts.
     """
 
-    taxpayer = models.OneToOneField(
+    number = models.PositiveSmallIntegerField(
+        _("number"),
+    )
+    issuance_type = models.CharField(
+        _("issuance type"),
+        max_length=24,
+        help_text="Indicates if this POS emits using CAE and CAEA.",
+    )
+    blocked = models.BooleanField(
+        _("blocked"),
+    )
+    drop_date = models.DateField(
+        _("drop date"),
+        null=True,
+        blank=True,
+    )
+
+    owner = models.ForeignKey(
         TaxPayer,
-        related_name="profile",
-        verbose_name=_("taxpayer"),
+        related_name="points_of_sales",
+        verbose_name=_("owner"),
         on_delete=models.CASCADE,
     )
+
+    # The following fields are only used for PDF generation.
     issuing_name = models.CharField(
         max_length=128,
+        null=True,
         verbose_name=_("issuing name"),
         help_text=_("The name of the issuing entity as shown on receipts."),
     )
     issuing_address = models.TextField(
         _("issuing address"),
+        null=True,
         help_text=_("The address of the issuing entity as shown on receipts."),
     )
     issuing_email = models.CharField(
         max_length=128,
         verbose_name=_("issuing email"),
         blank=True,
         null=True,
@@ -527,84 +567,44 @@
         choices=(
             (
                 condition,
                 condition,
             )
             for condition in VAT_CONDITIONS
         ),
+        null=True,
         verbose_name=_("vat condition"),
     )
     gross_income_condition = models.CharField(
         max_length=48,
+        null=True,
         verbose_name=_("gross income condition"),
     )
     sales_terms = models.CharField(
         max_length=48,
+        null=True,
         verbose_name=_("sales terms"),
         help_text=_(
             "The terms of the sale printed onto receipts by default "
             "(eg: single payment, checking account, etc)."
         ),
     )
 
-    def __str__(self):
-        return f"<TaxPayerProfile for TaxPayer {self.pk}>"
-
-    class Meta:
-        verbose_name = _("taxpayer profile")
-        verbose_name_plural = _("taxpayer profiles")
-
-
-class PointOfSales(models.Model):
-    """
-    Represents an existing AFIP point of sale.
-
-    Points of sales need to be created via AFIP's web interface and it is
-    recommended that you use :meth:`~.TaxPayer.fetch_points_of_sales` to fetch
-    these programatically.
-
-    Note that deleting or altering these models will not affect upstream point
-    of sales.
-    """
-
-    number = models.PositiveSmallIntegerField(
-        _("number"),
-    )
-    issuance_type = models.CharField(
-        _("issuance type"),
-        max_length=24,
-        help_text="Indicates if this POS emits using CAE and CAEA.",
-    )
-    blocked = models.BooleanField(
-        _("blocked"),
-    )
-    drop_date = models.DateField(
-        _("drop date"),
-        null=True,
-        blank=True,
-    )
-
-    owner = models.ForeignKey(
-        TaxPayer,
-        related_name="points_of_sales",
-        verbose_name=_("owner"),
-        on_delete=models.CASCADE,
-    )
-
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.number)
 
     class Meta:
         unique_together = (("number", "owner"),)
         verbose_name = _("point of sales")
         verbose_name_plural = _("points of sales")
 
 
 class AuthTicketManager(models.Manager):
-    def get_any_active(self, service):
+    def get_any_active(self, service: str) -> AuthTicket:
+        """Return a valid, active ticket for a given service."""
         ticket = AuthTicket.objects.filter(
             token__isnull=False,
             expires__gt=datetime.now(timezone.utc),
             service=service,
         ).first()
         if ticket:
             return ticket
@@ -615,33 +615,39 @@
             raise exceptions.AuthenticationError(
                 _("There are no taxpayers to generate a ticket."),
             )
 
         return taxpayer.create_ticket(service)
 
 
+def default_generated() -> datetime:
+    """The default generated date for new tickets."""
+    return datetime.now(TZ_AR)
+
+
+def default_expires() -> datetime:
+    """The default expiration date for new tickets."""
+    tomorrow = datetime.now(TZ_AR) + timedelta(hours=12)
+    return tomorrow
+
+
+def default_unique_id() -> int:
+    """A random unique id for new tickets."""
+    return random.randint(0, 2147483647)
+
+
 class AuthTicket(models.Model):
     """An AFIP Authorization ticket.
 
     This is a signed ticket used to communicate with AFIP's webservices.
 
     Applications should not generally have to deal with these tickets
     themselves; most services will find or create one as necessary.
     """
 
-    def default_generated():
-        return datetime.now(TZ_AR)
-
-    def default_expires():
-        tomorrow = datetime.now(TZ_AR) + timedelta(hours=12)
-        return tomorrow
-
-    def default_unique_id():
-        return random.randint(0, 2147483647)
-
     owner = models.ForeignKey(
         TaxPayer,
         verbose_name=_("owner"),
         related_name="auth_tickets",
         on_delete=models.CASCADE,
     )
     unique_id = models.IntegerField(
@@ -670,40 +676,41 @@
     )
 
     objects = AuthTicketManager()
 
     TOKEN_XPATH = "/loginTicketResponse/credentials/token"
     SIGN_XPATH = "/loginTicketResponse/credentials/sign"
 
-    def __create_request_xml(self):
+    def __create_request_xml(self) -> bytes:
         request_xml = E.loginTicketRequest(
             {"version": "1.0"},
             E.header(
                 E.uniqueId(str(self.unique_id)),
                 E.generationTime(serializers.serialize_datetime(self.generated)),
                 E.expirationTime(serializers.serialize_datetime(self.expires)),
             ),
             E.service(self.service),
         )
+        # Hint: tostring returns bytes.
         return etree.tostring(request_xml, pretty_print=True)
 
-    def __sign_request(self, request):
+    def __sign_request(self, request: bytes) -> bytes:
         with self.owner.certificate.file.open("rb") as f:
             cert = f.read()
 
         with self.owner.key.file.open("rb") as f:
             key = f.read()
 
         return crypto.create_embeded_pkcs7_signature(request, cert, key)
 
-    def authorize(self):
+    def authorize(self) -> None:
         """Send this ticket to AFIP for authorization."""
-        request = self.__create_request_xml()
-        request = self.__sign_request(request)
-        request = base64.b64encode(request).decode()
+        request_xml = self.__create_request_xml()
+        signed_request = self.__sign_request(request_xml)
+        request = base64.b64encode(signed_request).decode()
 
         client = clients.get_client("wsaa", self.owner.is_sandboxed)
         try:
             raw_response = client.service.loginCms(request)
         except Fault as e:
             if str(e) == "Certificado expirado":
                 raise exceptions.CertificateExpired(str(e)) from e
@@ -713,26 +720,26 @@
         response = etree.fromstring(raw_response.encode("utf-8"))
 
         self.token = response.xpath(self.TOKEN_XPATH)[0].text
         self.signature = response.xpath(self.SIGN_XPATH)[0].text
 
         self.save()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.unique_id)
 
     class Meta:
         verbose_name = _("authorization ticket")
         verbose_name_plural = _("authorization tickets")
 
 
 class ReceiptQuerySet(models.QuerySet):
     """The default queryset obtains when querying via :class:`~.ReceiptManager`."""
 
-    def _assign_numbers(self):
+    def _assign_numbers(self) -> None:
         """Assign numbers in preparation for validating these receipts.
 
         WARNING: Don't call the method manually unless you know what you're
         doing!
         """
         first = self.select_related("point_of_sales", "receipt_type").first()
 
@@ -747,15 +754,15 @@
         for receipt in self.filter(receipt_number__isnull=True):
             # Atomically update receipt number
             Receipt.objects.filter(pk=receipt.id, receipt_number__isnull=True,).update(
                 receipt_number=next_num,
             )
             next_num += 1
 
-    def check_groupable(self):
+    def check_groupable(self) -> ReceiptQuerySet:
         """Check that all receipts returned by this queryset are groupable.
 
         "Groupable" means that they can be validated together: they have the
         same POS and receipt type.
 
         Returns the same queryset is all receipts are groupable, otherwise,
         raises :class:`~.CannotValidateTogether`.
@@ -768,15 +775,15 @@
         )
 
         if set(types.values()) > {1}:
             raise exceptions.CannotValidateTogether()
 
         return self
 
-    def validate(self, ticket=None):
+    def validate(self, ticket: AuthTicket = None) -> list[str]:
         """Validate all receipts matching this queryset.
 
         Note that, due to how AFIP implements its numbering, this method is not
         thread-safe, or even multiprocess-safe.
 
         Because of this, it is possible that not all instances matching this
         queryset are validated properly. Obviously, only successfully validated
@@ -798,15 +805,15 @@
         qs = self.filter(validation__isnull=True).check_groupable()
         if qs.count() == 0:
             return []
         qs.order_by("issued_date", "id")._assign_numbers()
 
         return qs._validate(ticket)
 
-    def _validate(self, ticket=None):
+    def _validate(self, ticket=None) -> list[str]:
         first = self.first()
         ticket = ticket or first.point_of_sales.owner.get_or_create_ticket("wsfe")
         client = clients.get_client("wsfe", first.point_of_sales.owner.is_sandboxed)
         response = client.service.FECAESolicitar(
             serializers.serialize_ticket(ticket),
             serializers.serialize_multiple_receipts(self),
         )
@@ -849,15 +856,19 @@
 
 class ReceiptManager(models.Manager):
     """Default manager for the :class:`~.Receipt` class.
 
     You should generally access this using ``Receipt.objects``.
     """
 
-    def fetch_last_receipt_number(self, point_of_sales, receipt_type):
+    def fetch_last_receipt_number(
+        self,
+        point_of_sales: PointOfSales,
+        receipt_type: ReceiptType,
+    ) -> int:
         """Returns the number for the last validated receipt."""
         client = clients.get_client("wsfe", point_of_sales.owner.is_sandboxed)
         response_xml = client.service.FECompUltimoAutorizado(
             serializers.serialize_ticket(
                 point_of_sales.owner.get_or_create_ticket("wsfe")
             ),
             point_of_sales.number,
@@ -878,15 +889,41 @@
         #                Msg = "CUIT representada no incluida en Token"
         #             },
         #       }
         #  }
 
         return response_xml.CbteNro
 
-    def get_queryset(self):
+    def fetch_receipt_data(
+        self,
+        receipt_type: ReceiptType,
+        receipt_number: int,
+        point_of_sales: PointOfSales,
+    ):  # TODO: Wrap this in a dataclass
+        """Returns receipt related data"""
+
+        if not receipt_number:
+            return None
+
+        client = clients.get_client("wsfe", point_of_sales.owner.is_sandboxed)
+        response_xml = client.service.FECompConsultar(
+            serializers.serialize_ticket(
+                point_of_sales.owner.get_or_create_ticket("wsfe")
+            ),
+            serializers.serialize_receipt_data(
+                receipt_type, receipt_number, point_of_sales.number
+            ),
+        )
+        try:
+            check_response(response_xml)
+            return response_xml.ResultGet
+        except exceptions.AfipException:
+            return None
+
+    def get_queryset(self) -> ReceiptQuerySet:
         return ReceiptQuerySet(self.model, using=self._db).select_related(
             "receipt_type",
         )
 
 
 class Receipt(models.Model):
     """A receipt, as sent to AFIP.
@@ -1028,27 +1065,27 @@
 
     objects = ReceiptManager()
 
     # TODO: Not implemented: optionals
     # TODO: methods to validate totals
 
     @property
-    def total_vat(self):
+    def total_vat(self) -> int:
         """Returns the sum of all Vat objects."""
         q = Vat.objects.filter(receipt=self).aggregate(total=Sum("amount"))
         return q["total"] or 0
 
     @property
-    def total_tax(self):
+    def total_tax(self) -> int:
         """Returns the sum of all Tax objects."""
         q = Tax.objects.filter(receipt=self).aggregate(total=Sum("amount"))
         return q["total"] or 0
 
     @property
-    def formatted_number(self):
+    def formatted_number(self) -> str | None:
         """This receipt's number in the usual format: ``0001-00003087``."""
         if self.receipt_number:
             return "{:04d}-{:08d}".format(
                 self.point_of_sales.number,
                 self.receipt_number,
             )
         return None
@@ -1072,16 +1109,16 @@
             return False
 
         try:
             return self.validation.result == ReceiptValidation.RESULT_APPROVED
         except ReceiptValidation.DoesNotExist:
             return False
 
-    def validate(self, ticket=None, raise_=False):
-        """Validate this receipt.
+    def validate(self, ticket: AuthTicket = None, raise_=False) -> list[str]:
+        """Validates this receipt.
 
         This is a shortcut to :class:`~.ReceiptQuerySet`'s method of the same
         name. Calling this validates only this instance.
 
         :param AuthTicket ticket: Use this ticket. If None, one will be loaded
             or created automatically.
         :param bool raise_: If True, an exception will be raised when
@@ -1092,64 +1129,100 @@
         # Since we're operating via a queryset, this instance isn't properly
         # updated:
         self.refresh_from_db()
         if raise_ and rv:
             raise exceptions.ValidationError(rv[0])
         return rv
 
-    def __repr__(self):
+    def revalidate(self) -> ReceiptValidation | None:
+        """Revalidate this receipt.
+
+        Fetches data of a validated receipt from AFIP's servers.
+        If the receipt exists a ``ReceiptValidation`` instance is
+        created and returned, otherwise, returns ``None``.
+        If there is already a ``ReceiptValidation`` for this instance,
+        returns ``self.validation``.
+        This should be used for verification purpose, here's a list of
+        some use cases:
+         - Incomplete validation process
+         - Fetch CAE data from AFIP's servers
+        """
+        # This may avoid unnecessary revalidation
+        if self.is_validated:
+            return self.validation
+
+        receipt_data = Receipt.objects.fetch_receipt_data(
+            self.receipt_type.code, self.receipt_number, self.point_of_sales
+        )
+
+        if not receipt_data:
+            return None
+
+        if receipt_data.Resultado == ReceiptValidation.RESULT_APPROVED:
+            validation = ReceiptValidation.objects.create(
+                result=receipt_data.Resultado,
+                cae=receipt_data.CodAutorizacion,
+                cae_expiration=parsers.parse_date(receipt_data.FchVto),
+                receipt=self,
+                processed_date=parsers.parse_datetime(
+                    receipt_data.FchProceso,
+                ),
+            )
+            if receipt_data.Observaciones:
+                for obs in receipt_data.Observaciones.Obs:
+                    observation = Observation.objects.get_or_create(
+                        code=obs.Code,
+                        message=obs.Msg,
+                    )
+                validation.observations.add(observation)
+            return validation
+        return None
+
+    def __repr__(self) -> str:
         return "<Receipt {}: {} {} for {}>".format(
             self.pk,
             self.receipt_type,
             self.receipt_number,
             self.point_of_sales.owner,
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.receipt_number:
-            return "{} {}".format(self.receipt_type, self.formatted_number)
+            return f"{self.receipt_type} {self.formatted_number}"
         else:
             return _("Unnumbered %s") % self.receipt_type
 
     class Meta:
         ordering = ("issued_date",)
         verbose_name = _("receipt")
         verbose_name_plural = _("receipts")
         unique_together = [["point_of_sales", "receipt_type", "receipt_number"]]
         # TODO: index_together...
 
 
 class ReceiptPDFManager(models.Manager):
-    def create_for_receipt(self, receipt: Receipt, **kwargs):
+    def create_for_receipt(self, receipt: Receipt, **kwargs) -> ReceiptPDF:
         """Creates a ReceiptPDF object for a given receipt.
 
         Does not actually generate the related PDF file.
 
         All attributes will be completed with the information for the relevant
-        ``TaxPayerProfile`` instance.
+        :class:`~.PointOfSales` instance.
 
         :param Receipt receipt: The receipt for the PDF which will be
             generated.
         """
-        try:
-            profile = TaxPayerProfile.objects.get(
-                taxpayer__points_of_sales__receipts=receipt,
-            )
-        except TaxPayerProfile.DoesNotExist:
-            raise exceptions.DjangoAfipException(
-                "Cannot generate a PDF for taxpayer with no profile",
-            )
         pdf = ReceiptPDF.objects.create(
             receipt=receipt,
-            issuing_name=profile.issuing_name,
-            issuing_address=profile.issuing_address,
-            issuing_email=profile.issuing_email,
-            vat_condition=profile.vat_condition,
-            gross_income_condition=profile.gross_income_condition,
-            sales_terms=profile.sales_terms,
+            issuing_name=receipt.point_of_sales.issuing_name,
+            issuing_address=receipt.point_of_sales.issuing_address,
+            issuing_email=receipt.point_of_sales.issuing_email,
+            vat_condition=receipt.point_of_sales.vat_condition,
+            gross_income_condition=receipt.point_of_sales.gross_income_condition,
+            sales_terms=receipt.point_of_sales.sales_terms,
             **kwargs,
         )
         return pdf
 
 
 class ReceiptPDF(models.Model):
     """Printable version of a receipt.
@@ -1164,15 +1237,15 @@
     generated when saving the model for the first time. If any attributes are
     changed, you should manually call :meth:`~.ReceiptPDF.save_pdf` to
     regenerate the PDF file.
 
     PDF generation is skipped if the receipt has not been validated.
     """
 
-    def upload_to(self, filename="untitled", instance=None):
+    def upload_to(self, filename="untitled", instance: ReceiptPDF = None) -> str:
         """
         Returns the full path for generated receipts.
 
         These are bucketed inside nested directories, to avoid hundreds of
         thousands of children in single directories (which can make reading
         them excessively slow).
         """
@@ -1247,15 +1320,15 @@
         max_length=48,
         verbose_name=_("sales terms"),
         help_text=_('Should be something like "Cash", "Payable in 30 days", etc.'),
     )
 
     objects = ReceiptPDFManager()
 
-    def save_pdf(self, save_model: bool = True):
+    def save_pdf(self, save_model: bool = True) -> None:
         """
         Save the receipt as a PDF related to this model.
 
         The related :class:`~.Receipt` should be validated first, of course.
         This model instance must have been saved prior to calling this method.
 
         :param save_model: If True, immediately save this model instance.
@@ -1263,25 +1336,25 @@
         from django_afip.views import ReceiptPDFView
 
         if not self.receipt.is_validated:
             raise exceptions.DjangoAfipException(
                 _("Cannot generate pdf for non-authorized receipt")
             )
 
-        self.pdf_file = File(BytesIO(), name="{}.pdf".format(uuid4().hex))
+        self.pdf_file = File(BytesIO(), name=f"{uuid4().hex}.pdf")
         render_pdf(
             template=ReceiptPDFView().get_template_names(self.receipt),
             file_=self.pdf_file,
             context=ReceiptPDFView.get_context_for_pk(self.receipt_id),
         )
 
         if save_model:
             self.save()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return _("Receipt PDF for %s") % self.receipt_id
 
     class Meta:
         verbose_name = _("receipt pdf")
         verbose_name_plural = _("receipt pdfs")
 
 
@@ -1320,15 +1393,15 @@
         verbose_name=_("vat"),
         blank=True,
         null=True,
         on_delete=models.PROTECT,
     )
 
     @property
-    def total_price(self):
+    def total_price(self) -> int:
         """The total price for this line (quantity * price)."""
         return self.quantity * self.unit_price
 
     class Meta:
         verbose_name = _("receipt entry")
         verbose_name_plural = _("receipt entries")
 
@@ -1363,15 +1436,15 @@
 
     receipt = models.ForeignKey(
         Receipt,
         related_name="taxes",
         on_delete=models.PROTECT,
     )
 
-    def compute_amount(self):
+    def compute_amount(self) -> int:
         """Auto-assign and return the total amount for this tax."""
         self.amount = self.base_amount * self.aliquot / 100
         return self.amount
 
     class Meta:
         verbose_name = _("tax")
         verbose_name_plural = _("taxes")
@@ -1476,21 +1549,21 @@
         Receipt,
         related_name="validation",
         verbose_name=_("receipt"),
         help_text=_("The Receipt for which this validation applies."),
         on_delete=models.PROTECT,
     )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return _("Validation for %s. Result: %s") % (
             self.receipt,
             self.get_result_display(),
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<{} {}: {} for Receipt {}>".format(
             self.__class__.__name__,
             self.pk,
             self.result,
             self.receipt_id,
         )
```

### Comparing `django-afip-8.0.4/django_afip/pdf.py` & `django-afip-9.0.0/django_afip/pdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import json
 import logging
 from io import BytesIO
 
 import qrcode
 from PIL import Image
 
+from django_afip.models import Receipt
 
 logger = logging.getLogger(__name__)
 
 
 class ReceiptQrCode:
     # Note: There's a space in the middle in the docs.
     # I'm assuming it's a human error and that the URL doesn't take a space.
     BASE_URL = "https://www.afip.gob.ar/fe/qr/?p="
 
-    def __init__(self, receipt):
+    def __init__(self, receipt: Receipt):
         self._receipt = receipt
         # The examples on the website say that "importe" and "ctz" are both "decimal"
         # type. JS/JSON has no decimal type. The examples use integeres.
         #
         # Using integers would drop cents, which would result in mismatching
         # information. Using strings would add quotes, which likely breaks.
         #
```

### Comparing `django-afip-8.0.4/django_afip/serializers.py` & `django-afip-9.0.0/django_afip/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,7 +115,13 @@
 
 def serialize_vat(vat):
     return f.AlicIva(
         Id=vat.vat_type.code,
         BaseImp=vat.base_amount,
         Importe=vat.amount,
     )
+
+
+def serialize_receipt_data(receipt_type, receipt_number, point_of_sales):
+    return f.FECompConsultaReq(
+        CbteTipo=receipt_type, CbteNro=receipt_number, PtoVta=point_of_sales
+    )
```

### Comparing `django-afip-8.0.4/django_afip/signals.py` & `django-afip-9.0.0/django_afip/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from django.db.models.signals import pre_save
 from django.dispatch import receiver
 
 from django_afip import models
 
 
 @receiver(pre_save, sender=models.TaxPayer)
-def update_certificate_expiration(sender, instance, **kwargs):
+def update_certificate_expiration(sender, instance: models.TaxPayer, **kwargs):
     if instance.certificate:
         instance.certificate_expiration = instance.get_certificate_expiration()
 
 
 @receiver(post_save, sender=models.ReceiptPDF)
-def generate_receipt_pdf(sender, instance, **kwargs):
+def generate_receipt_pdf(sender, instance: models.ReceiptPDF, **kwargs):
     if not instance.pdf_file and instance.receipt.is_validated:
         instance.save_pdf(save_model=True)
```

### Comparing `django-afip-8.0.4/django_afip/static/receipts/receipt.css` & `django-afip-9.0.0/django_afip/static/receipts/receipt.css`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/templates/receipts/code_11.html` & `django-afip-9.0.0/django_afip/templates/receipts/code_11.html`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/templates/receipts/code_13.html` & `django-afip-9.0.0/django_afip/templates/receipts/code_13.html`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/templates/receipts/code_3.html` & `django-afip-9.0.0/django_afip/templates/receipts/code_3.html`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/templates/receipts/code_6.html` & `django-afip-9.0.0/django_afip/templates/receipts/code_6.html`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/templates/receipts/code_8.html` & `django-afip-9.0.0/django_afip/templates/receipts/code_8.html`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/testing/test.crt` & `django-afip-9.0.0/django_afip/testing/test.crt`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/testing/test.key` & `django-afip-9.0.0/django_afip/testing/test.key`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/testing/test2.crt` & `django-afip-9.0.0/django_afip/testing/test2.crt`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/testing/test2.key` & `django-afip-9.0.0/django_afip/testing/test2.key`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/testing/test_expired.crt` & `django-afip-9.0.0/django_afip/testing/test_expired.crt`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/testing/test_expired.key` & `django-afip-9.0.0/django_afip/testing/test_expired.key`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/django_afip/views.py` & `django-afip-9.0.0/django_afip/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.utils.functional import cached_property
 from django_renderpdf.views import PDFView
 
 from django_afip import models
 from django_afip.pdf import get_encoded_qrcode
 
-
 # Note: When updating this, be sure to update the docstring of the method that uses
 # these below.
 TEMPLATE_NAMES = [
     "receipts/{taxpayer}/pos_{point_of_sales}/code_{code}.html",
     "receipts/{taxpayer}/code_{code}.html",
     "receipts/code_{code}.html",
     "receipts/{code}.html",
```

### Comparing `django-afip-8.0.4/django_afip.egg-info/PKG-INFO` & `django-afip-9.0.0/django_afip.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,109 @@
 Metadata-Version: 2.1
 Name: django-afip
-Version: 8.0.4
+Version: 9.0.0
 Summary: AFIP integration for django
 Home-page: https://github.com/WhyNotHugo/django-afip
 Author: Hugo Osvaldo Barrera
 Author-email: hugo@barrera.io
 License: ISC
-Description: django-afip
-        ===========
-        
-        .. image:: https://travis-ci.com/WhyNotHugo/django-afip.svg?branch=main
-          :target: https://travis-ci.com/WhyNotHugo/django-afip
-          :alt: build status
-        
-        .. image:: https://codecov.io/gh/WhyNotHugo/django-afip/branch/main/graph/badge.svg
-          :target: https://codecov.io/gh/WhyNotHugo/django-afip
-          :alt: Build coverage
-        
-        .. image:: https://readthedocs.org/projects/django-afip/badge/?version=latest
-          :target: http://django-afip.readthedocs.io/en/latest/?badge=latest
-          :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/pypi/v/django-afip.svg
-          :target: https://pypi.python.org/pypi/django-afip
-          :alt: version on pypi
-        
-        .. image:: https://img.shields.io/pypi/dm/django-afip.svg
-          :target: https://pypi.python.org/pypi/django-afip
-          :alt: downloads
-        
-        .. image:: https://img.shields.io/pypi/l/django-afip.svg
-          :target: https://github.com/WhyNotHugo/django-afip/blob/main/LICENCE
-          :alt: licence
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-          :target: https://github.com/WhyNotHugo/django-afip/
-          :alt: code style: black
-        
-        What's this?
-        ------------
-        
-        AFIP is Argentina's tax collection agency. For emitting invoices, taxpayers are
-        required to inform AFIP of each invoice by using a dedicated SOAP-like web
-        service for that.
-        
-        **django-afip** is a Django application implementing the necessary bits for
-        Django-based applications to both store and comunícate invoicing information.
-        
-        Features
-        --------
-        
-        * Validate invoices and other receipt types with AFIP's WSFE service.
-        * Generate valid PDF files for those receipts to send to clients.
-        
-        Documentation
-        -------------
-        
-        The full documentation is available at https://django-afip.readthedocs.io/
-        
-        Donate
-        ------
-        
-        While some of the work done here is done for clients, much of it is done in my
-        free time. If you appreciate the work done here, please consider donating_.
-        
-        .. _donating: https://github.com/sponsors/WhyNotHugo
-        
-        Licence
-        -------
-        
-        This software is distributed under the ISC licence. See LICENCE for details.
-        
-        Copyright (c) 2015-2020 Hugo Osvaldo Barrera <hugo@barrera.io>
-        
+Project-URL: Documentation, https://django-afip.readthedocs.io/
+Project-URL: Issue Tracker, https://github.com/WhyNotHugo/django-afip/issues
+Project-URL: Donate, https://liberapay.com/WhyNotHugo/
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: postgres
 Provides-Extra: mysql
 Provides-Extra: factories
+License-File: LICENCE
+
+django-afip
+===========
+
+.. image:: https://github.com/WhyNotHugo/django-afip/actions/workflows/tests.yml/badge.svg
+  :target: https://github.com/WhyNotHugo/django-afip/actions/workflows/tests.yml
+  :alt: unit tests
+
+.. image:: https://github.com/WhyNotHugo/django-afip/actions/workflows/live.yml/badge.svg
+  :target: https://github.com/WhyNotHugo/django-afip/actions/workflows/live.yml
+  :alt: integrations tests
+
+.. image:: https://results.pre-commit.ci/badge/github/WhyNotHugo/django-afip/main.svg
+  :target: https://results.pre-commit.ci/latest/github/WhyNotHugo/django-afip/main
+  :alt: pre-commit.ci status
+
+.. image:: https://codecov.io/gh/WhyNotHugo/django-afip/branch/main/graph/badge.svg
+  :target: https://codecov.io/gh/WhyNotHugo/django-afip
+  :alt: Build coverage
+
+.. image:: https://readthedocs.org/projects/django-afip/badge/?version=latest
+  :target: http://django-afip.readthedocs.io/en/latest/?badge=latest
+  :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/django-afip.svg
+  :target: https://pypi.python.org/pypi/django-afip
+  :alt: version on pypi
+
+.. image:: https://img.shields.io/pypi/dm/django-afip.svg
+  :target: https://pypi.python.org/pypi/django-afip
+  :alt: downloads
+
+.. image:: https://img.shields.io/pypi/l/django-afip.svg
+  :target: https://github.com/WhyNotHugo/django-afip/blob/main/LICENCE
+  :alt: licence
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+  :target: https://github.com/WhyNotHugo/django-afip/
+  :alt: code style: black
+
+What's this?
+------------
+
+AFIP is Argentina's tax collection agency. For emitting invoices, taxpayers are
+required to inform AFIP of each invoice by using a dedicated SOAP-like web
+service for that.
+
+**django-afip** is a Django application implementing the necessary bits for
+Django-based applications to both store and comunícate invoicing information.
+
+Features
+--------
+
+* Validate invoices and other receipt types with AFIP's WSFE service.
+* Generate valid PDF files for those receipts to send to clients.
+
+Documentation
+-------------
+
+The full documentation is available at https://django-afip.readthedocs.io/
+
+Donate
+------
+
+While some of the work done here is done for clients, much of it is done in my
+free time. If you appreciate the work done here, please consider donating_.
+
+.. _donating: https://github.com/sponsors/WhyNotHugo
+
+Licence
+-------
+
+This software is distributed under the ISC licence. See LICENCE for details.
+
+Copyright (c) 2015-2020 Hugo Osvaldo Barrera <hugo@barrera.io>
+
+
```

### Comparing `django-afip-8.0.4/django_afip.egg-info/SOURCES.txt` & `django-afip-9.0.0/django_afip.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 .gitignore
 .pre-commit-config.yaml
 .pypirc
+.pyup.yml
+.readthedocs.yaml
 CHANGELOG.rst
 LICENCE
 README.rst
-codecov.yml
 setup.cfg
 setup.py
 tox.ini
 .github/.kodiak.toml
 .github/FUNDING.yml
 .github/no-response.yml
 .github/ISSUE_TEMPLATE/question.md
-.github/workflows/checks.yml
-.github/workflows/docs.yml
+.github/workflows/live.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 django_afip/__init__.py
 django_afip/admin.py
 django_afip/apps.py
 django_afip/clients.py
 django_afip/crypto.py
 django_afip/exceptions.py
 django_afip/factories.py
+django_afip/helpers.py
 django_afip/models.py
 django_afip/parsers.py
 django_afip/pdf.py
 django_afip/serializers.py
 django_afip/signals.py
 django_afip/version.py
 django_afip/views.py
@@ -46,14 +47,16 @@
 django_afip/management/commands/afipmetadata.py
 django_afip/migrations/0001_squashed_0036_receiptpdf__client_address__blank.py
 django_afip/migrations/0002_taxpayerextras.py
 django_afip/migrations/0003_issuance_type_length.py
 django_afip/migrations/0004_storages_and_help_texts.py
 django_afip/migrations/0005_flatten_taxpayer_extras.py
 django_afip/migrations/0006_delete_taxpayerextras.py
+django_afip/migrations/0007_auto_20210409_1641.py
+django_afip/migrations/0008_move_taxpayerprofile_to_pos.py
 django_afip/migrations/__init__.py
 django_afip/static/receipts/receipt.css
 django_afip/templates/receipts/code_11.html
 django_afip/templates/receipts/code_13.html
 django_afip/templates/receipts/code_3.html
 django_afip/templates/receipts/code_6.html
 django_afip/templates/receipts/code_8.html
@@ -79,27 +82,28 @@
 docs/usage.rst
 docs/_ext/django_models.py
 scripts/dump_metadata.py
 testapp/conftest.py
 testapp/django_afip
 testapp/manage.py
 testapp/signed_data.bin
+testapp/test_helpers.py
 testapp/testapp/__init__.py
 testapp/testapp/settings.py
 testapp/testapp/urls.py
 testapp/testapp/wsgi.py
 testapp/testapp/testmain/__init__.py
 testapp/testapp/testmain/views.py
 testapp/testapp/testmain/templates/receipts/20329642330/pos_9999/code_6.html
 testapp/testapp/testmain/tests/__init__.py
 testapp/testapp/testmain/tests/test_admin.py
 testapp/testapp/testmain/tests/test_clients.py
 testapp/testapp/testmain/tests/test_crypto.py
 testapp/testapp/testmain/tests/test_management.py
+testapp/testapp/testmain/tests/test_migrations.py
 testapp/testapp/testmain/tests/test_models.py
 testapp/testapp/testmain/tests/test_parsers.py
 testapp/testapp/testmain/tests/test_pdf.py
 testapp/testapp/testmain/tests/test_tags.py
 testapp/testapp/testmain/tests/test_taxpayer.py
 testapp/testapp/testmain/tests/test_views.py
-testapp/testapp/testmain/tests/test_webservices.py
-testapp/testapp/testmain/tests/testcases.py
+testapp/testapp/testmain/tests/test_webservices.py
```

### Comparing `django-afip-8.0.4/docs/Makefile` & `django-afip-9.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/docs/_ext/django_models.py` & `django-afip-9.0.0/docs/_ext/django_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 
             help_text = strip_tags(force_text(field.help_text))
             verbose_name = force_text(field.verbose_name).capitalize()
 
             if help_text:
                 # Add the model field to the end of the docstring as a param
                 # using the help text as the description
-                lines.append(":param {}: {}".format(field.attname, help_text))
+                lines.append(f":param {field.attname}: {help_text}")
             else:
                 # Add the model field to the end of the docstring as a param
                 # using the verbose name as the description
-                lines.append(":param {}: {}".format(field.attname, verbose_name))
+                lines.append(f":param {field.attname}: {verbose_name}")
 
             # Add the field's type to the docstring
             if isinstance(field, models.ForeignKey):
                 to = field.remote_field.model
                 lines.append(
                     ":type {}: {} to :class:`~{}.{}`".format(
                         field.attname, type(field).__name__, to.__module__, to.__name__
                     )
                 )
             else:
-                lines.append(":type {}: {}".format(field.attname, type(field).__name__))
+                lines.append(f":type {field.attname}: {type(field).__name__}")
 
     # Return the extended docstring
     return lines
 
 
 def setup(app):
     """Register the docstring processor with sphinx."""
```

### Comparing `django-afip-8.0.4/docs/api.rst` & `django-afip-9.0.0/docs/api.rst`

 * *Files 15% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 additional non-validated metadata. You DO NOT need any of these classes
 unless you intend to generate PDFs for receipts.
 
 .. autoclass:: django_afip.models.ReceiptEntry
     :members:
 .. autoclass:: django_afip.models.ReceiptPDF
     :members:
-.. autoclass:: django_afip.models.TaxPayerProfile
-    :members:
+
+.. _metadata-models:
 
 Metadata models
 ---------------
 
 These models represent metadata like currency types or document types.
 
 You should make sure you populate these tables either via the ``afipmetadata``
@@ -73,7 +73,15 @@
 ---------
 
 QuerySets are generally accessed via their models. For example,
 ``Receipt.objects.filter()`` will return a ``ReceiptQuerySet``.
 
 .. autoclass:: django_afip.models.ReceiptQuerySet
     :members:
+
+Helpers
+-------
+
+.. autofunction:: django_afip.helpers.get_server_status
+
+.. autoclass:: django_afip.helpers.ServerStatus
+    :members:
```

### Comparing `django-afip-8.0.4/docs/conf.py` & `django-afip-9.0.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from os.path import dirname
 from os.path import join
 
 import django
 
 import django_afip
 
-
 BASE_DIR = dirname(dirname(abspath(__file__)))
 
 sys.path.insert(0, abspath(join(dirname(__file__), "_ext")))
 sys.path.insert(0, abspath(join(BASE_DIR, "testapp")))
 
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", "testapp.settings")
 
@@ -45,16 +44,28 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "django_models",
+    "sphinx.ext.intersphinx",
 ]
 
+intersphinx_mapping = {
+    "django": (
+        "https://docs.djangoproject.com/en/stable/",
+        "https://docs.djangoproject.com/en/stable/_objects/",
+    ),
+    "weasyprint": (
+        "https://doc.courtbouillon.org/weasyprint/stable/",
+        None,
+    ),
+}
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 
 # The master toctree document.
 master_doc = "index"
 
@@ -65,20 +76,18 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_collapse": False,
-}
+# html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
```

### Comparing `django-afip-8.0.4/scripts/dump_metadata.py` & `django-afip-9.0.0/scripts/dump_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 This script is used to generate the fixtures with AFIP metadata. It is only used to
 BUILD django_afip, and should not be used directly by third-party apps.
 """
 import django
 from django.core import management
 
-
 if __name__ == "__main__":
     # Set up django...
     django.setup()
     management.call_command("migrate")
 
     from django_afip.factories import TaxPayerFactory
     from django_afip.models import GenericAfipType
```

### Comparing `django-afip-8.0.4/setup.py` & `django-afip-9.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 
 setup(
     name="django-afip",
     description="AFIP integration for django",
     author="Hugo Osvaldo Barrera",
     author_email="hugo@barrera.io",
     url="https://github.com/WhyNotHugo/django-afip",
+    project_urls={
+        "Documentation": "https://django-afip.readthedocs.io/",
+        "Issue Tracker": "https://github.com/WhyNotHugo/django-afip/issues",
+        "Donate": "https://liberapay.com/WhyNotHugo/",
+    },
     license="ISC",
     packages=find_packages(),
     include_package_data=True,
     long_description=open("README.rst").read(),
     install_requires=[
         "cryptography>=3.2,<4.0",
-        "django>=2.0.0,<3.2",
+        "django>=3.1,<3.3",
         "django_renderpdf>=3.0.0,<4.0.0",
         "lxml>=3.4.4",
         "pyopenssl>=16.2.0",
         "pytz>=2015.4",
         "setuptools-git>=1.1",
         "setuptools-scm>=1.7.0",
         "wheel>=0.24.0",
-        "zeep>=1.1.0,<4.0.0",
+        "zeep>=1.1.0,<5.0.0",
         "qrcode[pil]>=6.1,<7.0",
         "pyyaml>=5.3.1,<6.0.0",
     ],
     extras_require={
         "docs": ["Sphinx", "sphinx-autobuild"],
         "postgres": ["psycopg2"],
         "mysql": ["mysqlclient"],
@@ -37,21 +42,21 @@
         "write_to": "django_afip/version.py",
     },
     setup_requires=["setuptools_scm"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
+        "Framework :: Django :: 3.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: ISC License (ISCL)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `django-afip-8.0.4/testapp/signed_data.bin` & `django-afip-9.0.0/testapp/signed_data.bin`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/testapp/testapp/settings.py` & `django-afip-9.0.0/testapp/testapp/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
+from pathlib import Path
 
 import dj_database_url
 
 # Build paths inside the project like this: os.path.join(BASE_DIR, ...)
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+BASE_DIR = Path(__file__).resolve().parent.parent
 
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/1.8/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "dm=3#ff_%6wpr8ynq!r_+kdl$c!$gez$@x!o==k1k96im4ckk+"
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
-ALLOWED_HOSTS = []
+ALLOWED_HOSTS: list = []
 
 
 # Application definition
 
 INSTALLED_APPS = (
     "django.contrib.admin",
     "django.contrib.auth",
@@ -57,25 +58,16 @@
             ],
         },
     },
 ]
 
 WSGI_APPLICATION = "testapp.wsgi.application"
 
-
 # Database
-database_urls = {
-    "mysql": "mysql://root@localhost:3306",
-    "postgres": "postgres://postgres@localhost:5432",
-    "sqlite": "sqlite:///db.sqlite3",
-}
-database_type = os.environ.get("DB", "sqlite")
-
-DATABASES = {"default": dj_database_url.parse(database_urls[database_type])}
-
+DATABASES = {"default": dj_database_url.config()}
 
 # Internationalization
 # https://docs.djangoproject.com/en/1.8/topics/i18n/
 
 LANGUAGE_CODE = "en-us"
 
 TIME_ZONE = "UTC"
```

### Comparing `django-afip-8.0.4/testapp/testapp/testmain/tests/test_crypto.py` & `django-afip-9.0.0/testapp/testapp/testmain/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/testapp/testapp/testmain/tests/test_models.py` & `django-afip-9.0.0/testapp/testapp/testmain/tests/test_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,240 +1,329 @@
-from unittest.mock import call
 from unittest.mock import MagicMock
+from unittest.mock import call
 from unittest.mock import patch
 
-from django.test import TestCase
+import pytest
+from pytest_django.asserts import assertQuerysetEqual
 
 from django_afip import exceptions
 from django_afip import factories
 from django_afip import models
-from testapp.testmain.tests.testcases import PopulatedLiveAfipTestCase
+from django_afip.factories import ReceiptFactory
+from django_afip.factories import ReceiptValidationFactory
+from django_afip.factories import ReceiptWithApprovedValidation
+from django_afip.factories import ReceiptWithInconsistentVatAndTaxFactory
+from django_afip.factories import ReceiptWithVatAndTaxFactory
 
 
-class ReceiptQuerySetTestCase(TestCase):
-    def test_default_manager(self):
-        self.assertIsInstance(
-            models.Receipt.objects.all(),
-            models.ReceiptQuerySet,
-        )
+def test_default_receipt_queryset():
+    assert isinstance(models.Receipt.objects.all(), models.ReceiptQuerySet)
 
-    def test_validate(self):
-        receipt = factories.ReceiptFactory()
-        queryset = models.Receipt.objects.filter(pk=receipt.pk)
-        ticket = MagicMock()
 
-        with patch(
-            "django_afip.models.ReceiptQuerySet._assign_numbers",
-            spec=True,
-        ) as mocked_assign_numbers, patch(
-            "django_afip.models.ReceiptQuerySet._validate",
-            spec=True,
-        ) as mocked__validate:
-            queryset.validate(ticket)
+@pytest.mark.django_db
+def test_validate():
+    receipt = ReceiptFactory()
+    queryset = models.Receipt.objects.filter(pk=receipt.pk)
+    ticket = MagicMock()
 
-        self.assertEqual(mocked_assign_numbers.call_count, 1)
+    with patch(
+        "django_afip.models.ReceiptQuerySet._assign_numbers",
+        spec=True,
+    ) as mocked_assign_numbers, patch(
+        "django_afip.models.ReceiptQuerySet._validate",
+        spec=True,
+    ) as mocked__validate:
+        queryset.validate(ticket)
 
-        self.assertEqual(mocked__validate.call_count, 1)
-        self.assertEqual(mocked__validate.call_args, call(ticket))
+    assert mocked_assign_numbers.call_count == 1
+    assert mocked__validate.call_count == 1
+    assert mocked__validate.call_args == call(ticket)
 
-        # TODO: Also another tests that checks that we only pass filtered-out
-        # receipts
 
+# TODO: Also another tests that checks that we only pass filtered-out receipts.
 
-class ReceiptManagerTestCase(TestCase):
-    def test_default_manager(self):
-        self.assertIsInstance(models.Receipt.objects, models.ReceiptManager)
 
+def test_default_receipt_manager():
+    assert isinstance(models.Receipt.objects, models.ReceiptManager)
 
-class ReceiptTestCase(TestCase):
-    def test_validate(self):
-        receipt = factories.ReceiptFactory()
-        ticket = MagicMock()
-        self.called = False
 
-        def fake_validate(qs, ticket=None):
-            self.assertQuerysetEqual(qs, [receipt.pk], lambda r: r.pk)
-            self.called = True
+@pytest.mark.django_db
+def test_validate_receipt():
+    receipt = ReceiptFactory()
+    ticket = MagicMock()
+    ticket._called = False
 
-        with patch(
-            "django_afip.models.ReceiptQuerySet.validate",
-            fake_validate,
-        ):
-            receipt.validate(ticket)
+    def fake_validate(qs, ticket=None):
+        assertQuerysetEqual(qs, [receipt.pk], lambda r: r.pk)
+        ticket._called = True
 
-        self.assertTrue(self.called)
+    with patch(
+        "django_afip.models.ReceiptQuerySet.validate",
+        fake_validate,
+    ):
+        receipt.validate(ticket)
 
+    assert ticket._called is True
 
-class ReceiptSuccessfulValidateTestCase(PopulatedLiveAfipTestCase):
-    def create_receipt(self, receipt_type_code=6) -> models.Receipt:
-        """Create a receipt use for tests. Default type is Factura B."""
 
-        receipt = factories.ReceiptFactory(
-            point_of_sales=models.PointOfSales.objects.first(),
-            receipt_type__code=receipt_type_code,
-        )
-        factories.VatFactory(vat_type__code=5, receipt=receipt)
-        factories.TaxFactory(tax_type__code=3, receipt=receipt)
+@pytest.mark.django_db
+@pytest.mark.live
+def test_validate_invoice(populated_db):
+    """Test validating valid receipts."""
 
-        return receipt
+    receipt = ReceiptWithVatAndTaxFactory()
+    errs = receipt.validate()
 
-    def test_validate_invoice(self):
-        """Test validating valid receipts."""
+    assert len(errs) == 0
+    assert receipt.validation.result == models.ReceiptValidation.RESULT_APPROVED
+    assert models.ReceiptValidation.objects.count() == 1
 
-        receipt = self.create_receipt()
-        errs = receipt.validate()
 
-        assert len(errs) == 0
-        assert receipt.validation.result == models.ReceiptValidation.RESULT_APPROVED
-        assert models.ReceiptValidation.objects.count() == 1
+@pytest.mark.django_db
+@pytest.mark.live
+def test_validate_credit_note(populated_db):
+    """Test validating valid receipts."""
 
-    def test_validate_credit_note(self):
-        """Test validating valid receipts."""
+    # Create a receipt (this credit note relates to it):
+    receipt = ReceiptWithVatAndTaxFactory()
+    errs = receipt.validate()
+    assert len(errs) == 0
 
-        # Create a receipt (this credit note relates to it):
-        receipt = self.create_receipt()
-        errs = receipt.validate()
-        assert len(errs) == 0
+    # Create a credit note for the above receipt:
+    credit_note = ReceiptWithVatAndTaxFactory(receipt_type__code=8)  # Nota de Crédito B
+    credit_note.related_receipts.add(receipt)
+    credit_note.save()
 
-        # Create a credit note for the above receipt:
-        credit_note = self.create_receipt(receipt_type_code=8)  # Nota de Crédito B
-        credit_note.related_receipts.add(receipt)
-        credit_note.save()
+    credit_note.validate(raise_=True)
+    assert credit_note.receipt_number is not None
 
-        credit_note.validate(raise_=True)
-        assert credit_note.receipt_number is not None
 
+@pytest.mark.django_db
+@pytest.mark.live
+def test_failed_validation(populated_db):
+    """Test validating valid receipts."""
+    receipt = ReceiptWithInconsistentVatAndTaxFactory()
 
-class ReceiptFailedValidateTestCase(PopulatedLiveAfipTestCase):
-    def setUp(self):
-        super().setUp()
-        self.receipt = factories.ReceiptFactory(
-            document_type__code=80,
-            point_of_sales=models.PointOfSales.objects.first(),
-        )
-        factories.VatFactory(vat_type__code=5, receipt=self.receipt)
-        factories.TaxFactory(tax_type__code=3, receipt=self.receipt)
+    errs = receipt.validate()
 
-    def test_failed_validation(self):
-        """Test validating valid receipts."""
-        errs = self.receipt.validate()
-
-        self.assertEqual(len(errs), 1)
-        # FIXME: We're not creating rejection entries
-        # self.assertEqual(len(errs), 1)
-        # self.assertEqual(
-        #     receipt.validation.result,
-        #     models.ReceiptValidation.RESULT_REJECTED,
-        # )
-        self.assertEqual(models.ReceiptValidation.objects.count(), 0)
-
-    def test_raise_validation(self):
-        """Test validating valid receipts."""
-
-        with self.assertRaisesRegex(
-            exceptions.ValidationError,
-            # Note: AFIP apparently edited this message and added a typo:
-            "DocNro 203012345 no se encuentra registrado en los padrones",
-        ):
-            self.receipt.validate(raise_=True)
-
-        # FIXME: We're not creating rejection entries
-        # self.assertEqual(
-        #     receipt.validation.result,
-        #     models.ReceiptValidation.RESULT_REJECTED,
-        # )
-        self.assertEqual(models.ReceiptValidation.objects.count(), 0)
-
-
-class ReceiptIsValidatedTestCase(TestCase):
-    def test_not_validated(self):
-        receipt = factories.ReceiptFactory()
-        self.assertEqual(receipt.is_validated, False)
-
-    def test_validated(self):
-        receipt = factories.ReceiptFactory(receipt_number=1)
-        factories.ReceiptValidationFactory(receipt=receipt)
-        self.assertEqual(receipt.is_validated, True)
-
-    def test_failed_validation(self):
-        # These should never really exist,but oh well:
-        receipt = factories.ReceiptFactory()
-        factories.ReceiptValidationFactory(
-            receipt=receipt,
-            result=models.ReceiptValidation.RESULT_REJECTED,
-        )
-        self.assertEqual(receipt.is_validated, False)
+    assert len(errs) == 1
+    # FIXME: We're not creating rejection entries
+    # assert receipt.validation.result == models.ReceiptValidation.RESULT_REJECTED
+    assert models.ReceiptValidation.objects.count() == 0
+
+
+@pytest.mark.django_db
+@pytest.mark.live
+def test_raising_failed_validation(populated_db):
+    """Test validating valid receipts."""
+    receipt = ReceiptWithInconsistentVatAndTaxFactory()
+
+    with pytest.raises(
+        exceptions.ValidationError,
+        # Note: AFIP apparently edited this message and added a typo:
+        match="DocNro 203012345 no se encuentra registrado en los padrones",
+    ):
+        receipt.validate(raise_=True)
+
+    # FIXME: We're not creating rejection entries
+    # assert receipt.validation.result == models.ReceiptValidation.RESULT_REJECTED
+    assert models.ReceiptValidation.objects.count() == 0
+
+
+@pytest.mark.django_db
+@pytest.mark.live
+def test_fetch_existing_data(populated_db):
+    pos = models.PointOfSales.objects.first()
+    rt = models.ReceiptType.objects.get(code=6)
+    # last receipt number is needed for testing, it seems they flush old receipts
+    # so we can't use a fixed receipt number
+    last_receipt_number = models.Receipt.objects.fetch_last_receipt_number(pos, rt)
+    receipt = models.Receipt.objects.fetch_receipt_data(
+        receipt_type=6,
+        receipt_number=last_receipt_number,
+        point_of_sales=pos,
+    )
+
+    assert receipt.CbteDesde == last_receipt_number
+    assert receipt.PtoVta == pos.number
 
-        receipt = factories.ReceiptFactory(receipt_number=1)
-        factories.ReceiptValidationFactory(
-            receipt=receipt,
-            result=models.ReceiptValidation.RESULT_REJECTED,
+
+@pytest.mark.django_db
+@pytest.mark.live
+def test_revalidation_valid_receipt(populated_db):
+    """Test revalidation process of a valid receipt."""
+    receipt = factories.ReceiptWithVatAndTaxFactory()
+    receipt.validate()
+    receipt.refresh_from_db()
+
+    old_cae = receipt.validation.cae
+    old_validation_pk = receipt.validation.id
+
+    receipt.validation.delete()
+
+    receipt.refresh_from_db()
+    assert not receipt.is_validated
+
+    validation = receipt.revalidate()
+
+    assert validation is not None
+    assert validation.receipt == receipt
+    assert old_cae == validation.cae
+    assert old_validation_pk != validation.id
+
+
+@pytest.mark.live
+def test_revalidation_invalid_receipt(populated_db):
+    """Test revalidation process of an invalid receipt. (Unexistent receipt)"""
+    receipt = factories.ReceiptWithVatAndTaxFactory()
+    next_num = (
+        models.Receipt.objects.fetch_last_receipt_number(
+            receipt.point_of_sales,
+            receipt.receipt_type,
         )
-        self.assertEqual(receipt.is_validated, False)
+        + 1
+    )
 
+    receipt.receipt_number = next_num
+    receipt.save()
 
-class ReceiptDefaultCurrencyTestCase(TestCase):
-    def test_no_currencies(self):
-        receipt = models.Receipt()
-        with self.assertRaises(models.CurrencyType.DoesNotExist):
-            receipt.currency
+    receipt.refresh_from_db()
 
-    def test_multieple_currencies(self):
-        c1 = factories.CurrencyTypeFactory(pk=2)
-        c2 = factories.CurrencyTypeFactory(pk=1)
-        c3 = factories.CurrencyTypeFactory(pk=3)
+    validation = receipt.revalidate()
 
-        receipt = models.Receipt()
-        self.assertNotEqual(receipt.currency, c1)
-        self.assertEqual(receipt.currency, c2)
-        self.assertNotEqual(receipt.currency, c3)
+    assert validation is None
 
 
-class ReceiptTotalVatTestCase(TestCase):
-    def test_no_vat(self):
-        receipt = factories.ReceiptFactory()
+@pytest.mark.django_db
+def test_receipt_revalidate_without_receipt_number():
+    """Test revalidation process of an invalid receipt. (Receipt without number)"""
+    factories.PointOfSalesFactory()
+    receipt = factories.ReceiptWithVatAndTaxFactory()
+    receipt.refresh_from_db()
 
-        self.assertEqual(receipt.total_vat, 0)
+    validation = receipt.revalidate()
 
-    def test_multiple_vats(self):
-        receipt = factories.ReceiptFactory()
-        factories.VatFactory(receipt=receipt)
-        factories.VatFactory(receipt=receipt)
+    assert validation is None
 
-        self.assertEqual(receipt.total_vat, 42)
 
-    def test_proper_filtering(self):
-        receipt = factories.ReceiptFactory()
-        factories.VatFactory(receipt=receipt)
-        factories.VatFactory()
+@pytest.mark.django_db
+def test_receipt_is_validated_when_not_validated():
+    receipt = ReceiptFactory()
+    assert not receipt.is_validated
 
-        self.assertEqual(receipt.total_vat, 21)
 
+@pytest.mark.django_db
+def test_receipt_is_validated_when_validated():
+    receipt = ReceiptWithApprovedValidation()
+    assert receipt.is_validated
 
-class ReceiptTotalTaxTestCase(TestCase):
-    def test_no_tax(self):
-        receipt = factories.ReceiptFactory()
 
-        self.assertEqual(receipt.total_tax, 0)
+@pytest.mark.django_db
+def test_receipt_is_validted_when_failed_validation():
+    # These should never really exist,but oh well:
+    receipt = ReceiptFactory(receipt_number=None)
+    ReceiptValidationFactory(
+        receipt=receipt,
+        result=models.ReceiptValidation.RESULT_REJECTED,
+    )
+    assert not receipt.is_validated
 
-    def test_multiple_taxes(self):
-        receipt = factories.ReceiptFactory()
-        factories.TaxFactory(receipt=receipt)
-        factories.TaxFactory(receipt=receipt)
+    receipt = ReceiptFactory(receipt_number=1)
+    ReceiptValidationFactory(
+        receipt=receipt,
+        result=models.ReceiptValidation.RESULT_REJECTED,
+    )
+    assert not receipt.is_validated
 
-        self.assertEqual(receipt.total_tax, 18)
 
-    def test_proper_filtering(self):
-        receipt = factories.ReceiptFactory()
-        factories.TaxFactory(receipt=receipt)
-        factories.TaxFactory()
+@pytest.mark.django_db
+def test_default_currency_no_currencies():
+    receipt = models.Receipt()
+    with pytest.raises(models.CurrencyType.DoesNotExist):
+        receipt.currency
 
-        self.assertEqual(receipt.total_tax, 9)
 
+@pytest.mark.django_db
+def test_default_currency_multieple_currencies():
+    c1 = factories.CurrencyTypeFactory(pk=2)
+    c2 = factories.CurrencyTypeFactory(pk=1)
+    c3 = factories.CurrencyTypeFactory(pk=3)
 
-class CurrencyTypeStrTestCase(TestCase):
-    def test_success(self):
-        currency_type = models.CurrencyType(
-            code="011",
-            description="Pesos Uruguayos",
-        )
-        self.assertEqual(str(currency_type), "Pesos Uruguayos (011)")
+    receipt = models.Receipt()
+
+    assert receipt.currency != c1
+    assert receipt.currency == c2
+    assert receipt.currency != c3
+
+
+@pytest.mark.django_db
+def test_total_vat_no_vat():
+    receipt = ReceiptFactory()
+
+    assert receipt.total_vat == 0
+
+
+@pytest.mark.django_db
+def test_total_vat_multiple_vats():
+    receipt = ReceiptFactory()
+    factories.VatFactory(receipt=receipt)
+    factories.VatFactory(receipt=receipt)
+
+    assert receipt.total_vat == 42
+
+
+@pytest.mark.live
+def test_revalidation_validated_receipt(populated_db):
+    """Test revalidation process of a validated receipt."""
+    receipt_validation = factories.ReceiptValidationFactory()
+
+    revalidation = receipt_validation.receipt.revalidate()
+
+    assert revalidation is not None
+    assert revalidation == receipt_validation
+
+
+@pytest.mark.django_db
+def test_total_vat_proper_filtering():
+    receipt = ReceiptFactory()
+    factories.VatFactory(receipt=receipt)
+    factories.VatFactory()
+
+    assert receipt.total_vat == 21
+
+
+@pytest.mark.django_db
+def test_total_tax_no_tax():
+    receipt = ReceiptFactory()
+
+    assert receipt.total_tax == 0
+
+
+@pytest.mark.django_db
+def test_total_tax_multiple_taxes():
+    receipt = ReceiptFactory()
+    factories.TaxFactory(receipt=receipt)
+    factories.TaxFactory(receipt=receipt)
+
+    assert receipt.total_tax == 18
+
+
+@pytest.mark.django_db
+def test_total_tax_proper_filtering():
+    receipt = ReceiptFactory()
+    factories.TaxFactory(receipt=receipt)
+    factories.TaxFactory()
+
+    assert receipt.total_tax == 9
+
+
+def test_currenty_type_success():
+    currency_type = models.CurrencyType(code="011", description="Pesos Uruguayos")
+    assert str(currency_type) == "Pesos Uruguayos (011)"
+
+
+@pytest.mark.django_db
+@pytest.mark.live
+def test_populate_method(live_ticket):
+    assert models.CurrencyType.objects.count() == 0
+    models.CurrencyType.objects.populate()
+    assert models.CurrencyType.objects.count() == 50
```

### Comparing `django-afip-8.0.4/testapp/testapp/testmain/tests/test_parsers.py` & `django-afip-9.0.0/testapp/testapp/testmain/tests/test_parsers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 from datetime import date
 from datetime import datetime
 
 import pytz
-from django.test import TestCase
 
 from django_afip import parsers
 
 
-class ParseDatetimeTestCase(TestCase):
-    def test_parse_null(self):
-        self.assertEqual(parsers.parse_datetime("NULL"), None)
-
-    def test_parse_none(self):
-        self.assertEqual(parsers.parse_datetime(None), None)
-
-    def test_parse_datetimes(self):
-        tz = pytz.timezone(pytz.country_timezones["ar"][0])
-        self.assertEqual(
-            parsers.parse_datetime("20170730154330"),
-            datetime(2017, 7, 30, 15, 43, 30, tzinfo=tz),
-        )
-
-
-class ParseDateTestCase(TestCase):
-    def test_parse_null(self):
-        self.assertEqual(parsers.parse_date("NULL"), None)
-
-    def test_parse_none(self):
-        self.assertEqual(parsers.parse_date(None), None)
-
-    def test_parse_dates(self):
-        self.assertEqual(
-            parsers.parse_date("20170730"),
-            date(2017, 7, 30),
-        )
-
-
-class ParseString(TestCase):
-    def test_weirdly_encoded(self):
-        # This is the encoding AFIP sometimes uses:
-        string = "AÃ±adir paÃ\xads"
-        self.assertEqual(parsers.parse_string(string), "Añadir país")
+def test_parse_null_datetime():
+    assert parsers.parse_datetime("NULL") is None
+
+
+def test_parse_none_datetime():
+    assert parsers.parse_datetime(None) is None
+
+
+def test_parse_datetimes():
+    tz = pytz.timezone(pytz.country_timezones["ar"][0])
+
+    assert parsers.parse_datetime("20170730154330") == datetime(
+        2017, 7, 30, 15, 43, 30, tzinfo=tz
+    )
+
+
+def test_parse_null_date():
+    assert parsers.parse_date("NULL") is None
+
+
+def test_parse_none_date():
+    assert parsers.parse_date(None) is None
+
+
+def test_parse_dates():
+    assert parsers.parse_date("20170730") == date(2017, 7, 30)
+
+
+def test_weirdly_encoded():
+    # This is the encoding AFIP sometimes uses:
+    string = "AÃ±adir paÃ\xads"
+    assert parsers.parse_string(string) == "Añadir país"
```

### Comparing `django-afip-8.0.4/testapp/testapp/testmain/tests/test_pdf.py` & `django-afip-9.0.0/testapp/testapp/testmain/tests/test_pdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 import re
 from datetime import date
 
 import pytest
-from django.test import TestCase
 
 from django_afip import factories
 from django_afip import models
 from django_afip.pdf import ReceiptQrCode
 
 
-class ReceiptPDFGenerationTestCase(TestCase):
-    def test_pdf_generation(self):
-        """Test PDF file generation.
-
-        For the moment, this test case mostly verifies that pdf generation
-        *works*, but does not actually validate the pdf file itself.
-
-        Running this locally *will* yield the file itself, which is useful for
-        manual inspection.
-        """
-        pdf = factories.ReceiptPDFFactory(receipt__receipt_number=3)
-        factories.ReceiptValidationFactory(receipt=pdf.receipt)
+@pytest.mark.django_db
+def test_pdf_generation():
+    """Test PDF file generation.
+
+    For the moment, this test case mostly verifies that pdf generation
+    *works*, but does not actually validate the pdf file itself.
+
+    Running this locally *will* yield the file itself, which is useful for
+    manual inspection.
+    """
+    pdf = factories.ReceiptPDFFactory(receipt__receipt_number=3)
+    factories.ReceiptValidationFactory(receipt=pdf.receipt)
+    pdf.save_pdf()
+    regex = r"afip/receipts/[a-f0-9]{2}/[a-f0-9]{2}/[a-f0-9]{32}.pdf"
+
+    assert re.match(regex, pdf.pdf_file.name)
+    assert pdf.pdf_file.name.endswith(".pdf")
+
+
+@pytest.mark.django_db
+def test_unauthorized_receipt_generation():
+    """
+    Test PDF file generation for unauthorized receipts.
+
+    Confirm that attempting to generate a PDF for an unauthorized receipt
+    raises.
+    """
+    taxpayer = factories.TaxPayerFactory()
+    receipt = factories.ReceiptFactory(
+        receipt_number=None,
+        point_of_sales__owner=taxpayer,
+    )
+    pdf = models.ReceiptPDF.objects.create_for_receipt(
+        receipt=receipt,
+        client_name="John Doe",
+        client_address="12 Green Road\nGreenville\nUK",
+    )
+    with pytest.raises(
+        Exception, match="Cannot generate pdf for non-authorized receipt"
+    ):
         pdf.save_pdf()
-        regex = r"afip/receipts/[a-f0-9]{2}/[a-f0-9]{2}/[a-f0-9]{32}.pdf"
-        self.assertTrue(re.match(regex, pdf.pdf_file.name))
-        self.assertTrue(pdf.pdf_file.name.endswith(".pdf"))
-
-    def test_unauthorized_receipt_generation(self):
-        """
-        Test PDF file generation for unauthorized receipts.
-
-        Confirm that attempting to generate a PDF for an unauthorized receipt
-        raises.
-        """
-        taxpayer = factories.TaxPayerFactory()
-        factories.TaxPayerProfileFactory(taxpayer=taxpayer)
-        receipt = factories.ReceiptFactory(
-            receipt_number=None,
-            point_of_sales__owner=taxpayer,
-        )
-        pdf = models.ReceiptPDF.objects.create_for_receipt(
-            receipt=receipt,
-            client_name="John Doe",
-            client_address="12 Green Road\nGreenville\nUK",
-        )
-        with self.assertRaisesMessage(
-            Exception, "Cannot generate pdf for non-authorized receipt"
-        ):
-            pdf.save_pdf()
-
-
-class GenerateReceiptPDFSignalTestCase(TestCase):
-    def test_not_validated_receipt(self):
-        printable = factories.ReceiptPDFFactory()
-
-        self.assertFalse(printable.pdf_file)
-
-    def test_validated_receipt(self):
-        validation = factories.ReceiptValidationFactory()
-        printable = factories.ReceiptPDFFactory(receipt=validation.receipt)
 
-        self.assertTrue(printable.pdf_file)
-        self.assertTrue(printable.pdf_file.name.endswith(".pdf"))
+
+@pytest.mark.django_db
+def test_signal_generation_for_not_validated_receipt():
+    printable = factories.ReceiptPDFFactory()
+
+    assert not (printable.pdf_file)
+
+
+@pytest.mark.django_db
+def test_signal_generation_for_validated_receipt():
+    validation = factories.ReceiptValidationFactory()
+    printable = factories.ReceiptPDFFactory(receipt=validation.receipt)
+
+    assert printable.pdf_file
+    assert printable.pdf_file.name.endswith(".pdf")
 
 
 @pytest.mark.django_db
 def test_qrcode_data():
     pdf = factories.ReceiptPDFFactory(
         receipt__receipt_number=3,
         receipt__issued_date=date(2021, 3, 2),
```

### Comparing `django-afip-8.0.4/testapp/testapp/testmain/tests/test_tags.py` & `django-afip-9.0.0/testapp/testapp/testmain/tests/test_tags.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Tests for provided template tags."""
-from django.test import TestCase
-
 from django_afip.templatetags.django_afip import format_cuit
 
 
-class FormatCuitTagTestCase(TestCase):
-    """Test the format_cuit tag."""
+def test_format_cuit_tag_with_string():
+    """Test valid string inputs."""
+    assert format_cuit("20329642330") == "20-32964233-0"
+    assert format_cuit("20-32964233-0") == "20-32964233-0"
+
+
+def test_format_cuit_tag_with_number():
+    """Test valid numerical input."""
+    assert format_cuit(20329642330) == "20-32964233-0"
+
+
+def test_format_cuit_tag_with_bad_string():
+    """Test invalid string input."""
+    assert format_cuit("blah blah") == "blah blah"
+
 
-    def test_good_string_input(self):
-        """Test valid string inputs."""
-        self.assertEqual(format_cuit("20329642330"), "20-32964233-0")
-        self.assertEqual(format_cuit("20-32964233-0"), "20-32964233-0")
-
-    def test_good_numeric_input(self):
-        """Test valid numerical input."""
-        self.assertEqual(format_cuit(20329642330), "20-32964233-0")
-
-    def test_bad_string_input(self):
-        """Test invalid string input."""
-        self.assertEqual(format_cuit("blah blah"), "blah blah")
-
-    def test_bad_numeric_input(self):
-        """Test invalid numerical input."""
-        self.assertEqual(format_cuit(1234), 1234)
+def test_format_cuit_tag_with_bad_number():
+    """Test invalid numerical input."""
+    assert format_cuit(1234) == 1234
```

### Comparing `django-afip-8.0.4/testapp/testapp/testmain/tests/test_taxpayer.py` & `django-afip-9.0.0/testapp/testapp/testmain/tests/test_taxpayer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,109 @@
 from datetime import datetime
 
-from django.test import TestCase
+import pytest
 from factory.django import FileField
 from freezegun import freeze_time
 from OpenSSL import crypto
 
 from django_afip import factories
 
 
-class TestTaxPayerKeyManagement(TestCase):
-    def test_key_generation(self):
-        taxpayer = factories.TaxPayerFactory(key=None)
-        taxpayer.generate_key()
+@pytest.mark.django_db
+def test_key_generation():
+    taxpayer = factories.TaxPayerFactory.build(key=None)
+    taxpayer.generate_key()
 
-        key = taxpayer.key.file.read().decode()
-        self.assertEqual(key.splitlines()[0], "-----BEGIN PRIVATE KEY-----")
-        self.assertEqual(key.splitlines()[-1], "-----END PRIVATE KEY-----")
+    key = taxpayer.key.file.read().decode()
+    assert key.splitlines()[0] == "-----BEGIN PRIVATE KEY-----"
+    assert key.splitlines()[-1] == "-----END PRIVATE KEY-----"
 
-        loaded_key = crypto.load_privatekey(crypto.FILETYPE_PEM, key)
-        self.assertIsInstance(loaded_key, crypto.PKey)
+    loaded_key = crypto.load_privatekey(crypto.FILETYPE_PEM, key)
+    assert isinstance(loaded_key, crypto.PKey)
 
-    def test_dont_overwrite_keys(self):
-        text = b"Hello! I'm not really a key :D"
-        taxpayer = factories.TaxPayerFactory(key=FileField(data=text))
 
-        taxpayer.generate_key()
-        key = taxpayer.key.read()
+def test_dont_overwrite_keys():
+    text = b"Hello! I'm not really a key :D"
+    taxpayer = factories.TaxPayerFactory.build(key=FileField(data=text))
 
-        self.assertEqual(text, key)
+    taxpayer.generate_key()
+    key = taxpayer.key.read()
 
-    def test_overwrite_keys_force(self):
-        text = b"Hello! I'm not really a key :D"
-        taxpayer = factories.TaxPayerFactory(key__data=text)
+    assert text == key
 
-        taxpayer.generate_key(force=True)
-        key = taxpayer.key.file.read().decode()
 
-        self.assertNotEqual(text, key)
-        self.assertEqual(key.splitlines()[0], "-----BEGIN PRIVATE KEY-----")
-        self.assertEqual(key.splitlines()[-1], "-----END PRIVATE KEY-----")
+@pytest.mark.django_db
+def test_overwrite_keys_force():
+    text = b"Hello! I'm not really a key :D"
+    taxpayer = factories.TaxPayerFactory.build(key__data=text)
 
-        loaded_key = crypto.load_privatekey(crypto.FILETYPE_PEM, key)
-        self.assertIsInstance(loaded_key, crypto.PKey)
+    taxpayer.generate_key(force=True)
+    key = taxpayer.key.file.read().decode()
 
-    @freeze_time(datetime.fromtimestamp(1489537017))
-    def test_csr_generation(self):
-        taxpayer = factories.TaxPayerFactory(key=None)
-        taxpayer.generate_key()
+    assert text != key
+    assert key.splitlines()[0] == "-----BEGIN PRIVATE KEY-----"
+    assert key.splitlines()[-1] == "-----END PRIVATE KEY-----"
 
-        csr_file = taxpayer.generate_csr()
-        csr = csr_file.read().decode()
+    loaded_key = crypto.load_privatekey(crypto.FILETYPE_PEM, key)
+    assert isinstance(loaded_key, crypto.PKey)
 
-        self.assertEqual(csr.splitlines()[0], "-----BEGIN CERTIFICATE REQUEST-----")
 
-        self.assertEqual(csr.splitlines()[-1], "-----END CERTIFICATE REQUEST-----")
+@freeze_time(datetime.fromtimestamp(1489537017))
+@pytest.mark.django_db
+def test_csr_generation():
+    taxpayer = factories.TaxPayerFactory.build(key=None)
+    taxpayer.generate_key()
 
-        loaded_csr = crypto.load_certificate_request(crypto.FILETYPE_PEM, csr)
-        self.assertIsInstance(loaded_csr, crypto.X509Req)
+    csr_file = taxpayer.generate_csr()
+    csr = csr_file.read().decode()
 
-        expected_components = [
-            (b"O", b"John Smith"),
-            (b"CN", b"djangoafip1489537017"),
-            (b"serialNumber", b"CUIT 20329642330"),
-        ]
+    assert csr.splitlines()[0] == "-----BEGIN CERTIFICATE REQUEST-----"
 
-        self.assertEqual(expected_components, loaded_csr.get_subject().get_components())
+    assert csr.splitlines()[-1] == "-----END CERTIFICATE REQUEST-----"
 
+    loaded_csr = crypto.load_certificate_request(crypto.FILETYPE_PEM, csr)
+    assert isinstance(loaded_csr, crypto.X509Req)
 
-class TaxPayerCertificateObjectTestCase(TestCase):
-    def test_certificate_object(self):
-        taxpayer = factories.TaxPayerFactory()
-        cert = taxpayer.certificate_object
+    expected_components = [
+        (b"O", b"John Smith"),
+        (b"CN", b"djangoafip1489537017"),
+        (b"serialNumber", b"CUIT 20329642330"),
+    ]
 
-        self.assertIsInstance(cert, crypto.X509)
+    assert expected_components == loaded_csr.get_subject().get_components()
 
-    def test_null_certificate_object(self):
-        taxpayer = factories.TaxPayerFactory(certificate=None)
-        cert = taxpayer.certificate_object
 
-        self.assertIsNone(cert)
+def test_certificate_object():
+    taxpayer = factories.TaxPayerFactory.build()
+    cert = taxpayer.certificate_object
 
+    assert isinstance(cert, crypto.X509)
 
-class TaxPayerExpirationTestCase(TestCase):
-    def test_expiration_getter(self):
-        taxpayer = factories.TaxPayerFactory()
-        expiration = taxpayer.get_certificate_expiration()
 
-        self.assertIsInstance(expiration, datetime)
+def test_null_certificate_object():
+    taxpayer = factories.TaxPayerFactory.build(certificate=None)
+    cert = taxpayer.certificate_object
 
-    def test_expiration_signal_update(self):
-        taxpayer = factories.TaxPayerFactory(certificate_expiration=None)
-        taxpayer.save()
-        expiration = taxpayer.certificate_expiration
+    assert cert is None
 
-        self.assertIsInstance(expiration, datetime)
+
+def test_expiration_getter():
+    taxpayer = factories.TaxPayerFactory.build(certificate=None)
+    expiration = taxpayer.get_certificate_expiration()
+
+    assert expiration is None
+
+
+def test_expiration_getter_no_cert():
+    taxpayer = factories.TaxPayerFactory.build()
+    expiration = taxpayer.get_certificate_expiration()
+
+    assert isinstance(expiration, datetime)
+
+
+@pytest.mark.django_db
+def test_expiration_signal_update():
+    taxpayer = factories.TaxPayerFactory(certificate_expiration=None)
+    taxpayer.save()
+    expiration = taxpayer.certificate_expiration
+
+    assert isinstance(expiration, datetime)
```

### Comparing `django-afip-8.0.4/testapp/testapp/testmain/tests/test_views.py` & `django-afip-9.0.0/testapp/testapp/testmain/tests/test_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from datetime import date
 
 import pytest
 from django.test import Client
 from django.test import TestCase
 from django.urls import reverse
+from pytest_django.asserts import assertContains
+from pytest_django.asserts import assertHTMLEqual
 
 from django_afip import factories
 from django_afip import views
 
 
 class ReceiptPDFTestCase(TestCase):
     def test_html_view(self):
@@ -23,15 +25,15 @@
         client = Client()
         response = client.get(
             "{}?html=true".format(
                 reverse("receipt_displaypdf_view", args=(pdf.receipt.pk,))
             )
         )
 
-        self.assertHTMLEqual(
+        assertHTMLEqual(
             response.content.decode(),
             """
 <!DOCTYPE html>
 <html>
   <head>
     <meta charset="utf-8">
     <link rel="stylesheet" href="/static/receipts/receipt.css">
@@ -145,15 +147,15 @@
         client = Client()
         response = client.get(
             "{}?html=true".format(
                 reverse("receipt_displaypdf_view", args=(pdf.receipt.pk,))
             )
         )
 
-        self.assertContains(
+        assertContains(
             response,
             """
             <address>
             <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAIAAAACCAIAAAD91JpzAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH4QgLERgyoZWu2QAAAB1pVFh0Q29tbWVudAAAAAAAQ3JlYXRlZCB3aXRoIEdJTVBkLmUHAAAAEklEQVQI12P4//8/AwT8//8fACnkBft7DmIIAAAAAElFTkSuQmCC" alt="Logo"><br>
             <strong>Alice Doe</strong><br>
             Happy Street 123, CABA<br>
 
@@ -165,34 +167,32 @@
 
     def test_pdf_view(self):
         """
         Test the PDF generation view.
         """
         taxpayer = factories.TaxPayerFactory()
 
-        factories.TaxPayerProfileFactory(taxpayer=taxpayer)
         pdf = factories.ReceiptPDFFactory(
             receipt__point_of_sales__owner=taxpayer,
         )
         factories.ReceiptValidationFactory(receipt=pdf.receipt)
 
         client = Client()
         response = client.get(reverse("receipt_pdf_view", args=(pdf.receipt.pk,)))
 
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(response.content[:7], b"%PDF-1.")
+        assert response.status_code == 200
+        assert response.content[:7] == b"%PDF-1."
 
         headers = sorted(response.serialize_headers().decode().splitlines())
-        self.assertIn("Content-Type: application/pdf", headers)
+        assert "Content-Type: application/pdf" in headers
 
 
 @pytest.mark.django_db
 def test_template_discovery(client):
     taxpayer = factories.TaxPayerFactory(cuit="20329642330")
-    factories.TaxPayerProfileFactory(taxpayer=taxpayer)
     pdf = factories.ReceiptPDFFactory(
         receipt__point_of_sales__owner=taxpayer,
         receipt__point_of_sales__number=9999,
         receipt__receipt_type__code=6,
     )
     factories.ReceiptValidationFactory(receipt=pdf.receipt)
 
@@ -209,8 +209,8 @@
 class ReceiptPDFViewDownloadNameTestCase(TestCase):
     def test_download_name(self):
         factories.ReceiptFactory(pk=9, receipt_number=32)
 
         view = views.ReceiptPDFView()
         view.kwargs = {"pk": 9}
 
-        self.assertEqual(view.get_download_name(), "0001-00000032.pdf")
+        assert view.get_download_name() == "0001-00000032.pdf"
```

### Comparing `django-afip-8.0.4/testapp/testapp/urls.py` & `django-afip-9.0.0/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `django-afip-8.0.4/tox.ini` & `django-afip-9.0.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 [tox]
 envlist =
-  django{22,30,31}-{sqlite,postgres,mysql},
-  docs,
+  py{37,38,39}-django{31,32}-{sqlite,postgres,mysql},
   live
 
 [testenv]
 deps =
   dj-database-url
   coverage
   factory-boy
   freezegun
   pytest-django
   pytest-cov
   postgres: -e .[postgres]
   mysql: -e .[mysql]
-  django22: Django>=2.2,<2.3
-  django30: Django>=3.0,<3.1
   django31: Django>=3.1,<3.2
+  django32: Django>=3.2,<3.3
 commands = pytest -vv -m "not live" {posargs}
 setenv =
   PYTHONPATH={toxinidir}/testapp:{toxinidir}
+  sqlite: DATABASE_URL=sqlite:///:memory:
+  mysql: DATABASE_URL={env:DATABASE_URL:mysql://root:mysql@127.0.0.1:3306/mysql}
+  postgres: DATABASE_URL=postgres://postgres:postgres@localhost:5432/postgres
 passenv =
-  DATABASE_URL
   CODECOV_TOKEN
 
 [testenv:live]
+deps =
+  {[testenv]deps}
+  -e .[postgres]
 commands = pytest -vv -m "live" {posargs}
-
-[testenv:docs]
-extras=docs
-commands =
-  make -C docs html
-whitelist_externals =
-  make
+setenv =
+  PYTHONPATH={toxinidir}/testapp:{toxinidir}
+  DATABASE_URL=postgres://postgres:postgres@localhost:5432/postgres
 
 [testenv:fixtures]
 commands = python scripts/dump_metadata.py
 setenv =
   PYTHONPATH={toxinidir}/testapp:{toxinidir}
   DJANGO_SETTINGS_MODULE=testapp.settings
+
+[testenv:mypy]
+deps =
+  django-stubs
+  dj_database_url
+commands = mypy --show-traceback --pdb django_afip
```

