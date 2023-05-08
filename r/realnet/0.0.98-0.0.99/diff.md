# Comparing `tmp/realnet-0.0.98.tar.gz` & `tmp/realnet-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realnet-0.0.98.tar", last modified: Tue Apr 25 01:39:21 2023, max compression
+gzip compressed data, was "realnet-0.0.99.tar", last modified: Thu Apr 27 00:41:32 2023, max compression
```

## Comparing `realnet-0.0.98.tar` & `realnet-0.0.99.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.771448 realnet-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-25 01:36:27.000000 realnet-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-25 01:39:21.771448 realnet-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-25 01:36:27.000000 realnet-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.751448 realnet-0.0.98/realnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/cmd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/core/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/aws/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/generic/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/org.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/orgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/sql/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/postgres/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/sql/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/xml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/xml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/provider/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/provider/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/realnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/accounts/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/attributes/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/auths/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/auths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/auths/auths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/chatgpt/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/clients/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/ctrls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/ctrls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/ctrls/ctrls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/endpoints/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/files/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/forms/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.759448 realnet-0.0.98/realnet/resource/gltf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/gltf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/gltf/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/gltf/gltf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/groups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/groups/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35333 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/items/items.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/public/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/public/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/resource/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/resource/views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/http/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.747448 realnet-0.0.98/realnet/runner/http/static/font-awesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.763448 realnet-0.0.98/realnet/runner/http/static/font-awesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.747448 realnet-0.0.98/realnet/runner/http/static/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/runner/http/static/scripts/ace/
--rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/ace.js
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-beautify.js
--rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-language_tools.js
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-css.js
--rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-html.js
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-javascript.js
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-json.js
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-python.js
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/http/static/scripts/ace/theme-monokai.js
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/runner/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/runner/sqs/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/shell/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/shell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.767448 realnet-0.0.98/realnet/static/initialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/access.json
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/apps.json
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/controls.json
--rw-r--r--   0 runner    (1001) docker     (123)    38721 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/core.json
--rw-r--r--   0 runner    (1001) docker     (123)   114896 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/forms.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/geometry.json
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/static/initialization/views.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.771448 realnet-0.0.98/realnet/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/control.html
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/register.html
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/register_org.html
--rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-25 01:36:27.000000 realnet-0.0.98/realnet/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:39:21.755448 realnet-0.0.98/realnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 01:39:21.000000 realnet-0.0.98/realnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:39:21.771448 realnet-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-25 01:36:33.000000 realnet-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.670707 realnet-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-27 00:38:41.000000 realnet-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-27 00:41:32.670707 realnet-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-04-27 00:38:41.000000 realnet-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/cmd/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/cmd/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/cmd/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/cmd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/cmd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/core/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/core/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21596 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/core/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/aws/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/generic/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/generic/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17851 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/orgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/sql/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/postgres/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/sql/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/xml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/provider/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/provider/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/realnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/accounts/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/attributes/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/auths/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/auths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/auths/auths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/chatgpt/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/clients/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/ctrls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/ctrls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/ctrls/ctrls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/endpoints/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/files/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/forms/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/gltf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/gltf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/gltf/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/gltf/gltf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/groups/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35402 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/items/items.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/public/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/public/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21652 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/resource/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/resource/views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/runner/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/runner/http/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.654707 realnet-0.0.99/realnet/runner/http/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.662707 realnet-0.0.99/realnet/runner/http/static/font-awesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.666707 realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   134808 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.654707 realnet-0.0.99/realnet/runner/http/static/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.666707 realnet-0.0.99/realnet/runner/http/static/scripts/ace/
+-rw-r--r--   0 runner    (1001) docker     (123)   373401 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/ace.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/ext-beautify.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39778 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/ext-language_tools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-css.js
+-rw-r--r--   0 runner    (1001) docker     (123)   101769 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-html.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-javascript.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-json.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-python.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/http/static/scripts/ace/theme-monokai.js
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.666707 realnet-0.0.99/realnet/runner/sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/runner/sqs/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.666707 realnet-0.0.99/realnet/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/shell/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/shell/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/shell/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/shell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.666707 realnet-0.0.99/realnet/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.670707 realnet-0.0.99/realnet/static/initialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/access.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/apps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/controls.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33061 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/core.json
+-rw-r--r--   0 runner    (1001) docker     (123)   114896 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/forms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/geometry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/static/initialization/views.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.670707 realnet-0.0.99/realnet/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/control.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/register.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/register_org.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-04-27 00:38:41.000000 realnet-0.0.99/realnet/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:41:32.658707 realnet-0.0.99/realnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-27 00:41:32.000000 realnet-0.0.99/realnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-27 00:41:32.000000 realnet-0.0.99/realnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:41:32.000000 realnet-0.0.99/realnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 00:41:32.000000 realnet-0.0.99/realnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 00:41:32.000000 realnet-0.0.99/realnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 00:41:32.000000 realnet-0.0.99/realnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:41:32.670707 realnet-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-27 00:38:44.000000 realnet-0.0.99/setup.py
```

### Comparing `realnet-0.0.98/LICENSE` & `realnet-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/PKG-INFO` & `realnet-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.98
+Version: 0.0.99
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.98/README.md` & `realnet-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/cmd/server.py` & `realnet-0.0.99/realnet/cmd/server.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/core/config.py` & `realnet-0.0.99/realnet/core/config.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/core/hierarchy.py` & `realnet-0.0.99/realnet/core/hierarchy.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/core/provider.py` & `realnet-0.0.99/realnet/core/provider.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/core/type.py` & `realnet-0.0.99/realnet/core/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/aws/data.py` & `realnet-0.0.99/realnet/provider/aws/data.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/generic/endpoint.py` & `realnet-0.0.99/realnet/provider/generic/endpoint.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/generic/resource.py` & `realnet-0.0.99/realnet/provider/generic/resource.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/sql/client.py` & `realnet-0.0.99/realnet/provider/sql/client.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/sql/init.py` & `realnet-0.0.99/realnet/provider/sql/init.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/sql/models.py` & `realnet-0.0.99/realnet/provider/sql/models.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/sql/org.py` & `realnet-0.0.99/realnet/provider/sql/org.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,75 +145,75 @@
         if [acl for acl in item.acls if acl.type == AclType.public]:
             return True
 
         return False
 
     def can_account_execute_item(self, account, item):
         
