# Comparing `tmp/steamship-2.3.8.tar.gz` & `tmp/steamship-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamship-2.3.8.tar", last modified: Wed Jan 25 19:38:20 2023, max compression
+gzip compressed data, was "steamship-2.3.9.tar", last modified: Wed Jan 25 21:13:28 2023, max compression
```

## Comparing `steamship-2.3.8.tar` & `steamship-2.3.9.tar`

### file list

```diff
@@ -1,406 +1,407 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.742363 steamship-2.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.690359 steamship-2.3.8/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/base.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.694360 steamship-2.3.8/.devcontainer/library-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/library-scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    18654 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/library-scripts/common-debian.sh
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/library-scripts/meta.env
--rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/library-scripts/node-debian.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    14982 2023-01-25 19:38:02.000000 steamship-2.3.8/.devcontainer/library-scripts/python-debian.sh
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-25 19:38:02.000000 steamship-2.3.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.682359 steamship-2.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.694360 steamship-2.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-25 19:38:02.000000 steamship-2.3.8/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-25 19:38:02.000000 steamship-2.3.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-25 19:38:02.000000 steamship-2.3.8/.github/workflows/test-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-25 19:38:02.000000 steamship-2.3.8/.github/workflows/test-staging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-25 19:38:02.000000 steamship-2.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-01-25 19:38:02.000000 steamship-2.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-25 19:38:02.000000 steamship-2.3.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-25 19:38:02.000000 steamship-2.3.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-01-25 19:38:02.000000 steamship-2.3.8/DEVELOPING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-25 19:38:02.000000 steamship-2.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-25 19:38:20.742363 steamship-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-25 19:38:02.000000 steamship-2.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-01-25 19:38:02.000000 steamship-2.3.8/TESTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.694360 steamship-2.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.694360 steamship-2.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/_static/Steamship-symbol-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/_static/Steamship-symbol-light.png
--rw-r--r--   0 runner    (1001) docker     (123)   227249 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.694360 steamship-2.3.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/_templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.698360 steamship-2.3.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.invocable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.plugin.blockifier.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.plugin.inputs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.plugin.outputs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/api/steamship.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/changelog._rst
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.698360 steamship-2.3.8/docs/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/configuration/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/configuration/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/configuration/clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/configuration/http.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/configuration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.698360 steamship-2.3.8/docs/developing/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/deploying.rst
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/environment-setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/project-creation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/steamship-manifest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/storing-secrets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/developing/updating-web-listing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.698360 steamship-2.3.8/docs/packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/packages/cookbook/
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/adding-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/article-tagging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/collecting-and-querying-sentiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/modifying-an-existing-package.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/receiving-webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/return-audio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/return-image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/return-json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/cookbook/return-text.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/packages/developing/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/developing/project-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/packages/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/plugins/blockifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/blockifiers/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/blockifiers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/blockifiers/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/plugins/developing/
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/developing/async-plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/developing/blockifiers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/developing/embedders.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/developing/importers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/developing/project-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/developing/taggers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/plugins/embedders/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/embedders/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/embedders/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/plugins/importers/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/importers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/importers/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.702360 steamship-2.3.8/docs/plugins/taggers/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/taggers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/plugins/taggers/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.706361 steamship-2.3.8/docs/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/blockifying.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/creating.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.706361 steamship-2.3.8/docs/workspaces/data_model/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/data_model/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/data_model/files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/data_model/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/data_model/tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/importing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.706361 steamship-2.3.8/docs/workspaces/queries/
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-01-25 19:38:02.000000 steamship-2.3.8/docs/workspaces/queries/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-25 19:38:02.000000 steamship-2.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-25 19:38:02.000000 steamship-2.3.8/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-25 19:38:02.000000 steamship-2.3.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.706361 steamship-2.3.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-01-25 19:38:02.000000 steamship-2.3.8/scripts/build-docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-25 19:38:02.000000 steamship-2.3.8/scripts/create_engine_test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 19:38:20.742363 steamship-2.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.686359 steamship-2.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.706361 steamship-2.3.8/src/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.710361 steamship-2.3.8/src/steamship/base/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/package_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/request.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.710361 steamship-2.3.8/src/steamship/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/cli/manifest_init_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/cli/ship_spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.710361 steamship-2.3.8/src/steamship/client/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/client/skill_to_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/client/skills.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/client/steamship.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/client/vendors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.710361 steamship-2.3.8/src/steamship/data/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.710361 steamship-2.3.8/src/steamship/data/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/operations/blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/operations/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/operations/tagger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.714361 steamship-2.3.8/src/steamship/data/package/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/package/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/package/package_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/package/package_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.714361 steamship-2.3.8/src/steamship/data/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/plugin/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/plugin/index_plugin_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/plugin/plugin_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/plugin/plugin_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/plugin/prompt_generation_plugin_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.714361 steamship-2.3.8/src/steamship/data/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/tags/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/tags/tag_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/data/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.714361 steamship-2.3.8/src/steamship/invocable/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/invocable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/invocable_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/invocable_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/package_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/paramater_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/invocable/plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.718362 steamship-2.3.8/src/steamship/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.718362 steamship-2.3.8/src/steamship/plugin/blockifier/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/blockifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/blockifier/blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/blockifier/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/file_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.718362 steamship-2.3.8/src/steamship/plugin/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/inputs/block_and_tag_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/inputs/export_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/inputs/file_import_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/inputs/raw_data_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/inputs/train_plugin_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/inputs/training_parameter_plugin_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.718362 steamship-2.3.8/src/steamship/plugin/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/outputs/block_and_tag_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/outputs/embedded_items_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/outputs/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/outputs/raw_data_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/outputs/train_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/outputs/training_parameter_plugin_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/plugin/trainable_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.722362 steamship-2.3.8/src/steamship/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/huggingface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/kv_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/signed_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-25 19:38:02.000000 steamship-2.3.8/src/steamship/utils/zip_archives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.706361 steamship-2.3.8/src/steamship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-25 19:38:20.000000 steamship-2.3.8/src/steamship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-01-25 19:38:20.000000 steamship-2.3.8/src/steamship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 19:38:20.000000 steamship-2.3.8/src/steamship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-25 19:38:20.000000 steamship-2.3.8/src/steamship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-25 19:38:20.000000 steamship-2.3.8/src/steamship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-25 19:38:20.000000 steamship-2.3.8/src/steamship.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.722362 steamship-2.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.722362 steamship-2.3.8/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.722362 steamship-2.3.8/tests/assets/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/configs/empty_json.json
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/configs/one_string_one_int.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/configs/single_integer.json
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/demo_package_spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.722362 steamship-2.3.8/tests/assets/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/bad_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/configurable_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/demo_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/fancy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/optional_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/returns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/safe_loaded_bad_import.pyignore
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/safe_loaded_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/packages/signed_url_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/palm_tree.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.722362 steamship-2.3.8/tests/assets/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.726362 steamship-2.3.8/tests/assets/plugins/blockifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/blockifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/blockifiers/async_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/blockifiers/blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/blockifiers/csv_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/blockifiers/tsv_blockifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.726362 steamship-2.3.8/tests/assets/plugins/importers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer_by_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer_python_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.726362 steamship-2.3.8/tests/assets/plugins/taggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_configurable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_logging_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/utterances.csv
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/assets/utterances.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.726362 steamship-2.3.8/tests/steamship_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.726362 steamship-2.3.8/tests/steamship_tests/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.730363 steamship-2.3.8/tests/steamship_tests/app/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_configurable_package_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_package_error_visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_package_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_returns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_safe_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_signed_url_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/integration/test_use_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.730363 steamship-2.3.8/tests/steamship_tests/app/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/unit/test_config_template_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/unit/test_demo_app_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/unit/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/app/unit/test_training_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.730363 steamship-2.3.8/tests/steamship_tests/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/base/test_binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/base/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/base/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/base/test_steamship_error_serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/base/test_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.730363 steamship-2.3.8/tests/steamship_tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.734363 steamship-2.3.8/tests/steamship_tests/client/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_blockify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_convert_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_embed_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_embedding_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_embedding_index_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/operations/test_tag_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/client/test_task_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.734363 steamship-2.3.8/tests/steamship_tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.734363 steamship-2.3.8/tests/steamship_tests/data/tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/tags/test_file_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_app_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_img.png
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_task_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/test_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/data/utterances.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.734363 steamship-2.3.8/tests/steamship_tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.738363 steamship-2.3.8/tests/steamship_tests/plugin/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_corpus_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_use_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/integration/test_use_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.738363 steamship-2.3.8/tests/steamship_tests/plugin/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_blockifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_config_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_file_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_response_post_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_trainable_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.738363 steamship-2.3.8/tests/steamship_tests/plugin/unit/trainable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/trainable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/plugin/unit/trainable/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.738363 steamship-2.3.8/tests/steamship_tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/server/test_package_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/server/test_task_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 19:38:20.742363 steamship-2.3.8/tests/steamship_tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/deployables.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/test_camel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/test_kv_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/test_signed_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/test_static_instance_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-01-25 19:38:02.000000 steamship-2.3.8/tests/steamship_tests/utils/test_zip_archives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.293581 steamship-2.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.253581 steamship-2.3.9/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/base.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/.devcontainer/library-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18654 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/common-debian.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/meta.env
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/node-debian.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14982 2023-01-25 21:13:15.000000 steamship-2.3.9/.devcontainer/library-scripts/python-debian.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-25 21:13:15.000000 steamship-2.3.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.249581 steamship-2.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/test-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-25 21:13:15.000000 steamship-2.3.9/.github/workflows/test-staging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-25 21:13:15.000000 steamship-2.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-01-25 21:13:15.000000 steamship-2.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-25 21:13:15.000000 steamship-2.3.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-25 21:13:15.000000 steamship-2.3.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-01-25 21:13:15.000000 steamship-2.3.9/DEVELOPING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-25 21:13:15.000000 steamship-2.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-25 21:13:28.293581 steamship-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-25 21:13:15.000000 steamship-2.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-01-25 21:13:15.000000 steamship-2.3.9/TESTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/Steamship-symbol-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/Steamship-symbol-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   227249 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.257581 steamship-2.3.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/_templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.invocable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.blockifier.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.inputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.outputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/api/steamship.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/changelog._rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/http.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/configuration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/developing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/deploying.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/environment-setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/project-creation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/steamship-manifest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/storing-secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/developing/updating-web-listing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/packages/cookbook/
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/adding-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/article-tagging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/collecting-and-querying-sentiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/modifying-an-existing-package.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/receiving-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-audio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/cookbook/return-text.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/packages/developing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/developing/project-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/packages/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.261581 steamship-2.3.9/docs/plugins/blockifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/blockifiers/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/blockifiers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/blockifiers/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/developing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/async-plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/blockifiers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/embedders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/importers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/project-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/developing/taggers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/embedders/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/embedders/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/embedders/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/importers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/importers/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/plugins/taggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/taggers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/plugins/taggers/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/blockifying.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/creating.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/workspaces/data_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/data_model/tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/importing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/docs/workspaces/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-01-25 21:13:15.000000 steamship-2.3.9/docs/workspaces/queries/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-25 21:13:15.000000 steamship-2.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-25 21:13:15.000000 steamship-2.3.9/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-25 21:13:15.000000 steamship-2.3.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-01-25 21:13:15.000000 steamship-2.3.9/scripts/build-docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-25 21:13:15.000000 steamship-2.3.9/scripts/create_engine_test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 21:13:28.293581 steamship-2.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.249581 steamship-2.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/src/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/package_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/manifest_init_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/cli/ship_spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/skill_to_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/skills.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/steamship.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/client/vendors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/data/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/operations/tagger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.269581 steamship-2.3.9/src/steamship/data/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/package_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/package/package_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/data/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/index_plugin_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/plugin_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/plugin/prompt_generation_plugin_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/data/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/tags/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/tags/tag_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/data/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/invocable/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/invocable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/invocable_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/invocable_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/package_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/paramater_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/invocable/plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/plugin/blockifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/blockifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/blockifier/blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/blockifier/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/file_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.273581 steamship-2.3.9/src/steamship/plugin/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/block_and_tag_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/export_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/file_import_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/raw_data_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/train_plugin_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/inputs/training_parameter_plugin_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/src/steamship/plugin/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/block_and_tag_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/embedded_items_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/raw_data_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/train_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/outputs/training_parameter_plugin_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/plugin/trainable_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/src/steamship/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/huggingface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/kv_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/signed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-25 21:13:15.000000 steamship-2.3.9/src/steamship/utils/zip_archives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.265581 steamship-2.3.9/src/steamship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-25 21:13:28.000000 steamship-2.3.9/src/steamship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/configs/empty_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/configs/one_string_one_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/configs/single_integer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/demo_package_spec.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/bad_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/configurable_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/demo_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/fancy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/optional_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/returns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/safe_loaded_bad_import.pyignore
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/safe_loaded_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/packages/signed_url_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/palm_tree.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.277581 steamship-2.3.9/tests/assets/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/assets/plugins/blockifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/async_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/csv_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/blockifiers/tsv_blockifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/assets/plugins/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_by_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_python_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/assets/plugins/taggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_configurable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_logging_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/utterances.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/assets/utterances.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/app/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_configurable_package_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_package_error_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_package_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_returns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_safe_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_signed_url_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/integration/test_use_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.281581 steamship-2.3.9/tests/steamship_tests/app/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_config_template_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_demo_app_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/app/unit/test_training_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_steamship_error_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/base/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/client/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_blockify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_convert_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embedding_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_embedding_index_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/operations/test_tag_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/client/test_task_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/data/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/tags/test_file_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_app_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_img.png
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_task_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/test_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/data/utterances.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.285581 steamship-2.3.9/tests/steamship_tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/plugin/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_corpus_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_use_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/integration/test_use_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/plugin/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_blockifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_config_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_file_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_response_post_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.289581 steamship-2.3.9/tests/steamship_tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/server/test_package_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/server/test_task_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 21:13:28.293581 steamship-2.3.9/tests/steamship_tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/deployables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_camel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_kv_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_signed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_static_instance_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-01-25 21:13:15.000000 steamship-2.3.9/tests/steamship_tests/utils/test_zip_archives.py
```

### Comparing `steamship-2.3.8/.devcontainer/Dockerfile` & `steamship-2.3.9/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.devcontainer/base.Dockerfile` & `steamship-2.3.9/.devcontainer/base.Dockerfile`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.devcontainer/devcontainer.json` & `steamship-2.3.9/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.devcontainer/library-scripts/common-debian.sh` & `steamship-2.3.9/.devcontainer/library-scripts/common-debian.sh`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.devcontainer/library-scripts/node-debian.sh` & `steamship-2.3.9/.devcontainer/library-scripts/node-debian.sh`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.devcontainer/library-scripts/python-debian.sh` & `steamship-2.3.9/.devcontainer/library-scripts/python-debian.sh`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.github/workflows/docs-publish.yml` & `steamship-2.3.9/.github/workflows/docs-publish.yml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.github/workflows/python-publish.yml` & `steamship-2.3.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.github/workflows/test-main.yml` & `steamship-2.3.9/.github/workflows/test-main.yml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.github/workflows/test-staging.yml` & `steamship-2.3.9/.github/workflows/test-staging.yml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.gitignore` & `steamship-2.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/.pre-commit-config.yaml` & `steamship-2.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/DEVELOPING.md` & `steamship-2.3.9/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/LICENSE` & `steamship-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/TESTING.md` & `steamship-2.3.9/TESTING.md`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/Makefile` & `steamship-2.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/README.txt` & `steamship-2.3.9/docs/README.txt`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/_static/Steamship-symbol-dark.png` & `steamship-2.3.9/docs/_static/Steamship-symbol-dark.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/_static/Steamship-symbol-light.png` & `steamship-2.3.9/docs/_static/Steamship-symbol-light.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/_static/favicon.ico` & `steamship-2.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/_templates/base.html` & `steamship-2.3.9/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.base.rst` & `steamship-2.3.9/docs/api/steamship.base.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.client.rst` & `steamship-2.3.9/docs/api/steamship.client.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.invocable.rst` & `steamship-2.3.9/docs/api/steamship.invocable.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.plugin.blockifier.rst` & `steamship-2.3.9/docs/api/steamship.plugin.blockifier.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.plugin.inputs.rst` & `steamship-2.3.9/docs/api/steamship.plugin.inputs.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.plugin.outputs.rst` & `steamship-2.3.9/docs/api/steamship.plugin.outputs.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.plugin.rst` & `steamship-2.3.9/docs/api/steamship.plugin.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/api/steamship.utils.rst` & `steamship-2.3.9/docs/api/steamship.utils.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/conf.py` & `steamship-2.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/configuration/authentication.rst` & `steamship-2.3.9/docs/configuration/authentication.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/configuration/clients.rst` & `steamship-2.3.9/docs/configuration/clients.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/configuration/http.rst` & `steamship-2.3.9/docs/configuration/http.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/configuration.rst` & `steamship-2.3.9/docs/developing/configuration.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/deploying.rst` & `steamship-2.3.9/docs/developing/deploying.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/environment-setup.rst` & `steamship-2.3.9/docs/developing/environment-setup.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/index.rst` & `steamship-2.3.9/docs/developing/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/project-creation.rst` & `steamship-2.3.9/docs/developing/project-creation.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/steamship-manifest.rst` & `steamship-2.3.9/docs/developing/steamship-manifest.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/storing-secrets.rst` & `steamship-2.3.9/docs/developing/storing-secrets.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/testing.rst` & `steamship-2.3.9/docs/developing/testing.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/developing/updating-web-listing.rst` & `steamship-2.3.9/docs/developing/updating-web-listing.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/index.rst` & `steamship-2.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/adding-configuration.rst` & `steamship-2.3.9/docs/packages/cookbook/adding-configuration.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/article-tagging.rst` & `steamship-2.3.9/docs/packages/cookbook/article-tagging.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/collecting-and-querying-sentiment.rst` & `steamship-2.3.9/docs/packages/cookbook/collecting-and-querying-sentiment.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst` & `steamship-2.3.9/docs/packages/cookbook/how-to-extract-outline-from-markdown.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/index.rst` & `steamship-2.3.9/docs/packages/cookbook/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/modifying-an-existing-package.rst` & `steamship-2.3.9/docs/packages/cookbook/modifying-an-existing-package.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/receiving-webhooks.rst` & `steamship-2.3.9/docs/packages/cookbook/receiving-webhooks.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/return-audio.rst` & `steamship-2.3.9/docs/packages/cookbook/return-audio.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/return-image.rst` & `steamship-2.3.9/docs/packages/cookbook/return-image.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/return-json.rst` & `steamship-2.3.9/docs/packages/cookbook/return-json.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/cookbook/return-text.rst` & `steamship-2.3.9/docs/packages/cookbook/return-text.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/developing/index.rst` & `steamship-2.3.9/docs/packages/developing/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/developing/project-structure.rst` & `steamship-2.3.9/docs/packages/developing/project-structure.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/index.rst` & `steamship-2.3.9/docs/packages/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/packages/using.rst` & `steamship-2.3.9/docs/packages/using.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/blockifiers/developing.rst` & `steamship-2.3.9/docs/plugins/blockifiers/developing.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/blockifiers/index.rst` & `steamship-2.3.9/docs/plugins/blockifiers/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/blockifiers/using.rst` & `steamship-2.3.9/docs/plugins/blockifiers/using.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/developing/async-plugins.rst` & `steamship-2.3.9/docs/plugins/developing/async-plugins.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/developing/blockifiers.rst` & `steamship-2.3.9/docs/plugins/developing/blockifiers.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/developing/index.rst` & `steamship-2.3.9/docs/plugins/developing/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/developing/project-structure.rst` & `steamship-2.3.9/docs/plugins/developing/project-structure.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/importers/using.rst` & `steamship-2.3.9/docs/plugins/importers/using.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/index.rst` & `steamship-2.3.9/docs/plugins/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/plugins/taggers/using.rst` & `steamship-2.3.9/docs/plugins/taggers/using.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/blockifying.rst` & `steamship-2.3.9/docs/workspaces/blockifying.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/creating.rst` & `steamship-2.3.9/docs/workspaces/creating.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/data_model/blocks.rst` & `steamship-2.3.9/docs/workspaces/data_model/blocks.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/data_model/files.rst` & `steamship-2.3.9/docs/workspaces/data_model/files.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/data_model/index.rst` & `steamship-2.3.9/docs/workspaces/data_model/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/data_model/tags.rst` & `steamship-2.3.9/docs/workspaces/data_model/tags.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/importing.rst` & `steamship-2.3.9/docs/workspaces/importing.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/index.rst` & `steamship-2.3.9/docs/workspaces/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/docs/workspaces/queries/index.rst` & `steamship-2.3.9/docs/workspaces/queries/index.rst`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/pyproject.toml` & `steamship-2.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/requirements.dev.txt` & `steamship-2.3.9/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/scripts/create_engine_test_assets.py` & `steamship-2.3.9/scripts/create_engine_test_assets.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/__init__.py` & `steamship-2.3.9/src/steamship/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,23 @@
     dist_name = __name__
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
-from .base import Configuration, MimeTypes, SteamshipError, Task, TaskState
+from .base import (
+    Configuration,
+    MimeTypes,
+    RuntimeEnvironments,
+    SteamshipError,
+    Task,
+    TaskState,
+    check_environment,
+)
 from .data import (
     Block,
     DocTag,
     EmbeddingIndex,
     File,
     Package,
     PackageInstance,
@@ -38,12 +46,12 @@
     "Task",
     "TaskState",
     "Block",
     "Tag",
     "Workspace",
     "PluginInstance",
     "PluginVersion",
-    "SentimentTag",
-    "EmotionTag",
     "DocTag",
     "EmbeddingIndex",
+    "check_environment",
+    "RuntimeEnvironments",
 ]
```

