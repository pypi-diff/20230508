# Comparing `tmp/jupyterlab_code_formatter-1.6.1.tar.gz` & `tmp/jupyterlab_code_formatter-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_code_formatter-1.6.1.tar", last modified: Sun Apr 16 18:07:31 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_code_formatter-1.6.1.tar` & `jupyterlab_code_formatter-2.0.0rc1.tar`

### file list

```diff
@@ -1,45 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/
--rw-rw-r--   0 root         (0) root         (0)     1052 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      447 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3429 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2668 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      211 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/install.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.845280 jupyterlab_code_formatter-1.6.1/jupyter-config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.849280 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_notebook_config.d/
--rw-rw-r--   0 root         (0) root         (0)      102 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_notebook_config.d/jupyterlab_code_formatter.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.849280 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_server_config.d/
--rw-rw-r--   0 root         (0) root         (0)      100 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_server_config.d/jupyterlab_code_formatter.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.849280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/
--rw-rw-r--   0 root         (0) root         (0)      819 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      459 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/_version.py
--rw-rw-r--   0 root         (0) root         (0)    12749 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/formatters.py
--rw-rw-r--   0 root         (0) root         (0)     4316 2023-04-16 16:44:42.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/
--rw-rw-r--   0 root         (0) root         (0)     2734 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.845280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.845280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/
--rw-rw-r--   0 root         (0) root         (0)     2618 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/package.json.orig
--rw-rw-r--   0 root         (0) root         (0)    13640 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/
--rw-r--r--   0 root         (0) root         (0)     8139 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/160.ee2bfa087021ad817bae.js
--rw-r--r--   0 root         (0) root         (0)     6650 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/remoteEntry.d347e3dfbeaa4b572523.js
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/style.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3429 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 17:20:18.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     2618 2023-04-16 17:56:10.000000 jupyterlab_code_formatter-1.6.1/package.json
--rw-rw-r--   0 root         (0) root         (0)      145 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2725 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/src/
--rw-rw-r--   0 root         (0) root         (0)     1184 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/src/client.ts
--rw-rw-r--   0 root         (0) root         (0)     1350 2023-04-16 17:56:10.000000 jupyterlab_code_formatter-1.6.1/src/constants.ts
--rw-rw-r--   0 root         (0) root         (0)     7391 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/src/formatter.ts
--rw-rw-r--   0 root         (0) root         (0)     7789 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/src/index.ts
--rw-rw-r--   0 root         (0) root         (0)      534 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/tsconfig.json
--rw-rw-r--   0 root         (0) root         (0)     3817 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/tslint.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/.prettierignore
+-rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/RELEASE.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/Taskfile.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/babel.config.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/conftest.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/dev.Dockerfile
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/dev.md
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docker-compose.dev.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jest.config.js
+-rw-r--r--   0        0        0     6568 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/package.json
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/requirements-dev.txt
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/requirements-test.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/tsconfig.json
+-rw-r--r--   0        0        0   383940 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/yarn.lock
+-rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/changelog.md
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/conf.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/configuration.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/custom-formatter.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/dev.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/faq.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/index.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/installation.md
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/jupyterhub.md
+-rw-r--r--   0        0        0    27767 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/logo.png
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/usage.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/your-support.md
+-rw-r--r--   0        0        0   493973 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/_static/format-all.gif
+-rw-r--r--   0        0        0   836371 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/_static/format-selected.gif
+-rw-r--r--   0        0        0  1862680 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/_static/format-specific.gif
+-rw-r--r--   0        0        0  1408342 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/docs/_static/settings.gif
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyter-config/nb-config/jupyterlab_code_formatter.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyter-config/server-config/jupyterlab_code_formatter.json
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/_version.py
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/formatters.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/handlers.py
+-rw-r--r--   0        0        0    20715 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/build_log.json
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/package.json
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/package.json.orig
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/settings.json
+-rw-r--r--   0        0        0    22284 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/lib_index_js.fa888f63ee8b6baa7702.js
+-rw-r--r--   0        0        0    18763 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/lib_index_js.fa888f63ee8b6baa7702.js.map
+-rw-r--r--   0        0        0    29560 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/remoteEntry.9e630a82597c575616f5.js
+-rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/remoteEntry.9e630a82597c575616f5.js.map
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/style.js
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js.map
+-rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js.map
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/tests/__init__.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/tests/conftest.py
+-rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/tests/test_handlers.py
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/schema/settings.json
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/scripts/format.sh
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/scripts/test.sh
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/src/client.ts
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/src/constants.ts
+-rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/src/formatter.ts
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/src/index.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/src/__tests__/jupyterlab_code_formatter.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/style/index.js
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/test_snippets/some_python.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/test_snippets/test_notebook.ipynb
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/test_snippets/test_notebook_crablang.ipynb
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/ui-tests/tests/jupyterlab_code_formatter.spec.ts
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/README.md
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc1/PKG-INFO
```

