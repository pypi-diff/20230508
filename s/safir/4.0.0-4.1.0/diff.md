# Comparing `tmp/safir-4.0.0.tar.gz` & `tmp/safir-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safir-4.0.0.tar", last modified: Wed Apr 19 16:56:55 2023, max compression
+gzip compressed data, was "safir-4.1.0.tar", last modified: Mon May  8 18:06:39 2023, max compression
```

## Comparing `safir-4.0.0.tar` & `safir-4.1.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.778174 safir-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 16:56:40.000000 safir-4.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 16:56:40.000000 safir-4.0.0/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 16:56:40.000000 safir-4.0.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 16:56:40.000000 safir-4.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-19 16:56:40.000000 safir-4.0.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-19 16:56:40.000000 safir-4.0.0/.github/workflows/periodic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-19 16:56:40.000000 safir-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-19 16:56:40.000000 safir-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-04-19 16:56:40.000000 safir-4.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-19 16:56:40.000000 safir-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 16:56:40.000000 safir-4.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-19 16:56:55.778174 safir-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-19 16:56:40.000000 safir-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-19 16:56:40.000000 safir-4.0.0/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-19 16:56:40.000000 safir-4.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-04-19 16:56:40.000000 safir-4.0.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-19 16:56:40.000000 safir-4.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.750174 safir-4.0.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-19 16:56:40.000000 safir-4.0.0/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 16:56:40.000000 safir-4.0.0/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-19 16:56:40.000000 safir-4.0.0/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-19 16:56:40.000000 safir-4.0.0/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-19 16:56:40.000000 safir-4.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.754174 safir-4.0.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/arq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/fastapi-errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/gafaelfawr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/gcs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.758174 safir-4.0.0/docs/user-guide/github-apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/api-resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/create-a-github-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/handling-webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/github-apps/webhook-models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/http-client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/ivoa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/kubernetes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/pydantic-redis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/pydantic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/set-up-from-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/slack-webhook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/uvicorn.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-19 16:56:40.000000 safir-4.0.0/docs/user-guide/x-forwarded.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-19 16:56:40.000000 safir-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:56:55.778174 safir-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.746174 safir-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.762174 safir-4.0.0/src/safir/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.762174 safir-4.0.0/src/safir/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/arq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/db_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/gafaelfawr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/dependencies/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/github/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/github/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/middleware/ivoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/middleware/x_forwarded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/slack/blockkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/slack/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.766174 safir-4.0.0/src/safir/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40255 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-19 16:56:40.000000 safir-4.0.0/src/safir/testing/uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.762174 safir-4.0.0/src/safir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 16:56:55.000000 safir-4.0.0/src/safir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.770174 safir-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 16:56:40.000000 safir-4.0.0/tests/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 16:56:40.000000 safir-4.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-19 16:56:40.000000 safir-4.0.0/tests/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-19 16:56:40.000000 safir-4.0.0/tests/datetime_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.770174 safir-4.0.0/tests/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/arq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/db_session_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/gafaelfawr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/http_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-19 16:56:40.000000 safir-4.0.0/tests/dependencies/logger_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-19 16:56:40.000000 safir-4.0.0/tests/fastapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-19 16:56:40.000000 safir-4.0.0/tests/gcs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.746174 safir-4.0.0/tests/github/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/github/data/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/check_run_created.json
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/check_suite_completed.json
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/installation.json
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/installation_repositories.json
--rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/pull_request_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/data/webhooks/push_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-19 16:56:40.000000 safir-4.0.0/tests/github/webhooks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-19 16:56:40.000000 safir-4.0.0/tests/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-19 16:56:40.000000 safir-4.0.0/tests/logging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-19 16:56:40.000000 safir-4.0.0/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-19 16:56:40.000000 safir-4.0.0/tests/middleware/ivoa_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-19 16:56:40.000000 safir-4.0.0/tests/middleware/x_forwarded_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-19 16:56:40.000000 safir-4.0.0/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-19 16:56:40.000000 safir-4.0.0/tests/pydantic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-19 16:56:40.000000 safir-4.0.0/tests/redis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-19 16:56:40.000000 safir-4.0.0/tests/safir_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-04-19 16:56:40.000000 safir-4.0.0/tests/slack/blockkit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-19 16:56:40.000000 safir-4.0.0/tests/slack/webhook_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:55.774174 safir-4.0.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/gcs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-19 16:56:40.000000 safir-4.0.0/tests/testing/kubernetes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-19 16:56:40.000000 safir-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 18:06:21.000000 safir-4.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-08 18:06:21.000000 safir-4.1.0/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 18:06:21.000000 safir-4.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 18:06:21.000000 safir-4.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 18:06:21.000000 safir-4.1.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-08 18:06:21.000000 safir-4.1.0/.github/workflows/periodic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-08 18:06:21.000000 safir-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 18:06:21.000000 safir-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-05-08 18:06:21.000000 safir-4.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-08 18:06:21.000000 safir-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 18:06:21.000000 safir-4.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-08 18:06:39.485432 safir-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-08 18:06:21.000000 safir-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-08 18:06:21.000000 safir-4.1.0/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 18:06:21.000000 safir-4.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-05-08 18:06:21.000000 safir-4.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 18:06:21.000000 safir-4.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-08 18:06:21.000000 safir-4.1.0/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 18:06:21.000000 safir-4.1.0/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 18:06:21.000000 safir-4.1.0/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-08 18:06:21.000000 safir-4.1.0/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-08 18:06:21.000000 safir-4.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.469431 safir-4.1.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/arq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/fastapi-errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/gafaelfawr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/gcs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.473431 safir-4.1.0/docs/user-guide/github-apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/api-resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/create-a-github-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/handling-webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/github-apps/webhook-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/http-client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/ivoa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/kubernetes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/pydantic-redis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/pydantic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/set-up-from-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/slack-webhook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/uvicorn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-08 18:06:21.000000 safir-4.1.0/docs/user-guide/x-forwarded.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-08 18:06:21.000000 safir-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:06:39.485432 safir-4.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.465431 safir-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.473431 safir-4.1.0/src/safir/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/arq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/db_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/gafaelfawr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/dependencies/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/github/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/middleware/ivoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/middleware/x_forwarded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/slack/blockkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/slack/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.477431 safir-4.1.0/src/safir/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49522 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-08 18:06:21.000000 safir-4.1.0/src/safir/testing/uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.473431 safir-4.1.0/src/safir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 18:06:39.000000 safir-4.1.0/src/safir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 18:06:21.000000 safir-4.1.0/tests/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 18:06:21.000000 safir-4.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-08 18:06:21.000000 safir-4.1.0/tests/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-08 18:06:21.000000 safir-4.1.0/tests/datetime_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/arq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/db_session_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/gafaelfawr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/http_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-08 18:06:21.000000 safir-4.1.0/tests/dependencies/logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-08 18:06:21.000000 safir-4.1.0/tests/fastapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 18:06:21.000000 safir-4.1.0/tests/gcs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.465431 safir-4.1.0/tests/github/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.481431 safir-4.1.0/tests/github/data/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/check_run_created.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/check_suite_completed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/installation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/installation_repositories.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26334 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/pull_request_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/data/webhooks/push_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-08 18:06:21.000000 safir-4.1.0/tests/github/webhooks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-08 18:06:21.000000 safir-4.1.0/tests/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-05-08 18:06:21.000000 safir-4.1.0/tests/logging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-08 18:06:21.000000 safir-4.1.0/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/tests/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-08 18:06:21.000000 safir-4.1.0/tests/middleware/ivoa_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-08 18:06:21.000000 safir-4.1.0/tests/middleware/x_forwarded_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-08 18:06:21.000000 safir-4.1.0/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-08 18:06:21.000000 safir-4.1.0/tests/pydantic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-08 18:06:21.000000 safir-4.1.0/tests/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 18:06:21.000000 safir-4.1.0/tests/safir_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/tests/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-08 18:06:21.000000 safir-4.1.0/tests/slack/blockkit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-08 18:06:21.000000 safir-4.1.0/tests/slack/webhook_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:39.485432 safir-4.1.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/gcs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-08 18:06:21.000000 safir-4.1.0/tests/testing/kubernetes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-08 18:06:21.000000 safir-4.1.0/tox.ini
```

### Comparing `safir-4.0.0/.github/workflows/ci.yaml` & `safir-4.1.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/.github/workflows/periodic.yaml` & `safir-4.1.0/.github/workflows/periodic.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/.gitignore` & `safir-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/.pre-commit-config.yaml` & `safir-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/CHANGELOG.md` & `safir-4.1.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 # Change log
 
 <!--
 Headline template:
 X.Y.Z (YYYY-MM-DD)
 -->
 