### Comparing `steamship-2.3.8/src/steamship/base/client.py` & `steamship-2.3.9/src/steamship/base/client.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/base/configuration.py` & `steamship-2.3.9/src/steamship/base/configuration.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/base/error.py` & `steamship-2.3.9/src/steamship/base/error.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/base/mime_types.py` & `steamship-2.3.9/src/steamship/base/mime_types.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/base/model.py` & `steamship-2.3.9/src/steamship/base/model.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/base/package_spec.py` & `steamship-2.3.9/src/steamship/base/package_spec.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/base/tasks.py` & `steamship-2.3.9/src/steamship/base/tasks.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/cli/cli.py` & `steamship-2.3.9/src/steamship/cli/cli.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/cli/deploy.py` & `steamship-2.3.9/src/steamship/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/cli/login.py` & `steamship-2.3.9/src/steamship/cli/login.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/cli/manifest_init_wizard.py` & `steamship-2.3.9/src/steamship/cli/manifest_init_wizard.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/cli/ship_spinner.py` & `steamship-2.3.9/src/steamship/cli/ship_spinner.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/client/skill_to_provider.py` & `steamship-2.3.9/src/steamship/client/skill_to_provider.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/client/steamship.py` & `steamship-2.3.9/src/steamship/client/steamship.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         client = Steamship(**kwargs)
         temporary_handle = "temp-" + str(uuid.uuid4())
         client.switch_workspace(temporary_handle)
 
         # Safety check that we are now working form the new workspace.
         if client.config.workspace_handle != temporary_handle:
             raise SteamshipError(
-                message=f"Attempted to switch totemporary workspace {temporary_handle} but the client claimed to be working from {client.config.workspace_handle}"
+                message=f"Attempted to switch to temporary workspace {temporary_handle} but the client claimed to be working from {client.config.workspace_handle}"
             )
 
         yield client
 
         # Safely delete the temporary workspace. Here we re-fetch the workspace using the temporary_handle
         # in case the user switched workspaces yet again upon the client.
         workspace = Workspace.get(client, handle=temporary_handle)