-        if [acl for acl in item.acls if acl.type == AclType.public]:
+        if [acl for acl in item.acls if acl.type.value == AclType.public.value]:
             return True
 
-        if [acl for acl in item.acls if acl.type == AclType.user and acl.target_id == account.id and acl.permission and  'e' in acl.permission]:
+        if [acl for acl in item.acls if acl.type.value == AclType.user.value and acl.target_id == account.id and acl.permission and  'e' in acl.permission]:
             return True
 
         account_groups = db.query(AccountGroupModel).filter(AccountGroupModel.account_id == account.id).all()
         group_ids = []
         for account_group in account_groups:
             group_ids.append(account_group.group_id)
 
-        if [acl for acl in item.acls if acl.type == AclType.org and acl.org_id == account.org_id and  acl.permission and 'e' in acl.permission]:
+        if [acl for acl in item.acls if acl.type.value == AclType.org.value and acl.org_id == account.org.id and  acl.permission and 'e' in acl.permission]:
             return True
 
-        if [acl for acl in item.acls if acl.type == AclType.group and acl.target_id in group_ids and  acl.permission and 'e' in acl.permission]:
+        if [acl for acl in item.acls if acl.type.value == AclType.group.value and acl.target_id in group_ids and  acl.permission and 'e' in acl.permission]:
             return True
 
         if item.owner_id == account.id:
             return True
 
 
     def can_account_message_item(self, account, item):
 
-        if [acl for acl in item.acls if acl.type == AclType.public]:
+        if [acl for acl in item.acls if acl.type.value == AclType.public.value]:
             return True
 
-        if [acl for acl in item.acls if acl.type == AclType.user and acl.target_id == account.id and  acl.permission and 'm' in acl.permission]:
+        if [acl for acl in item.acls if acl.type.value == AclType.user.value and acl.target_id == account.id and  acl.permission and 'm' in acl.permission]:
             return True
 
         account_groups = db.query(AccountGroupModel).filter(AccountGroupModel.account_id == account.id).all()
         group_ids = []
         for account_group in account_groups:
             group_ids.append(account_group.group_id)
 
