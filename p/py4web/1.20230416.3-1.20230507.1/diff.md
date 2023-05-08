# Comparing `tmp/py4web-1.20230416.3.tar.gz` & `tmp/py4web-1.20230507.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230416.3.tar", last modified: Mon Apr 17 05:04:36 2023, max compression
+gzip compressed data, was "py4web-1.20230507.1.tar", last modified: Mon May  8 02:45:11 2023, max compression
```

## Comparing `py4web-1.20230416.3.tar` & `py4web-1.20230507.1.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.818078 py4web-1.20230416.3/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 05:04:36.818078 py4web-1.20230416.3/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     7120 2022-01-11 05:54:38.000000 py4web-1.20230416.3/README.rst
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.798077 py4web-1.20230416.3/py4web/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      721 2023-04-17 05:02:51.000000 py4web-1.20230416.3/py4web/__init__.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.810078 py4web-1.20230416.3/py4web/assets/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  2995768 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._dashboard.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   187155 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._default.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  4287226 2023-04-17 05:03:23.000000 py4web-1.20230416.3/py4web/assets/py4web.app._documentation.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5245 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._minimal.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    21524 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._scaffold.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  1392585 2023-04-17 05:03:23.000000 py4web-1.20230416.3/py4web/assets/py4web.app.showcase.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    67378 2023-04-16 18:21:53.000000 py4web-1.20230416.3/py4web/core.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2022-06-30 06:41:15.000000 py4web-1.20230416.3/py4web/server_adapters.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.814077 py4web-1.20230416.3/py4web/utils/
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2019-07-23 06:20:41.000000 py4web-1.20230416.3/py4web/utils/__init__.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    69664 2023-04-10 05:23:42.000000 py4web-1.20230416.3/py4web/utils/auth.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.818078 py4web-1.20230416.3/py4web/utils/auth_plugins/
--rw-r--r--   0 massimo   (1000) massimo   (1000)     6207 2023-04-10 03:57:23.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-04-10 01:56:10.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     8154 2022-03-15 04:37:19.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/cas_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-04-10 01:56:10.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-04-10 03:57:06.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     3563 2022-03-14 19:17:56.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/newsamlplugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1759 2022-02-21 23:58:14.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      654 2020-10-10 04:20:35.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      514 2023-04-10 03:57:06.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      524 2020-10-10 04:20:35.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      489 2020-10-10 04:20:35.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      187 2023-04-10 01:56:10.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/cors.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-01-11 05:50:14.000000 py4web-1.20230416.3/py4web/utils/dbstore.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/downloader.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/factories.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-04-15 18:09:37.000000 py4web-1.20230416.3/py4web/utils/form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-04-10 02:55:45.000000 py4web-1.20230416.3/py4web/utils/grid.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2022-06-08 06:27:50.000000 py4web-1.20230416.3/py4web/utils/jsonrpc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2022-11-11 06:40:11.000000 py4web-1.20230416.3/py4web/utils/mailer.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2022-06-03 04:17:49.000000 py4web-1.20230416.3/py4web/utils/misc.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      502 2020-09-13 06:17:02.000000 py4web-1.20230416.3/py4web/utils/param.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/populate.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2022-05-31 06:26:42.000000 py4web-1.20230416.3/py4web/utils/publisher.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-03-19 21:28:12.000000 py4web-1.20230416.3/py4web/utils/recaptcha.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.3/py4web/utils/scheduler.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.3/py4web/utils/scheduler_old.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/security.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-04-15 18:18:02.000000 py4web-1.20230416.3/py4web/utils/url_signer.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.798077 py4web-1.20230416.3/py4web.egg-info/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1727 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)       44 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/entry_points.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2020-09-07 23:01:39.000000 py4web-1.20230416.3/py4web.egg-info/not-zip-safe
--rw-r--r--   0 massimo   (1000) massimo   (1000)      215 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/requires.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        7 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/top_level.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-04-17 05:04:36.818078 py4web-1.20230416.3/setup.cfg
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1758 2023-03-12 23:37:12.000000 py4web-1.20230416.3/setup.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.905419 py4web-1.20230507.1/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230507.1/LICENSE.md
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-08 02:45:11.905419 py4web-1.20230507.1/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230507.1/README.rst
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.893419 py4web-1.20230507.1/py4web/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      721 2023-05-08 00:45:22.000000 py4web-1.20230507.1/py4web/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    67416 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/core.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/server_adapters.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.901419 py4web-1.20230507.1/py4web/utils/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    69664 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.901419 py4web-1.20230507.1/py4web/utils/auth_plugins/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      514 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/pam.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/cors.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/dbstore.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/downloader.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/factories.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/grid.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/jsonrpc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/mailer.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/misc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/param.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/populate.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/publisher.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/recaptcha.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/security.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-05-08 00:39:45.000000 py4web-1.20230507.1/py4web/utils/url_signer.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.893419 py4web-1.20230507.1/py4web.egg-info/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1593 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/SOURCES.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/dependency_links.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       43 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/entry_points.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      239 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/requires.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        7 2023-05-08 02:45:11.000000 py4web-1.20230507.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1211 2023-05-08 02:44:58.000000 py4web-1.20230507.1/pyproject.toml
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-08 02:45:11.905419 py4web-1.20230507.1/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-08 02:45:11.905419 py4web-1.20230507.1/tests/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_action.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_auth.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_cache.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_fixture.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_get_error_snapshot.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_json.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_main.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_session.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_template.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230507.1/tests/test_url.py
```

### Comparing `py4web-1.20230416.3/README.rst` & `py4web-1.20230507.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/__init__.py` & `py4web-1.20230507.1/py4web/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSDv3"
-__version__ = "1.20230416.3"
+__version__ = "1.20230507.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230416.3/py4web/core.py` & `py4web-1.20230507.1/py4web/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1365,16 +1365,18 @@
         ICECUBE.update(threadsafevariable.ThreadSafeVariable.freeze())
 
     @staticmethod
     def register_route(app_name, rule, kwargs, func):
         url_prefix = os.environ.get("PY4WEB_URL_PREFIX", "")
         if url_prefix and rule == "/":
             rule = ""
+        else:
+            rule = url_prefix + rule
         dec_func = action.catch_errors(app_name, func)
-        bottle.route(url_prefix + rule, **kwargs)(dec_func)
+        bottle.route(rule, **kwargs)(dec_func)
         filename = module2filename(func.__module__)
         methods = kwargs.get("method", ["GET"])
         if isinstance(methods, str):
             methods = [methods]
         for method in methods:
             Reloader.ROUTES[app_name].append(
                 {
```

### Comparing `py4web-1.20230416.3/py4web/server_adapters.py` & `py4web-1.20230507.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth.py` & `py4web-1.20230507.1/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2github.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230507.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/cors.py` & `py4web-1.20230507.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/dbstore.py` & `py4web-1.20230507.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/downloader.py` & `py4web-1.20230507.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/factories.py` & `py4web-1.20230507.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/form.py` & `py4web-1.20230507.1/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/grid.py` & `py4web-1.20230507.1/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/jsonrpc.py` & `py4web-1.20230507.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/mailer.py` & `py4web-1.20230507.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/misc.py` & `py4web-1.20230507.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/populate.py` & `py4web-1.20230507.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/publisher.py` & `py4web-1.20230507.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/recaptcha.py` & `py4web-1.20230507.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/security.py` & `py4web-1.20230507.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.3/py4web/utils/url_signer.py` & `py4web-1.20230507.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

