# Comparing `tmp/pollination-apps-0.7.1.tar.gz` & `tmp/pollination-apps-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-apps-0.7.1.tar", last modified: Wed Oct 19 10:18:05 2022, max compression
+gzip compressed data, was "dist/pollination-apps-0.7.2.tar", last modified: Mon May  8 19:13:08 2023, max compression
```

## Comparing `pollination-apps-0.7.1.tar` & `pollination-apps-0.7.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/.dependabot/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/.dependabot/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/docs/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7136 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     8277 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/cli/assets/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/cli/assets/art.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/login.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/assets/
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/assets/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3525 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/config.ini
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/app.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/vtk.Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/pollination_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:18:05.000000 pollination-apps-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-19 10:16:43.000000 pollination-apps-0.7.1/tests/test_true.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.dependabot/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.dependabot/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/cli/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/cli/assets/art.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/vtk.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/tests/test_true.py
```

### Comparing `pollination-apps-0.7.1/.devcontainer/Dockerfile` & `pollination-apps-0.7.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/.devcontainer/devcontainer.json` & `pollination-apps-0.7.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/.github/workflows/ci.yaml` & `pollination-apps-0.7.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/LICENSE` & `pollination-apps-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/PKG-INFO` & `pollination-apps-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-apps
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library to setup and deploy Apps to Pollination!
 Home-page: https://github.com/pollination/pollination-apps
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: MIT
 Description: # Pollination Apps
```

### Comparing `pollination-apps-0.7.1/README.md` & `pollination-apps-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/docs/conf.py` & `pollination-apps-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/cli/__init__.py` & `pollination-apps-0.7.2/pollination_apps/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 from .context import Context
 from ..config import Config
 
 
 MODULE_PATH = os.path.abspath(os.path.dirname(__file__))
 
 
+def _slugify(name):
+    """An internal function to slugify names."""
+    return slugify(name, replacements=[['_', '-']])
+
+
 @click.group(invoke_without_command=True)
 @click.version_option()
 @click.pass_context
 def main(ctx: click.Context):
     """ The Pollination Apps CLI
 
     Use this CLI to create a new app and deploy it to Pollination.
@@ -106,15 +111,15 @@
     for required_file in ('Dockerfile', 'app.py'):
         if not path.joinpath(required_file).is_file():
             raise ClickException(
                 f'Application folder is missing a required file: {required_file}'
             )
 
     owner, name, slug = _read_config(path, owner, name)
-    slug = slug or slugify(name)
+    slug = slug or _slugify(name)
 
     if tag is None:
         tag = 'latest'
 
     try:
         client.update_app(owner=owner, slug=slug, public=public)
     except:
@@ -181,19 +186,19 @@
         if not path.joinpath(required_file).is_file():
             raise ClickException(
                 f'Application folder is missing a required file: {required_file}'
             )
 
     owner, name, slug = _read_config(path, owner, name)
 
-    slug = slug or slugify(name)
+    slug = slug or _slugify(name)
 
     if tag is None:
         tag = 'latest'
-    
+
     # optionally mount the current path as a volume to the container
     volume = f'-v {path}/:/app' if editable else ''
     container_manager = 'docker' if docker else 'podman'
     docker_file = path.joinpath('Dockerfile')
     build_image = f'{container_manager} build -f {docker_file} -t {owner}/{slug}:{tag} {path}'
     run_app = f'{container_manager} run -t -i --expose 8501 -p 8501:8501 {volume} {owner}/{slug}:{tag} streamlit run app.py'
     click.echo(f'Building an image for {owner}/{slug}:{tag}')
@@ -231,26 +236,25 @@
     except KeyboardInterrupt:
         p.send_signal(signal.SIGINT)
 
 
 def _read_config(path, owner, name):
     try:
         config = Config.from_folder(folder=path)
-    except FileNotFoundError as e:
+    except FileNotFoundError:
         if not owner:
             raise ClickException(
                 'To deploy or run an app without a config file you must provide an owner.'
             )
         if not name:
             raise ClickException(
                 'To deploy or run an app without a config file you must provide a name.'
             )
-        slug = slugify(name)
         # create a config file
-        config = Config(name=name, slug=slug, owner=owner)
+        config = Config(name=name, owner=owner)
         config.write(folder=path)
     else:
         owner = config.owner
         name = config.name
-        slug = config.slug
 
+    slug = _slugify(name)
     return owner, name, slug
```

### Comparing `pollination-apps-0.7.1/pollination_apps/cli/assets/art.txt` & `pollination-apps-0.7.2/pollination_apps/cli/assets/art.txt`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/cli/context.py` & `pollination-apps-0.7.2/pollination_apps/cli/context.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/client.py` & `pollination-apps-0.7.2/pollination_apps/client.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/config.py` & `pollination-apps-0.7.2/pollination_apps/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 """Pollination App Config"""
 from dataclasses import dataclass
 import configparser
 import pathlib
 
+
 @dataclass()
 class Config:
     """Pollination app configuration.
 
     Args:
         name: App human readable name. e.g. My first app
-        slug: App's slug. e.g. my-first-app
         owner: App's owner on pollination. e.g. ladybug-tools
 
     """
     name: str
-    slug: str
     owner: str
 
     @classmethod
     def from_file(cls, path: str):
         """Create a config object from a config file.
 
         Args:
             path: Full path to the config.ini file.
 
         """
         parser = configparser.ConfigParser()
         parser.read(path)
         app_info = parser['app']
-        slug = app_info.get('slug')
         owner = app_info.get('owner')
         name = app_info.get('name')
-        return cls(name, slug, owner)
+        return cls(name, owner)
 
     @classmethod
     def from_folder(cls, folder: str):
         """Create a config object from an app folder.
-        
+
         Args:
             folder: Path to app folder. The config file should be located at
                 .pollination/config.ini
 
         """
         config_file = pathlib.Path(folder).joinpath('.pollination', 'config.ini')
         if not config_file.is_file():
@@ -56,11 +54,9 @@
         """
         config_file = pathlib.Path(folder).joinpath('.pollination', 'config.ini')
         config_file.parent.mkdir(parents=True, exist_ok=True)
         config = configparser.ConfigParser()
         config.add_section('app')
         config['app']['owner'] = self.owner
         config['app']['name'] = self.name
-        config['app']['slug'] = self.slug
         with config_file.open('w') as out_ini:
             config.write(out_ini)
-
```

### Comparing `pollination-apps-0.7.1/pollination_apps/env.py` & `pollination-apps-0.7.2/pollination_apps/env.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/login.py` & `pollination-apps-0.7.2/pollination_apps/login.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/template/assets/hooks/post_gen_project.py` & `pollination-apps-0.7.2/pollination_apps/template/assets/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml` & `pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml` & `pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md` & `pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/pollination_apps.egg-info/PKG-INFO` & `pollination-apps-0.7.2/pollination_apps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-apps
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library to setup and deploy Apps to Pollination!
 Home-page: https://github.com/pollination/pollination-apps
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: MIT
 Description: # Pollination Apps
```

### Comparing `pollination-apps-0.7.1/pollination_apps.egg-info/SOURCES.txt` & `pollination-apps-0.7.2/pollination_apps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.1/setup.py` & `pollination-apps-0.7.2/setup.py`

 * *Files identical despite different names*