### Comparing `jupyterlab_code_formatter-1.6.1/LICENSE` & `jupyterlab_code_formatter-2.0.0rc1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2018 Hin Hong TAM
+Copyright 2023 Ryan TAM
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `jupyterlab_code_formatter-1.6.1/README.md` & `jupyterlab_code_formatter-2.0.0rc1/docs/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,146 @@
-00000000: 215b 5d28 646f 6373 5f73 7263 2f6c 6f67  ![](docs_src/log
-00000010: 6f2e 706e 6729 0a0a 2a41 204a 7570 7974  o.png)..*A Jupyt
-00000020: 6572 4c61 6220 706c 7567 696e 2074 6f20  erLab plugin to 
-00000030: 6661 6369 6c69 7461 7465 2069 6e76 6f63  facilitate invoc
-00000040: 6174 696f 6e20 6f66 2063 6f64 6520 666f  ation of code fo
-00000050: 726d 6174 7465 7273 2e2a 0a0a 5b21 5b42  rmatters.*..[![B
-00000060: 696e 6465 725d 2868 7474 7073 3a2f 2f6d  inder](https://m
-00000070: 7962 696e 6465 722e 6f72 672f 6261 6467  ybinder.org/badg
-00000080: 655f 6c6f 676f 2e73 7667 295d 2868 7474  e_logo.svg)](htt
-00000090: 7073 3a2f 2f6d 7962 696e 6465 722e 6f72  ps://mybinder.or
-000000a0: 672f 7632 2f67 682f 7279 616e 7461 6d36  g/v2/gh/ryantam6
-000000b0: 3236 2f6a 7570 7974 6572 6c61 625f 636f  26/jupyterlab_co
-000000c0: 6465 5f66 6f72 6d61 7474 6572 2f6d 6173  de_formatter/mas
-000000d0: 7465 723f 7572 6c70 6174 683d 6c61 6229  ter?urlpath=lab)
-000000e0: 0a5b 215b 6e70 6d20 7665 7273 696f 6e5d  .[![npm version]
-000000f0: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
-00000100: 7572 792e 696f 2f6a 732f 2534 3072 7961  ury.io/js/%40rya
-00000110: 6e74 616d 3632 3625 3246 6a75 7079 7465  ntam626%2Fjupyte
-00000120: 726c 6162 5f63 6f64 655f 666f 726d 6174  rlab_code_format
-00000130: 7465 722e 7376 6729 5d28 6874 7470 733a  ter.svg)](https:
-00000140: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
-00000150: 6a73 2f25 3430 7279 616e 7461 6d36 3236  js/%40ryantam626
-00000160: 2532 466a 7570 7974 6572 6c61 625f 636f  %2Fjupyterlab_co
-00000170: 6465 5f66 6f72 6d61 7474 6572 290a 5b21  de_formatter).[!
-00000180: 5b6e 706d 2064 6f77 6e6c 6f61 6473 5d28  [npm downloads](
-00000190: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000001a0: 6c64 732e 696f 2f6e 706d 2f64 772f 2534  lds.io/npm/dw/%4
-000001b0: 3072 7961 6e74 616d 3632 3625 3246 6a75  0ryantam626%2Fju
-000001c0: 7079 7465 726c 6162 5f63 6f64 655f 666f  pyterlab_code_fo
-000001d0: 726d 6174 7465 722e 7376 6729 5d28 6874  rmatter.svg)](ht
-000001e0: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-000001f0: 2e69 6f2f 6a73 2f25 3430 7279 616e 7461  .io/js/%40ryanta
-00000200: 6d36 3236 2532 466a 7570 7974 6572 6c61  m626%2Fjupyterla
-00000210: 625f 636f 6465 5f66 6f72 6d61 7474 6572  b_code_formatter
-00000220: 290a 5b21 5b63 6f64 6520 7374 796c 655d  ).[![code style]
-00000230: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000240: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-00000250: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-00000260: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
-00000270: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000280: 2f61 6d62 762f 626c 6163 6b29 0a5b 215b  /ambv/black).[![
-00000290: 4769 7468 7562 2041 6374 696f 6e73 2053  Github Actions S
-000002a0: 7461 7475 735d 2868 7474 7073 3a2f 2f67  tatus](https://g
-000002b0: 6974 6875 622e 636f 6d2f 7279 616e 7461  ithub.com/ryanta
-000002c0: 6d36 3236 2f6a 7570 7974 6572 6c61 625f  m626/jupyterlab_
-000002d0: 636f 6465 5f66 6f72 6d61 7474 6572 2f77  code_formatter/w
-000002e0: 6f72 6b66 6c6f 7773 2f43 492f 6261 6467  orkflows/CI/badg
-000002f0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000300: 6769 7468 7562 2e63 6f6d 2f72 7961 6e74  github.com/ryant
-00000310: 616d 3632 362f 6a75 7079 7465 726c 6162  am626/jupyterlab
-00000320: 5f63 6f64 655f 666f 726d 6174 7465 722f  _code_formatter/
-00000330: 6163 7469 6f6e 7329 0a0a 2d2d 2d2d 0a0a  actions)..----..
-00000340: 446f 6375 6d65 6e74 6174 696f 6e3a 205b  Documentation: [
-00000350: 486f 7374 6564 206f 6e20 4769 7448 7562  Hosted on GitHub
-00000360: 2050 6167 6573 5d28 6874 7470 733a 2f2f   Pages](https://
-00000370: 7279 616e 7461 6d36 3236 2e67 6974 6875  ryantam626.githu
-00000380: 622e 696f 2f6a 7570 7974 6572 6c61 625f  b.io/jupyterlab_
-00000390: 636f 6465 5f66 6f72 6d61 7474 6572 2f69  code_formatter/i
-000003a0: 6e64 6578 2e68 746d 6c29 0a0a 2d2d 2d2d  ndex.html)..----
-000003b0: 0a0a 2323 2044 656d 6f0a 0a21 5b5d 2864  ..## Demo..![](d
-000003c0: 6f63 735f 7372 632f 5f73 7461 7469 632f  ocs_src/_static/
-000003d0: 666f 726d 6174 2d61 6c6c 2e67 6966 290a  format-all.gif).
-000003e0: 0a2d 2d2d 2d0a 0a23 2320 5175 6963 6b20  .----..## Quick 
-000003f0: 5374 6172 740a 0a49 2072 6563 6f6d 6d65  Start..I recomme
-00000400: 6e64 2079 6f75 2067 6f69 6e67 2074 6f20  nd you going to 
-00000410: 7468 6520 5b64 6f63 756d 656e 7461 7469  the [documentati
-00000420: 6f6e 2073 6974 655d 2868 7474 7073 3a2f  on site](https:/
-00000430: 2f72 7961 6e74 616d 3632 362e 6769 7468  /ryantam626.gith
-00000440: 7562 2e69 6f2f 6a75 7079 7465 726c 6162  ub.io/jupyterlab
-00000450: 5f63 6f64 655f 666f 726d 6174 7465 722f  _code_formatter/
-00000460: 696e 6465 782e 6874 6d6c 2371 7569 636b  index.html#quick
-00000470: 2d73 7461 7274 292c 2062 7574 2074 6869  -start), but thi
-00000480: 7320 7368 6f75 6c64 2077 6f72 6b20 746f  s should work to
-00000490: 6f2e 0a0a 312e 202a 2a49 6e73 7461 6c6c  o...1. **Install
-000004a0: 2074 6865 2070 6163 6b61 6765 2a2a 0a60   the package**.`
-000004b0: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
-000004c0: 6c6c 206a 7570 7974 6572 6c61 622d 636f  ll jupyterlab-co
-000004d0: 6465 2d66 6f72 6d61 7474 6572 0a60 6060  de-formatter.```
-000004e0: 0a0a 322e 202a 2a49 6e73 7461 6c6c 2073  ..2. **Install s
-000004f0: 6f6d 6520 7375 7070 6f72 7465 6420 666f  ome supported fo
-00000500: 726d 6174 7465 7273 2a2a 2028 6973 6f72  rmatters** (isor
-00000510: 742b 626c 6163 6b20 6172 6520 6465 6661  t+black are defa
-00000520: 756c 7420 666f 7220 5079 7468 6f6e 290a  ult for Python).
-00000530: 6060 6062 6173 680a 2320 4e4f 5445 3a20  ```bash.# NOTE: 
-00000540: 496e 7374 616c 6c20 626c 6163 6b20 616e  Install black an
-00000550: 6420 6973 6f72 742c 0a23 2020 2020 2020  d isort,.#      
-00000560: 204a 4c20 636f 6465 2066 6f72 6d61 7474   JL code formatt
-00000570: 6572 2069 7320 636f 6e66 6967 7572 6564  er is configured
-00000580: 2074 6f20 696e 766f 6b65 2069 736f 7274   to invoke isort
-00000590: 2061 6e64 2062 6c61 636b 2062 7920 6465   and black by de
-000005a0: 6661 756c 740a 7069 7020 696e 7374 616c  fault.pip instal
-000005b0: 6c20 626c 6163 6b20 6973 6f72 740a 6060  l black isort.``
-000005c0: 600a 0a33 2e20 2a2a 5265 7374 6172 7420  `..3. **Restart 
-000005d0: 4a75 7079 7465 724c 6162 2a2a 0a0a 5468  JupyterLab**..Th
-000005e0: 6973 2070 6c75 6769 6e20 696e 636c 7564  is plugin includ
-000005f0: 6573 2061 2073 6572 7665 7220 706c 7567  es a server plug
-00000600: 696e 2c20 7265 7374 6172 7420 4a75 7079  in, restart Jupy
-00000610: 7465 724c 6162 2069 6620 796f 7520 6861  terLab if you ha
-00000620: 7665 2066 6f6c 6c6f 7765 6420 7468 6520  ve followed the 
-00000630: 6162 6f76 6520 7374 6570 7320 7768 696c  above steps whil
-00000640: 6520 6974 2773 2072 756e 6e69 6e67 2e0a  e it's running..
-00000650: 0a34 2e20 2a2a 436f 6e66 6967 7572 6520  .4. **Configure 
-00000660: 706c 7567 696e 2a2a 0a0a 546f 2063 6f6e  plugin**..To con
-00000670: 6669 6775 7265 2077 6869 6368 2f68 6f77  figure which/how
-00000680: 2066 6f72 6d61 7474 6572 7320 6172 6520   formatters are 
-00000690: 696e 766f 6b65 642c 2073 6565 205b 636f  invoked, see [co
-000006a0: 6e66 6967 7572 6174 696f 6e5d 2868 7474  nfiguration](htt
-000006b0: 7073 3a2f 2f72 7961 6e74 616d 3632 362e  ps://ryantam626.
-000006c0: 6769 7468 7562 2e69 6f2f 6a75 7079 7465  github.io/jupyte
-000006d0: 726c 6162 5f63 6f64 655f 666f 726d 6174  rlab_code_format
-000006e0: 7465 722f 636f 6e66 6967 7572 6174 696f  ter/configuratio
-000006f0: 6e2e 6874 6d6c 292e 0a0a 2d2d 2d2d 0a0a  n.html)...----..
-00000700: 2323 2059 6f75 7220 5375 7070 6f72 740a  ## Your Support.
-00000710: 0a49 2063 6f75 6c64 2072 6561 6c6c 7920  .I could really 
-00000720: 7573 6520 796f 7572 2073 7570 706f 7274  use your support
-00000730: 2069 6e20 6769 7669 6e67 206d 6520 6120   in giving me a 
-00000740: 7374 6172 206f 6e20 4769 7448 7562 2c20  star on GitHub, 
-00000750: 7265 636f 6d6d 656e 6469 6e67 2066 6561  recommending fea
-00000760: 7475 7265 732c 2066 6978 696e 6720 6275  tures, fixing bu
-00000770: 6773 206f 7220 6d61 7962 6520 6576 656e  gs or maybe even
-00000780: 2070 726f 7669 6469 6e67 206d 6f6e 6574   providing monet
-00000790: 6172 7920 7375 7070 6f72 7421 0a0a 2d20  ary support!..- 
-000007a0: 5b52 6563 6f6d 6d65 6e64 696e 6720 6665  [Recommending fe
-000007b0: 6174 7572 6573 2076 6961 2047 6974 4875  atures via GitHu
-000007c0: 6220 4973 7375 6573 5d28 6874 7470 733a  b Issues](https:
-000007d0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 7961  //github.com/rya
-000007e0: 6e74 616d 3632 362f 6a75 7079 7465 726c  ntam626/jupyterl
-000007f0: 6162 5f63 6f64 655f 666f 726d 6174 7465  ab_code_formatte
-00000800: 722f 6973 7375 6573 290a 2d20 5b53 756d  r/issues).- [Sum
-00000810: 6974 7469 6e67 2079 6f75 7220 5052 206f  itting your PR o
-00000820: 6e20 4769 7448 7562 5d28 6874 7470 733a  n GitHub](https:
-00000830: 2f2f 6769 7468 7562 2e63 6f6d 2f72 7961  //github.com/rya
-00000840: 6e74 616d 3632 362f 6a75 7079 7465 726c  ntam626/jupyterl
-00000850: 6162 5f63 6f64 655f 666f 726d 6174 7465  ab_code_formatte
-00000860: 722f 7075 6c6c 7329 0a2d 205b 4275 7920  r/pulls).- [Buy 
-00000870: 6d65 2061 2063 6f66 6565 5d28 6874 7470  me a cofee](http
-00000880: 733a 2f2f 7777 772e 6275 796d 6561 636f  s://www.buymeaco
-00000890: 6666 6565 2e63 6f6d 2f72 7961 6e74 616d  ffee.com/ryantam
-000008a0: 3632 3629 0a2d 205b 446f 6e61 7469 6e67  626).- [Donating
-000008b0: 2056 6961 2053 6f6c 616e 615d 2868 7474   Via Solana](htt
-000008c0: 7073 3a2f 2f73 6f6c 616e 612e 636f 6d2f  ps://solana.com/
-000008d0: 293a 2036 4b37 614b 3552 7073 6b4a 6b68  ): 6K7aK5RpskJkh
-000008e0: 456b 775a 6931 5a51 7236 384c 6861 5664  EkwZi1ZQr68LhaVd
-000008f0: 666e 5466 576a 5a45 5156 3356 6262 440a  fnTfWjZEQV3VbbD.
-00000900: 0a2d 2d2d 2d0a 0a23 2320 436f 6e74 7269  .----..## Contri
-00000910: 6275 746f 7273 0a0a 4d61 7373 6976 6520  butors..Massive 
-00000920: 7468 616e 6b73 2074 6f20 7468 6520 6265  thanks to the be
-00000930: 6c6f 7720 6c69 7374 206f 6620 7065 6f70  low list of peop
-00000940: 6c65 2077 686f 206d 6164 6520 7061 7374  le who made past
-00000950: 2063 6f6e 7472 6962 7574 696f 6e73 2074   contributions t
-00000960: 6f20 7468 6520 7072 6f6a 6563 7421 0a0a  o the project!..
-00000970: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000980: 2f67 6974 6875 622e 636f 6d2f 7279 616e  /github.com/ryan
-00000990: 7461 6d36 3236 2f6a 7570 7974 6572 6c61  tam626/jupyterla
-000009a0: 625f 636f 6465 5f66 6f72 6d61 7474 6572  b_code_formatter
-000009b0: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-000009c0: 746f 7273 223e 0a20 203c 696d 6720 7372  tors">.  <img sr
-000009d0: 633d 2268 7474 7073 3a2f 2f63 6f6e 7472  c="https://contr
-000009e0: 6962 2e72 6f63 6b73 2f69 6d61 6765 3f72  ib.rocks/image?r
-000009f0: 6570 6f3d 7279 616e 7461 6d36 3236 2f6a  epo=ryantam626/j
-00000a00: 7570 7974 6572 6c61 625f 636f 6465 5f66  upyterlab_code_f
-00000a10: 6f72 6d61 7474 6572 2220 2f3e 0a3c 2f61  ormatter" />.</a
-00000a20: 3e0a 0a23 2320 4c69 6365 6e73 650a 0a54  >..## License..T
-00000a30: 6869 7320 7072 6f6a 6563 7420 6973 206c  his project is l
-00000a40: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
-00000a50: 6520 7465 726d 7320 6f66 2074 6865 204d  e terms of the M
-00000a60: 4954 206c 6963 656e 7365 2e0a            IT license..
+00000000: 6060 607b 746f 6374 7265 657d 0a3a 6869  ```{toctree}.:hi
+00000010: 6464 656e 3a0a 0a69 6e73 7461 6c6c 6174  dden:..installat
+00000020: 696f 6e2e 6d64 0a75 7361 6765 2e6d 640a  ion.md.usage.md.
+00000030: 636f 6e66 6967 7572 6174 696f 6e2e 6d64  configuration.md
+00000040: 0a63 7573 746f 6d2d 666f 726d 6174 7465  .custom-formatte
+00000050: 722e 6d64 0a66 6171 2e6d 640a 6a75 7079  r.md.faq.md.jupy
+00000060: 7465 7268 7562 2e6d 640a 6368 616e 6765  terhub.md.change
+00000070: 6c6f 672e 6d64 0a64 6576 2e6d 640a 796f  log.md.dev.md.yo
+00000080: 7572 2d73 7570 706f 7274 2e6d 640a 0a60  ur-support.md..`
+00000090: 6060 0a0a 2320 4a75 7079 7465 724c 6162  ``..# JupyterLab
+000000a0: 2043 6f64 6520 466f 726d 6174 7465 720a   Code Formatter.
+000000b0: 0a5b 215b 4269 6e64 6572 5d28 6874 7470  .[![Binder](http
+000000c0: 733a 2f2f 6d79 6269 6e64 6572 2e6f 7267  s://mybinder.org
+000000d0: 2f62 6164 6765 5f6c 6f67 6f2e 7376 6729  /badge_logo.svg)
+000000e0: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
+000000f0: 6572 2e6f 7267 2f76 322f 6768 2f72 7961  er.org/v2/gh/rya
+00000100: 6e74 616d 3632 362f 6a75 7079 7465 726c  ntam626/jupyterl
+00000110: 6162 5f63 6f64 655f 666f 726d 6174 7465  ab_code_formatte
+00000120: 722f 6d61 7374 6572 3f75 726c 7061 7468  r/master?urlpath
+00000130: 3d6c 6162 290a 5b21 5b6e 706d 2076 6572  =lab).[![npm ver
+00000140: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
+00000150: 6467 652e 6675 7279 2e69 6f2f 6a73 2f25  dge.fury.io/js/%
+00000160: 3430 7279 616e 7461 6d36 3236 2532 466a  40ryantam626%2Fj
+00000170: 7570 7974 6572 6c61 625f 636f 6465 5f66  upyterlab_code_f
+00000180: 6f72 6d61 7474 6572 2e73 7667 295d 2868  ormatter.svg)](h
+00000190: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
+000001a0: 792e 696f 2f6a 732f 2534 3072 7961 6e74  y.io/js/%40ryant
+000001b0: 616d 3632 3625 3246 6a75 7079 7465 726c  am626%2Fjupyterl
+000001c0: 6162 5f63 6f64 655f 666f 726d 6174 7465  ab_code_formatte
+000001d0: 7229 0a5b 215b 6e70 6d20 646f 776e 6c6f  r).[![npm downlo
+000001e0: 6164 735d 2868 7474 7073 3a2f 2f69 6d67  ads](https://img
+000001f0: 2e73 6869 656c 6473 2e69 6f2f 6e70 6d2f  .shields.io/npm/
+00000200: 6477 2f25 3430 7279 616e 7461 6d36 3236  dw/%40ryantam626
+00000210: 2532 466a 7570 7974 6572 6c61 625f 636f  %2Fjupyterlab_co
+00000220: 6465 5f66 6f72 6d61 7474 6572 2e73 7667  de_formatter.svg
+00000230: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
+00000240: 2e66 7572 792e 696f 2f6a 732f 2534 3072  .fury.io/js/%40r
+00000250: 7961 6e74 616d 3632 3625 3246 6a75 7079  yantam626%2Fjupy
+00000260: 7465 726c 6162 5f63 6f64 655f 666f 726d  terlab_code_form
+00000270: 6174 7465 7229 0a5b 215b 636f 6465 2073  atter).[![code s
+00000280: 7479 6c65 5d28 6874 7470 733a 2f2f 696d  tyle](https://im
+00000290: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000002a0: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
+000002b0: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
+000002c0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+000002d0: 622e 636f 6d2f 616d 6276 2f62 6c61 636b  b.com/ambv/black
+000002e0: 290a 5b21 5b47 6974 6875 6220 4163 7469  ).[![Github Acti
+000002f0: 6f6e 7320 5374 6174 7573 5d28 6874 7470  ons Status](http
+00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
+00000310: 7961 6e74 616d 3632 362f 6a75 7079 7465  yantam626/jupyte
+00000320: 726c 6162 5f63 6f64 655f 666f 726d 6174  rlab_code_format
+00000330: 7465 722f 776f 726b 666c 6f77 732f 4349  ter/workflows/CI
+00000340: 2f62 6164 6765 2e73 7667 295d 2868 7474  /badge.svg)](htt
+00000350: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000360: 7279 616e 7461 6d36 3236 2f6a 7570 7974  ryantam626/jupyt
+00000370: 6572 6c61 625f 636f 6465 5f66 6f72 6d61  erlab_code_forma
+00000380: 7474 6572 2f61 6374 696f 6e73 290a 0a2a  tter/actions)..*
+00000390: 4120 4a75 7079 7465 724c 6162 2070 6c75  A JupyterLab plu
+000003a0: 6769 6e20 746f 2066 6163 696c 6974 6174  gin to facilitat
+000003b0: 6520 696e 766f 6361 7469 6f6e 206f 6620  e invocation of 
+000003c0: 636f 6465 2066 6f72 6d61 7474 6572 732e  code formatters.
+000003d0: 2a0a 0a2a 2a53 6f75 7263 6520 436f 6465  *..**Source Code
+000003e0: 2a2a 3a20 5b47 6974 4875 625d 2868 7474  **: [GitHub](htt
+000003f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000400: 7279 616e 7461 6d36 3236 2f6a 7570 7974  ryantam626/jupyt
+00000410: 6572 6c61 625f 636f 6465 5f66 6f72 6d61  erlab_code_forma
+00000420: 7474 6572 2f29 2e0a 0a23 2320 4465 6d6f  tter/)...## Demo
+00000430: 0a0a 215b 666f 726d 6174 2d61 6c6c 5d28  ..![format-all](
+00000440: 5f73 7461 7469 632f 666f 726d 6174 2d61  _static/format-a
+00000450: 6c6c 2e67 6966 290a 0a23 2320 5265 7175  ll.gif)..## Requ
+00000460: 6972 656d 656e 7473 0a0a 2d20 5079 7468  irements..- Pyth
+00000470: 6f6e 2033 2e36 2b0a 2d20 4a75 7079 7465  on 3.6+.- Jupyte
+00000480: 724c 6162 203e 3d20 332e 302e 300a 2d20  rLab >= 3.0.0.- 
+00000490: 416e 7920 7375 7070 6f72 7465 6420 636f  Any supported co
+000004a0: 6465 2066 6f72 6d61 7474 6572 7320 2879  de formatters (y
+000004b0: 6f75 2063 616e 2061 6c73 6f20 7370 6563  ou can also spec
+000004c0: 6966 7920 796f 7572 206f 776e 2c20 7365  ify your own, se
+000004d0: 6520 5b63 7573 746f 6d20 666f 726d 6174  e [custom format
+000004e0: 7465 725d 2863 7573 746f 6d2d 666f 726d  ter](custom-form
+000004f0: 6174 7465 722e 6d64 2929 2e0a 0a3a 3a3a  atter.md))...:::
+00000500: 7b69 6d70 6f72 7461 6e74 7d0a 4a75 7079  {important}.Jupy
+00000510: 7465 724c 6162 2043 6f64 6520 466f 726d  terLab Code Form
+00000520: 6174 7465 7220 6f6e 6c79 2070 726f 7669  atter only provi
+00000530: 6465 7320 616e 2069 6e74 6572 6661 6365  des an interface
+00000540: 2066 6f72 2069 6e76 6f6b 696e 6720 636f   for invoking co
+00000550: 6465 2066 6f72 6d61 7474 6572 7320 6f6e  de formatters on
+00000560: 204a 7570 7974 6572 2053 6572 7665 722c   Jupyter Server,
+00000570: 2061 6e64 2064 6f65 7320 6e6f 7420 696e   and does not in
+00000580: 636c 7564 6520 616e 7920 636f 6465 2066  clude any code f
+00000590: 6f72 6d61 7474 6572 2062 7920 6465 6661  ormatter by defa
+000005a0: 756c 742e 0a3a 3a3a 0a0a 2323 2051 7569  ult..:::..## Qui
+000005b0: 636b 2053 7461 7274 0a0a 5b2f 2f5d 3a20  ck Start..[//]: 
+000005c0: 2320 2854 4f44 4f3a 2041 6464 2074 6162  # (TODO: Add tab
+000005d0: 2066 6f72 2063 6f6d 6d6f 6e20 7061 636b   for common pack
+000005e0: 6167 6520 6d61 6e61 6765 7273 290a 0a31  age managers)..1
+000005f0: 2e20 2a2a 496e 7374 616c 6c20 7468 6520  . **Install the 
+00000600: 7061 636b 6167 652a 2a0a 6060 6060 7b74  package**.````{t
+00000610: 6162 7d20 5069 700a 6060 6062 6173 680a  ab} Pip.```bash.
+00000620: 7069 7020 696e 7374 616c 6c20 6a75 7079  pip install jupy
+00000630: 7465 726c 6162 2d63 6f64 652d 666f 726d  terlab-code-form
+00000640: 6174 7465 720a 6060 600a 6060 6060 0a0a  atter.```.````..
+00000650: 6060 6060 7b74 6162 7d20 436f 6e64 610a  ````{tab} Conda.
+00000660: 6060 6062 6173 680a 636f 6e64 6120 696e  ```bash.conda in
+00000670: 7374 616c 6c20 2d63 2063 6f6e 6461 2d66  stall -c conda-f
+00000680: 6f72 6765 206a 7570 7974 6572 6c61 625f  orge jupyterlab_
+00000690: 636f 6465 5f66 6f72 6d61 7474 6572 0a60  code_formatter.`
+000006a0: 6060 0a60 6060 600a 0a60 6060 607b 7461  ``.````..````{ta
+000006b0: 627d 2050 6f65 7472 790a 6060 6062 6173  b} Poetry.```bas
+000006c0: 680a 706f 6574 7279 2061 6464 206a 7570  h.poetry add jup
+000006d0: 7974 6572 6c61 622d 636f 6465 2d66 6f72  yterlab-code-for
+000006e0: 6d61 7474 6572 0a60 6060 0a60 6060 600a  matter.```.````.
+000006f0: 0a60 6060 607b 7461 627d 2050 6970 656e  .````{tab} Pipen
+00000700: 760a 6060 6062 6173 680a 7069 7065 6e76  v.```bash.pipenv
+00000710: 2069 6e73 7461 6c6c 206a 7570 7974 6572   install jupyter
+00000720: 6c61 622d 636f 6465 2d66 6f72 6d61 7474  lab-code-formatt
+00000730: 6572 0a60 6060 0a60 6060 600a 0a32 2e20  er.```.````..2. 
+00000740: 2a2a 496e 7374 616c 6c20 736f 6d65 2073  **Install some s
+00000750: 7570 706f 7274 6564 2066 6f72 6d61 7474  upported formatt
+00000760: 6572 732a 2a20 2869 736f 7274 2b62 6c61  ers** (isort+bla
+00000770: 636b 2061 7265 2064 6566 6175 6c74 2066  ck are default f
+00000780: 6f72 2050 7974 686f 6e29 0a60 6060 6261  or Python).```ba
+00000790: 7368 0a23 204e 4f54 453a 2049 6e73 7461  sh.# NOTE: Insta
+000007a0: 6c6c 2062 6c61 636b 2061 6e64 2069 736f  ll black and iso
+000007b0: 7274 2c0a 2320 2020 2020 2020 4a4c 2063  rt,.#       JL c
+000007c0: 6f64 6520 666f 726d 6174 7465 7220 6973  ode formatter is
+000007d0: 2063 6f6e 6669 6775 7265 6420 746f 2069   configured to i
+000007e0: 6e76 6f6b 6520 6973 6f72 7420 616e 6420  nvoke isort and 
+000007f0: 626c 6163 6b20 6279 2064 6566 6175 6c74  black by default
+00000800: 0a70 6970 2069 6e73 7461 6c6c 2062 6c61  .pip install bla
+00000810: 636b 2069 736f 7274 0a60 6060 0a0a 332e  ck isort.```..3.
+00000820: 202a 2a52 6573 7461 7274 204a 7570 7974   **Restart Jupyt
+00000830: 6572 4c61 622a 2a0a 0a54 6869 7320 706c  erLab**..This pl
+00000840: 7567 696e 2069 6e63 6c75 6465 7320 6120  ugin includes a 
+00000850: 7365 7276 6572 2070 6c75 6769 6e2c 2072  server plugin, r
+00000860: 6573 7461 7274 204a 7570 7974 6572 4c61  estart JupyterLa
+00000870: 6220 6966 2079 6f75 2068 6176 6520 666f  b if you have fo
+00000880: 6c6c 6f77 6564 2074 6865 2061 626f 7665  llowed the above
+00000890: 2073 7465 7073 2077 6869 6c65 2069 7427   steps while it'
+000008a0: 7320 7275 6e6e 696e 672e 0a0a 342e 202a  s running...4. *
+000008b0: 2a43 6f6e 6669 6775 7265 2070 6c75 6769  *Configure plugi
+000008c0: 6e2a 2a0a 0a54 6f20 636f 6e66 6967 7572  n**..To configur
+000008d0: 6520 7768 6963 682f 686f 7720 666f 726d  e which/how form
+000008e0: 6174 7465 7273 2061 7265 2069 6e76 6f6b  atters are invok
+000008f0: 6564 2c20 7365 6520 5b63 6f6e 6669 6775  ed, see [configu
+00000900: 7261 7469 6f6e 5d28 636f 6e66 6967 7572  ration](configur
+00000910: 6174 696f 6e2e 6d64 292e 0a              ation.md)..
```

