# Comparing `tmp/jupyterlab_code_formatter-2.0.0rc2.tar.gz` & `tmp/jupyterlab_code_formatter-2.1.0rc0.tar.gz`

## Comparing `jupyterlab_code_formatter-2.0.0rc2.tar` & `jupyterlab_code_formatter-2.1.0rc0.tar`

### file list

```diff
@@ -1,81 +1,80 @@
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/.prettierignore
--rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/CHANGELOG.md
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/RELEASE.md
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/Taskfile.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/babel.config.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/conftest.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/dev.Dockerfile
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/dev.md
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docker-compose.dev.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jest.config.js
--rw-r--r--   0        0        0     6568 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/package.json
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/requirements-dev.txt
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/requirements-docs.txt
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/requirements-test.txt
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/tsconfig.json
--rw-r--r--   0        0        0   383940 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/yarn.lock
--rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/changelog.md
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/conf.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/configuration.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/custom-formatter.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/dev.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/faq.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/index.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/installation.md
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/jupyterhub.md
--rw-r--r--   0        0        0    27767 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/logo.png
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/usage.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/your-support.md
--rw-r--r--   0        0        0   493973 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/_static/format-all.gif
--rw-r--r--   0        0        0   836371 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/_static/format-selected.gif
--rw-r--r--   0        0        0  1862680 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/_static/format-specific.gif
--rw-r--r--   0        0        0  1408342 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/docs/_static/settings.gif
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyter-config/nb-config/jupyterlab_code_formatter.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyter-config/server-config/jupyterlab_code_formatter.json
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/_version.py
--rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/formatters.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/handlers.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/build_log.json
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/package.json
--rw-r--r--   0        0        0     6568 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/package.json.orig
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/settings.json
--rw-r--r--   0        0        0    22284 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/lib_index_js.7fcef9ea39c2b4846c2b.js
--rw-r--r--   0        0        0    29117 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/lib_index_js.7fcef9ea39c2b4846c2b.js.map
--rw-r--r--   0        0        0    29564 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/remoteEntry.26ea8ddf38b373b61cfc.js
--rw-r--r--   0        0        0    28472 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/remoteEntry.26ea8ddf38b373b61cfc.js.map
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/style.js
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js.map
--rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js
--rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js.map
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/tests/__init__.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/tests/conftest.py
--rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/tests/test_handlers.py
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/schema/settings.json
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/scripts/format.sh
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/scripts/test.sh
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/src/client.ts
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/src/constants.ts
--rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/src/formatter.ts
--rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/src/index.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/src/__tests__/jupyterlab_code_formatter.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/style/index.js
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/test_snippets/some_python.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/test_snippets/test_notebook.ipynb
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/test_snippets/test_notebook_crablang.ipynb
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/ui-tests/tests/jupyterlab_code_formatter.spec.ts
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/LICENSE
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/.prettierignore
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/RELEASE.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/Taskfile.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/babel.config.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/conftest.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/dev.Dockerfile
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docker-compose.dev.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jest.config.js
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/package.json
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/requirements-dev.txt
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/requirements-readthedocs.txt
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/requirements-test.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/tsconfig.json
+-rw-r--r--   0        0        0   384000 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/yarn.lock
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/changelog.md
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/conf.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/configuration.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/custom-formatter.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/dev.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/faq.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/index.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/installation.md
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/jupyterhub.md
+-rw-r--r--   0        0        0    27767 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/logo.png
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/usage.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/your-support.md
+-rw-r--r--   0        0        0   493973 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/_static/format-all.gif
+-rw-r--r--   0        0        0   836371 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/_static/format-selected.gif
+-rw-r--r--   0        0        0  1862680 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/_static/format-specific.gif
+-rw-r--r--   0        0        0  1408342 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/docs/_static/settings.gif
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyter-config/nb-config/jupyterlab_code_formatter.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyter-config/server-config/jupyterlab_code_formatter.json
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/_version.py
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/formatters.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/handlers.py
+-rw-r--r--   0        0        0    20714 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/build_log.json
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/package.json
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/package.json.orig
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/settings.json
+-rw-r--r--   0        0        0    22337 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/lib_index_js.7aa378f926383c6ad3f0.js
+-rw-r--r--   0        0        0    29166 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/lib_index_js.7aa378f926383c6ad3f0.js.map
+-rw-r--r--   0        0        0    29560 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/remoteEntry.401d3ea4715fec19e0e1.js
+-rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/remoteEntry.401d3ea4715fec19e0e1.js.map
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/style.js
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js.map
+-rw-r--r--   0        0        0    12080 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js.map
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/tests/__init__.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/tests/conftest.py
+-rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/tests/test_handlers.py
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/schema/settings.json
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/scripts/format.sh
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/scripts/test.sh
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/src/client.ts
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/src/constants.ts
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/src/formatter.ts
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/src/index.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/src/__tests__/jupyterlab_code_formatter.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/style/index.js
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/test_snippets/some_python.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/test_snippets/test_notebook.ipynb
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/test_snippets/test_notebook_crablang.ipynb
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/ui-tests/tests/jupyterlab_code_formatter.spec.ts
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/README.md
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 jupyterlab_code_formatter-2.1.0rc0/PKG-INFO
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/CHANGELOG.md` & `jupyterlab_code_formatter-2.1.0rc0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changelog
 
-## Unreleased
+## 2.0.0 2023-05-08
 
 **General**
 
 - Major refactor of repo, now based off the update jupyterlab extension cookiecutter;
 - Introduce an actually working dockerised dev env;
 
 **Server extension**
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/RELEASE.md` & `jupyterlab_code_formatter-2.1.0rc0/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 This extension can be distributed as Python
 packages. All of the Python
 packaging instructions in the `pyproject.toml` file to wrap your extension in a
 Python package. Before generating a package, we first need to install `build`.
 
 ```bash
-pip install build twine hatch
+pip install build twine hatch hatch-pip-deepfreeze
 ```
 
 Bump the version using `hatch`. By default this will create a tag.
 See the docs on [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version#semver) for details.
 
 ```bash
 hatch version <new-version>
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/Taskfile.yml` & `jupyterlab_code_formatter-2.1.0rc0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/dev.Dockerfile` & `jupyterlab_code_formatter-2.1.0rc0/dev.Dockerfile`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/dev.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/dev.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-### Development environment
+# Development
 
 Prerequisites:
 
 - Install [task](https://taskfile.dev);
 - Install docker, with buildkit;
 
 1. Spin up docker compose based dev env - `task dev:up`
 2. Run `jlpm watch` inside dev container - `task dev:jlpm-watch`
 3. In another terminal, run `jupyter lab` inside dev container - `task dev:jupyter-lab`
 
 This watches the source directory and run JupyterLab at the same time in different terminals to watch for changes in the
 extension's source and automatically rebuild the extension inside the dev docker container.
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
-
-### Packaging the extension
-
-See [RELEASE](RELEASE.md)
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jest.config.js` & `jupyterlab_code_formatter-2.1.0rc0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/package.json` & `jupyterlab_code_formatter-2.1.0rc0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9712752525252526%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.0 || ~4.0.0', '@jupyterlab/settingregistry': "*

 * *                   "'^3.6.0 || ~4.0.0', '@jupyterlab/fileeditor': '^3.6.0 || ~4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.6.0 || ~4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.0 || ~4.0.0', '@jupyterlab/testutils': "*

 * *                      "'^3.6.0 || ~4.0.0'}",*

 * * "'version'": "'2.1.0-rc0'"}*

```diff
@@ -3,27 +3,27 @@
         "email": "ryantam626@gmail.com",
         "name": "Ryan Tam"
     },
     "bugs": {
         "url": " https://github.com/ryantam626/jupyterlab_code_formatter/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
+        "@jupyterlab/application": "^3.6.0 || ~4.0.0",
         "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/fileeditor": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
+        "@jupyterlab/fileeditor": "^3.6.0 || ~4.0.0",
+        "@jupyterlab/mainmenu": "^3.6.0 || ~4.0.0",
         "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0"
+        "@jupyterlab/settingregistry": "^3.6.0 || ~4.0.0"
     },
     "description": " A JupyterLab plugin to facilitate invocation of code formatters.",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
+        "@jupyterlab/builder": "^3.6.0 || ~4.0.0",
+        "@jupyterlab/testutils": "^3.6.0 || ~4.0.0",
         "@types/jest": "^26.0.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "jest": "^26.0.0",
@@ -186,9 +186,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.0.0-rc2"
+    "version": "2.1.0-rc0"
 }
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/requirements-dev.txt` & `jupyterlab_code_formatter-2.1.0rc0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/requirements-test.txt` & `jupyterlab_code_formatter-2.1.0rc0/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/requirements.txt` & `jupyterlab_code_formatter-2.1.0rc0/requirements.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/tsconfig.json` & `jupyterlab_code_formatter-2.1.0rc0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/yarn.lock` & `jupyterlab_code_formatter-2.1.0rc0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1281,15 +1281,15 @@
     "@jupyterlab/nbformat" "^3.0.0 || ^4.0.0-alpha.15"
     "@lumino/coreutils" "^1.11.0 || ^2.0.0-alpha.6"
     "@lumino/disposable" "^1.10.0 || ^2.0.0-alpha.6"
     "@lumino/signaling" "^1.10.0 || ^2.0.0-alpha.6"
     y-protocols "^1.0.5"
     yjs "^13.5.40"
 
-"@jupyterlab/application@^3.1.0":
+"@jupyterlab/application@^3.6.0 || ~4.0.0":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/application/-/application-3.6.3.tgz#7e199f77a4536bc7429fbecf9ba1850f51d9de52"
   integrity sha512-G0tR6sUSCuHB8vGQnaB5lfihKNJVHtqYNoMlsZYF9rYpZEhW1TRD4uE5rg4RfDDR+GghjckQlP3rRNB2Vn4tMA==
   dependencies:
     "@fortawesome/fontawesome-free" "^5.12.0"
     "@jupyterlab/apputils" "^3.6.3"
     "@jupyterlab/coreutils" "^5.6.3"
@@ -1348,15 +1348,15 @@
     "@jupyterlab/nbformat" "^3.6.3"
     "@jupyterlab/observables" "^4.6.3"
     "@jupyterlab/rendermime" "^3.6.3"
     "@jupyterlab/rendermime-interfaces" "^3.6.3"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
-"@jupyterlab/builder@^3.1.0":
+"@jupyterlab/builder@^3.6.0 || ~4.0.0":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-3.6.3.tgz#a4b22efe34e9598b84122ff10509d3d890017b6a"
   integrity sha512-oY1a/r75RMoPzhSmuVu+DfjL0cKk1ceHTniZsM2wPuhjjyoF875u6CDzArJatpOOuTgLm7CY5OcU3LCIK1OAgg==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/application" "^1.31.4"
     "@lumino/commands" "^1.19.0"