+## 4.1.0 (2023-05-08)
+
+### New features
+
+- Add `read_*` methods for `ConfigMap` and `ResourceQuota` to the mock Kubernetes API for testing.
+- Add `patch_namespaced_pod_status` to the mock Kubernetes API for testing. Application code is unlikely to call this, but it's useful for test suites.
+- The mock `list_namespaced_pod` Kubernetes API now supports watches (but be aware that all changes must be made through the API).
+
+### Bug fixes
+
+- Fix concurrency locking when watching namespace events in the Kubernetes testing mock. The previous logic degenerated into busy-waiting rather than correctly waiting on a condition variable.
+- Watches for namespace events using the mock Kubernetes API now start with the next event, not the first stored event, if `resource_version` is not set, aligning behavior with the Kubernetes API.
+
 ## 4.0.0 (2023-04-19)
 
 ### Backwards-incompatible changes
 
 - Safir now requires a minimum Python version of 3.11.
 - `safir.pydantic.validate_exactly_one_of` is now a Pydantic root validator instead of an individual field validator, which simplifies how it should be called.
 - Custom Kubernetes objects are no longer copied before being stored in the Kubernetes mock by `create_namespaced_custom_object`, and no longer automatically get a `metadata.uid` value. This brings handling of custom objects in line with the behavior of other mocked `create_*` and `replace_*` APIs.
```

### Comparing `safir-4.0.0/LICENSE` & `safir-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/PKG-INFO` & `safir-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.0.0
+Version: 4.1.0
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.0.0/README.md` & `safir-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/_rst_epilog.rst` & `safir-4.1.0/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/api.rst` & `safir-4.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/changelog.md` & `safir-4.1.0/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 # Change log
 
 <!--
 Headline template:
 X.Y.Z (YYYY-MM-DD)
 -->
 