-        if [acl for acl in item.acls if acl.type == AclType.org and acl.org_id == account.org_id and acl.permission and  'm' in acl.permission]:
+        if [acl for acl in item.acls if acl.type.value == AclType.org.value and acl.org_id == account.org.id and acl.permission and  'm' in acl.permission]:
             return True
 
-        if [acl for acl in item.acls if acl.type == AclType.group and acl.target_id in group_ids and acl.permission and  'm' in acl.permission]:
+        if [acl for acl in item.acls if acl.type.value == AclType.group.value and acl.target_id in group_ids and acl.permission and  'm' in acl.permission]:
             return True
 
         if item.owner_id == account.id:
             return True
 
 
     def can_account_read_item(self, account, item):
 
-        if [acl for acl in item.acls if acl.type == AclType.public]:
+        if [acl for acl in item.acls if acl.type.value == AclType.public.value]:
             return True
 
-        if [acl for acl in item.acls if acl.type == AclType.user and acl.target_id == account.id and acl.permission and ('r' in acl.permission or 'w' in acl.permission)]:
+        if [acl for acl in item.acls if acl.type.value == AclType.user.value and acl.target_id == account.id and acl.permission and ('r' in acl.permission or 'w' in acl.permission)]:
             return True
 
         account_groups = db.query(AccountGroupModel).filter(AccountGroupModel.account_id == account.id).all()
         group_ids = []
         for account_group in account_groups:
             group_ids.append(account_group.group_id)
 
-        if [acl for acl in item.acls if acl.type == AclType.group and acl.target_id in group_ids and acl.permission and  ('r' in acl.permission or 'w' in acl.permission)]:
+        if [acl for acl in item.acls if acl.type.value == AclType.group.value and acl.target_id in group_ids and acl.permission and  ('r' in acl.permission or 'w' in acl.permission)]:
             return True
 
-        if [acl for acl in item.acls if acl.type == AclType.org and acl.org_id == account.org_id and acl.permission and  ('r' in acl.permission or 'w' in acl.permission)]:
+        if [acl for acl in item.acls if acl.type.value == AclType.org.value and acl.org_id == account.org.id and acl.permission and  ('r' in acl.permission or 'w' in acl.permission)]:
             return True
 
         if item.owner_id == account.id:
             return True
 
 
     def can_account_write_item(self, account, item):
@@ -224,25 +224,25 @@
 
         account_groups = db.query(AccountGroupModel).filter(AccountGroupModel.account_id == account.id).all()
         group_ids = []
         for account_group in account_groups:
             group_ids.append(account_group.group_id)
 
         if [acl for acl in item.acls if
-            acl.type == AclType.group and acl.target_id in group_ids and acl.permission and 'w' in acl.permission]:
+            acl.type.value == AclType.group.value and acl.target_id in group_ids and acl.permission and 'w' in acl.permission]:
             return True
 
-        if [acl for acl in item.acls if acl.type == AclType.org and acl.org_id == account.org_id and acl.permission and  'w' in acl.permission]:
+        if [acl for acl in item.acls if acl.type.value == AclType.org.value and acl.org_id == account.org.id and acl.permission and  'w' in acl.permission]:
             return True
 
         if item.owner_id == account.id:
             return True
 
     def can_account_delete_item(self, account, item):
-        return item.owner_id == account.id and account.org_id == item.org_id
+        return item.owner_id == account.id and account.org.id == item.org_id
 
     # group provider
 
     def get_groups(self):
         pass
 
     # account provider
```

### Comparing `realnet-0.0.98/realnet/provider/sql/orgs.py` & `realnet-0.0.99/realnet/provider/sql/orgs.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/sql/postgres/item.py` & `realnet-0.0.99/realnet/provider/sql/postgres/item.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/sql/roles.py` & `realnet-0.0.99/realnet/provider/sql/roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         return Role(role.id, role.name, org, [])
         
 
     def delete_role(self, id):
         role = db.query(RoleModel).filter(RoleModel.org_id == self.org_id, RoleModel.id == id).first()
         if role:
             db.delete(role)
+            db.commit()
 
     def update_role(self, id, **kwargs):
         pass
 
     def get_role(self, id):
         tbn = get_types_by_name(self.org_id)
         role = db.query(RoleModel).filter(RoleModel.org_id == self.org_id, or_(RoleModel.id == id, RoleModel.name == id)).first()
