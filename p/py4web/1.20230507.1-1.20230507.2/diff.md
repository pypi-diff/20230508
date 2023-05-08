# Comparing `tmp/py4web-1.20230507.1.tar.gz` & `tmp/py4web-1.20230507.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230507.1.tar", last modified: Mon May  8 02:45:11 2023, max compression
+gzip compressed data, was "py4web-1.20230507.2.tar", last modified: Mon May  8 02:51:59 2023, max compression
```

## Comparing `py4web-1.20230507.1.tar` & `py4web-1.20230507.2.tar`

### file list

```diff
@@ -1,65 +1,72 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.905419 py4web-1.20230507.1/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230507.1/LICENSE.md
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-08 02:45:11.905419 py4web-1.20230507.1/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230507.1/README.rst
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.893419 py4web-1.20230507.1/py4web/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      721 2023-05-08 00:45:22.000000 py4web-1.20230507.1/py4web/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    67416 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/core.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/server_adapters.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.901419 py4web-1.20230507.1/py4web/utils/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    69664 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.901419 py4web-1.20230507.1/py4web/utils/auth_plugins/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      514 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2github.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2google.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/pam.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/cors.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/dbstore.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/downloader.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/factories.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/grid.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/jsonrpc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/mailer.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/misc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/param.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/populate.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/publisher.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/recaptcha.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/security.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/url_signer.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.893419 py4web-1.20230507.1/py4web.egg-info/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1593 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/SOURCES.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/dependency_links.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       43 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/entry_points.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      239 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/requires.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        7 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/top_level.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1211 2023-05-08 02:44:58.000000 py4web-1.20230507.1/pyproject.toml
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-08 02:45:11.905419 py4web-1.20230507.1/setup.cfg
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.905419 py4web-1.20230507.1/tests/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_action.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_auth.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_cache.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_fixture.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_get_error_snapshot.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_json.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_main.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_session.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_template.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_url.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:51:59.834663 py4web-1.20230507.2/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230507.2/LICENSE.md
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-08 02:51:59.834663 py4web-1.20230507.2/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230507.2/README.rst
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:51:59.810663 py4web-1.20230507.2/py4web/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      721 2023-05-08 02:50:34.000000 py4web-1.20230507.2/py4web/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:51:59.822663 py4web-1.20230507.2/py4web/assets/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  2995867 2023-05-08 02:51:48.000000 py4web-1.20230507.2/py4web/assets/py4web.app._dashboard.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)   187155 2023-05-08 02:51:48.000000 py4web-1.20230507.2/py4web/assets/py4web.app._default.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  4356813 2023-05-08 02:51:49.000000 py4web-1.20230507.2/py4web/assets/py4web.app._documentation.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5245 2023-05-08 02:51:48.000000 py4web-1.20230507.2/py4web/assets/py4web.app._minimal.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    21524 2023-05-08 02:51:48.000000 py4web-1.20230507.2/py4web/assets/py4web.app._scaffold.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  1385465 2023-05-08 02:51:49.000000 py4web-1.20230507.2/py4web/assets/py4web.app.showcase.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    67416 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/core.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/server_adapters.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:51:59.826663 py4web-1.20230507.2/py4web/utils/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    69664 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:51:59.830663 py4web-1.20230507.2/py4web/utils/auth_plugins/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2discord.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      514 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2github.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2google.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2okta.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2server.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/pam.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/pam_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/cors.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/dbstore.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/downloader.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/factories.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/grid.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/jsonrpc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/mailer.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/misc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/param.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/populate.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/publisher.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/recaptcha.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/security.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-05-08 00:39:45.000000 py4web-1.20230507.2/py4web/utils/url_signer.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:51:59.810663 py4web-1.20230507.2/py4web.egg-info/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-08 02:51:59.000000 py4web-1.20230507.2/py4web.egg-info/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1830 2023-05-08 02:51:59.000000 py4web-1.20230507.2/py4web.egg-info/SOURCES.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 02:51:59.000000 py4web-1.20230507.2/py4web.egg-info/dependency_links.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       43 2023-05-08 02:51:59.000000 py4web-1.20230507.2/py4web.egg-info/entry_points.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      239 2023-05-08 02:51:59.000000 py4web-1.20230507.2/py4web.egg-info/requires.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        7 2023-05-08 02:51:59.000000 py4web-1.20230507.2/py4web.egg-info/top_level.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1211 2023-05-08 02:50:45.000000 py4web-1.20230507.2/pyproject.toml
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-08 02:51:59.834663 py4web-1.20230507.2/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:51:59.834663 py4web-1.20230507.2/tests/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_action.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_auth.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_cache.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_fixture.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_get_error_snapshot.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_json.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_main.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_session.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_template.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230507.2/tests/test_url.py
```

### Comparing `py4web-1.20230507.1/LICENSE.md` & `py4web-1.20230507.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/PKG-INFO` & `py4web-1.20230507.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230507.1
+Version: 1.20230507.2
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230507.1/README.rst` & `py4web-1.20230507.2/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/__init__.py` & `py4web-1.20230507.2/py4web/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSDv3"
-__version__ = "1.20230507.1"
+__version__ = "1.20230507.2"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230507.1/py4web/core.py` & `py4web-1.20230507.2/py4web/core.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/server_adapters.py` & `py4web-1.20230507.2/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth.py` & `py4web-1.20230507.2/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2github.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230507.2/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/cors.py` & `py4web-1.20230507.2/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/dbstore.py` & `py4web-1.20230507.2/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/downloader.py` & `py4web-1.20230507.2/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/factories.py` & `py4web-1.20230507.2/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/form.py` & `py4web-1.20230507.2/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/grid.py` & `py4web-1.20230507.2/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/jsonrpc.py` & `py4web-1.20230507.2/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/mailer.py` & `py4web-1.20230507.2/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/misc.py` & `py4web-1.20230507.2/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/populate.py` & `py4web-1.20230507.2/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/publisher.py` & `py4web-1.20230507.2/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/recaptcha.py` & `py4web-1.20230507.2/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/security.py` & `py4web-1.20230507.2/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web/utils/url_signer.py` & `py4web-1.20230507.2/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/py4web.egg-info/PKG-INFO` & `py4web-1.20230507.2/py4web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230507.1
+Version: 1.20230507.2
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230507.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20230507.2/py4web.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 py4web/server_adapters.py
 py4web.egg-info/PKG-INFO
 py4web.egg-info/SOURCES.txt
 py4web.egg-info/dependency_links.txt
 py4web.egg-info/entry_points.txt
 py4web.egg-info/requires.txt
 py4web.egg-info/top_level.txt