@@ -1561,15 +1561,15 @@
     "@lumino/messaging" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/virtualdom" "^1.14.0"
     "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/fileeditor@^3.0.0":
+"@jupyterlab/fileeditor@^3.6.0 || ~4.0.0":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/fileeditor/-/fileeditor-3.6.3.tgz#3eff401fe35e3c3f0b960d0252e1c7068aeb1d96"
   integrity sha512-O3VM2Dd5tsMNC/mvwGGTBdrQuQYVqqQ7SUAlF8eFnDLnmMranq05s5fNRADQLJez6FtR8lDZR8vmxRcOhUN5iw==
   dependencies:
     "@jupyterlab/apputils" "^3.6.3"
     "@jupyterlab/codeeditor" "^3.6.3"
     "@jupyterlab/docregistry" "^3.6.3"
@@ -1577,15 +1577,15 @@
     "@jupyterlab/translation" "^3.6.3"
     "@jupyterlab/ui-components" "^3.6.3"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     react "^17.0.1"
 
-"@jupyterlab/mainmenu@^3.0.0":
+"@jupyterlab/mainmenu@^3.6.0 || ~4.0.0":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/mainmenu/-/mainmenu-3.6.3.tgz#5d322db9b8d742b7042109ab7e8c733696ae38fc"
   integrity sha512-ohZzHDeReKX3zbLz2bUsYRSdkX6bVhNoCer3Rat8gjfb8vr/bqK9ReAvvoA4rRqm0mrfqwotpZSzbE4+y5KqZA==
   dependencies:
     "@jupyterlab/apputils" "^3.6.3"
     "@jupyterlab/services" "^6.6.3"
     "@jupyterlab/translation" "^3.6.3"
@@ -1707,15 +1707,15 @@
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.1.0", "@jupyterlab/settingregistry@^3.6.3":
+"@jupyterlab/settingregistry@^3.6.0 || ~4.0.0", "@jupyterlab/settingregistry@^3.6.3":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.3.tgz#642f8b6449d626821ef13a7e778ae716fa8331c9"
   integrity sha512-pnzIge0ZC8V63R97HiNroJ0eaPM0DN6x65SStyLuv/K8Qez4XqpOdc0Wfell5ri5mxMvm1qKekuFeTikqSXQKQ==
   dependencies:
     "@jupyterlab/statedb" "^3.6.3"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
@@ -1751,15 +1751,15 @@
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     csstype "~3.0.3"
     react "^17.0.1"
     typestyle "^2.0.4"
 
-"@jupyterlab/testutils@^3.0.0":
+"@jupyterlab/testutils@^3.6.0 || ~4.0.0":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/testutils/-/testutils-3.6.3.tgz#f6785f616ad23c37a07f6c7350def440a9a0cffa"
   integrity sha512-ryydfRiTWCWebLWevKyY/ZqEV5MIdH4VV4Cdn3KsBhZ/jD/wN9BGpX4w/PlXkz211KfC6izbuhC8NwOV33SH4g==
   dependencies:
     "@jupyterlab/apputils" "^3.6.3"
     "@jupyterlab/cells" "^3.6.3"
     "@jupyterlab/codeeditor" "^3.6.3"
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/changelog.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Changelog
 
-## Unreleased
+## Dev
+
+**Jupyterlab extension**
+
+- Support for JupyterLab 3.6+/4+ and Notebook v7, courtesy of mcrutch;
+
+## 2.0.0 2023-05-08
 
 **General**
 
 - Major refactor of repo, now based off the update jupyterlab extension cookiecutter;
 - Introduce an actually working dockerised dev env;
 
 **Server extension**
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/conf.py` & `jupyterlab_code_formatter-2.1.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/configuration.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/configuration.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,22 @@
     ]
   }
 }
 ```
 
 :::{warning}
 This plugin does not pick up file based configuration at the moment (e.g. setup.cfg, pyproject.yml, etc.)
+
+Ticket is already opened at [#167](https://github.com/ryantam626/jupyterlab_code_formatter/issues/167).
+:::
+
+:::{warning}
+This plugin might be out of sync with the list of possibilities of configuration option.
+
+See [settings.json](https://github.com/ryantam626/jupyterlab_code_formatter/blob/master/schema/settings.json) for the JSON schema used, feel free to open a PR for updating it.
 :::
 
 ## Chaining Formatters Invocation
 
 The `jupyterlab_code_formatter:format` and `jupyterlab_code_formatter:format_all` JupyterLab commands support invocation of multiple formatters one after the other via settings.
 
 :::{note}
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/custom-formatter.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/custom-formatter.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/faq.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/index.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/index.md`

 * *Files 25% similar despite different names*

```diff
@@ -5,142 +5,115 @@
 00000040: 0a63 7573 746f 6d2d 666f 726d 6174 7465  .custom-formatte
 00000050: 722e 6d64 0a66 6171 2e6d 640a 6a75 7079  r.md.faq.md.jupy
 00000060: 7465 7268 7562 2e6d 640a 6368 616e 6765  terhub.md.change
 00000070: 6c6f 672e 6d64 0a64 6576 2e6d 640a 796f  log.md.dev.md.yo
 00000080: 7572 2d73 7570 706f 7274 2e6d 640a 0a60  ur-support.md..`
 00000090: 6060 0a0a 2320 4a75 7079 7465 724c 6162  ``..# JupyterLab
 000000a0: 2043 6f64 6520 466f 726d 6174 7465 720a   Code Formatter.