```

### Comparing `realnet-0.0.98/realnet/provider/sql/type.py` & `realnet-0.0.99/realnet/provider/sql/type.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/provider/sql/utility.py` & `realnet-0.0.99/realnet/provider/sql/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,18 @@
         if str(item_data['item_is_public']).lower() == 'true':
             create_public_acl = True
 
     if create_public_acl:
         acl = AclModel(id=str(uuid.uuid4()),type='public', org_id=org_id, item_id=item_id)
         db.add(acl)
         db.commit()
+    else:
+        acl = AclModel(id=str(uuid.uuid4()),type='org', org_id=org_id, item_id=item_id, permission='r')
+        db.add(acl)
+        db.commit()
     
     # instances1 = instance.type.instances
     # instances2 = instance.type.base.instances
     instances = get_type_instances(instance.type)
     for child_instance in instances:
         attributes = get_type_attributes(child_instance.type)
         if attributes:
```

### Comparing `realnet-0.0.98/realnet/resource/accounts/accounts.py` & `realnet-0.0.99/realnet/resource/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/apps/apps.py` & `realnet-0.0.99/realnet/resource/apps/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from realnet.resource.items.items import Items
 
 class Apps(Items):
     
     def get_query(self, module, account, query, parent_item=None):
         return {'types':['App']}
     
+    def get_items(self, module, endpoint, args, path, account, query, parent_item=None):
+        return module.get_apps(module)
+    
     def post(self, module, endpoint, args, path=None, content_type='text/html'):
         
         # app_type = module.create_type(name=args.get('name'), base='App')
         
         resource = module.get_resource(module, args.get('resource'))
         if not resource:
             resource_item = module.create_item(name=args.get('resource'), type='Resource', attributes={'module':'true'}, public='true')
```

### Comparing `realnet-0.0.98/realnet/resource/auths/auths.py` & `realnet-0.0.99/realnet/resource/auths/auths.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/chatgpt/chatgpt.py` & `realnet-0.0.99/realnet/resource/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/clients/clients.py` & `realnet-0.0.99/realnet/resource/clients/clients.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/ctrls/ctrls.py` & `realnet-0.0.99/realnet/resource/ctrls/ctrls.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/files/files.py` & `realnet-0.0.99/realnet/resource/files/files.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/gltf/export.py` & `realnet-0.0.99/realnet/resource/gltf/export.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/gltf/gltf.py` & `realnet-0.0.99/realnet/resource/gltf/gltf.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/groups/groups.py` & `realnet-0.0.99/realnet/resource/groups/groups.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/items/items.py` & `realnet-0.0.99/realnet/resource/items/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -593,14 +593,17 @@
         
         active_subview_name = args.get('subview')
 
         if active_subview_name and not isinstance(active_subview_name, str):
             active_subview_name = active_subview_name[0]
 
         app = next((a for a in apps if a.name.lower() == endpoint.item.name), None)
+
+        if not app:
+            app = next((a for a in apps), None)
         
         if apps:
             if active_app_name:
                 app = next((a for a in apps if a.name.lower() == active_app_name), app)
 
         path_item = app
         target_item = app