+## 4.1.0 (2023-05-08)
+
+### New features
+
+- Add `read_*` methods for `ConfigMap` and `ResourceQuota` to the mock Kubernetes API for testing.
+- Add `patch_namespaced_pod_status` to the mock Kubernetes API for testing. Application code is unlikely to call this, but it's useful for test suites.
+- The mock `list_namespaced_pod` Kubernetes API now supports watches (but be aware that all changes must be made through the API).
+
+### Bug fixes
+
+- Fix concurrency locking when watching namespace events in the Kubernetes testing mock. The previous logic degenerated into busy-waiting rather than correctly waiting on a condition variable.
+- Watches for namespace events using the mock Kubernetes API now start with the next event, not the first stored event, if `resource_version` is not set, aligning behavior with the Kubernetes API.
+
 ## 4.0.0 (2023-04-19)
 
 ### Backwards-incompatible changes
 
 - Safir now requires a minimum Python version of 3.11.
 - `safir.pydantic.validate_exactly_one_of` is now a Pydantic root validator instead of an individual field validator, which simplifies how it should be called.
 - Custom Kubernetes objects are no longer copied before being stored in the Kubernetes mock by `create_namespaced_custom_object`, and no longer automatically get a `metadata.uid` value. This brings handling of custom objects in line with the behavior of other mocked `create_*` and `replace_*` APIs.