```

### Comparing `steamship-2.3.8/src/steamship/data/__init__.py` & `steamship-2.3.9/src/steamship/data/__init__.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/block.py` & `steamship-2.3.9/src/steamship/data/block.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/embeddings.py` & `steamship-2.3.9/src/steamship/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/file.py` & `steamship-2.3.9/src/steamship/data/file.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/package/package.py` & `steamship-2.3.9/src/steamship/data/package/package.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/package/package_instance.py` & `steamship-2.3.9/src/steamship/data/package/package_instance.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/package/package_version.py` & `steamship-2.3.9/src/steamship/data/package/package_version.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/plugin/hosting.py` & `steamship-2.3.9/src/steamship/data/plugin/hosting.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/plugin/index_plugin_instance.py` & `steamship-2.3.9/src/steamship/data/plugin/index_plugin_instance.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/plugin/plugin.py` & `steamship-2.3.9/src/steamship/data/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/plugin/plugin_instance.py` & `steamship-2.3.9/src/steamship/data/plugin/plugin_instance.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/plugin/plugin_version.py` & `steamship-2.3.9/src/steamship/data/plugin/plugin_version.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/plugin/prompt_generation_plugin_instance.py` & `steamship-2.3.9/src/steamship/data/plugin/prompt_generation_plugin_instance.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/search.py` & `steamship-2.3.9/src/steamship/data/search.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/tags/tag.py` & `steamship-2.3.9/src/steamship/data/tags/tag.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/tags/tag_constants.py` & `steamship-2.3.9/src/steamship/data/tags/tag_constants.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/user.py` & `steamship-2.3.9/src/steamship/data/user.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/data/workspace.py` & `steamship-2.3.9/src/steamship/data/workspace.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/__init__.py` & `steamship-2.3.9/src/steamship/invocable/__init__.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/config.py` & `steamship-2.3.9/src/steamship/invocable/config.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/entrypoint.py` & `steamship-2.3.9/src/steamship/invocable/entrypoint.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/invocable.py` & `steamship-2.3.9/src/steamship/invocable/invocable.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/invocable_request.py` & `steamship-2.3.9/src/steamship/invocable/invocable_request.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/invocable_response.py` & `steamship-2.3.9/src/steamship/invocable/invocable_response.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/lambda_handler.py` & `steamship-2.3.9/src/steamship/invocable/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/manifest.py` & `steamship-2.3.9/src/steamship/invocable/manifest.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/package_service.py` & `steamship-2.3.9/src/steamship/invocable/package_service.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/invocable/plugin_service.py` & `steamship-2.3.9/src/steamship/invocable/plugin_service.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/blockifier/blockifier.py` & `steamship-2.3.9/src/steamship/plugin/blockifier/blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/blockifier/transcriber.py` & `steamship-2.3.9/src/steamship/plugin/blockifier/transcriber.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/embedder.py` & `steamship-2.3.9/src/steamship/plugin/embedder.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/file_importer.py` & `steamship-2.3.9/src/steamship/plugin/file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/inputs/block_and_tag_plugin_input.py` & `steamship-2.3.9/src/steamship/plugin/inputs/block_and_tag_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/inputs/raw_data_plugin_input.py` & `steamship-2.3.9/src/steamship/plugin/inputs/raw_data_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/inputs/train_plugin_input.py` & `steamship-2.3.9/src/steamship/plugin/inputs/train_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/inputs/training_parameter_plugin_input.py` & `steamship-2.3.9/src/steamship/plugin/inputs/training_parameter_plugin_input.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/outputs/model_checkpoint.py` & `steamship-2.3.9/src/steamship/plugin/outputs/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/outputs/raw_data_plugin_output.py` & `steamship-2.3.9/src/steamship/plugin/outputs/raw_data_plugin_output.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/outputs/train_plugin_output.py` & `steamship-2.3.9/src/steamship/plugin/outputs/train_plugin_output.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/outputs/training_parameter_plugin_output.py` & `steamship-2.3.9/src/steamship/plugin/outputs/training_parameter_plugin_output.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/request.py` & `steamship-2.3.9/src/steamship/plugin/request.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/tagger.py` & `steamship-2.3.9/src/steamship/plugin/tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/plugin/trainable_model.py` & `steamship-2.3.9/src/steamship/plugin/trainable_model.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/utils/binary_utils.py` & `steamship-2.3.9/src/steamship/utils/binary_utils.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/utils/huggingface_helper.py` & `steamship-2.3.9/src/steamship/utils/huggingface_helper.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/utils/kv_store.py` & `steamship-2.3.9/src/steamship/utils/kv_store.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/utils/signed_urls.py` & `steamship-2.3.9/src/steamship/utils/signed_urls.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/utils/url.py` & `steamship-2.3.9/src/steamship/utils/url.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship/utils/zip_archives.py` & `steamship-2.3.9/src/steamship/utils/zip_archives.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/src/steamship.egg-info/SOURCES.txt` & `steamship-2.3.9/src/steamship.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 src/steamship.egg-info/dependency_links.txt
 src/steamship.egg-info/entry_points.txt
 src/steamship.egg-info/requires.txt
 src/steamship.egg-info/top_level.txt
 src/steamship/base/__init__.py
 src/steamship/base/client.py
 src/steamship/base/configuration.py