-000000b0: 0a5b 215b 4269 6e64 6572 5d28 6874 7470  .[![Binder](http
-000000c0: 733a 2f2f 6d79 6269 6e64 6572 2e6f 7267  s://mybinder.org
-000000d0: 2f62 6164 6765 5f6c 6f67 6f2e 7376 6729  /badge_logo.svg)
-000000e0: 5d28 6874 7470 733a 2f2f 6d79 6269 6e64  ](https://mybind
-000000f0: 6572 2e6f 7267 2f76 322f 6768 2f72 7961  er.org/v2/gh/rya
-00000100: 6e74 616d 3632 362f 6a75 7079 7465 726c  ntam626/jupyterl
-00000110: 6162 5f63 6f64 655f 666f 726d 6174 7465  ab_code_formatte
-00000120: 722f 6d61 7374 6572 3f75 726c 7061 7468  r/master?urlpath
-00000130: 3d6c 6162 290a 5b21 5b6e 706d 2076 6572  =lab).[![npm ver
-00000140: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
-00000150: 6467 652e 6675 7279 2e69 6f2f 6a73 2f25  dge.fury.io/js/%
-00000160: 3430 7279 616e 7461 6d36 3236 2532 466a  40ryantam626%2Fj
-00000170: 7570 7974 6572 6c61 625f 636f 6465 5f66  upyterlab_code_f
-00000180: 6f72 6d61 7474 6572 2e73 7667 295d 2868  ormatter.svg)](h
-00000190: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
-000001a0: 792e 696f 2f6a 732f 2534 3072 7961 6e74  y.io/js/%40ryant
-000001b0: 616d 3632 3625 3246 6a75 7079 7465 726c  am626%2Fjupyterl
-000001c0: 6162 5f63 6f64 655f 666f 726d 6174 7465  ab_code_formatte
-000001d0: 7229 0a5b 215b 6e70 6d20 646f 776e 6c6f  r).[![npm downlo
-000001e0: 6164 735d 2868 7474 7073 3a2f 2f69 6d67  ads](https://img
-000001f0: 2e73 6869 656c 6473 2e69 6f2f 6e70 6d2f  .shields.io/npm/
-00000200: 6477 2f25 3430 7279 616e 7461 6d36 3236  dw/%40ryantam626
-00000210: 2532 466a 7570 7974 6572 6c61 625f 636f  %2Fjupyterlab_co
-00000220: 6465 5f66 6f72 6d61 7474 6572 2e73 7667  de_formatter.svg
-00000230: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
-00000240: 2e66 7572 792e 696f 2f6a 732f 2534 3072  .fury.io/js/%40r
-00000250: 7961 6e74 616d 3632 3625 3246 6a75 7079  yantam626%2Fjupy
-00000260: 7465 726c 6162 5f63 6f64 655f 666f 726d  terlab_code_form
-00000270: 6174 7465 7229 0a5b 215b 636f 6465 2073  atter).[![code s
-00000280: 7479 6c65 5d28 6874 7470 733a 2f2f 696d  tyle](https://im
-00000290: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000002a0: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
-000002b0: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
-000002c0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-000002d0: 622e 636f 6d2f 616d 6276 2f62 6c61 636b  b.com/ambv/black
-000002e0: 290a 5b21 5b47 6974 6875 6220 4163 7469  ).[![Github Acti
-000002f0: 6f6e 7320 5374 6174 7573 5d28 6874 7470  ons Status](http
-00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00000310: 7961 6e74 616d 3632 362f 6a75 7079 7465  yantam626/jupyte
-00000320: 726c 6162 5f63 6f64 655f 666f 726d 6174  rlab_code_format
-00000330: 7465 722f 776f 726b 666c 6f77 732f 4349  ter/workflows/CI
-00000340: 2f62 6164 6765 2e73 7667 295d 2868 7474  /badge.svg)](htt
-00000350: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000360: 7279 616e 7461 6d36 3236 2f6a 7570 7974  ryantam626/jupyt
-00000370: 6572 6c61 625f 636f 6465 5f66 6f72 6d61  erlab_code_forma
-00000380: 7474 6572 2f61 6374 696f 6e73 290a 0a2a  tter/actions)..*
-00000390: 4120 4a75 7079 7465 724c 6162 2070 6c75  A JupyterLab plu
-000003a0: 6769 6e20 746f 2066 6163 696c 6974 6174  gin to facilitat
-000003b0: 6520 696e 766f 6361 7469 6f6e 206f 6620  e invocation of 
-000003c0: 636f 6465 2066 6f72 6d61 7474 6572 732e  code formatters.
-000003d0: 2a0a 0a2a 2a53 6f75 7263 6520 436f 6465  *..**Source Code
-000003e0: 2a2a 3a20 5b47 6974 4875 625d 2868 7474  **: [GitHub](htt
-000003f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000400: 7279 616e 7461 6d36 3236 2f6a 7570 7974  ryantam626/jupyt
-00000410: 6572 6c61 625f 636f 6465 5f66 6f72 6d61  erlab_code_forma
-00000420: 7474 6572 2f29 2e0a 0a23 2320 4465 6d6f  tter/)...## Demo
-00000430: 0a0a 215b 666f 726d 6174 2d61 6c6c 5d28  ..![format-all](
-00000440: 5f73 7461 7469 632f 666f 726d 6174 2d61  _static/format-a
-00000450: 6c6c 2e67 6966 290a 0a23 2320 5265 7175  ll.gif)..## Requ
-00000460: 6972 656d 656e 7473 0a0a 2d20 5079 7468  irements..- Pyth
-00000470: 6f6e 2033 2e36 2b0a 2d20 4a75 7079 7465  on 3.6+.- Jupyte
-00000480: 724c 6162 203e 3d20 332e 302e 300a 2d20  rLab >= 3.0.0.- 
-00000490: 416e 7920 7375 7070 6f72 7465 6420 636f  Any supported co
-000004a0: 6465 2066 6f72 6d61 7474 6572 7320 2879  de formatters (y
-000004b0: 6f75 2063 616e 2061 6c73 6f20 7370 6563  ou can also spec
-000004c0: 6966 7920 796f 7572 206f 776e 2c20 7365  ify your own, se
-000004d0: 6520 5b63 7573 746f 6d20 666f 726d 6174  e [custom format
-000004e0: 7465 725d 2863 7573 746f 6d2d 666f 726d  ter](custom-form
-000004f0: 6174 7465 722e 6d64 2929 2e0a 0a3a 3a3a  atter.md))...:::
-00000500: 7b69 6d70 6f72 7461 6e74 7d0a 4a75 7079  {important}.Jupy
-00000510: 7465 724c 6162 2043 6f64 6520 466f 726d  terLab Code Form
-00000520: 6174 7465 7220 6f6e 6c79 2070 726f 7669  atter only provi
-00000530: 6465 7320 616e 2069 6e74 6572 6661 6365  des an interface
-00000540: 2066 6f72 2069 6e76 6f6b 696e 6720 636f   for invoking co
-00000550: 6465 2066 6f72 6d61 7474 6572 7320 6f6e  de formatters on
-00000560: 204a 7570 7974 6572 2053 6572 7665 722c   Jupyter Server,
-00000570: 2061 6e64 2064 6f65 7320 6e6f 7420 696e   and does not in
-00000580: 636c 7564 6520 616e 7920 636f 6465 2066  clude any code f
-00000590: 6f72 6d61 7474 6572 2062 7920 6465 6661  ormatter by defa
-000005a0: 756c 742e 0a3a 3a3a 0a0a 2323 2051 7569  ult..:::..## Qui
-000005b0: 636b 2053 7461 7274 0a0a 5b2f 2f5d 3a20  ck Start..[//]: 
-000005c0: 2320 2854 4f44 4f3a 2041 6464 2074 6162  # (TODO: Add tab
-000005d0: 2066 6f72 2063 6f6d 6d6f 6e20 7061 636b   for common pack
-000005e0: 6167 6520 6d61 6e61 6765 7273 290a 0a31  age managers)..1
-000005f0: 2e20 2a2a 496e 7374 616c 6c20 7468 6520  . **Install the 
-00000600: 7061 636b 6167 652a 2a0a 6060 6060 7b74  package**.````{t
-00000610: 6162 7d20 5069 700a 6060 6062 6173 680a  ab} Pip.```bash.
-00000620: 7069 7020 696e 7374 616c 6c20 6a75 7079  pip install jupy
-00000630: 7465 726c 6162 2d63 6f64 652d 666f 726d  terlab-code-form
-00000640: 6174 7465 720a 6060 600a 6060 6060 0a0a  atter.```.````..
-00000650: 6060 6060 7b74 6162 7d20 436f 6e64 610a  ````{tab} Conda.
-00000660: 6060 6062 6173 680a 636f 6e64 6120 696e  ```bash.conda in
-00000670: 7374 616c 6c20 2d63 2063 6f6e 6461 2d66  stall -c conda-f
-00000680: 6f72 6765 206a 7570 7974 6572 6c61 625f  orge jupyterlab_
-00000690: 636f 6465 5f66 6f72 6d61 7474 6572 0a60  code_formatter.`
-000006a0: 6060 0a60 6060 600a 0a60 6060 607b 7461  ``.````..````{ta
-000006b0: 627d 2050 6f65 7472 790a 6060 6062 6173  b} Poetry.```bas
-000006c0: 680a 706f 6574 7279 2061 6464 206a 7570  h.poetry add jup
-000006d0: 7974 6572 6c61 622d 636f 6465 2d66 6f72  yterlab-code-for
-000006e0: 6d61 7474 6572 0a60 6060 0a60 6060 600a  matter.```.````.
-000006f0: 0a60 6060 607b 7461 627d 2050 6970 656e  .````{tab} Pipen
-00000700: 760a 6060 6062 6173 680a 7069 7065 6e76  v.```bash.pipenv
-00000710: 2069 6e73 7461 6c6c 206a 7570 7974 6572   install jupyter
-00000720: 6c61 622d 636f 6465 2d66 6f72 6d61 7474  lab-code-formatt
-00000730: 6572 0a60 6060 0a60 6060 600a 0a32 2e20  er.```.````..2. 
-00000740: 2a2a 496e 7374 616c 6c20 736f 6d65 2073  **Install some s
-00000750: 7570 706f 7274 6564 2066 6f72 6d61 7474  upported formatt
-00000760: 6572 732a 2a20 2869 736f 7274 2b62 6c61  ers** (isort+bla
-00000770: 636b 2061 7265 2064 6566 6175 6c74 2066  ck are default f
-00000780: 6f72 2050 7974 686f 6e29 0a60 6060 6261  or Python).```ba
-00000790: 7368 0a23 204e 4f54 453a 2049 6e73 7461  sh.# NOTE: Insta
-000007a0: 6c6c 2062 6c61 636b 2061 6e64 2069 736f  ll black and iso
-000007b0: 7274 2c0a 2320 2020 2020 2020 4a4c 2063  rt,.#       JL c
-000007c0: 6f64 6520 666f 726d 6174 7465 7220 6973  ode formatter is
-000007d0: 2063 6f6e 6669 6775 7265 6420 746f 2069   configured to i
-000007e0: 6e76 6f6b 6520 6973 6f72 7420 616e 6420  nvoke isort and 
-000007f0: 626c 6163 6b20 6279 2064 6566 6175 6c74  black by default
-00000800: 0a70 6970 2069 6e73 7461 6c6c 2062 6c61  .pip install bla
-00000810: 636b 2069 736f 7274 0a60 6060 0a0a 332e  ck isort.```..3.
-00000820: 202a 2a52 6573 7461 7274 204a 7570 7974   **Restart Jupyt
-00000830: 6572 4c61 622a 2a0a 0a54 6869 7320 706c  erLab**..This pl
-00000840: 7567 696e 2069 6e63 6c75 6465 7320 6120  ugin includes a 
-00000850: 7365 7276 6572 2070 6c75 6769 6e2c 2072  server plugin, r
-00000860: 6573 7461 7274 204a 7570 7974 6572 4c61  estart JupyterLa
-00000870: 6220 6966 2079 6f75 2068 6176 6520 666f  b if you have fo
-00000880: 6c6c 6f77 6564 2074 6865 2061 626f 7665  llowed the above
-00000890: 2073 7465 7073 2077 6869 6c65 2069 7427   steps while it'
-000008a0: 7320 7275 6e6e 696e 672e 0a0a 342e 202a  s running...4. *
-000008b0: 2a43 6f6e 6669 6775 7265 2070 6c75 6769  *Configure plugi
-000008c0: 6e2a 2a0a 0a54 6f20 636f 6e66 6967 7572  n**..To configur
-000008d0: 6520 7768 6963 682f 686f 7720 666f 726d  e which/how form
-000008e0: 6174 7465 7273 2061 7265 2069 6e76 6f6b  atters are invok
-000008f0: 6564 2c20 7365 6520 5b63 6f6e 6669 6775  ed, see [configu
-00000900: 7261 7469 6f6e 5d28 636f 6e66 6967 7572  ration](configur
-00000910: 6174 696f 6e2e 6d64 292e 0a              ation.md)..
+000000b0: 0a2a 4120 4a75 7079 7465 724c 6162 2070  .*A JupyterLab p
+000000c0: 6c75 6769 6e20 746f 2066 6163 696c 6974  lugin to facilit
+000000d0: 6174 6520 696e 766f 6361 7469 6f6e 206f  ate invocation o
+000000e0: 6620 636f 6465 2066 6f72 6d61 7474 6572  f code formatter
+000000f0: 732e 2a0a 0a2a 2a53 6f75 7263 6520 436f  s.*..**Source Co
+00000100: 6465 2a2a 3a20 5b47 6974 4875 625d 2868  de**: [GitHub](h
+00000110: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000120: 6d2f 7279 616e 7461 6d36 3236 2f6a 7570  m/ryantam626/jup
+00000130: 7974 6572 6c61 625f 636f 6465 5f66 6f72  yterlab_code_for
+00000140: 6d61 7474 6572 2f29 2e0a 0a23 2320 4465  matter/)...## De
+00000150: 6d6f 0a0a 215b 666f 726d 6174 2d61 6c6c  mo..![format-all
+00000160: 5d28 5f73 7461 7469 632f 666f 726d 6174  ](_static/format
+00000170: 2d61 6c6c 2e67 6966 290a 0a23 2320 5265  -all.gif)..## Re
+00000180: 7175 6972 656d 656e 7473 0a0a 2d20 5079  quirements..- Py
+00000190: 7468 6f6e 2033 2e37 2b0a 2d20 4a75 7079  thon 3.7+.- Jupy
+000001a0: 7465 724c 6162 203e 3d20 332e 302e 300a  terLab >= 3.0.0.
+000001b0: 2d20 416e 7920 7375 7070 6f72 7465 6420  - Any supported 
+000001c0: 636f 6465 2066 6f72 6d61 7474 6572 7320  code formatters 
+000001d0: 2879 6f75 2063 616e 2061 6c73 6f20 7370  (you can also sp
+000001e0: 6563 6966 7920 796f 7572 206f 776e 2c20  ecify your own, 
+000001f0: 7365 6520 5b63 7573 746f 6d20 666f 726d  see [custom form
+00000200: 6174 7465 725d 2863 7573 746f 6d2d 666f  atter](custom-fo
+00000210: 726d 6174 7465 722e 6d64 2929 2e0a 0a3a  rmatter.md))...:
+00000220: 3a3a 7b69 6d70 6f72 7461 6e74 7d0a 4a75  ::{important}.Ju
+00000230: 7079 7465 724c 6162 2043 6f64 6520 466f  pyterLab Code Fo
+00000240: 726d 6174 7465 7220 6f6e 6c79 2070 726f  rmatter only pro
+00000250: 7669 6465 7320 616e 2069 6e74 6572 6661  vides an interfa
+00000260: 6365 2066 6f72 2069 6e76 6f6b 696e 6720  ce for invoking 
+00000270: 636f 6465 2066 6f72 6d61 7474 6572 7320  code formatters 
+00000280: 6f6e 204a 7570 7974 6572 2053 6572 7665  on Jupyter Serve
+00000290: 722c 2061 6e64 2064 6f65 7320 6e6f 7420  r, and does not 
+000002a0: 696e 636c 7564 6520 616e 7920 636f 6465  include any code
+000002b0: 2066 6f72 6d61 7474 6572 2062 7920 6465   formatter by de
+000002c0: 6661 756c 742e 0a3a 3a3a 0a0a 2323 2051  fault..:::..## Q
+000002d0: 7569 636b 2053 7461 7274 0a0a 5b2f 2f5d  uick Start..[//]
+000002e0: 3a20 2320 2854 4f44 4f3a 2041 6464 2074  : # (TODO: Add t
+000002f0: 6162 2066 6f72 2063 6f6d 6d6f 6e20 7061  ab for common pa
+00000300: 636b 6167 6520 6d61 6e61 6765 7273 290a  ckage managers).
+00000310: 0a31 2e20 2a2a 496e 7374 616c 6c20 7468  .1. **Install th
+00000320: 6520 7061 636b 6167 652a 2a0a 6060 6060  e package**.````
+00000330: 7b74 6162 7d20 5069 700a 6060 6062 6173  {tab} Pip.```bas
+00000340: 680a 7069 7020 696e 7374 616c 6c20 6a75  h.pip install ju
+00000350: 7079 7465 726c 6162 2d63 6f64 652d 666f  pyterlab-code-fo
+00000360: 726d 6174 7465 720a 6060 600a 6060 6060  rmatter.```.````
+00000370: 0a0a 6060 6060 7b74 6162 7d20 506f 6574  ..````{tab} Poet
+00000380: 7279 0a60 6060 6261 7368 0a70 6f65 7472  ry.```bash.poetr
+00000390: 7920 6164 6420 6a75 7079 7465 726c 6162  y add jupyterlab
+000003a0: 2d63 6f64 652d 666f 726d 6174 7465 720a  -code-formatter.
+000003b0: 6060 600a 6060 6060 0a0a 6060 6060 7b74  ```.````..````{t
+000003c0: 6162 7d20 5069 7065 6e76 0a60 6060 6261  ab} Pipenv.```ba
+000003d0: 7368 0a70 6970 656e 7620 696e 7374 616c  sh.pipenv instal
+000003e0: 6c20 6a75 7079 7465 726c 6162 2d63 6f64  l jupyterlab-cod
+000003f0: 652d 666f 726d 6174 7465 720a 6060 600a  e-formatter.```.
+00000400: 6060 6060 0a0a 322e 202a 2a49 6e73 7461  ````..2. **Insta
+00000410: 6c6c 2073 6f6d 6520 7375 7070 6f72 7465  ll some supporte
+00000420: 6420 666f 726d 6174 7465 7273 2a2a 2028  d formatters** (
+00000430: 6973 6f72 742b 626c 6163 6b20 6172 6520  isort+black are 
+00000440: 6465 6661 756c 7420 666f 7220 5079 7468  default for Pyth
+00000450: 6f6e 290a 6060 6060 7b74 6162 7d20 5069  on).````{tab} Pi
+00000460: 700a 6060 6062 6173 680a 2320 4e4f 5445  p.```bash.# NOTE
+00000470: 3a20 496e 7374 616c 6c20 626c 6163 6b20  : Install black 
+00000480: 616e 6420 6973 6f72 742c 0a23 2020 2020  and isort,.#    
+00000490: 2020 204a 4c20 636f 6465 2066 6f72 6d61     JL code forma
+000004a0: 7474 6572 2069 7320 636f 6e66 6967 7572  tter is configur
+000004b0: 6564 2074 6f20 696e 766f 6b65 2069 736f  ed to invoke iso
+000004c0: 7274 2061 6e64 2062 6c61 636b 2062 7920  rt and black by 
+000004d0: 6465 6661 756c 740a 7069 7020 696e 7374  default.pip inst
+000004e0: 616c 6c20 626c 6163 6b20 6973 6f72 740a  all black isort.
+000004f0: 6060 600a 6060 6060 0a0a 6060 6060 7b74  ```.````..````{t
+00000500: 6162 7d20 506f 6574 7279 0a60 6060 6261  ab} Poetry.```ba
+00000510: 7368 0a23 204e 4f54 453a 2049 6e73 7461  sh.# NOTE: Insta
+00000520: 6c6c 2062 6c61 636b 2061 6e64 2069 736f  ll black and iso
+00000530: 7274 2c0a 2320 2020 2020 2020 4a4c 2063  rt,.#       JL c
+00000540: 6f64 6520 666f 726d 6174 7465 7220 6973  ode formatter is
+00000550: 2063 6f6e 6669 6775 7265 6420 746f 2069   configured to i
+00000560: 6e76 6f6b 6520 6973 6f72 7420 616e 6420  nvoke isort and 
+00000570: 626c 6163 6b20 6279 2064 6566 6175 6c74  black by default
+00000580: 0a70 6f65 7472 7920 6164 6420 626c 6163  .poetry add blac
+00000590: 6b20 6973 6f72 740a 6060 600a 6060 6060  k isort.```.````
+000005a0: 0a0a 6060 6060 7b74 6162 7d20 5069 7065  ..````{tab} Pipe
+000005b0: 6e76 0a60 6060 6261 7368 0a23 204e 4f54  nv.```bash.# NOT
+000005c0: 453a 2049 6e73 7461 6c6c 2062 6c61 636b  E: Install black
+000005d0: 2061 6e64 2069 736f 7274 2c0a 2320 2020   and isort,.#   
+000005e0: 2020 2020 4a4c 2063 6f64 6520 666f 726d      JL code form
+000005f0: 6174 7465 7220 6973 2063 6f6e 6669 6775  atter is configu
+00000600: 7265 6420 746f 2069 6e76 6f6b 6520 6973  red to invoke is
+00000610: 6f72 7420 616e 6420 626c 6163 6b20 6279  ort and black by
+00000620: 2064 6566 6175 6c74 0a70 6970 656e 7620   default.pipenv 
+00000630: 696e 7374 616c 6c20 626c 6163 6b20 6973  install black is
+00000640: 6f72 740a 6060 600a 6060 6060 0a0a 332e  ort.```.````..3.
+00000650: 202a 2a52 6573 7461 7274 204a 7570 7974   **Restart Jupyt
+00000660: 6572 4c61 622a 2a0a 0a54 6869 7320 706c  erLab**..This pl
+00000670: 7567 696e 2069 6e63 6c75 6465 7320 6120  ugin includes a 
+00000680: 7365 7276 6572 2070 6c75 6769 6e2c 2061  server plugin, a
+00000690: 7320 7375 636b 2079 6f75 2077 696c 6c20  s suck you will 
+000006a0: 6e65 6564 2074 6f20 7265 7374 6172 7420  need to restart 
+000006b0: 4a75 7079 7465 724c 6162 2069 6620 796f  JupyterLab if yo
+000006c0: 7520 6861 7665 2066 6f6c 6c6f 7765 640a  u have followed.
+000006d0: 7468 6520 6162 6f76 6520 7374 6570 7320  the above steps 
+000006e0: 7768 696c 6520 6974 2773 2072 756e 6e69  while it's runni
+000006f0: 6e67 2e0a 0a34 2e20 2a2a 436f 6e66 6967  ng...4. **Config
+00000700: 7572 6520 706c 7567 696e 2a2a 0a0a 546f  ure plugin**..To
+00000710: 2063 6f6e 6669 6775 7265 2077 6869 6368   configure which
+00000720: 2f68 6f77 2066 6f72 6d61 7474 6572 7320  /how formatters 
+00000730: 6172 6520 696e 766f 6b65 642c 2073 6565  are invoked, see
+00000740: 205b 636f 6e66 6967 7572 6174 696f 6e5d   [configuration]
+00000750: 2863 6f6e 6669 6775 7261 7469 6f6e 2e6d  (configuration.m
+00000760: 6429 2e0a                                d)..
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/installation.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/logo.png` & `jupyterlab_code_formatter-2.1.0rc0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/usage.md` & `jupyterlab_code_formatter-2.1.0rc0/docs/usage.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - `jupyterlab_code_formatter:isort`
 - `jupyterlab_code_formatter:yapf`
 - `jupyterlab_code_formatter:formatr`
 - `jupyterlab_code_formatter:styler`
 
 These commands invoke the specified code formatter in the current focused cell.
 
-To find out what formatters are available, you can query http://localhost:8888/jupyterlab_code_formatter/formatters?bypassVersionCheck=1 (you might need to replace the port and address), the keys of formatter are shown there.
+To find out what formatters are available, you can query http://localhost:8888/jupyterlab_code_formatter/formatters (you might need to replace the port and address), the keys of formatter are shown there.
 
 ---
 
 In addition to the above commands, this plugin also adds two non-formatter-specific commands:
 
 - `jupyterlab_code_formatter:format`
 - `jupyterlab_code_formatter:format_all`
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/_static/format-all.gif` & `jupyterlab_code_formatter-2.1.0rc0/docs/_static/format-all.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/_static/format-selected.gif` & `jupyterlab_code_formatter-2.1.0rc0/docs/_static/format-selected.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/_static/format-specific.gif` & `jupyterlab_code_formatter-2.1.0rc0/docs/_static/format-specific.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/docs/_static/settings.gif` & `jupyterlab_code_formatter-2.1.0rc0/docs/_static/settings.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/__init__.py` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/formatters.py` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/formatters.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/handlers.py` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/build_log.json` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993110670194%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'jupyterlab_code_formatter': {'version': "*

 * *      "'2.0.0'}}}}}}"}*

```diff
@@ -601,15 +601,15 @@
                             "import": false,
                             "requiredVersion": "^1.37.2",
                             "singleton": true
                         },
                         "jupyterlab_code_formatter": {
                             "import": "/plugin/lib/index.js",
                             "singleton": true,
-                            "version": "2.0.0-rc1"
+                            "version": "2.0.0"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/package.json` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9709280303030304%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.0 || ~4.0.0', '@jupyterlab/settingregistry': "*

 * *                   "'^3.6.0 || ~4.0.0', '@jupyterlab/fileeditor': '^3.6.0 || ~4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.6.0 || ~4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.0 || ~4.0.0', '@jupyterlab/testutils': "*

 * *                      "'^3.6.0 || ~4.0.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.401d3ea4715fec19e0e1.js'}}",*

 * * "'version'": "'2.0.0'"}*

```diff
@@ -3,27 +3,27 @@
         "email": "ryantam626@gmail.com",
         "name": "Ryan Tam"
     },
     "bugs": {
         "url": " https://github.com/ryantam626/jupyterlab_code_formatter/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
+        "@jupyterlab/application": "^3.6.0 || ~4.0.0",
         "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/fileeditor": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
+        "@jupyterlab/fileeditor": "^3.6.0 || ~4.0.0",
+        "@jupyterlab/mainmenu": "^3.6.0 || ~4.0.0",
         "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0"
+        "@jupyterlab/settingregistry": "^3.6.0 || ~4.0.0"
     },
     "description": " A JupyterLab plugin to facilitate invocation of code formatters.",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
+        "@jupyterlab/builder": "^3.6.0 || ~4.0.0",
+        "@jupyterlab/testutils": "^3.6.0 || ~4.0.0",
         "@types/jest": "^26.0.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "jest": "^26.0.0",
@@ -107,15 +107,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": " https://github.com/ryantam626/jupyterlab_code_formatter",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.26ea8ddf38b373b61cfc.js",
+            "load": "static/remoteEntry.401d3ea4715fec19e0e1.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_code_formatter"
                 },
@@ -191,9 +191,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.0.0-rc1"
+    "version": "2.0.0"
 }
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/package.json.orig` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9712752525252526%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.0 || ~4.0.0', '@jupyterlab/settingregistry': "*

 * *                   "'^3.6.0 || ~4.0.0', '@jupyterlab/fileeditor': '^3.6.0 || ~4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^3.6.0 || ~4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.0 || ~4.0.0', '@jupyterlab/testutils': "*

 * *                      "'^3.6.0 || ~4.0.0'}",*

 * * "'version'": "'2.0.0'"}*