```

### Comparing `safir-4.0.0/docs/dev/development.rst` & `safir-4.1.0/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/dev/release.rst` & `safir-4.1.0/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/documenteer.toml` & `safir-4.1.0/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/index.rst` & `safir-4.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/arq.rst` & `safir-4.1.0/docs/user-guide/arq.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/database.rst` & `safir-4.1.0/docs/user-guide/database.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/datetime.rst` & `safir-4.1.0/docs/user-guide/datetime.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/fastapi-errors.rst` & `safir-4.1.0/docs/user-guide/fastapi-errors.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/gafaelfawr.rst` & `safir-4.1.0/docs/user-guide/gafaelfawr.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/gcs.rst` & `safir-4.1.0/docs/user-guide/gcs.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/github-apps/api-resources.rst` & `safir-4.1.0/docs/user-guide/github-apps/api-resources.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/github-apps/create-a-github-client.rst` & `safir-4.1.0/docs/user-guide/github-apps/create-a-github-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/github-apps/handling-webhooks.rst` & `safir-4.1.0/docs/user-guide/github-apps/handling-webhooks.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/github-apps/index.rst` & `safir-4.1.0/docs/user-guide/github-apps/index.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/github-apps/webhook-models.rst` & `safir-4.1.0/docs/user-guide/github-apps/webhook-models.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/http-client.rst` & `safir-4.1.0/docs/user-guide/http-client.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/ivoa.rst` & `safir-4.1.0/docs/user-guide/ivoa.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/kubernetes.rst` & `safir-4.1.0/docs/user-guide/kubernetes.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/logging.rst` & `safir-4.1.0/docs/user-guide/logging.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/pydantic-redis.rst` & `safir-4.1.0/docs/user-guide/pydantic-redis.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/pydantic.rst` & `safir-4.1.0/docs/user-guide/pydantic.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/set-up-from-template.rst` & `safir-4.1.0/docs/user-guide/set-up-from-template.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/slack-webhook.rst` & `safir-4.1.0/docs/user-guide/slack-webhook.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/uvicorn.rst` & `safir-4.1.0/docs/user-guide/uvicorn.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/docs/user-guide/x-forwarded.rst` & `safir-4.1.0/docs/user-guide/x-forwarded.rst`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/pyproject.toml` & `safir-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/__init__.py` & `safir-4.1.0/src/safir/__init__.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/arq.py` & `safir-4.1.0/src/safir/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/asyncio.py` & `safir-4.1.0/src/safir/asyncio.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/database.py` & `safir-4.1.0/src/safir/database.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/datetime.py` & `safir-4.1.0/src/safir/datetime.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/dependencies/arq.py` & `safir-4.1.0/src/safir/dependencies/arq.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/dependencies/db_session.py` & `safir-4.1.0/src/safir/dependencies/db_session.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/dependencies/gafaelfawr.py` & `safir-4.1.0/src/safir/dependencies/gafaelfawr.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/dependencies/http_client.py` & `safir-4.1.0/src/safir/dependencies/http_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/dependencies/logger.py` & `safir-4.1.0/src/safir/dependencies/logger.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/fastapi.py` & `safir-4.1.0/src/safir/fastapi.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/gcs.py` & `safir-4.1.0/src/safir/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/github/_client.py` & `safir-4.1.0/src/safir/github/_client.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/github/models.py` & `safir-4.1.0/src/safir/github/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/github/webhooks.py` & `safir-4.1.0/src/safir/github/webhooks.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/kubernetes.py` & `safir-4.1.0/src/safir/kubernetes.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/logging.py` & `safir-4.1.0/src/safir/logging.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/metadata.py` & `safir-4.1.0/src/safir/metadata.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/middleware/ivoa.py` & `safir-4.1.0/src/safir/middleware/ivoa.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/middleware/x_forwarded.py` & `safir-4.1.0/src/safir/middleware/x_forwarded.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/models.py` & `safir-4.1.0/src/safir/models.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/pydantic.py` & `safir-4.1.0/src/safir/pydantic.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/redis.py` & `safir-4.1.0/src/safir/redis.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/slack/blockkit.py` & `safir-4.1.0/src/safir/slack/blockkit.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/slack/webhook.py` & `safir-4.1.0/src/safir/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/testing/gcs.py` & `safir-4.1.0/src/safir/testing/gcs.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/testing/kubernetes.py` & `safir-4.1.0/src/safir/testing/kubernetes.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,14 +80,183 @@
                     item = strip_none(item)
                 list_result.append(item)
             value = list_result
         result[key] = value
     return result
 
 
+class _EventStream:
+    """Holds the data for a stream of watchable events.
+
+    This is an internal implementation detail of the Kubernetes mock. It holds
+    a stream of watchable events and a list of `asyncio.Event` triggers. A
+    watch can register interest in this event stream, in which case its
+    trigger will be notified when anything new is added to the event stream.
+    The events are generic dicts, which will be interpreted by the Kubernetes
+    library differently depending on which underlying API is using this data
+    structure.
+    """
+
+    def __init__(self) -> None:
+        self._events: list[dict[str, Any]] = []
+        self._triggers: list[asyncio.Event] = []
+
+    @property
+    def next_resource_version(self) -> str:
+        """Resource version of the next event.
+
+        This starts with ``1`` to ensure that a resource version of ``0`` is
+        special and means to return all known events, so it must be adjusted
+        when indexing into a list of events.
+        """
+        return str(len(self._events) + 1)
+
+    def add_event(self, event: dict[str, Any]) -> None:
+        """Add a new event and notify all watchers.
+
+        Parameters
+        ----------
+        event
+            New event.
+        """
+        self._events.append(event)
+        for trigger in self._triggers:
+            trigger.set()
+
+    def build_watch_response(
+        self,
+        resource_version: Optional[str] = None,
+        timeout_seconds: Optional[int] = None,
+        *,
+        field_selector: Optional[str] = None,
+    ) -> Mock:
+        """Construct a response to a watch request.
+
+        Wraps a watch iterator in the appropriate mock to behave as expected
+        when called from ``kubernetes_asyncio``. This simulates an aiohttp
+        response.
+
+        Parameters
+        ----------
+        resource_version
+            Starting resource version for the watch. The resource versions
+            must be the position in the events stream, stringified.
+        timeout_seconds
+            How long to watch. This is total elapsed time, not the time
+            between events. It matches the corresponding parameter in the
+            Kubernetes API. If `None`, watch forever.
+        field_selector
+            Which events to retrieve when performing a watch. If set, it must
+            be set to ``metadata.name=...`` to match a specific object name.
+
+        Returns
+        -------
+        Mock
+            Simulation of an aiohttp response whose ``readline`` method wraps
+            the iterator.
+
+        Raises
+        ------
+        AssertionError
+            Some other ``field_selector`` was provided.
+        """
+        generator = self._build_watcher(
+            resource_version, timeout_seconds, field_selector
+        )
+
+        async def readline() -> bytes:
+            return await generator.__anext__()
+
+        response = Mock()
+        response.content.readline = AsyncMock()
+        response.content.readline.side_effect = readline
+        return response
+
+    def _build_watcher(
+        self,
+        resource_version: str | None,
+        timeout_seconds: int | None,
+        field_selector: str | None,
+    ) -> AsyncIterator[bytes]:
+        """Construct a watcher for this event stream.
+
+        Parameters
+        ----------
+        resource_version
+            Starting resource version for the watch. The resource version
+            must be the position in the events stream, stringified. If not
+            given, start after the most recent event.
+        timeout_seconds
+            How long to watch. This is total elapsed time, not the time
+            between events. It matches the corresponding parameter in the
+            Kubernetes API. If `None`, watch forever.
+        field_selector
+            Which events to retrieve when performing a watch. If set, it must
+            be set to ``metadata.name=...`` to match a specific object name.
+
+        Returns
+        -------
+        AsyncIterator
+            An async iterator that will return each new event in the stream,
+            encoded as expected by the Kubernetes API, until the timeout
+            occurs.
+
+        Raises
+        ------
+        AssertionError
+            Some other ``field_selector`` was provided.
+        """
+        timeout = None
+        if timeout_seconds is not None:
+            timeout = current_datetime() + timedelta(seconds=timeout_seconds)
+
+        # Parse the field selector, if one was provided.
+        name = None
+        if field_selector:
+            match = re.match(r"metadata\.name=(.*)$", field_selector)
+            assert match and match.group(1)
+            name = match.group(1)
+
+        # Create and register a new trigger.
+        trigger = asyncio.Event()
+        self._triggers.append(trigger)
+
+        # Construct the iterator.
+        async def next_event() -> AsyncIterator[bytes]:
+            if resource_version:
+                position = int(resource_version)
+            else:
+                position = len(self._events)
+            while True:
+                for event in self._events[position:]:
+                    position += 1
+                    if name and event["object"]["metadata"]["name"] != name:
+                        continue
+                    yield json.dumps(event).encode()
+                if not timeout:
+                    await trigger.wait()
+                else:
+                    now = current_datetime()
+                    timeout_left = (timeout - now).total_seconds()
+                    if timeout_left <= 0:
+                        yield b""
+                        break
+                    try:
+                        async with asyncio.timeout(timeout_left):
+                            await trigger.wait()
+                    except TimeoutError:
+                        yield b""
+                        break
+                trigger.clear()
+            self._triggers = [t for t in self._triggers if t != trigger]
+
+        # Return the iterator.
+        return next_event()
+
+
 class MockKubernetesApi:
     """Mock Kubernetes API for testing.
 
     This object simulates (with almost everything left out) the ``CoreV1Api``,
     ``CustomObjectApi``, and ``NetworkingV1Api`` client objects while keeping
     simple internal state. It is intended to be used as a mock inside tests.
 
@@ -134,19 +303,19 @@
     """
 
     def __init__(self) -> None:
         self.error_callback: Optional[Callable[..., None]] = None
         self.initial_pod_phase = "Running"
 
         self._custom_kinds: dict[str, str] = {}
-        self._events: defaultdict[str, list[CoreV1Event]] = defaultdict(list)
-        self._new_events: defaultdict[str, asyncio.Event]
-        self._new_events = defaultdict(asyncio.Event)
         self._nodes = V1NodeList(items=[])
         self._objects: dict[str, dict[str, dict[str, Any]]] = {}
+        self._events: defaultdict[str, list[CoreV1Event]] = defaultdict(list)
+        self._event_streams: defaultdict[str, dict[str, _EventStream]]
+        self._event_streams = defaultdict(lambda: defaultdict(_EventStream))
 
     def get_all_objects_for_test(self, kind: str) -> list[Any]:
         """Return all objects of a given kind sorted by namespace and name.
 
         Parameters
         ----------
         kind
@@ -467,14 +636,39 @@
         ------
         kubernetes_asyncio.client.ApiException
             Raised with 404 status if the object does not exist.
         """
         self._maybe_error("delete_namespaced_config_map", name, namespace)
         return self._delete_object(namespace, "ConfigMap", name)
 
+    async def read_namespaced_config_map(
+        self, name: str, namespace: str
+    ) -> V1ConfigMap:
+        """Read a config map object.
+
+        Parameters
+        ----------
+        name
+            Name of object.
+        namespace
+            Namespace of object.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1ConfigMap
+            Corresponding object.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the config map was not found.
+        """
+        self._maybe_error("read_namespaced_config_map", name, namespace)
+        return self._get_object(namespace, "ConfigMap", name)
+
     # EVENTS API
 
     async def create_namespaced_event(
         self, namespace: str, body: CoreV1Event
     ) -> None:
         """Store a new namespaced event.
 
@@ -485,24 +679,25 @@
         namespace
             Namespace of the event.
         body
             New event to store.
         """
         self._maybe_error("create_namespaced_event", namespace, body)
         self._update_metadata(body, "v1", "Event", namespace)
-        body.metadata.resource_version = str(len(self._events[namespace]))
+        stream = self._event_streams[namespace]["Event"]
+        body.metadata.resource_version = stream.next_resource_version
+        stream.add_event({"type": "ADDED", "object": body.to_dict()})
         self._events[namespace].append(body)
-        self._new_events[namespace].set()
 
     async def list_namespaced_event(
         self,
         namespace: str,
         *,
         field_selector: Optional[str] = None,
-        resource_version: str = "0",
+        resource_version: Optional[str] = None,
         timeout_seconds: Optional[int] = None,
         watch: bool = False,
         _preload_content: bool = True,
         _request_timeout: Optional[int] = None,
     ) -> CoreV1EventList | Mock:
         """List namespaced events.
 
@@ -539,55 +734,17 @@
         if not watch:
             return CoreV1EventList(items=self._events[namespace])
 
         # All watches must not preload content since we're returning raw JSON.
         # This is done by the Kubernetes API Watch object.
         assert not _preload_content
 
-        # When the timeout has expired.
-        timeout = None
-        if timeout_seconds is not None:
-            timeout = current_datetime() + timedelta(seconds=timeout_seconds)
-
-        # Returns all available events for this namespace, and then waits for
-        # new events and returns them up to the timeout.
-        async def next_event() -> AsyncIterator[bytes]:
-            position = int(resource_version)
-            while True:
-                for event in self._events[namespace][position:]:
-                    raw = {"type": "ADDED", "object": event.to_dict()}
-                    yield json.dumps(raw).encode()
-                    position += 1
-                wait_event = self._new_events[namespace]
-                if not timeout:
-                    await wait_event.wait()
-                else:
-                    now = current_datetime()
-                    timeout_left = (timeout - now).total_seconds()
-                    if timeout_left < 0:
-                        yield b""
-                        return
-                    try:
-                        await asyncio.wait_for(wait_event.wait(), timeout_left)
-                    except TimeoutError:
-                        yield b""
-                        return
-
-        event_generator = next_event()
-
-        async def readline() -> bytes:
-            return await event_generator.__anext__()
-
-        # To support the watch interface, we have to simulate a streaming
-        # aiohttp response. Thankfully, the watch only uses a minimal
-        # interface, so we can get away with a simple mock.
-        response = Mock()
-        response.content.readline = AsyncMock()
-        response.content.readline.side_effect = readline
-        return response
+        # Return the mock response expected by the Kubernetes API.
+        stream = self._event_streams[namespace]["Event"]
+        return stream.build_watch_response(resource_version, timeout_seconds)
 
     # NAMESPACE API
 
     async def create_namespace(self, body: V1Namespace) -> None:
         """Create a namespace.
 
         The mock doesn't truly track namespaces since it autocreates them when
@@ -740,15 +897,18 @@
         ------
         kubernetes_asyncio.client.ApiException
             Raised with 409 status if the pod already exists.
         """
         self._maybe_error("create_namespaced_pod", namespace, body)
         self._update_metadata(body, "v1", "Pod", namespace)
         body.status = V1PodStatus(phase=self.initial_pod_phase)
+        stream = self._event_streams[namespace]["Pod"]
+        body.metadata.resource_version = stream.next_resource_version
         self._store_object(namespace, "Pod", body.metadata.name, body)
+        stream.add_event({"type": "ADDED", "object": body.to_dict()})
         if self.initial_pod_phase == "Running":
             event = CoreV1Event(
                 metadata=V1ObjectMeta(
                     name=f"{body.metadata.name}-start", namespace=namespace
                 ),
                 message=f"Pod {body.metadata.name} started",
                 involved_object=V1ObjectReference(
@@ -776,58 +936,136 @@
 
         Raises
         ------
         kubernetes_asyncio.client.ApiException
             Raised with 404 status if the pod was not found.
         """
         self._maybe_error("delete_namespaced_pod", name, namespace)
-        return self._delete_object(namespace, "Pod", name)
+        pod = self._get_object(namespace, "Pod", name)
+        result = self._delete_object(namespace, "Pod", name)
+        stream = self._event_streams[namespace]["Pod"]
+        stream.add_event({"type": "DELETED", "object": pod.to_dict()})
+        return result
 
     async def list_namespaced_pod(
-        self, namespace: str, *, field_selector: Optional[str] = None
-    ) -> V1PodList:
+        self,
+        namespace: str,
+        *,
+        field_selector: Optional[str] = None,
+        resource_version: Optional[str] = None,
+        timeout_seconds: Optional[int] = None,
+        watch: bool = False,
+        _preload_content: bool = True,
+        _request_timeout: Optional[int] = None,
+    ) -> V1PodList | Mock:
         """List pod objects in a namespace.
 
+        This does support watches.
+
         Parameters
         ----------
         namespace
             Namespace of pods to list.
         field_selector
             Only ``metadata.name=...`` is supported. It is parsed to find the
             pod name and only pods matching that name will be returned.
+        resource_version
+            Where to start in the event stream when performing a watch. If
+            `None`, starts with the next change.
+        timeout_seconds
+            How long to return events for before exiting when performing a
+            watch.
+        watch
+            Whether to act as a watch.
+        _preload_content
+            Verified to be `False` when performing a watch.
+        _request_timeout
+            Ignored, accepted for compatibility with the watch API.
 
         Returns
         -------
-        kubernetes_asyncio.client.V1PodList
-            List of pods in that namespace.
+        kubernetes_asyncio.client.V1PodList or unittest.mock.Mock
+            List of pods in that namespace, when not called as a watch. If
+            called as a watch, returns a mock ``aiohttp.Response`` with a
+            ``readline`` metehod that yields the events.
 
         Raises
         ------
-        kubernetes_asyncio.client.ApiException
-            Raised with 404 status if the namespace does not exist.
         AssertionError
             Some other ``field_selector`` was provided.
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the namespace does not exist.
         """
         self._maybe_error("list_namespaced_pod", namespace, field_selector)
         if namespace not in self._objects:
             msg = f"Namespace {namespace} not found"
             raise ApiException(status=404, reason=msg)
-        if field_selector:
-            match = re.match(r"metadata\.name=(.*)$", field_selector)
-            assert match and match.group(1)
-            try:
-                pod = self._get_object(namespace, "Pod", match.group(1))
-                return V1PodList(kind="Pod", items=[pod])
-            except ApiException:
-                return V1PodList(kind="Pod", items=[])
-        else:
-            pods = []
-            for obj in self._objects[namespace]["Pod"].values():
-                pods.append(obj)
-            return V1PodList(kind="Pod", items=pods)
+        if not watch:
+            if field_selector:
+                match = re.match(r"metadata\.name=(.*)$", field_selector)
+                assert match and match.group(1)
+                try:
+                    pod = self._get_object(namespace, "Pod", match.group(1))
+                    return V1PodList(kind="Pod", items=[pod])
+                except ApiException:
+                    return V1PodList(kind="Pod", items=[])
+            else:
+                pods = []
+                for obj in self._objects[namespace]["Pod"].values():
+                    pods.append(obj)
+                return V1PodList(kind="Pod", items=pods)
+
+        # All watches must not preload content since we're returning raw JSON.
+        # This is done by the Kubernetes API Watch object.
+        assert not _preload_content
+
+        # Return the mock response expected by the Kubernetes API.
+        stream = self._event_streams[namespace]["Pod"]
+        return stream.build_watch_response(
+            resource_version, timeout_seconds, field_selector=field_selector
+        )
+
+    async def patch_namespaced_pod_status(
+        self, name: str, namespace: str, body: list[dict[str, Any]]
+    ) -> V1Secret:
+        """Patch the status of a pod object.
+
+        Parameters
+        ----------
+        name
+            Name of pod object.
+        namespace
+            Namespace of secret object.
+        body
+            Patches to apply. Only patches with ``op`` of ``replace`` are
+            supported, and only with ``path`` of ``/status/phase``.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1Pod
+            Patched pod object.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the secret does not exist.
+        AssertionError
+            Raised if any other type of patch was provided.
+        """
+        self._maybe_error("patch_namespaced_pod", name, namespace)
+        pod = copy.deepcopy(self._get_object(namespace, "Pod", name))
+        for change in body:
+            assert change["op"] == "replace"
+            assert change["path"] == "/status/phase"
+            pod.status.phase = change["value"]
+        stream = self._event_streams[namespace]["Pod"]
+        pod.metadata.resource_version = stream.next_resource_version
+        self._store_object(namespace, "Pod", name, pod, replace=True)
+        stream.add_event({"type": "MODIFIED", "object": pod.to_dict()})
+        return pod
 
     async def read_namespaced_pod(self, name: str, namespace: str) -> V1Pod:
         """Read a pod object.
 
         Parameters
         ----------
         name
@@ -896,14 +1134,39 @@
             Raised with 409 status if the object already exists.
         """
         self._maybe_error("create_namespaced_resource_quota", namespace, body)
         self._update_metadata(body, "v1", "ResourceQuota", namespace)
         name = body.metadata.name
         self._store_object(namespace, "ResourceQuota", name, body)
 
+    async def read_namespaced_resource_quota(
+        self, name: str, namespace: str
+    ) -> V1ResourceQuota:
+        """Read a resource quota object.
+
+        Parameters
+        ----------
+        name
+            Name of object.
+        namespace
+            Namespace of object.
+
+        Returns
+        -------
+        kubernetes_asyncio.client.V1ResourceQuota
+            Corresponding object.
+
+        Raises
+        ------
+        kubernetes_asyncio.client.ApiException
+            Raised with 404 status if the resource quota was not found.
+        """
+        self._maybe_error("read_namespaced_resource_quota", name, namespace)
+        return self._get_object(namespace, "ResourceQuota", name)
+
     # SECRETS API
 
     async def create_namespaced_secret(
         self, namespace: str, body: V1Secret
     ) -> None:
         """Create a secret object.
```