```

### Comparing `realnet-0.0.98/realnet/resource/login/login.py` & `realnet-0.0.99/realnet/resource/login/login.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/roles/roles.py` & `realnet-0.0.99/realnet/resource/roles/roles.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/types/types.py` & `realnet-0.0.99/realnet/resource/types/types.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/resource/views/views.py` & `realnet-0.0.99/realnet/resource/views/views.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/app.py` & `realnet-0.0.99/realnet/runner/http/app.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/auth.py` & `realnet-0.0.99/realnet/runner/http/auth.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/router.py` & `realnet-0.0.99/realnet/runner/http/router.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.css` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/css/font-awesome.min.css` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2` & `realnet-0.0.99/realnet/runner/http/static/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/ace.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/ace.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-beautify.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/ext-beautify.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/ext-language_tools.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/ext-language_tools.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-css.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-css.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-html.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-html.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-javascript.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-javascript.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-json.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-json.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/mode-python.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/runner/http/static/scripts/ace/theme-monokai.js` & `realnet-0.0.99/realnet/runner/http/static/scripts/ace/theme-monokai.js`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/shell/cmd.py` & `realnet-0.0.99/realnet/shell/cmd.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/shell/proto.py` & `realnet-0.0.99/realnet/shell/proto.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/shell/shell.py` & `realnet-0.0.99/realnet/shell/shell.py`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/static/initialization/access.json` & `realnet-0.0.99/realnet/static/initialization/access.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/static/initialization/apps.json` & `realnet-0.0.99/realnet/static/initialization/apps.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/static/initialization/controls.json` & `realnet-0.0.99/realnet/static/initialization/controls.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/static/initialization/core.json` & `realnet-0.0.99/realnet/static/initialization/core.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9892636684303351%*

 * *Differences: {"'types'": "{0: {'attributes': {'icon': 'extension', 'resource': 'types', 'menu': {0: {'name': "*

 * *            "'Add Instance', 'attributes': {'form': 'InstanceCreateForm'}}, 1: {'attributes': "*

 * *            "{'path': 'types'}}, 2: {'attributes': {'path': 'types'}}, 3: {'attributes': {'path': "*

 * *            "'types'}}, delete: [3]}, 'forms': {0: {'attributes': {'path': 'types', 'form': "*

 * *            "'TypeCreateForm'}}, 1: {'attributes': {'path': 'types', 'form': 'TypeEditForm'}}, 2: "*

 * *            "{'attribute […]*

```diff
@@ -1,79 +1,157 @@
 {
     "types": [
         {
             "attributes": {
                 "forms": [
                     {
                         "attributes": {
-                            "form": "ItemCreateForm",
-                            "path": "items"
+                            "form": "TypeCreateForm",
+                            "path": "types"
                         },
                         "name": "create",
                         "type": "FormItem"
                     },
                     {
                         "attributes": {
-                            "form": "ItemEditForm",
-                            "path": "items"
+                            "form": "TypeEditForm",
+                            "path": "types"
                         },
                         "name": "edit",
                         "type": "FormItem"
                     },
                     {
                         "attributes": {
                             "form": "DeleteForm",
-                            "path": "items"
+                            "path": "types"
                         },
                         "name": "delete",
                         "type": "FormItem"
                     }
                 ],
-                "icon": "square",
+                "icon": "extension",
                 "menu": [
                     {
                         "attributes": {
-                            "form": "ItemCreateForm",
+                            "form": "InstanceCreateForm",
                             "icon": "add"
                         },
-                        "name": "Add Item",
+                        "name": "Add Instance",
                         "type": "MenuItem"
                     },
                     {
                         "attributes": {
                             "form": "ViewCreateForm",
                             "icon": "add_box",
-                            "path": "items"
+                            "path": "types"
                         },
                         "name": "Add View",
                         "type": "MenuItem"
                     },
                     {
                         "attributes": {
                             "form": "QueryForm",
                             "icon": "search",
-                            "path": "items"
+                            "path": "types"
                         },
                         "name": "Query",
                         "type": "MenuItem"
                     },
                     {
                         "attributes": {
-                            "form": "CodeForm",
-                            "icon": "functions",
-                            "path": "items"
+                            "form": "SettingsForm",
+                            "icon": "settings",
+                            "path": "types"
+                        },
+                        "name": "Settings",
+                        "type": "MenuItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "SharingForm",
+                            "icon": "lock"
+                        },
+                        "name": "Sharing",
+                        "type": "MenuItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "UploadForm",
+                            "icon": "file_upload",
+                            "import": "true"
+                        },
+                        "name": "Import",
+                        "type": "MenuItem"
+                    }
+                ],
+                "resource": "types"
+            },
+            "name": "Type"
+        },
+        {
+            "attributes": {
+                "forms": [
+                    {
+                        "attributes": {
+                            "form": "InstanceCreateForm",
+                            "path": "types"
+                        },
+                        "name": "create",
+                        "type": "FormItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "InstanceEditForm",
+                            "path": "types"
+                        },
+                        "name": "edit",
+                        "type": "FormItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "DeleteForm",
+                            "path": "types"
+                        },
+                        "name": "delete",
+                        "type": "FormItem"
+                    }
+                ],
+                "icon": "extension",
+                "menu": [
+                    {
+                        "attributes": {
+                            "form": "InstanceCreateForm",
+                            "icon": "add"
+                        },
+                        "name": "Add Instance",
+                        "type": "MenuItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "ViewCreateForm",
+                            "icon": "add_box",
+                            "path": "types"
+                        },
+                        "name": "Add View",
+                        "type": "MenuItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "QueryForm",
+                            "icon": "search",
+                            "path": "types"
                         },
-                        "name": "Code",
+                        "name": "Query",
                         "type": "MenuItem"
                     },
                     {
                         "attributes": {
                             "form": "SettingsForm",
                             "icon": "settings",
-                            "path": "items"
+                            "path": "types"
                         },
                         "name": "Settings",
                         "type": "MenuItem"
                     },
                     {
                         "attributes": {
                             "form": "SharingForm",
@@ -88,287 +166,103 @@
                             "icon": "file_upload",
                             "import": "true"
                         },
                         "name": "Import",
                         "type": "MenuItem"
                     }
                 ],
-                "resource": "items",
-                "views": [
+                "resource": "types"
+            },
+            "base": "Type",
+            "name": "Instance"
+        },
+        {
+            "attributes": {
+                "forms": [
                     {
                         "attributes": {
-                            "menu": [
-                                {
-                                    "attributes": {
-                                        "form": "ItemCreateForm",
-                                        "icon": "add"
-                                    },
-                                    "name": "Add Item",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "ViewCreateForm",
-                                        "icon": "add_box",
-                                        "path": "items"
-                                    },
-                                    "name": "Add View",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "DeleteForm",
-                                        "icon": "delete",
-                                        "path": "items"
-                                    },
-                                    "name": "Delete",
-                                    "type": "MenuItem"
-                                }
-                            ],
-                            "query": {
-                                "children": "true",
-                                "types": [
-                                    "Item"
-                                ]
-                            },
-                            "types": [
-                                "Item"
-                            ]
-                        },
-                        "name": "Items",
-                        "type": "ListView"
-                    },
-                    {
-                        "attributes": {
-                            "columns": [
-                                {
-                                    "attributes": {
-                                        "namespace": "attributes",
-                                        "target": "value"
-                                    },
-                                    "name": "Value",
-                                    "type": "Column"
-                                }
-                            ],
-                            "hidden": "true",
-                            "internal": "true",
-                            "menu": [
-                                {
-                                    "attributes": {
-                                        "form": "AttributeCreateForm",
-                                        "icon": "add",
-                                        "path": "items"
-                                    },
-                                    "name": "Add Attribute",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "ViewCreateForm",
-                                        "icon": "add_box",
-                                        "path": "items"
-                                    },
-                                    "name": "Add View",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "DeleteForm",
-                                        "icon": "delete",
-                                        "path": "items"
-                                    },
-                                    "name": "Delete",
-                                    "type": "MenuItem"
-                                }
-                            ],
-                            "source": "attributes"
-                        },
-                        "name": "Attributes",
-                        "type": "ListView"
-                    },
-                    {
-                        "attributes": {
-                            "columns": [
-                                {
-                                    "attributes": {
-                                        "target": "form"
-                                    },
-                                    "name": "Form",
-                                    "type": "Column"
-                                },
-                                {
-                                    "attributes": {
-                                        "target": "path"
-                                    },
-                                    "name": "Path",
-                                    "type": "Column"
-                                }
-                            ],
-                            "hidden": "true",
-                            "internal": "true",
-                            "menu": [
-                                {
-                                    "attributes": {
-                                        "form": "FormItemCreateForm",
-                                        "icon": "add",
-                                        "path": "items"
-                                    },
-                                    "name": "Add Form",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "ViewCreateForm",
-                                        "icon": "add_box",
-                                        "path": "items"
-                                    },
-                                    "name": "Add View",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "DeleteForm",
-                                        "icon": "delete",
-                                        "path": "items"
-                                    },
-                                    "name": "Delete",
-                                    "type": "FormItem"
-                                }
-                            ],
-                            "source": "forms"
-                        },
-                        "name": "Forms",
-                        "type": "ListView"
-                    },
-                    {
-                        "attributes": {
-                            "columns": [
-                                {
-                                    "attributes": {
-                                        "namespace": "attributes",
-                                        "target": "form"
-                                    },
-                                    "name": "Form",
-                                    "type": "Column"
-                                },
-                                {
-                                    "attributes": {
-                                        "target": "path"
-                                    },
-                                    "name": "Path",
-                                    "type": "Column"
-                                }
-                            ],
-                            "hidden": "true",
-                            "internal": "true",
-                            "menu": [
-                                {
-                                    "attributes": {
-                                        "form": "MenuItemCreateForm",
-                                        "icon": "add",
-                                        "path": "items"
-                                    },
-                                    "name": "Add Menu Item",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "ViewCreateForm",
-                                        "icon": "add_box",
-                                        "path": "items"
-                                    },
-                                    "name": "Add View",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "DeleteForm",
-                                        "icon": "delete",
-                                        "path": "items"
-                                    },
-                                    "name": "Delete",
-                                    "type": "MenuItem"
-                                }
-                            ],
-                            "source": "menu"
+                            "form": "ItemCreateForm",
+                            "path": "items"
                         },
-                        "name": "Menu",
-                        "type": "ListView"
+                        "name": "create",
+                        "type": "FormItem"
                     },
                     {
                         "attributes": {
                             "form": "ItemEditForm",
-                            "hidden": "true"
+                            "path": "items"
                         },
-                        "name": "Settings",
-                        "type": "FormView"
+                        "name": "edit",
+                        "type": "FormItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "DeleteForm",
+                            "path": "items"
+                        },
+                        "name": "delete",
+                        "type": "FormItem"
+                    }
+                ],
+                "menu": [
+                    {
+                        "attributes": {
+                            "form": "ItemCreateForm",
+                            "icon": "add"
+                        },
+                        "name": "Add Item",
+                        "type": "MenuItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "ViewCreateForm",
+                            "icon": "add_box",
+                            "path": "items"
+                        },
+                        "name": "Add View",
+                        "type": "MenuItem"
                     },
                     {
                         "attributes": {
                             "form": "QueryForm",
-                            "hidden": "true"
+                            "icon": "search",
+                            "path": "items"
                         },
                         "name": "Query",
-                        "type": "FormView"
+                        "type": "MenuItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "SettingsForm",
+                            "icon": "settings",
+                            "path": "items"
+                        },
+                        "name": "Settings",
+                        "type": "MenuItem"
                     },
                     {
                         "attributes": {
-                            "hidden": "true",
-                            "menu": [
-                                {
-                                    "attributes": {
-                                        "form": "ItemUploadForm",
-                                        "icon": "file_upload",
-                                        "import": "true",
-                                        "path": "items"
-                                    },
-                                    "name": "Import",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "ViewCreateForm",
-                                        "icon": "add_box",
-                                        "path": "items"
-                                    },
-                                    "name": "Add View",
-                                    "type": "MenuItem"
-                                },
-                                {
-                                    "attributes": {
-                                        "form": "DeleteForm",
-                                        "icon": "delete",
-                                        "path": "items"
-                                    },
-                                    "name": "Delete",
-                                    "type": "MenuItem"
-                                }
-                            ],
-                            "query": {
-                                "children": "true",
-                                "types": [
-                                    "Media"
-                                ]
-                            },
-                            "types": [
-                                "Media"
-                            ]
+                            "form": "SharingForm",
+                            "icon": "lock"
                         },
-                        "name": "Files",
-                        "type": "ListView"
+                        "name": "Sharing",
+                        "type": "MenuItem"
+                    },
+                    {
+                        "attributes": {
+                            "form": "UploadForm",
+                            "icon": "file_upload",
+                            "import": "true"
+                        },
+                        "name": "Import",
+                        "type": "MenuItem"
                     }
-                ]
+                ],
+                "resource": "items"
             },
-            "name": "Type"
-        },
-        {
-            "base": "Type",
-            "name": "Instance"
-        },
-        {
             "base": "Instance",
             "name": "Item"
         },
         {
             "attributes": {
                 "icon": "link"
             },
```

### Comparing `realnet-0.0.98/realnet/static/initialization/forms.json` & `realnet-0.0.99/realnet/static/initialization/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998800505050505%*

 * *Differences: {"'types'": "{37: {'attributes': {'path': 'items'}}, 38: {'attributes': {'path': 'items'}}, 39: "*

 * *            "{'attributes': {'path': 'items'}}, 40: {'attributes': {'path': 'items'}}, 41: "*

 * *            "{'attributes': {'path': 'items'}}, 42: {'attributes': {'path': 'items'}}, 43: "*

 * *            "{'attributes': {'path': 'items'}}, 44: {'attributes': {'path': 'items'}}, 45: "*

 * *            "{'attributes': {'path': 'items'}}, 46: {'attributes': {'path': 'items'}}, 47: "*

 * *            "{'attributes': {'path': 'item […]*

```diff
@@ -2311,15 +2311,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Create",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "title_prefix": "Add Attribute",
                 "type": "Attribute"
             },
             "base": "CreateForm",
             "name": "AttributeCreateForm"
         },
         {
@@ -2385,15 +2385,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Save",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "title_prefix": "Edit",
                 "type": "Attribute"
             },
             "base": "EditForm",
             "name": "AttributeEditForm"
         },
         {
@@ -2445,15 +2445,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Delete",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "type": "Attribute"
             },
             "base": "DeleteForm",
             "name": "AttributeDeleteForm"
         },
         {
             "attributes": {
@@ -2520,15 +2520,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Create",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "title_prefix": "Add MenuItem",
                 "type": "MenuItem"
             },
             "base": "CreateForm",
             "name": "MenuItemCreateForm"
         },
         {
@@ -2604,15 +2604,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Save",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "title_prefix": "Edit",
                 "type": "Attribute"
             },
             "base": "EditForm",
             "name": "MenuItemEditForm"
         },
         {
@@ -2664,15 +2664,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Delete",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "type": "MenuItem"
             },
             "base": "DeleteForm",
             "name": "MenuItemDeleteForm"
         },
         {
             "attributes": {
@@ -2732,15 +2732,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Create",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "title_prefix": "Add MenuItem",
                 "type": "MenuItem"
             },
             "base": "CreateForm",
             "name": "FormItemCreateForm"
         },
         {
@@ -2809,15 +2809,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Save",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "title_prefix": "Edit",
                 "type": "Attribute"
             },
             "base": "EditForm",
             "name": "FormItemEditForm"
         },
         {
@@ -2869,15 +2869,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Delete",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "type": "MenuItem"
             },
             "base": "DeleteForm",
             "name": "FormItemDeleteForm"
         },
         {
             "attributes": {
@@ -2922,15 +2922,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Create",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "type": "View"
             },
             "base": "CreateForm",
             "name": "ViewCreateForm"
         },
         {
             "attributes": {
@@ -2982,15 +2982,15 @@
                             "default": "true",
                             "order": "9"
                         },
                         "name": "Delete",
                         "type": "ButtonCtrl"
                     }
                 ],
-                "path": "types",
+                "path": "items",
                 "type": "View"
             },
             "base": "DeleteForm",
             "name": "ViewDeleteForm"
         },
         {
             "attributes": {
```

### Comparing `realnet-0.0.98/realnet/static/initialization/geometry.json` & `realnet-0.0.99/realnet/static/initialization/geometry.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/static/initialization/views.json` & `realnet-0.0.99/realnet/static/initialization/views.json`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/control.html` & `realnet-0.0.99/realnet/templates/control.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/form.html` & `realnet-0.0.99/realnet/templates/form.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/item.html` & `realnet-0.0.99/realnet/templates/item.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/login.html` & `realnet-0.0.99/realnet/templates/login.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/main.html` & `realnet-0.0.99/realnet/templates/main.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/nav.html` & `realnet-0.0.99/realnet/templates/nav.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/register.html` & `realnet-0.0.99/realnet/templates/register.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/register_org.html` & `realnet-0.0.99/realnet/templates/register_org.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet/templates/view.html` & `realnet-0.0.99/realnet/templates/view.html`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/realnet.egg-info/PKG-INFO` & `realnet-0.0.99/realnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realnet
-Version: 0.0.98
+Version: 0.0.99
 Summary: Realnet command line interface
 Home-page: https://github.com/virtual-space/realnet
 Author: Marko Laban
 Author-email: marko.laban@l33tsystems.com
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `realnet-0.0.98/realnet.egg-info/SOURCES.txt` & `realnet-0.0.99/realnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `realnet-0.0.98/setup.py` & `realnet-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="realnet",
-    version="0.0.98",
+    version="0.0.99",
     description="Realnet command line interface",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/virtual-space/realnet",
     author="Marko Laban",
     author_email="marko.laban@l33tsystems.com",
     license="BSD",
```