### Comparing `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/formatters.py` & `jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from typing import List, Type
 
 try:
     import rpy2
     import rpy2.robjects
 except ImportError:
     pass
-from packaging import version
 from functools import cache
 
+from packaging import version
 
 logger = logging.getLogger(__name__)
 
 
 INCOMPATIBLE_MAGIC_LANGUAGES = [
     "html",
     "js",
@@ -70,15 +70,15 @@
 
     def __init__(self, code: str) -> None:
         self.code = code
 
     @property
     @abc.abstractmethod
     def langs(self) -> List[str]:
-        return
+        pass
 
     @abc.abstractmethod
     def escape(self, line: str) -> str:
         pass
 
     @abc.abstractmethod
     def unescape(self, line: str) -> str:
@@ -114,15 +114,14 @@
     def unescape(self, line: str) -> str:
         if line.lstrip().startswith(self.escaped_line_start):
             line = line[self.unesacpe_start :]
         return line
 
 
 class HelpEscaper(BaseLineEscaper):
-
     langs = ["python"]
     escaped_line_start = "# \x01 "
     unesacpe_start = len(escaped_line_start)
 
     def escape(self, line: str) -> str:
         lstripped = line.lstrip()
         if (
@@ -137,15 +136,14 @@
     def unescape(self, line: str) -> str:
         if line.lstrip().startswith(self.escaped_line_start):
             line = line[self.unesacpe_start :]
         return line
 
 
 class CommandEscaper(BaseLineEscaper):
-
     langs = ["python"]
     escaped_line_start = "# \x01 "
     unesacpe_start = len(escaped_line_start)
 
     def escape(self, line: str) -> str:
         if line.lstrip().startswith("!"):
             line = f"{self.escaped_line_start}{line}"
@@ -154,15 +152,14 @@
     def unescape(self, line: str) -> str:
         if line.lstrip().startswith(self.escaped_line_start):
             line = line[self.unesacpe_start :]
         return line
 
 
 class QuartoCommentEscaper(BaseLineEscaper):
-
     langs = ["python"]
     escaped_line_start = "# \x01 "
     unesacpe_start = len(escaped_line_start)
 
     def escape(self, line: str) -> str:
         if line.lstrip().startswith("#| "):
             line = f"{self.escaped_line_start}{line}"
@@ -182,17 +179,17 @@
     RunScriptEscaper,
 ]
 
 
 def handle_line_ending_and_magic(func):
     @wraps(func)
     def wrapped(self, code: str, notebook: bool, **options) -> str:
-        if any(
-            code.startswith(f"%{lang}") for lang in INCOMPATIBLE_MAGIC_LANGUAGES
-        ) or any(code.startswith(f"%%{lang}") for lang in INCOMPATIBLE_MAGIC_LANGUAGES):
+        if any(code.startswith(f"%{lang}") for lang in INCOMPATIBLE_MAGIC_LANGUAGES) or any(
+            code.startswith(f"%%{lang}") for lang in INCOMPATIBLE_MAGIC_LANGUAGES
+        ):
             logger.info("Non compatible magic language cell block detected, ignoring.")
             return code
 
         has_semicolon = code.strip().endswith(";")
 
         escapers = [escaper_cls(code) for escaper_cls in ESCAPER_CLASSES]
 
@@ -259,15 +256,14 @@
         blue.monkey_patch_black(blue.Mode.synchronous)
         BLUE_MONKEY_PATCHED = True
 
     return blue
 
 
 class BlueFormatter(BaseFormatter):
-
     label = "Apply Blue Formatter"
 
     @property
     def importable(self) -> bool:
         return is_importable("blue")
 
     @staticmethod
@@ -281,15 +277,14 @@
         blue = import_blue()
 
         code = blue.black.format_str(code, **self.handle_options(**options))
         return code
 
 
 class BlackFormatter(BaseFormatter):
-
     label = "Apply Black Formatter"
 
     @property
     def importable(self) -> bool:
         return is_importable("black")
 
     @staticmethod
@@ -308,45 +303,42 @@
         black = import_black()
 
         code = black.format_str(code, **self.handle_options(**options))
         return code
 
 
 class Autopep8Formatter(BaseFormatter):
-
     label = "Apply Autopep8 Formatter"
 
     @property
     def importable(self) -> bool:
         return is_importable("autopep8")
 
     @handle_line_ending_and_magic
     def format_code(self, code: str, notebook: bool, **options) -> str:
         from autopep8 import fix_code
 
         return fix_code(code, options=options)
 
 
 class YapfFormatter(BaseFormatter):
-
     label = "Apply YAPF Formatter"
 
     @property
     def importable(self) -> bool:
         return is_importable("yapf")
 
     @handle_line_ending_and_magic
     def format_code(self, code: str, notebook: bool, **options) -> str:
         from yapf.yapflib.yapf_api import FormatCode
 
         return FormatCode(code, **options)[0]
 
 
 class IsortFormatter(BaseFormatter):
-
     label = "Apply Isort Formatter"
 
     @property
     def importable(self) -> bool:
         return is_importable("isort")
 
     @handle_line_ending_and_magic
@@ -358,15 +350,14 @@
         except ImportError:
             import isort
 
             return isort.code(code=code, **options)
 
 
 class FormatRFormatter(BaseFormatter):
-
     label = "Apply FormatR Formatter"
     package_name = "formatR"
 
     @property
     def importable(self) -> bool:
         try:
             import rpy2.robjects.packages as rpackages
@@ -377,23 +368,20 @@
         except Exception:
             return False
 
     @handle_line_ending_and_magic
     def format_code(self, code: str, notebook: bool, **options) -> str:
         import rpy2.robjects.packages as rpackages
 
-        format_r = rpackages.importr(
-            self.package_name, robject_translations={".env": "env"}
-        )
+        format_r = rpackages.importr(self.package_name, robject_translations={".env": "env"})
         formatted_code = format_r.tidy_source(text=code, output=False, **options)
         return "\n".join(formatted_code[0])
 
 
 class StylerFormatter(BaseFormatter):
-
     label = "Apply Styler Formatter"
     package_name = "styler"
 
     @property
     def importable(self) -> bool:
         try:
             import rpy2.robjects.packages as rpackages
@@ -405,17 +393,15 @@
             return False
 
     @handle_line_ending_and_magic
     def format_code(self, code: str, notebook: bool, **options) -> str:
         import rpy2.robjects.packages as rpackages
 
         styler_r = rpackages.importr(self.package_name)
-        formatted_code = styler_r.style_text(
-            code, **self._transform_options(styler_r, options)
-        )
+        formatted_code = styler_r.style_text(code, **self._transform_options(styler_r, options))
         return "\n".join(formatted_code)
 
     @staticmethod
     def _transform_options(styler_r, options):
         transformed_options = copy.deepcopy(options)
 
         if "math_token_spacing" in transformed_options:
@@ -426,17 +412,15 @@
             else:
                 transformed_options["math_token_spacing"] = rpy2.robjects.ListVector(
                     getattr(styler_r, options["math_token_spacing"])()
                 )
 
         if "reindention" in transformed_options:
             if isinstance(options["reindention"], dict):
-                transformed_options["reindention"] = rpy2.robjects.ListVector(
-                    options["reindention"]
-                )
+                transformed_options["reindention"] = rpy2.robjects.ListVector(options["reindention"])
             else:
                 transformed_options["reindention"] = rpy2.robjects.ListVector(
                     getattr(styler_r, options["reindention"])()
                 )
         return transformed_options
 
 
@@ -451,38 +435,52 @@
         return f"Apply {self.command[0]} Formatter"
 
     @property
     def importable(self) -> bool:
         return command_exist(self.command[0])
 
     @handle_line_ending_and_magic
-    def format_code(
-        self, code: str, notebook: bool, args: List[str] = [], **options
-    ) -> str:
+    def format_code(self, code: str, notebook: bool, args: List[str] = [], **options) -> str:
         process = subprocess.run(
             self.command + args,
             input=code,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             universal_newlines=True,
         )
 
         if process.stderr:
-            logger.info(f"An error with {self.command[0]} has ocurred:")
+            logger.info(f"An error with {self.command[0]} has occurred:")
             logger.info(process.stderr)
             return code
         else:
             return process.stdout
 
 
+class RuffFixFormatter(CommandLineFormatter):
+    @property
+    def label(self) -> str:
+        return f"Apply ruff Formatter"
+
+    def __init__(self):
+        try:
+            from ruff.__main__ import find_ruff_bin
+
+            ruff_command = find_ruff_bin()
+        except (ImportError, FileNotFoundError):
+            ruff_command = "ruff"
+        self.command = [ruff_command, "check", "--fix-only", "-"]
+
+
 SERVER_FORMATTERS = {
     "black": BlackFormatter(),
     "blue": BlueFormatter(),
     "autopep8": Autopep8Formatter(),
     "yapf": YapfFormatter(),
     "isort": IsortFormatter(),
+    "ruff": RuffFixFormatter(),
     "formatR": FormatRFormatter(),
     "styler": StylerFormatter(),
     "scalafmt": CommandLineFormatter(command=["scalafmt", "--stdin"]),
     "rustfmt": CommandLineFormatter(command=["rustfmt"]),
     "astyle": CommandLineFormatter(command=["astyle"]),
 }
```

### Comparing `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/settings.json` & `jupyterlab_code_formatter-2.0.0rc1/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/settings.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'definitions'": "{'ruff': OrderedDict([('properties', OrderedDict([('args', "*

 * *                  "OrderedDict([('type', 'array'), ('items', OrderedDict([('type', "*

 * *                  "'string')]))]))])), ('additionalProperties', False), ('type', 'object')])}",*

 * * "'properties'": "{'ruff': OrderedDict([('title', 'Ruff Config'), ('description', 'Command line "*

 * *                 "options to be passed to ruff.'), ('$ref', '#/definitions/ruff'), ('default', "*

 * *                 "OrderedDict([('args', ['--select=I'])] […]*

```diff
@@ -257,14 +257,26 @@
                         }
                     },
                     "type": "object"
                 }
             },
             "type": "object"
         },
+        "ruff": {
+            "additionalProperties": false,
+            "properties": {
+                "args": {
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                }
+            },
+            "type": "object"
+        },
         "styler": {
             "additionalProperties": false,
             "properties": {
                 "indent_by": {
                     "type": "number"
                 },
                 "math_token_spacing": {
@@ -429,14 +441,24 @@
                     ],
                     "rust": "rustfmt"
                 }
             },
             "description": "Preferences for this plugin",
             "title": "Code Formatter Preferences"
         },
+        "ruff": {
+            "$ref": "#/definitions/ruff",
+            "default": {
+                "args": [
+                    "--select=I"
+                ]
+            },
+            "description": "Command line options to be passed to ruff.",
+            "title": "Ruff Config"
+        },
         "styler": {
             "$ref": "#/definitions/styler",
             "default": {},
             "description": "Config to be passed into styler's style_text function call.",
             "title": "Styler Config"
         },
         "suppressFormatterErrors": {
```

### Comparing `jupyterlab_code_formatter-1.6.1/src/client.ts` & `jupyterlab_code_formatter-2.0.0rc1/src/client.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import { URLExt } from '@jupyterlab/coreutils';
 import { ServerConnection } from '@jupyterlab/services';
 import { Constants } from './constants';
 
 class JupyterlabCodeFormatterClient {
   public request(path: string, method: string, body: any): Promise<any> {
     const settings = ServerConnection.makeSettings();
-    const fullUrl = URLExt.join(
-      settings.baseUrl,
-      Constants.SHORT_PLUGIN_NAME,
-      path
-    );
+    const fullUrl = URLExt.join(settings.baseUrl, Constants.PLUGIN_NAME, path);
     return ServerConnection.makeRequest(
       fullUrl,
       {
         body,
-        method,
-        headers: new Headers({
-          'Plugin-Version': Constants.PLUGIN_VERSION
-        })
+        method
       },
       settings
     ).then(response => {
       if (response.status !== 200) {
         return response.text().then(() => {
           throw new ServerConnection.ResponseError(
             response,
@@ -32,14 +25,10 @@
       return response.text();
     });
   }
 
   public getAvailableFormatters(cache: boolean) {
     return this.request('formatters' + (cache ? '?cached' : ''), 'GET', null);
   }
-
-  public getVersion() {
-    return this.request('version', 'GET', null);
-  }
 }
 
 export default JupyterlabCodeFormatterClient;
```

### Comparing `jupyterlab_code_formatter-1.6.1/src/constants.ts` & `jupyterlab_code_formatter-2.0.0rc1/src/constants.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 export namespace Constants {
-  export const SHORT_PLUGIN_NAME = 'jupyterlab_code_formatter';
-  export const FORMAT_COMMAND = `${SHORT_PLUGIN_NAME}:format`;
-  export const FORMAT_ALL_COMMAND = `${SHORT_PLUGIN_NAME}:format_all`;
+  export const PLUGIN_NAME = 'jupyterlab_code_formatter';
+  export const FORMAT_COMMAND = `${PLUGIN_NAME}:format`;
+  export const FORMAT_ALL_COMMAND = `${PLUGIN_NAME}:format_all`;
   // TODO: Extract this to style and import svg as string
   export const ICON_FORMAT_ALL_SVG =
     '<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" focusable="false" width="1em" height="1em" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);" preserveAspectRatio="xMidYMid meet" viewBox="0 0 1792 1792"><path class="jp-icon3" d="M1473 929q7-118-33-226.5t-113-189t-177-131T929 325q-116-7-225.5 32t-192 110.5t-135 175T317 863q-7 118 33 226.5t113 189t177.5 131T862 1467q155 9 293-59t224-195.5t94-283.5zM1792 0l-349 348q120 117 180.5 272t50.5 321q-11 183-102 339t-241 255.5T999 1660L0 1792l347-347q-120-116-180.5-271.5T116 852q11-184 102-340t241.5-255.5T792 132q167-22 500-66t500-66z" fill="#626262"/></svg>';
   export const ICON_FORMAT_ALL = 'fa fa-superpowers';
-  export const LONG_PLUGIN_NAME = `@ryantam626/${SHORT_PLUGIN_NAME}`;
-  export const SETTINGS_SECTION = `${LONG_PLUGIN_NAME}:settings`;
+  export const SETTINGS_SECTION = `${PLUGIN_NAME}:settings`;
   export const COMMAND_SECTION_NAME = 'Jupyterlab Code Formatter';
   // TODO: Use package.json info
   export const PLUGIN_VERSION = '1.6.1';
 }
```

### Comparing `jupyterlab_code_formatter-1.6.1/src/formatter.ts` & `jupyterlab_code_formatter-2.0.0rc1/src/formatter.ts`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import { INotebookTracker, Notebook } from '@jupyterlab/notebook';
 import JupyterlabCodeFormatterClient from './client';
 import { IEditorTracker } from '@jupyterlab/fileeditor';
 import { Widget } from '@lumino/widgets';
 import { showErrorMessage } from '@jupyterlab/apputils';
 
 class JupyterlabCodeFormatter {
+  working = false;
   protected client: JupyterlabCodeFormatterClient;
-  protected working: boolean;
   constructor(client: JupyterlabCodeFormatterClient) {
     this.client = client;
   }
 
   protected formatCode(
     code: string[],
     formatter: string,
@@ -69,28 +69,29 @@
     if (!this.notebookTracker.currentWidget) {
       return [];
     }
     const codeCells: CodeCell[] = [];
     notebook = notebook || this.notebookTracker.currentWidget.content;
     notebook.widgets.forEach((cell: Cell) => {
       if (cell.model.type === 'code') {
-        if (!selectedOnly || notebook.isSelectedOrActive(cell)) {
+        if (!selectedOnly || (<Notebook>notebook).isSelectedOrActive(cell)) {
           codeCells.push(cell as CodeCell);
         }
       }
     });
     return codeCells;
   }
 
   private getNotebookType() {
     if (!this.notebookTracker.currentWidget) {
       return null;
     }
 
-    const metadata = this.notebookTracker.currentWidget.content.model.metadata.toJSON();
+    const metadata =
+      this.notebookTracker.currentWidget.content.model!.metadata.toJSON();
 
     if (!metadata) {
       return null;
     }
 
     // prefer kernelspec language
     // @ts-ignore
@@ -119,14 +120,76 @@
       } else if (defaultFormatter !== undefined) {
         return [defaultFormatter];
       }
     }
     return [];
   }
 
+  private async getFormattersToUse(config: any, formatter?: string) {
+    const defaultFormatters = this.getDefaultFormatters(config);
+    const formattersToUse =
+      formatter !== undefined ? [formatter] : defaultFormatters;
+
+    if (formattersToUse.length === 0) {
+      await showErrorMessage(
+        'Jupyterlab Code Formatter Error',
+        'Unable to find default formatters to use, please file an issue on GitHub.'
+      );
+    }
+
+    return formattersToUse;
+  }
+
+  private async applyFormatters(
+    selectedCells: CodeCell[],
+    formattersToUse: string[],
+    config: any
+  ) {
+    for (const formatterToUse of formattersToUse) {
+      if (formatterToUse === 'noop' || formatterToUse === 'skip') {
+        continue;
+      }
+      const currentTexts = selectedCells.map(cell => cell.model.value.text);
+      const formattedTexts = await this.formatCode(
+        currentTexts,
+        formatterToUse,
+        config[formatterToUse],
+        true,
+        config.cacheFormatters
+      );
+
+      const showErrors = !(config.suppressFormatterErrors ?? false);
+      for (let i = 0; i < selectedCells.length; ++i) {
+        const cell = selectedCells[i];
+        const currentText = currentTexts[i];
+        const formattedText = formattedTexts.code[i];
+        const cellValueHasNotChanged = cell.model.value.text === currentText;
+        if (cellValueHasNotChanged) {
+          if (formattedText.error) {
+            if (showErrors) {
+              await showErrorMessage(
+                'Jupyterlab Code Formatter Error',
+                formattedText.error
+              );
+            }
+          } else {
+            cell.model.value.text = formattedText.code;
+          }
+        } else {
+          if (showErrors) {
+            await showErrorMessage(
+              'Jupyterlab Code Formatter Error',
+              `Cell value changed since format request was sent, formatting for cell ${i} skipped.`
+            );
+          }
+        }
+      }
+    }
+  }
+
   private async formatCells(
     selectedOnly: boolean,
     config: any,
     formatter?: string,
     notebook?: Notebook
   ) {
     if (this.working) {
@@ -135,62 +198,17 @@
     try {
       this.working = true;
       const selectedCells = this.getCodeCells(selectedOnly, notebook);
       if (selectedCells.length === 0) {
         this.working = false;
         return;
       }
-      const defaultFormatters = this.getDefaultFormatters(config);
-      const formattersToUse =
-        formatter !== undefined ? [formatter] : defaultFormatters;
-
-      if (formattersToUse.length === 0) {
-        await showErrorMessage(
-          'Jupyterlab Code Formatter Error',
-          `Unable to find default formatters to use, please file an issue on GitHub.`
-        );
-      }
 
-      for (let formatterToUse of formattersToUse) {
-        if (formatterToUse === 'noop' || formatterToUse === 'skip') {
-          continue;
-        }
-        const currentTexts = selectedCells.map(cell => cell.model.value.text);
-        const formattedTexts = await this.formatCode(
-          currentTexts,
-          formatterToUse,
-          config[formatterToUse],
-          true,
-          config.cacheFormatters
-        );
-        for (let i = 0; i < selectedCells.length; ++i) {
-          const cell = selectedCells[i];
-          const currentText = currentTexts[i];
-          const formattedText = formattedTexts.code[i];
-          if (cell.model.value.text === currentText) {
-            if (formattedText.error) {
-              if (!(config.suppressFormatterErrors ?? false)) {
-                await showErrorMessage(
-                  'Jupyterlab Code Formatter Error',
-                  formattedText.error
-                );
-              }
-            } else {
-              cell.model.value.text = formattedText.code;
-            }
-          } else {
-            if (!(config.suppressFormatterErrors ?? false)) {
-              await showErrorMessage(
-                'Jupyterlab Code Formatter Error',
-                `Cell value changed since format request was sent, formatting for cell ${i} skipped.`
-              );
-            }
-          }
-        }
-      }
+      const formattersToUse = await this.getFormattersToUse(config, formatter);
+      await this.applyFormatters(selectedCells, formattersToUse, config);
     } catch (error) {
       await showErrorMessage('Jupyterlab Code Formatter Error', error);
     }
     this.working = false;
   }
 
   applicable(formatter: string, currentWidget: Widget) {
@@ -213,15 +231,15 @@
 
   formatAction(config: any, formatter: string) {
     if (this.working) {
       return;
     }
     const editorWidget = this.editorTracker.currentWidget;
     this.working = true;
-    const editor = editorWidget.content.editor;
+    const editor = editorWidget!.content.editor;
     const code = editor.model.value.text;
     this.formatCode(
       [code],
       formatter,
       config[formatter],
       false,
       config.cacheFormatters
@@ -231,15 +249,15 @@
           void showErrorMessage(
             'Jupyterlab Code Formatter Error',
             data.code[0].error
           );
           this.working = false;
           return;
         }
-        this.editorTracker.currentWidget.content.editor.model.value.text =
+        this.editorTracker.currentWidget!.content.editor.model.value.text =
           data.code[0].code;
         this.working = false;
       })
       .catch(error => {
         this.working = false;
         void showErrorMessage('Jupyterlab Code Formatter Error', error);
       });
```

### Comparing `jupyterlab_code_formatter-1.6.1/src/index.ts` & `jupyterlab_code_formatter-2.0.0rc1/src/index.ts`

 * *Files 16% similar despite different names*

```diff
@@ -4,43 +4,41 @@
   INotebookTracker,
   NotebookPanel
 } from '@jupyterlab/notebook';
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
-import {
-  ICommandPalette,
-  showErrorMessage,
-  ToolbarButton
-} from '@jupyterlab/apputils';
+import { ICommandPalette, ToolbarButton } from '@jupyterlab/apputils';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { IMainMenu } from '@jupyterlab/mainmenu';
 import { IEditorTracker } from '@jupyterlab/fileeditor';
 import JupyterlabCodeFormatterClient from './client';
 import {
   JupyterlabFileEditorCodeFormatter,
   JupyterlabNotebookCodeFormatter
 } from './formatter';
 import { DisposableDelegate, IDisposable } from '@lumino/disposable';
 import { Constants } from './constants';
 import { LabIcon } from '@jupyterlab/ui-components';
+import { Widget } from '@lumino/widgets';
 
 class JupyterLabCodeFormatter
-  implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel> {
+  implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
+{
   private app: JupyterFrontEnd;
-  private tracker: INotebookTracker;
+  private readonly tracker: INotebookTracker;
   private palette: ICommandPalette;
   private settingRegistry: ISettingRegistry;
   private menu: IMainMenu;
   private config: any;
-  private editorTracker: IEditorTracker;
-  private client: JupyterlabCodeFormatterClient;
-  private notebookCodeFormatter: JupyterlabNotebookCodeFormatter;
-  private fileEditorCodeFormatter: JupyterlabFileEditorCodeFormatter;
+  private readonly editorTracker: IEditorTracker;
+  private readonly client: JupyterlabCodeFormatterClient;
+  private readonly notebookCodeFormatter: JupyterlabNotebookCodeFormatter;
+  private readonly fileEditorCodeFormatter: JupyterlabFileEditorCodeFormatter;
 
   constructor(
     app: JupyterFrontEnd,
     tracker: INotebookTracker,
     palette: ICommandPalette,
     settingRegistry: ISettingRegistry,
     menu: IMainMenu,
@@ -58,37 +56,34 @@
       this.tracker
     );
     this.fileEditorCodeFormatter = new JupyterlabFileEditorCodeFormatter(
       this.client,
       this.editorTracker
     );
 
-    this.checkVersion().then(async versionMatches => {
-      if (versionMatches) {
-        await this.setupSettings();
-        this.setupAllCommands();
-        this.setupContextMenu();
-        this.setupWidgetExtension();
-      }
+    this.setupSettings().then(() => {
+      this.setupAllCommands();
+      this.setupContextMenu();
+      this.setupWidgetExtension();
     });
+    console.log('222wat');
   }
 
   public createNew(
     nb: NotebookPanel,
     context: DocumentRegistry.IContext<INotebookModel>
   ): IDisposable {
-    const self = this;
     const button = new ToolbarButton({
       tooltip: 'Format notebook',
       icon: new LabIcon({
         name: Constants.FORMAT_ALL_COMMAND,
         svgstr: Constants.ICON_FORMAT_ALL_SVG
       }),
       onClick: async () => {
-        await self.notebookCodeFormatter.formatAllCodeCells(
+        await this.notebookCodeFormatter.formatAllCodeCells(
           this.config,
           undefined,
           nb.content
         );
       }
     });
     nb.toolbar.insertAfter(
@@ -128,15 +123,15 @@
     this.client
       .getAvailableFormatters(this.config.cacheFormatters)
       .then(data => {
         const formatters = JSON.parse(data).formatters;
         const menuGroup: Array<{ command: string }> = [];
         Object.keys(formatters).forEach(formatter => {
           if (formatters[formatter].enabled) {
-            const command = `${Constants.SHORT_PLUGIN_NAME}:${formatter}`;
+            const command = `${Constants.PLUGIN_NAME}:${formatter}`;
             this.setupCommand(formatter, formatters[formatter].label, command);
             menuGroup.push({ command });
           }
         });
         this.menu.editMenu.addGroup(menuGroup);
       });
 
@@ -154,89 +149,70 @@
       iconClass: Constants.ICON_FORMAT_ALL,
       iconLabel: 'Format notebook'
       // TODO: Add back isVisible
     });
   }
 
   private async setupSettings() {
-    const self = this;
-    try {
-      const settings = await this.settingRegistry.load(
-        Constants.SETTINGS_SECTION
-      );
-      function onSettingsUpdated(jsettings: ISettingRegistry.ISettings) {
-        self.config = jsettings.composite;
-      }
-      settings.changed.connect(onSettingsUpdated);
-      onSettingsUpdated(settings);
-    } catch (error) {
-      void showErrorMessage('Jupyterlab Code Formatter Error', error);
-    }
+    const settings = await this.settingRegistry.load(
+      Constants.SETTINGS_SECTION
+    );
+    const onSettingsUpdated = (jsettings: ISettingRegistry.ISettings) => {
+      this.config = jsettings.composite;
+    };
+    settings.changed.connect(onSettingsUpdated);
+    onSettingsUpdated(settings);
   }
 
   private setupCommand(name: string, label: string, command: string) {
     this.app.commands.addCommand(command, {
       execute: async () => {
-        for (let formatter of [
+        for (const formatter of [
           this.notebookCodeFormatter,
           this.fileEditorCodeFormatter
         ]) {
-          if (formatter.applicable(name, this.app.shell.currentWidget)) {
+          if (
+            formatter.applicable(name, <Widget>this.app.shell.currentWidget)
+          ) {
             await formatter.formatAction(this.config, name);
           }
         }
       },
       isVisible: () => {
-        for (let formatter of [
+        for (const formatter of [
           this.notebookCodeFormatter,
           this.fileEditorCodeFormatter
         ]) {
-          if (formatter.applicable(name, this.app.shell.currentWidget)) {
+          if (
+            formatter.applicable(name, <Widget>this.app.shell.currentWidget)
+          ) {
             return true;
           }
         }
         return false;
       },
       label
     });
     this.palette.addItem({ command, category: Constants.COMMAND_SECTION_NAME });
   }
-
-  private async checkVersion() {
-    return this.client
-      .getVersion()
-      .then(data => {
-        let serverPluginVersion = JSON.parse(data).version;
-        let versionMatches = serverPluginVersion === Constants.PLUGIN_VERSION;
-        if (!versionMatches) {
-          void showErrorMessage(
-            'Jupyterlab Code Formatter Version Mismatch',
-            `Lab plugin version: ${Constants.PLUGIN_VERSION}. ` +
-              `Server plugin version: ${serverPluginVersion}. ` +
-              `Please re-install the plugin with the latest instruction.`
-          );
-        }
-        return versionMatches;
-      })
-      .catch(error => {
-        void showErrorMessage(
-          'Jupyterlab Code Formatter Error',
-          'Unable to find server plugin version. You may need to restart your JupyterLab server, ' +
-            'If that does not fix the issue please open an issue at: ' +
-            'https://github.com/ryantam626/jupyterlab_code_formatter/issues/new/choose'
-        );
-        return false;
-      });
-  }
 }
 
 /**
  * Initialization data for the jupyterlab_code_formatter extension.
  */
-const extension: JupyterFrontEndPlugin<void> = {
+const plugin: JupyterFrontEndPlugin<void> = {
+  id: Constants.PLUGIN_NAME,
+  autoStart: true,
+  requires: [
+    ICommandPalette,
+    INotebookTracker,
+    ISettingRegistry,
+    IMainMenu,
+    IEditorTracker
+  ],
   activate: (
     app: JupyterFrontEnd,
     palette: ICommandPalette,
     tracker: INotebookTracker,
     settingRegistry: ISettingRegistry,
     menu: IMainMenu,
     editorTracker: IEditorTracker
@@ -245,20 +221,12 @@
       app,
       tracker,
       palette,
       settingRegistry,
       menu,
       editorTracker
     );
-  },
-  autoStart: true,
-  id: Constants.SHORT_PLUGIN_NAME,
-  requires: [
-    ICommandPalette,
-    INotebookTracker,
-    ISettingRegistry,
-    IMainMenu,
-    IEditorTracker
-  ]
+    console.log('JupyterLab extension jupyterlab_code_formatter is activated!');
+  }
 };
 
-export default extension;
+export default plugin;
```

### Comparing `jupyterlab_code_formatter-1.6.1/tsconfig.json` & `jupyterlab_code_formatter-2.0.0rc1/tsconfig.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9671052631578947%*

 * *Differences: {"'compilerOptions'": "{'strictNullChecks': True, 'target': 'ES2018', 'types': ['jest'], 'jsx': "*

 * *                      "'react'}"}*

```diff
@@ -1,25 +1,28 @@
 {
     "compilerOptions": {
         "allowSyntheticDefaultImports": true,
         "composite": true,
         "declaration": true,
         "esModuleInterop": true,
         "incremental": true,
+        "jsx": "react",
         "module": "esnext",
         "moduleResolution": "node",
         "noEmitOnError": true,
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
-        "strictNullChecks": false,
-        "target": "es2017",
-        "types": []
+        "strictNullChecks": true,
+        "target": "ES2018",
+        "types": [
+            "jest"
+        ]
     },
     "include": [
         "src/*"
     ]
 }
```