+src/steamship/base/environments.py
 src/steamship/base/error.py
 src/steamship/base/mime_types.py
 src/steamship/base/model.py
 src/steamship/base/package_spec.py
 src/steamship/base/request.py
 src/steamship/base/response.py
 src/steamship/base/tasks.py
```

### Comparing `steamship-2.3.8/tests/assets/demo_package_spec.json` & `steamship-2.3.9/tests/assets/demo_package_spec.json`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/packages/configurable_hello_world.py` & `steamship-2.3.9/tests/assets/packages/configurable_hello_world.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/packages/demo_package.py` & `steamship-2.3.9/tests/assets/packages/demo_package.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/packages/fancy_types.py` & `steamship-2.3.9/tests/assets/packages/fancy_types.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/packages/hello_world.py` & `steamship-2.3.9/tests/assets/packages/hello_world.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/packages/safe_loaded_bad_import.pyignore` & `steamship-2.3.9/tests/assets/packages/safe_loaded_bad_import.pyignore`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/packages/signed_url_package.py` & `steamship-2.3.9/tests/assets/packages/signed_url_package.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/palm_tree.png` & `steamship-2.3.9/tests/assets/palm_tree.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/blockifiers/async_blockifier.py` & `steamship-2.3.9/tests/assets/plugins/blockifiers/async_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/blockifiers/blockifier.py` & `steamship-2.3.9/tests/assets/plugins/blockifiers/blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/blockifiers/csv_blockifier.py` & `steamship-2.3.9/tests/assets/plugins/blockifiers/csv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/blockifiers/tsv_blockifier.py` & `steamship-2.3.9/tests/assets/plugins/blockifiers/tsv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer.py` & `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer_by_url.py` & `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_by_url.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer_python_error.py` & `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_python_error.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py` & `steamship-2.3.9/tests/assets/plugins/importers/plugin_file_importer_steamship_error.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_configurable_tagger.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_configurable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_embedder.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_embedder.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_logging_tagger.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_logging_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_parser.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_parser.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_prompt_generator.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_tagger_bad_import.pyignore`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_third_party_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_trainable_tagger.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py` & `steamship-2.3.9/tests/assets/plugins/taggers/plugin_trainable_tagger_config.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/integration/test_configurable_package_instance.py` & `steamship-2.3.9/tests/steamship_tests/app/integration/test_configurable_package_instance.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/integration/test_package_error_visibility.py` & `steamship-2.3.9/tests/steamship_tests/app/integration/test_package_error_visibility.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/integration/test_package_instance.py` & `steamship-2.3.9/tests/steamship_tests/app/integration/test_package_instance.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/integration/test_returns_list.py` & `steamship-2.3.9/tests/steamship_tests/app/integration/test_returns_list.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py` & `steamship-2.3.9/tests/steamship_tests/app/integration/test_safe_loaded_package_with_bad_import.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/integration/test_signed_url_package.py` & `steamship-2.3.9/tests/steamship_tests/app/integration/test_signed_url_package.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/integration/test_use_package.py` & `steamship-2.3.9/tests/steamship_tests/app/integration/test_use_package.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/unit/test_config_template_extraction.py` & `steamship-2.3.9/tests/steamship_tests/app/unit/test_config_template_extraction.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/unit/test_demo_app_spec.py` & `steamship-2.3.9/tests/steamship_tests/app/unit/test_demo_app_spec.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/app/unit/test_response.py` & `steamship-2.3.9/tests/steamship_tests/app/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/base/test_binary_utils.py` & `steamship-2.3.9/tests/steamship_tests/base/test_binary_utils.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/base/test_configuration.py` & `steamship-2.3.9/tests/steamship_tests/base/test_configuration.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/base/test_serialization.py` & `steamship-2.3.9/tests/steamship_tests/base/test_serialization.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/base/test_steamship_error_serializable.py` & `steamship-2.3.9/tests/steamship_tests/base/test_steamship_error_serializable.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/base/test_task.py` & `steamship-2.3.9/tests/steamship_tests/base/test_task.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_blockify.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_blockify.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_classify.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_classify.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_convert_ocr.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_convert_ocr.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_embed.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_embed.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_embed_file.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_embed_file.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_embedding_index.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_embedding_index.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_embedding_index_snapshot.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_embedding_index_snapshot.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_tag.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_tag.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/operations/test_tag_file.py` & `steamship-2.3.9/tests/steamship_tests/client/operations/test_tag_file.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/test_client.py` & `steamship-2.3.9/tests/steamship_tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/client/test_task_dependencies.py` & `steamship-2.3.9/tests/steamship_tests/client/test_task_dependencies.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/tags/test_file_tags.py` & `steamship-2.3.9/tests/steamship_tests/data/tags/test_file_tags.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/test_block.py` & `steamship-2.3.9/tests/steamship_tests/data/test_block.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/test_file.py` & `steamship-2.3.9/tests/steamship_tests/data/test_file.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/test_img.png` & `steamship-2.3.9/tests/steamship_tests/data/test_img.png`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/test_package_version.py` & `steamship-2.3.9/tests/steamship_tests/data/test_package_version.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/test_plugins.py` & `steamship-2.3.9/tests/steamship_tests/data/test_plugins.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/test_task_comments.py` & `steamship-2.3.9/tests/steamship_tests/data/test_task_comments.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/data/test_workspace.py` & `steamship-2.3.9/tests/steamship_tests/data/test_workspace.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_async_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_blockifier_markdown.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_configurable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_csv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_embedder.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_embedder.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_file_importer_by_url.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_get_training_parameters.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_logging_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_prompt_plugin.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_tagger.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_third_party_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_e2e_tsv_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_use_plugin.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_use_plugin.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/integration/test_use_skill.py` & `steamship-2.3.9/tests/steamship_tests/plugin/integration/test_use_skill.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_blockifier.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_blockifier.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_config_block.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_config_block.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_file_importer.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_file_importer.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_response_post_update.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_response_post_update.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_service.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_tagger.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_trainable_tagger.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/test_trainable_tagger_config.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/test_model_checkpoints.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/plugin/unit/trainable/util.py` & `steamship-2.3.9/tests/steamship_tests/plugin/unit/trainable/util.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/server/test_package_local.py` & `steamship-2.3.9/tests/steamship_tests/server/test_package_local.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/server/test_task_timeout.py` & `steamship-2.3.9/tests/steamship_tests/server/test_task_timeout.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/client.py` & `steamship-2.3.9/tests/steamship_tests/utils/client.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/deployables.py` & `steamship-2.3.9/tests/steamship_tests/utils/deployables.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/fixtures.py` & `steamship-2.3.9/tests/steamship_tests/utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/random.py` & `steamship-2.3.9/tests/steamship_tests/utils/random.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/test_camel_model.py` & `steamship-2.3.9/tests/steamship_tests/utils/test_camel_model.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/test_client.py` & `steamship-2.3.9/tests/steamship_tests/utils/test_client.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/test_enums.py` & `steamship-2.3.9/tests/steamship_tests/utils/test_enums.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/test_kv_store.py` & `steamship-2.3.9/tests/steamship_tests/utils/test_kv_store.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/test_signed_urls.py` & `steamship-2.3.9/tests/steamship_tests/utils/test_signed_urls.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/test_static_instance_methods.py` & `steamship-2.3.9/tests/steamship_tests/utils/test_static_instance_methods.py`

 * *Files identical despite different names*

### Comparing `steamship-2.3.8/tests/steamship_tests/utils/test_zip_archives.py` & `steamship-2.3.9/tests/steamship_tests/utils/test_zip_archives.py`

 * *Files identical despite different names*