+py4web/assets/py4web.app._dashboard.zip
+py4web/assets/py4web.app._default.zip
+py4web/assets/py4web.app._documentation.zip
+py4web/assets/py4web.app._minimal.zip
+py4web/assets/py4web.app._scaffold.zip
+py4web/assets/py4web.app.showcase.zip
 py4web/utils/__init__.py
 py4web/utils/auth.py
 py4web/utils/cors.py
 py4web/utils/dbstore.py
 py4web/utils/downloader.py
 py4web/utils/factories.py
 py4web/utils/form.py
```

### Comparing `py4web-1.20230507.1/pyproject.toml` & `py4web-1.20230507.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py4web"
-version = "1.20230507.1"
+version = "1.20230507.2"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20230507.1/tests/test_action.py` & `py4web-1.20230507.2/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_auth.py` & `py4web-1.20230507.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_cache.py` & `py4web-1.20230507.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_fixture.py` & `py4web-1.20230507.2/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_form.py` & `py4web-1.20230507.2/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_get_error_snapshot.py` & `py4web-1.20230507.2/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_json.py` & `py4web-1.20230507.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_main.py` & `py4web-1.20230507.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_session.py` & `py4web-1.20230507.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230507.1/tests/test_tags.py` & `py4web-1.20230507.2/tests/test_tags.py`

 * *Files identical despite different names*