```diff
@@ -3,27 +3,27 @@
         "email": "ryantam626@gmail.com",
         "name": "Ryan Tam"
     },
     "bugs": {
         "url": " https://github.com/ryantam626/jupyterlab_code_formatter/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
+        "@jupyterlab/application": "^3.6.0 || ~4.0.0",
         "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/fileeditor": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
+        "@jupyterlab/fileeditor": "^3.6.0 || ~4.0.0",
+        "@jupyterlab/mainmenu": "^3.6.0 || ~4.0.0",
         "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0"
+        "@jupyterlab/settingregistry": "^3.6.0 || ~4.0.0"
     },
     "description": " A JupyterLab plugin to facilitate invocation of code formatters.",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
-        "@jupyterlab/builder": "^3.1.0",
-        "@jupyterlab/testutils": "^3.0.0",
+        "@jupyterlab/builder": "^3.6.0 || ~4.0.0",
+        "@jupyterlab/testutils": "^3.6.0 || ~4.0.0",
         "@types/jest": "^26.0.0",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "jest": "^26.0.0",
@@ -186,9 +186,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.0.0-rc1"
+    "version": "2.0.0"
 }
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/settings.json` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/schemas/jupyterlab_code_formatter/settings.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/lib_index_js.7fcef9ea39c2b4846c2b.js` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/lib_index_js.7aa378f926383c6ad3f0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -157,15 +157,15 @@
                         });
                         return codeCells;
                     }
                     getNotebookType() {
                         if (!this.notebookTracker.currentWidget) {
                             return null;
                         }
-                        const metadata = this.notebookTracker.currentWidget.content.model.metadata.toJSON();
+                        const metadata = this.notebookTracker.currentWidget.content.model.sharedModel.metadata;;
                         if (!metadata) {
                             return null;
                         }
                         // prefer kernelspec language
                         // @ts-ignore
                         if (metadata.kernelspec && metadata.kernelspec.language) {
                             // @ts-ignore
@@ -201,29 +201,29 @@
                     }
                     async applyFormatters(selectedCells, formattersToUse, config) {
                         var _a;
                         for (const formatterToUse of formattersToUse) {
                             if (formatterToUse === 'noop' || formatterToUse === 'skip') {
                                 continue;
                             }
-                            const currentTexts = selectedCells.map(cell => cell.model.value.text);
+                            const currentTexts = selectedCells.map(cell => cell.model.sharedModel.source);
                             const formattedTexts = await this.formatCode(currentTexts, formatterToUse, config[formatterToUse], true, config.cacheFormatters);
                             const showErrors = !((_a = config.suppressFormatterErrors) !== null && _a !== void 0 ? _a : false);
                             for (let i = 0; i < selectedCells.length; ++i) {
                                 const cell = selectedCells[i];
                                 const currentText = currentTexts[i];
                                 const formattedText = formattedTexts.code[i];
-                                const cellValueHasNotChanged = cell.model.value.text === currentText;
+                                const cellValueHasNotChanged = cell.model.sharedModel.source === currentText;
                                 if (cellValueHasNotChanged) {
                                     if (formattedText.error) {
                                         if (showErrors) {
                                             await (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showErrorMessage)('Jupyterlab Code Formatter Error', formattedText.error);
                                         }
                                     } else {
-                                        cell.model.value.text = formattedText.code;
+                                        cell.model.sharedModel.source = formattedText.code;
                                     }
                                 } else {
                                     if (showErrors) {
                                         await (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showErrorMessage)('Jupyterlab Code Formatter Error', `Cell value changed since format request was sent, formatting for cell ${i} skipped.`);
                                     }
                                 }
                             }
@@ -261,23 +261,23 @@
                     formatAction(config, formatter) {
                         if (this.working) {
                             return;
                         }
                         const editorWidget = this.editorTracker.currentWidget;
                         this.working = true;
                         const editor = editorWidget.content.editor;
-                        const code = editor.model.value.text;
+                        const code = editor.model.sharedModel.source;
                         this.formatCode([code], formatter, config[formatter], false, config.cacheFormatters)
                             .then(data => {
                                 if (data.code[0].error) {
                                     void(0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showErrorMessage)('Jupyterlab Code Formatter Error', data.code[0].error);
                                     this.working = false;
                                     return;
                                 }
-                                this.editorTracker.currentWidget.content.editor.model.value.text =
+                                this.editorTracker.currentWidget.content.editor.model.sharedModel.source =
                                     data.code[0].code;
                                 this.working = false;
                             })
                             .catch(error => {
                                 this.working = false;
                                 void(0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showErrorMessage)('Jupyterlab Code Formatter Error', error);
                             });
@@ -496,8 +496,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.7fcef9ea39c2b4846c2b.js.map
+//# sourceMappingURL=lib_index_js.7aa378f926383c6ad3f0.js.map
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/lib_index_js.7fcef9ea39c2b4846c2b.js.map` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/lib_index_js.7aa378f926383c6ad3f0.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8285714285714285%*

 * *Differences: {"'file'": "'lib_index_js.7aa378f926383c6ad3f0.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;AAA+C;AACS;AAChB;AAExC,MAAM,6BAA6B;IAC1B,OAAO,CAAC,IAAY,EAAE,MAAc,EAAE,IAAS;QACpD,MAAM,QAAQ,GAAG,+EAA6B,EAAE,CAAC;QACjD,MAAM,OAAO,GAAG,8DAAW,CAAC,QAAQ,CAAC,OAAO,EAAE,6DAAqB,EAAE,IAAI,CAAC,CAAC;QAC3E,OAAO,8EAA4B,CACjC,OAAO,EACP;YACE,IAAI;YACJ,MAAM;SACP,EACD,QAAQ,CACT,CAAC,IAAI,CAAC,QAAQ,CAAC,EAAE;YAChB,IAAI,QAAQ,CAAC,MAAM,KAAK,GAAG,EAAE;gBAC3B,OAAO,QAAQ,CAAC,IAAI,EAAE,CAAC,IAAI,CAAC,GAAG,EAAE;oBAC/B,MAAM,IAAI,gFAA8B,CACtC […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "lib_index_js.7fcef9ea39c2b4846c2b.js",
-    "mappings": "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",
+    "file": "lib_index_js.7aa378f926383c6ad3f0.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_code_formatter/./src/client.ts",
         "webpack://jupyterlab_code_formatter/./src/constants.ts",
         "webpack://jupyterlab_code_formatter/./src/formatter.ts",
         "webpack://jupyterlab_code_formatter/./src/index.ts"
     ],
     "sourcesContent": [
         "import { URLExt } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\nimport { Constants } from './constants';\n\nclass JupyterlabCodeFormatterClient {\n  public request(path: string, method: string, body: any): Promise<any> {\n    const settings = ServerConnection.makeSettings();\n    const fullUrl = URLExt.join(settings.baseUrl, Constants.PLUGIN_NAME, path);\n    return ServerConnection.makeRequest(\n      fullUrl,\n      {\n        body,\n        method\n      },\n      settings\n    ).then(response => {\n      if (response.status !== 200) {\n        return response.text().then(() => {\n          throw new ServerConnection.ResponseError(\n            response,\n            response.statusText\n          );\n        });\n      }\n      return response.text();\n    });\n  }\n\n  public getAvailableFormatters(cache: boolean) {\n    return this.request('formatters' + (cache ? '?cached' : ''), 'GET', null);\n  }\n}\n\nexport default JupyterlabCodeFormatterClient;\n",
         "export namespace Constants {\n  export const PLUGIN_NAME = 'jupyterlab_code_formatter';\n  export const FORMAT_COMMAND = `${PLUGIN_NAME}:format`;\n  export const FORMAT_ALL_COMMAND = `${PLUGIN_NAME}:format_all`;\n  // TODO: Extract this to style and import svg as string\n  export const ICON_FORMAT_ALL_SVG =\n    '<svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" focusable=\"false\" width=\"1em\" height=\"1em\" style=\"-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);\" preserveAspectRatio=\"xMidYMid meet\" viewBox=\"0 0 1792 1792\"><path class=\"jp-icon3\" d=\"M1473 929q7-118-33-226.5t-113-189t-177-131T929 325q-116-7-225.5 32t-192 110.5t-135 175T317 863q-7 118 33 226.5t113 189t177.5 131T862 1467q155 9 293-59t224-195.5t94-283.5zM1792 0l-349 348q120 117 180.5 272t50.5 321q-11 183-102 339t-241 255.5T999 1660L0 1792l347-347q-120-116-180.5-271.5T116 852q11-184 102-340t241.5-255.5T792 132q167-22 500-66t500-66z\" fill=\"#626262\"/></svg>';\n  export const ICON_FORMAT_ALL = 'fa fa-superpowers';\n  export const SETTINGS_SECTION = `${PLUGIN_NAME}:settings`;\n  export const COMMAND_SECTION_NAME = 'Jupyterlab Code Formatter';\n  // TODO: Use package.json info\n  export const PLUGIN_VERSION = '1.6.1';\n}\n",
-        "import { Cell, CodeCell } from '@jupyterlab/cells';\nimport { INotebookTracker, Notebook } from '@jupyterlab/notebook';\nimport JupyterlabCodeFormatterClient from './client';\nimport { IEditorTracker } from '@jupyterlab/fileeditor';\nimport { Widget } from '@lumino/widgets';\nimport { showErrorMessage } from '@jupyterlab/apputils';\n\nclass JupyterlabCodeFormatter {\n  working = false;\n  protected client: JupyterlabCodeFormatterClient;\n  constructor(client: JupyterlabCodeFormatterClient) {\n    this.client = client;\n  }\n\n  protected formatCode(\n    code: string[],\n    formatter: string,\n    options: any,\n    notebook: boolean,\n    cache: boolean\n  ) {\n    return this.client\n      .request(\n        'format' + (cache ? '?cached' : ''),\n        'POST',\n        JSON.stringify({\n          code,\n          notebook,\n          formatter,\n          options\n        })\n      )\n      .then(resp => JSON.parse(resp));\n  }\n}\n\nexport class JupyterlabNotebookCodeFormatter extends JupyterlabCodeFormatter {\n  protected notebookTracker: INotebookTracker;\n\n  constructor(\n    client: JupyterlabCodeFormatterClient,\n    notebookTracker: INotebookTracker\n  ) {\n    super(client);\n    this.notebookTracker = notebookTracker;\n  }\n\n  public async formatAction(config: any, formatter?: string) {\n    return this.formatCells(true, config, formatter);\n  }\n\n  public async formatSelectedCodeCells(\n    config: any,\n    formatter?: string,\n    notebook?: Notebook\n  ) {\n    return this.formatCells(true, config, formatter, notebook);\n  }\n\n  public async formatAllCodeCells(\n    config: any,\n    formatter?: string,\n    notebook?: Notebook\n  ) {\n    return this.formatCells(false, config, formatter, notebook);\n  }\n\n  private getCodeCells(selectedOnly = true, notebook?: Notebook): CodeCell[] {\n    if (!this.notebookTracker.currentWidget) {\n      return [];\n    }\n    const codeCells: CodeCell[] = [];\n    notebook = notebook || this.notebookTracker.currentWidget.content;\n    notebook.widgets.forEach((cell: Cell) => {\n      if (cell.model.type === 'code') {\n        if (!selectedOnly || (<Notebook>notebook).isSelectedOrActive(cell)) {\n          codeCells.push(cell as CodeCell);\n        }\n      }\n    });\n    return codeCells;\n  }\n\n  private getNotebookType() {\n    if (!this.notebookTracker.currentWidget) {\n      return null;\n    }\n\n    const metadata =\n      this.notebookTracker.currentWidget.content.model!.metadata.toJSON();\n\n    if (!metadata) {\n      return null;\n    }\n\n    // prefer kernelspec language\n    // @ts-ignore\n    if (metadata.kernelspec && metadata.kernelspec.language) {\n      // @ts-ignore\n      return metadata.kernelspec.language.toLowerCase();\n    }\n\n    // otherwise, check language info code mirror mode\n    // @ts-ignore\n    if (metadata.language_info && metadata.language_info.codemirror_mode) {\n      // @ts-ignore\n      return metadata.language_info.codemirror_mode.name.toLowerCase();\n    }\n\n    return null;\n  }\n\n  private getDefaultFormatters(config: any): Array<string> {\n    const notebookType = this.getNotebookType();\n    if (notebookType) {\n      const defaultFormatter =\n        config.preferences.default_formatter[notebookType];\n      if (defaultFormatter instanceof Array) {\n        return defaultFormatter;\n      } else if (defaultFormatter !== undefined) {\n        return [defaultFormatter];\n      }\n    }\n    return [];\n  }\n\n  private async getFormattersToUse(config: any, formatter?: string) {\n    const defaultFormatters = this.getDefaultFormatters(config);\n    const formattersToUse =\n      formatter !== undefined ? [formatter] : defaultFormatters;\n\n    if (formattersToUse.length === 0) {\n      await showErrorMessage(\n        'Jupyterlab Code Formatter Error',\n        'Unable to find default formatters to use, please file an issue on GitHub.'\n      );\n    }\n\n    return formattersToUse;\n  }\n\n  private async applyFormatters(\n    selectedCells: CodeCell[],\n    formattersToUse: string[],\n    config: any\n  ) {\n    for (const formatterToUse of formattersToUse) {\n      if (formatterToUse === 'noop' || formatterToUse === 'skip') {\n        continue;\n      }\n      const currentTexts = selectedCells.map(cell => cell.model.value.text);\n      const formattedTexts = await this.formatCode(\n        currentTexts,\n        formatterToUse,\n        config[formatterToUse],\n        true,\n        config.cacheFormatters\n      );\n\n      const showErrors = !(config.suppressFormatterErrors ?? false);\n      for (let i = 0; i < selectedCells.length; ++i) {\n        const cell = selectedCells[i];\n        const currentText = currentTexts[i];\n        const formattedText = formattedTexts.code[i];\n        const cellValueHasNotChanged = cell.model.value.text === currentText;\n        if (cellValueHasNotChanged) {\n          if (formattedText.error) {\n            if (showErrors) {\n              await showErrorMessage(\n                'Jupyterlab Code Formatter Error',\n                formattedText.error\n              );\n            }\n          } else {\n            cell.model.value.text = formattedText.code;\n          }\n        } else {\n          if (showErrors) {\n            await showErrorMessage(\n              'Jupyterlab Code Formatter Error',\n              `Cell value changed since format request was sent, formatting for cell ${i} skipped.`\n            );\n          }\n        }\n      }\n    }\n  }\n\n  private async formatCells(\n    selectedOnly: boolean,\n    config: any,\n    formatter?: string,\n    notebook?: Notebook\n  ) {\n    if (this.working) {\n      return;\n    }\n    try {\n      this.working = true;\n      const selectedCells = this.getCodeCells(selectedOnly, notebook);\n      if (selectedCells.length === 0) {\n        this.working = false;\n        return;\n      }\n\n      const formattersToUse = await this.getFormattersToUse(config, formatter);\n      await this.applyFormatters(selectedCells, formattersToUse, config);\n    } catch (error) {\n      await showErrorMessage('Jupyterlab Code Formatter Error', error);\n    }\n    this.working = false;\n  }\n\n  applicable(formatter: string, currentWidget: Widget) {\n    const currentNotebookWidget = this.notebookTracker.currentWidget;\n    // TODO: Handle showing just the correct formatter for the language later\n    return currentNotebookWidget && currentWidget === currentNotebookWidget;\n  }\n}\n\nexport class JupyterlabFileEditorCodeFormatter extends JupyterlabCodeFormatter {\n  protected editorTracker: IEditorTracker;\n\n  constructor(\n    client: JupyterlabCodeFormatterClient,\n    editorTracker: IEditorTracker\n  ) {\n    super(client);\n    this.editorTracker = editorTracker;\n  }\n\n  formatAction(config: any, formatter: string) {\n    if (this.working) {\n      return;\n    }\n    const editorWidget = this.editorTracker.currentWidget;\n    this.working = true;\n    const editor = editorWidget!.content.editor;\n    const code = editor.model.value.text;\n    this.formatCode(\n      [code],\n      formatter,\n      config[formatter],\n      false,\n      config.cacheFormatters\n    )\n      .then(data => {\n        if (data.code[0].error) {\n          void showErrorMessage(\n            'Jupyterlab Code Formatter Error',\n            data.code[0].error\n          );\n          this.working = false;\n          return;\n        }\n        this.editorTracker.currentWidget!.content.editor.model.value.text =\n          data.code[0].code;\n        this.working = false;\n      })\n      .catch(error => {\n        this.working = false;\n        void showErrorMessage('Jupyterlab Code Formatter Error', error);\n      });\n  }\n\n  applicable(formatter: string, currentWidget: Widget) {\n    const currentEditorWidget = this.editorTracker.currentWidget;\n    // TODO: Handle showing just the correct formatter for the language later\n    return currentEditorWidget && currentWidget === currentEditorWidget;\n  }\n}\n",
+        "import { Cell, CodeCell } from '@jupyterlab/cells';\nimport { INotebookTracker, Notebook } from '@jupyterlab/notebook';\nimport JupyterlabCodeFormatterClient from './client';\nimport { IEditorTracker } from '@jupyterlab/fileeditor';\nimport { Widget } from '@lumino/widgets';\nimport { showErrorMessage } from '@jupyterlab/apputils';\n\nclass JupyterlabCodeFormatter {\n  working = false;\n  protected client: JupyterlabCodeFormatterClient;\n  constructor(client: JupyterlabCodeFormatterClient) {\n    this.client = client;\n  }\n\n  protected formatCode(\n    code: string[],\n    formatter: string,\n    options: any,\n    notebook: boolean,\n    cache: boolean\n  ) {\n    return this.client\n      .request(\n        'format' + (cache ? '?cached' : ''),\n        'POST',\n        JSON.stringify({\n          code,\n          notebook,\n          formatter,\n          options\n        })\n      )\n      .then(resp => JSON.parse(resp));\n  }\n}\n\nexport class JupyterlabNotebookCodeFormatter extends JupyterlabCodeFormatter {\n  protected notebookTracker: INotebookTracker;\n\n  constructor(\n    client: JupyterlabCodeFormatterClient,\n    notebookTracker: INotebookTracker\n  ) {\n    super(client);\n    this.notebookTracker = notebookTracker;\n  }\n\n  public async formatAction(config: any, formatter?: string) {\n    return this.formatCells(true, config, formatter);\n  }\n\n  public async formatSelectedCodeCells(\n    config: any,\n    formatter?: string,\n    notebook?: Notebook\n  ) {\n    return this.formatCells(true, config, formatter, notebook);\n  }\n\n  public async formatAllCodeCells(\n    config: any,\n    formatter?: string,\n    notebook?: Notebook\n  ) {\n    return this.formatCells(false, config, formatter, notebook);\n  }\n\n  private getCodeCells(selectedOnly = true, notebook?: Notebook): CodeCell[] {\n    if (!this.notebookTracker.currentWidget) {\n      return [];\n    }\n    const codeCells: CodeCell[] = [];\n    notebook = notebook || this.notebookTracker.currentWidget.content;\n    notebook.widgets.forEach((cell: Cell) => {\n      if (cell.model.type === 'code') {\n        if (!selectedOnly || (<Notebook>notebook).isSelectedOrActive(cell)) {\n          codeCells.push(cell as CodeCell);\n        }\n      }\n    });\n    return codeCells;\n  }\n\n  private getNotebookType() {\n    if (!this.notebookTracker.currentWidget) {\n      return null;\n    }\n\n    const metadata =\n      this.notebookTracker.currentWidget.content.model!.sharedModel.metadata;;\n\n    if (!metadata) {\n      return null;\n    }\n\n    // prefer kernelspec language\n    // @ts-ignore\n    if (metadata.kernelspec && metadata.kernelspec.language) {\n      // @ts-ignore\n      return metadata.kernelspec.language.toLowerCase();\n    }\n\n    // otherwise, check language info code mirror mode\n    // @ts-ignore\n    if (metadata.language_info && metadata.language_info.codemirror_mode) {\n      // @ts-ignore\n      return metadata.language_info.codemirror_mode.name.toLowerCase();\n    }\n\n    return null;\n  }\n\n  private getDefaultFormatters(config: any): Array<string> {\n    const notebookType = this.getNotebookType();\n    if (notebookType) {\n      const defaultFormatter =\n        config.preferences.default_formatter[notebookType];\n      if (defaultFormatter instanceof Array) {\n        return defaultFormatter;\n      } else if (defaultFormatter !== undefined) {\n        return [defaultFormatter];\n      }\n    }\n    return [];\n  }\n\n  private async getFormattersToUse(config: any, formatter?: string) {\n    const defaultFormatters = this.getDefaultFormatters(config);\n    const formattersToUse =\n      formatter !== undefined ? [formatter] : defaultFormatters;\n\n    if (formattersToUse.length === 0) {\n      await showErrorMessage(\n        'Jupyterlab Code Formatter Error',\n        'Unable to find default formatters to use, please file an issue on GitHub.'\n      );\n    }\n\n    return formattersToUse;\n  }\n\n  private async applyFormatters(\n    selectedCells: CodeCell[],\n    formattersToUse: string[],\n    config: any\n  ) {\n    for (const formatterToUse of formattersToUse) {\n      if (formatterToUse === 'noop' || formatterToUse === 'skip') {\n        continue;\n      }\n      const currentTexts = selectedCells.map(cell => cell.model.sharedModel.source);\n      const formattedTexts = await this.formatCode(\n        currentTexts,\n        formatterToUse,\n        config[formatterToUse],\n        true,\n        config.cacheFormatters\n      );\n\n      const showErrors = !(config.suppressFormatterErrors ?? false);\n      for (let i = 0; i < selectedCells.length; ++i) {\n        const cell = selectedCells[i];\n        const currentText = currentTexts[i];\n        const formattedText = formattedTexts.code[i];\n        const cellValueHasNotChanged = cell.model.sharedModel.source === currentText;\n        if (cellValueHasNotChanged) {\n          if (formattedText.error) {\n            if (showErrors) {\n              await showErrorMessage(\n                'Jupyterlab Code Formatter Error',\n                formattedText.error\n              );\n            }\n          } else {\n            cell.model.sharedModel.source = formattedText.code;\n          }\n        } else {\n          if (showErrors) {\n            await showErrorMessage(\n              'Jupyterlab Code Formatter Error',\n              `Cell value changed since format request was sent, formatting for cell ${i} skipped.`\n            );\n          }\n        }\n      }\n    }\n  }\n\n  private async formatCells(\n    selectedOnly: boolean,\n    config: any,\n    formatter?: string,\n    notebook?: Notebook\n  ) {\n    if (this.working) {\n      return;\n    }\n    try {\n      this.working = true;\n      const selectedCells = this.getCodeCells(selectedOnly, notebook);\n      if (selectedCells.length === 0) {\n        this.working = false;\n        return;\n      }\n\n      const formattersToUse = await this.getFormattersToUse(config, formatter);\n      await this.applyFormatters(selectedCells, formattersToUse, config);\n    } catch (error) {\n      await showErrorMessage('Jupyterlab Code Formatter Error', error);\n    }\n    this.working = false;\n  }\n\n  applicable(formatter: string, currentWidget: Widget) {\n    const currentNotebookWidget = this.notebookTracker.currentWidget;\n    // TODO: Handle showing just the correct formatter for the language later\n    return currentNotebookWidget && currentWidget === currentNotebookWidget;\n  }\n}\n\nexport class JupyterlabFileEditorCodeFormatter extends JupyterlabCodeFormatter {\n  protected editorTracker: IEditorTracker;\n\n  constructor(\n    client: JupyterlabCodeFormatterClient,\n    editorTracker: IEditorTracker\n  ) {\n    super(client);\n    this.editorTracker = editorTracker;\n  }\n\n  formatAction(config: any, formatter: string) {\n    if (this.working) {\n      return;\n    }\n    const editorWidget = this.editorTracker.currentWidget;\n    this.working = true;\n    const editor = editorWidget!.content.editor;\n    const code = editor.model.sharedModel.source;\n    this.formatCode(\n      [code],\n      formatter,\n      config[formatter],\n      false,\n      config.cacheFormatters\n    )\n      .then(data => {\n        if (data.code[0].error) {\n          void showErrorMessage(\n            'Jupyterlab Code Formatter Error',\n            data.code[0].error\n          );\n          this.working = false;\n          return;\n        }\n        this.editorTracker.currentWidget!.content.editor.model.sharedModel.source =\n          data.code[0].code;\n        this.working = false;\n      })\n      .catch(error => {\n        this.working = false;\n        void showErrorMessage('Jupyterlab Code Formatter Error', error);\n      });\n  }\n\n  applicable(formatter: string, currentWidget: Widget) {\n    const currentEditorWidget = this.editorTracker.currentWidget;\n    // TODO: Handle showing just the correct formatter for the language later\n    return currentEditorWidget && currentWidget === currentEditorWidget;\n  }\n}\n",
         "import { DocumentRegistry } from '@jupyterlab/docregistry';\nimport {\n  INotebookModel,\n  INotebookTracker,\n  NotebookPanel\n} from '@jupyterlab/notebook';\nimport {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\nimport { ICommandPalette, ToolbarButton } from '@jupyterlab/apputils';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IEditorTracker } from '@jupyterlab/fileeditor';\nimport JupyterlabCodeFormatterClient from './client';\nimport {\n  JupyterlabFileEditorCodeFormatter,\n  JupyterlabNotebookCodeFormatter\n} from './formatter';\nimport { DisposableDelegate, IDisposable } from '@lumino/disposable';\nimport { Constants } from './constants';\nimport { LabIcon } from '@jupyterlab/ui-components';\nimport { Widget } from '@lumino/widgets';\n\nclass JupyterLabCodeFormatter\n  implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>\n{\n  private app: JupyterFrontEnd;\n  private readonly tracker: INotebookTracker;\n  private palette: ICommandPalette;\n  private settingRegistry: ISettingRegistry;\n  private menu: IMainMenu;\n  private config: any;\n  private readonly editorTracker: IEditorTracker;\n  private readonly client: JupyterlabCodeFormatterClient;\n  private readonly notebookCodeFormatter: JupyterlabNotebookCodeFormatter;\n  private readonly fileEditorCodeFormatter: JupyterlabFileEditorCodeFormatter;\n\n  constructor(\n    app: JupyterFrontEnd,\n    tracker: INotebookTracker,\n    palette: ICommandPalette,\n    settingRegistry: ISettingRegistry,\n    menu: IMainMenu,\n    editorTracker: IEditorTracker\n  ) {\n    this.app = app;\n    this.tracker = tracker;\n    this.editorTracker = editorTracker;\n    this.palette = palette;\n    this.settingRegistry = settingRegistry;\n    this.menu = menu;\n    this.client = new JupyterlabCodeFormatterClient();\n    this.notebookCodeFormatter = new JupyterlabNotebookCodeFormatter(\n      this.client,\n      this.tracker\n    );\n    this.fileEditorCodeFormatter = new JupyterlabFileEditorCodeFormatter(\n      this.client,\n      this.editorTracker\n    );\n\n    this.setupSettings().then(() => {\n      this.setupAllCommands();\n      this.setupContextMenu();\n      this.setupWidgetExtension();\n    });\n    console.log('222wat');\n  }\n\n  public createNew(\n    nb: NotebookPanel,\n    context: DocumentRegistry.IContext<INotebookModel>\n  ): IDisposable {\n    const button = new ToolbarButton({\n      tooltip: 'Format notebook',\n      icon: new LabIcon({\n        name: Constants.FORMAT_ALL_COMMAND,\n        svgstr: Constants.ICON_FORMAT_ALL_SVG\n      }),\n      onClick: async () => {\n        await this.notebookCodeFormatter.formatAllCodeCells(\n          this.config,\n          undefined,\n          nb.content\n        );\n      }\n    });\n    nb.toolbar.insertAfter(\n      'cellType',\n      this.app.commands.label(Constants.FORMAT_ALL_COMMAND),\n      button\n    );\n\n    context.saveState.connect(this.onSave, this);\n\n    return new DisposableDelegate(() => {\n      button.dispose();\n    });\n  }\n\n  private async onSave(\n    context: DocumentRegistry.IContext<INotebookModel>,\n    state: DocumentRegistry.SaveState\n  ) {\n    if (state === 'started' && this.config.formatOnSave) {\n      await this.notebookCodeFormatter.formatAllCodeCells(this.config);\n    }\n  }\n\n  private setupWidgetExtension() {\n    this.app.docRegistry.addWidgetExtension('Notebook', this);\n  }\n\n  private setupContextMenu() {\n    this.app.contextMenu.addItem({\n      command: Constants.FORMAT_COMMAND,\n      selector: '.jp-Notebook'\n    });\n  }\n\n  private setupAllCommands() {\n    this.client\n      .getAvailableFormatters(this.config.cacheFormatters)\n      .then(data => {\n        const formatters = JSON.parse(data).formatters;\n        const menuGroup: Array<{ command: string }> = [];\n        Object.keys(formatters).forEach(formatter => {\n          if (formatters[formatter].enabled) {\n            const command = `${Constants.PLUGIN_NAME}:${formatter}`;\n            this.setupCommand(formatter, formatters[formatter].label, command);\n            menuGroup.push({ command });\n          }\n        });\n        this.menu.editMenu.addGroup(menuGroup);\n      });\n\n    this.app.commands.addCommand(Constants.FORMAT_COMMAND, {\n      execute: async () => {\n        await this.notebookCodeFormatter.formatSelectedCodeCells(this.config);\n      },\n      // TODO: Add back isVisible\n      label: 'Format cell'\n    });\n    this.app.commands.addCommand(Constants.FORMAT_ALL_COMMAND, {\n      execute: async () => {\n        await this.notebookCodeFormatter.formatAllCodeCells(this.config);\n      },\n      iconClass: Constants.ICON_FORMAT_ALL,\n      iconLabel: 'Format notebook'\n      // TODO: Add back isVisible\n    });\n  }\n\n  private async setupSettings() {\n    const settings = await this.settingRegistry.load(\n      Constants.SETTINGS_SECTION\n    );\n    const onSettingsUpdated = (jsettings: ISettingRegistry.ISettings) => {\n      this.config = jsettings.composite;\n    };\n    settings.changed.connect(onSettingsUpdated);\n    onSettingsUpdated(settings);\n  }\n\n  private setupCommand(name: string, label: string, command: string) {\n    this.app.commands.addCommand(command, {\n      execute: async () => {\n        for (const formatter of [\n          this.notebookCodeFormatter,\n          this.fileEditorCodeFormatter\n        ]) {\n          if (\n            formatter.applicable(name, <Widget>this.app.shell.currentWidget)\n          ) {\n            await formatter.formatAction(this.config, name);\n          }\n        }\n      },\n      isVisible: () => {\n        for (const formatter of [\n          this.notebookCodeFormatter,\n          this.fileEditorCodeFormatter\n        ]) {\n          if (\n            formatter.applicable(name, <Widget>this.app.shell.currentWidget)\n          ) {\n            return true;\n          }\n        }\n        return false;\n      },\n      label\n    });\n    this.palette.addItem({ command, category: Constants.COMMAND_SECTION_NAME });\n  }\n}\n\n/**\n * Initialization data for the jupyterlab_code_formatter extension.\n */\nconst plugin: JupyterFrontEndPlugin<void> = {\n  id: Constants.PLUGIN_NAME,\n  autoStart: true,\n  requires: [\n    ICommandPalette,\n    INotebookTracker,\n    ISettingRegistry,\n    IMainMenu,\n    IEditorTracker\n  ],\n  activate: (\n    app: JupyterFrontEnd,\n    palette: ICommandPalette,\n    tracker: INotebookTracker,\n    settingRegistry: ISettingRegistry,\n    menu: IMainMenu,\n    editorTracker: IEditorTracker\n  ) => {\n    new JupyterLabCodeFormatter(\n      app,\n      tracker,\n      palette,\n      settingRegistry,\n      menu,\n      editorTracker\n    );\n    console.log('JupyterLab extension jupyterlab_code_formatter is activated!');\n  }\n};\n\nexport default plugin;\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/remoteEntry.26ea8ddf38b373b61cfc.js` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/remoteEntry.401d3ea4715fec19e0e1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "7fcef9ea39c2b4846c2b",
+                "lib_index_js": "7aa378f926383c6ad3f0",
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "e47ec9bcc4e2b2cf64ff",
                 "style_index_js": "1e55589b5efea822f161"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
@@ -427,15 +427,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab_code_formatter", "2.0.0-rc1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab_code_formatter", "2.0.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1104,8 +1104,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab_code_formatter");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyterlab_code_formatter = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.26ea8ddf38b373b61cfc.js.map
+//# sourceMappingURL=remoteEntry.401d3ea4715fec19e0e1.js.map
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/remoteEntry.26ea8ddf38b373b61cfc.js.map` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/remoteEntry.401d3ea4715fec19e0e1.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.401d3ea4715fec19e0e1.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"7aa378f926383c6ad3f0","vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1":"e47ec9bcc4e2b2cf64ff","style_index […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.26ea8ddf38b373b61cfc.js",
+    "file": "remoteEntry.401d3ea4715fec19e0e1.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC1LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_code_formatter/webpack/container-entry",
         "webpack://jupyterlab_code_formatter/webpack/bootstrap",
         "webpack://jupyterlab_code_formatter/webpack/runtime/compat get default export",
@@ -25,20 +25,20 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"7fcef9ea39c2b4846c2b\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"e47ec9bcc4e2b2cf64ff\",\"style_index_js\":\"1e55589b5efea822f161\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"7aa378f926383c6ad3f0\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"e47ec9bcc4e2b2cf64ff\",\"style_index_js\":\"1e55589b5efea822f161\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_code_formatter:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab_code_formatter\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_code_formatter\", \"2.0.0-rc1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab_code_formatter\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_code_formatter\", \"2.0.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/fileeditor\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,6,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\",\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_code_formatter\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_code_formatter\"] = self[\"webpackChunkjupyterlab_code_formatter\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab_code_formatter\");\n",
         ""
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js.map` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/style_index_js.1e55589b5efea822f161.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js.map` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.e47ec9bcc4e2b2cf64ff.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/tests/conftest.py` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/jupyterlab_code_formatter/tests/test_handlers.py` & `jupyterlab_code_formatter-2.1.0rc0/jupyterlab_code_formatter/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/schema/settings.json` & `jupyterlab_code_formatter-2.1.0rc0/schema/settings.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/src/client.ts` & `jupyterlab_code_formatter-2.1.0rc0/src/client.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/src/constants.ts` & `jupyterlab_code_formatter-2.1.0rc0/src/constants.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/src/formatter.ts` & `jupyterlab_code_formatter-2.1.0rc0/src/formatter.ts`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
   private getNotebookType() {
     if (!this.notebookTracker.currentWidget) {
       return null;
     }
 
     const metadata =
-      this.notebookTracker.currentWidget.content.model!.metadata.toJSON();
+      this.notebookTracker.currentWidget.content.model!.sharedModel.metadata;;
 
     if (!metadata) {
       return null;
     }
 
     // prefer kernelspec language
     // @ts-ignore
@@ -144,39 +144,39 @@
     formattersToUse: string[],
     config: any
   ) {
     for (const formatterToUse of formattersToUse) {
       if (formatterToUse === 'noop' || formatterToUse === 'skip') {
         continue;
       }
-      const currentTexts = selectedCells.map(cell => cell.model.value.text);
+      const currentTexts = selectedCells.map(cell => cell.model.sharedModel.source);
       const formattedTexts = await this.formatCode(
         currentTexts,
         formatterToUse,
         config[formatterToUse],
         true,
         config.cacheFormatters
       );
 
       const showErrors = !(config.suppressFormatterErrors ?? false);
       for (let i = 0; i < selectedCells.length; ++i) {
         const cell = selectedCells[i];
         const currentText = currentTexts[i];
         const formattedText = formattedTexts.code[i];
-        const cellValueHasNotChanged = cell.model.value.text === currentText;
+        const cellValueHasNotChanged = cell.model.sharedModel.source === currentText;
         if (cellValueHasNotChanged) {
           if (formattedText.error) {
             if (showErrors) {
               await showErrorMessage(
                 'Jupyterlab Code Formatter Error',
                 formattedText.error
               );
             }
           } else {
-            cell.model.value.text = formattedText.code;
+            cell.model.sharedModel.source = formattedText.code;
           }
         } else {
           if (showErrors) {
             await showErrorMessage(
               'Jupyterlab Code Formatter Error',
               `Cell value changed since format request was sent, formatting for cell ${i} skipped.`
             );
@@ -232,15 +232,15 @@
   formatAction(config: any, formatter: string) {
     if (this.working) {
       return;
     }
     const editorWidget = this.editorTracker.currentWidget;
     this.working = true;
     const editor = editorWidget!.content.editor;
-    const code = editor.model.value.text;
+    const code = editor.model.sharedModel.source;
     this.formatCode(
       [code],
       formatter,
       config[formatter],
       false,
       config.cacheFormatters
     )
@@ -249,15 +249,15 @@
           void showErrorMessage(
             'Jupyterlab Code Formatter Error',
             data.code[0].error
           );
           this.working = false;
           return;
         }
-        this.editorTracker.currentWidget!.content.editor.model.value.text =
+        this.editorTracker.currentWidget!.content.editor.model.sharedModel.source =
           data.code[0].code;
         this.working = false;
       })
       .catch(error => {
         this.working = false;
         void showErrorMessage('Jupyterlab Code Formatter Error', error);
       });
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/src/index.ts` & `jupyterlab_code_formatter-2.1.0rc0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/test_snippets/some_python.py` & `jupyterlab_code_formatter-2.1.0rc0/test_snippets/some_python.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/test_snippets/test_notebook.ipynb` & `jupyterlab_code_formatter-2.1.0rc0/test_snippets/test_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/test_snippets/test_notebook_crablang.ipynb` & `jupyterlab_code_formatter-2.1.0rc0/test_snippets/test_notebook_crablang.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/ui-tests/README.md` & `jupyterlab_code_formatter-2.1.0rc0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/ui-tests/jupyter_server_test_config.py` & `jupyterlab_code_formatter-2.1.0rc0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/ui-tests/tests/jupyterlab_code_formatter.spec.ts` & `jupyterlab_code_formatter-2.1.0rc0/ui-tests/tests/jupyterlab_code_formatter.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/.gitignore` & `jupyterlab_code_formatter-2.1.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/LICENSE` & `jupyterlab_code_formatter-2.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/README.md` & `jupyterlab_code_formatter-2.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-2.0.0rc2/pyproject.toml` & `jupyterlab_code_formatter-2.1.0rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.4.0", "jupyterlab>=3.4.7,<4.0.0", "hatch-nodejs-version"]
+requires = ["hatchling>=1.4.0", "jupyterlab>=3.6,<5", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_code_formatter"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
@@ -48,22 +48,18 @@
     "pytest-cov",
     "pytest-jupyter[server]>=0.6.0",
     "black==22.1.0",
     "blue==0.9.1",
     "isort",
     "yapf",
 ]
-docs = [
-    "furo",
-    "sphinx"
-]
 
 [tool.hatch.envs.default]
 type = "pip-deepfreeze"
-features = ["dev", "test", "docs"]
+features = ["dev", "test"]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
```

### Comparing `jupyterlab_code_formatter-2.0.0rc2/PKG-INFO` & `jupyterlab_code_formatter-2.1.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_code_formatter
-Version: 2.0.0rc2
+Version: 2.1.0rc0
 Summary:  A JupyterLab plugin to facilitate invocation of code formatters.
 Project-URL: Homepage,  https://github.com/ryantam626/jupyterlab_code_formatter
 Project-URL: Bug Tracker,  https://github.com/ryantam626/jupyterlab_code_formatter/issues
 Project-URL: Repository,  https://github.com/ryantam626/jupyterlab_code_formatter.git
 Author-email: Ryan Tam <ryantam626@gmail.com>
 License: Copyright 2023 Ryan TAM
         
@@ -36,17 +36,14 @@
 Requires-Dist: blue==0.9.1; extra == 'dev'
 Requires-Dist: click==8.0.2; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: jupyterlab>=3.0.0; extra == 'dev'
 Requires-Dist: rpy2; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: yapf; extra == 'dev'
-Provides-Extra: docs
-Requires-Dist: furo; extra == 'docs'
-Requires-Dist: sphinx; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: black==22.1.0; extra == 'test'
 Requires-Dist: blue==0.9.1; extra == 'test'
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: isort; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
```