### Comparing `safir-4.0.0/src/safir/testing/slack.py` & `safir-4.1.0/src/safir/testing/slack.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir/testing/uvicorn.py` & `safir-4.1.0/src/safir/testing/uvicorn.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/src/safir.egg-info/PKG-INFO` & `safir-4.1.0/src/safir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safir
-Version: 4.0.0
+Version: 4.1.0
 Summary: The Rubin Observatory SQuaRE framework for FastAPI services.
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2020 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `safir-4.0.0/src/safir.egg-info/SOURCES.txt` & `safir-4.1.0/src/safir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/conftest.py` & `safir-4.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/database_test.py` & `safir-4.1.0/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/datetime_test.py` & `safir-4.1.0/tests/datetime_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/dependencies/arq_test.py` & `safir-4.1.0/tests/dependencies/arq_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/dependencies/db_session_test.py` & `safir-4.1.0/tests/dependencies/db_session_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/dependencies/gafaelfawr_test.py` & `safir-4.1.0/tests/dependencies/gafaelfawr_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/dependencies/http_client_test.py` & `safir-4.1.0/tests/dependencies/http_client_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/dependencies/logger_test.py` & `safir-4.1.0/tests/dependencies/logger_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/fastapi_test.py` & `safir-4.1.0/tests/fastapi_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/gcs_test.py` & `safir-4.1.0/tests/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/github/data/webhooks/check_run_created.json` & `safir-4.1.0/tests/github/data/webhooks/check_run_created.json`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/github/data/webhooks/check_suite_completed.json` & `safir-4.1.0/tests/github/data/webhooks/check_suite_completed.json`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/github/data/webhooks/installation.json` & `safir-4.1.0/tests/github/data/webhooks/installation.json`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/github/data/webhooks/installation_repositories.json` & `safir-4.1.0/tests/github/data/webhooks/installation_repositories.json`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/github/data/webhooks/pull_request_event.json` & `safir-4.1.0/tests/github/data/webhooks/pull_request_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/github/data/webhooks/push_event.json` & `safir-4.1.0/tests/github/data/webhooks/push_event.json`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/github/webhooks_test.py` & `safir-4.1.0/tests/github/webhooks_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/logging_test.py` & `safir-4.1.0/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/metadata_test.py` & `safir-4.1.0/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/middleware/ivoa_test.py` & `safir-4.1.0/tests/middleware/ivoa_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/middleware/x_forwarded_test.py` & `safir-4.1.0/tests/middleware/x_forwarded_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/pydantic_test.py` & `safir-4.1.0/tests/pydantic_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/redis_test.py` & `safir-4.1.0/tests/redis_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/slack/blockkit_test.py` & `safir-4.1.0/tests/slack/blockkit_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/slack/webhook_test.py` & `safir-4.1.0/tests/slack/webhook_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/testing/conftest.py` & `safir-4.1.0/tests/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/testing/gcs_test.py` & `safir-4.1.0/tests/testing/gcs_test.py`

 * *Files identical despite different names*

### Comparing `safir-4.0.0/tests/testing/kubernetes_test.py` & `safir-4.1.0/tests/testing/kubernetes_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 These are just basic sanity checks that the mocking is working correctly and
 the basic calls work. There is no attempt to test all of the supported APIs.
 """
 
 from __future__ import annotations
 
 import asyncio
-from typing import Any
+from typing import Any, Optional
 
 import pytest
 from kubernetes_asyncio.client import (
     CoreV1Event,
     V1Container,
     V1ObjectMeta,
     V1ObjectReference,
@@ -103,40 +103,46 @@
             "gafaelfawr-secret",
             custom,
         )
     assert str(excinfo.value) == "some exception"
 
 
 async def watch_events(
-    mock_kubernetes: MockKubernetesApi, namespace: str
+    mock_kubernetes: MockKubernetesApi,
+    namespace: str,
+    *,
+    resource_version: Optional[str] = None,
 ) -> list[CoreV1Event]:
     """Watch events, returning when an event with message ``Done`` is seen."""
     method = mock_kubernetes.list_namespaced_event
     watch_args = {
         "namespace": namespace,
         "timeout_seconds": 10,  # Just in case, so tests don't hang
     }
+    if resource_version:
+        watch_args["resource_version"] = resource_version
     async with Watch().stream(method, **watch_args) as stream:
         seen = []
         async for event in stream:
             assert event["type"] == "ADDED"
             obj = event["raw_object"]
             seen.append(obj)
-            if obj.get("message") == "Done":
+            if "Done" in obj.get("message"):
                 return seen
         return seen
 
 
 @pytest.mark.asyncio
 async def test_mock_events(mock_kubernetes: MockKubernetesApi) -> None:
     watchers = [
         asyncio.create_task(watch_events(mock_kubernetes, "stuff")),
         asyncio.create_task(watch_events(mock_kubernetes, "stuff")),
         asyncio.create_task(watch_events(mock_kubernetes, "stuff")),
     ]
+    await asyncio.sleep(0.2)
 
     # Creating a pod should by default create an event in that namespace.
     pod = V1Pod(
         metadata=V1ObjectMeta(name="foo"),
         spec=V1PodSpec(
             containers=[
                 V1Container(
@@ -176,14 +182,58 @@
 
     # The first event should have been the pod running event.
     assert result[0]["message"] == "Pod foo started"
     assert result[0]["involved_object"]["kind"] == "Pod"
     assert result[0]["involved_object"]["name"] == "foo"
     assert result[0]["involved_object"]["namespace"] == "stuff"
 
+    # Starting with resource version "1" should skip the first event, since
+    # the semantics of a watch are to show any events *after* the provided
+    # resource version.
+    events = await watch_events(mock_kubernetes, "stuff", resource_version="1")
+    assert events == result[1:]
+
+    # Not specifying a resource version should wait for new events but not see
+    # any of the existing events. (Tasks do not start immediately, so we have
+    # to wait after creating the task to ensure that it starts running and
+    # decides what resource version to start waiting at before we post another
+    # event.)
+    watcher = asyncio.create_task(watch_events(mock_kubernetes, "stuff"))
+    await asyncio.sleep(0.1)
+    event = CoreV1Event(
+        metadata=V1ObjectMeta(name="some-event"),
+        message="Done second time",
+        involved_object=V1ObjectReference(
+            kind="Pod", name="foo", namespace="stuff"
+        ),
+    )
+    await mock_kubernetes.create_namespaced_event("stuff", event)
+    events = await watcher
+    assert len(events) == 1
+    assert events[0]["message"] == "Done second time"
+
+
+async def watch_pod_events(
+    mock_kubernetes: MockKubernetesApi, name: str, namespace: str
+) -> list[dict[str, Any]]:
+    """Watch pod events, returning when the pod is deleted."""
+    method = mock_kubernetes.list_namespaced_pod
+    watch_args = {
+        "field_selector": f"metadata.name={name}",
+        "namespace": namespace,
+        "timeout_seconds": 10,  # Just in case, so tests don't hang
+    }
+    async with Watch().stream(method, **watch_args) as stream:
+        seen = []
+        async for event in stream:
+            seen.append(event)
+            if event["type"] == "DELETED":
+                return seen
+        return seen
+
 
 @pytest.mark.asyncio
 async def test_pod_status(mock_kubernetes: MockKubernetesApi) -> None:
     pod = V1Pod(
         metadata=V1ObjectMeta(name="foo"),
         spec=V1PodSpec(
             containers=[
@@ -215,7 +265,30 @@
         ),
     )
     await mock_kubernetes.create_namespaced_pod("other", pod)
     status = await mock_kubernetes.read_namespaced_pod_status("foo", "other")
     assert status.status.phase == "Starting"
     events = await mock_kubernetes.list_namespaced_event("other")
     assert events.items == []
+    watchers = [
+        asyncio.create_task(watch_pod_events(mock_kubernetes, "foo", "other")),
+        asyncio.create_task(watch_pod_events(mock_kubernetes, "foo", "other")),
+        asyncio.create_task(watch_pod_events(mock_kubernetes, "foo", "other")),
+    ]
+    await asyncio.sleep(0.1)
+    await mock_kubernetes.patch_namespaced_pod_status(
+        "foo",
+        "other",
+        [{"op": "replace", "path": "/status/phase", "value": "Running"}],
+    )
+    await mock_kubernetes.delete_namespaced_pod("foo", "other")
+
+    # All three watches should see the same thing.
+    results = await asyncio.gather(*watchers)
+    assert len(results) == 3
+    assert results[0] == results[1]
+    assert results[0] == results[2]
+    result = results[0]
+    assert result[0]["type"] == "MODIFIED"
+    assert result[0]["object"]["status"]["phase"] == "Running"
+    assert result[1]["type"] == "DELETED"
+    assert result[1]["object"] == result[0]["object"]
```

### Comparing `safir-4.0.0/tox.ini` & `safir-4.1.0/tox.ini`

 * *Files identical despite different names*

