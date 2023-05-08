# Comparing `tmp/project-structure-0.8.28b0.tar.gz` & `tmp/project-structure-0.8.28b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-structure-0.8.28b0.tar", last modified: Fri May  5 22:56:26 2023, max compression
+gzip compressed data, was "project-structure-0.8.28b3.tar", last modified: Mon May  8 18:13:02 2023, max compression
```

## Comparing `project-structure-0.8.28b0.tar` & `project-structure-0.8.28b3.tar`

### file list

```diff
@@ -1,134 +1,139 @@
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      821 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.cz.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.dir-locals.el.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1716 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.dockerignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1058 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.env.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.123400 project-structure-0.8.28b0/.github/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/.github/workflows/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4573 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1716 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6288 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.gitlab-ci.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.pre-commit-config.yaml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2471 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.prospector.yaml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/.reuse/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.reuse/dep5
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/.tox/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5403 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/CONTRIBUTING.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2555 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/Dockerfile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3374 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/Dockerfile.devel
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/LICENSES/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/LICENSES/MIT.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    59098 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      140 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/NEWS-VERSION.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    13245 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/NEWS.rst
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17779 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/PKG-INFO
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/README.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/TODO.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/cz-check-bump
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/entrypoint
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/get-base-version
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/bin/hadolint
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/build-host/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2150 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/Dockerfile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/README.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/build-host/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/bin/entrypoint
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/build-host/requirements.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/dist/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/dist/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5290 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/docker-compose.override.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/gitlab-runner/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/gitlab-runner/config/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/home/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/home/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/home/.pypirc.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/newsfragments/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/newsfragments/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/pyproject.toml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/build.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2383 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py310/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5053 2023-05-05 22:53:41.000000 project-structure-0.8.28b0/requirements/py310/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-05 22:53:31.000000 project-structure-0.8.28b0/requirements/py310/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2383 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py311/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4827 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py311/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py311/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2660 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py37/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5501 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py37/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py37/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2503 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py38/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5093 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py38/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py38/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/requirements/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2381 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py39/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5080 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py39/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/requirements/py39/user.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1652 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/setup.cfg
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.123400 project-structure-0.8.28b0/src/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/src/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/project_structure.egg-info/.gitignore
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17779 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/PKG-INFO
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2460 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/entry_points.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      143 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/requires.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/src/projectstructure/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/__main__.py
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/src/projectstructure/tests/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/tests/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/tests/test_cli.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/src/projectstructure/utils.py
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      164 2023-05-05 22:56:26.000000 project-structure-0.8.28b0/src/projectstructure/version.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/towncrier.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3306 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/tox.ini
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py310/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py310/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py310/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py310/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py310/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py311/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py311/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py311/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py311/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py311/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py37/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py37/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py37/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py37/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py37/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py38/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py38/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py38/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py38/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py38/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py39/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py39/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py39/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-05 22:56:26.127400 project-structure-0.8.28b0/var-docker/py39/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-05 22:47:20.000000 project-structure-0.8.28b0/var-docker/py39/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      821 2023-05-08 18:03:37.000000 project-structure-0.8.28b3/.cz.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.dir-locals.el.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.dockerignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1064 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.env.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.831143 project-structure-0.8.28b3/.github/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/.github/workflows/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4573 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.github/workflows/build-test.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6288 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.gitlab-ci.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.pre-commit-config.yaml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2472 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.prospector.yaml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/.reuse/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.reuse/dep5
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.tox/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5411 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/CONTRIBUTING.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4838 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/Dockerfile
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/LICENSES/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/LICENSES/MIT.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    59879 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      140 2023-05-08 18:03:35.000000 project-structure-0.8.28b3/NEWS-VERSION.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    13718 2023-05-08 18:03:37.000000 project-structure-0.8.28b3/NEWS.rst
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/PKG-INFO
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/README.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/TODO.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/cz-check-bump
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/entrypoint
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/get-base-version
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/hadolint
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1480 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/host-install
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/build-host/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2151 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/Dockerfile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/README.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/build-host/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/bin/entrypoint
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-08 18:12:07.000000 project-structure-0.8.28b3/build-host/requirements-py310.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py311.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py37.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py38.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py39.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/dist/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/dist/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5277 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/docker-compose.override.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/gitlab-runner/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/gitlab-runner/config/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/home/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/home/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/home/.pypirc.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/newsfragments/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/newsfragments/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/pyproject.toml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/build.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py310/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4720 2023-05-08 18:12:07.000000 project-structure-0.8.28b3/requirements/py310/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      864 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py310/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-08 18:12:07.000000 project-structure-0.8.28b3/requirements/py310/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4548 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      749 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2659 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5138 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1072 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2502 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4760 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2380 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4747 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/user.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1660 2023-05-08 18:13:02.839143 project-structure-0.8.28b3/setup.cfg
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.831143 project-structure-0.8.28b3/src/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/src/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/project_structure.egg-info/.gitignore
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2597 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      151 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/requires.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/src/projectstructure/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/__main__.py
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/src/projectstructure/tests/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/tests/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/tests/test_cli.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/utils.py
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      164 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/projectstructure/version.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/towncrier.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3579 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/tox.ini
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py310/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py310/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py310/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py310/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py310/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py311/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py311/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py311/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py311/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py311/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py37/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py37/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py37/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py37/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py37/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py38/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py38/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py38/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py38/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py38/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py39/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py39/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py39/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py39/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py39/project_structure.egg-info/.gitignore
```

### Comparing `project-structure-0.8.28b0/.cz.toml` & `project-structure-0.8.28b3/.cz.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.28b0"
+version = "0.8.28b3"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `project-structure-0.8.28b0/.dir-locals.el.in` & `project-structure-0.8.28b3/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/.dockerignore` & `project-structure-0.8.28b3/.dockerignore`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 # pyenv
 .python-version
 
 # celery beat schedule file
 celerybeat-schedule
 
 # dotenv
-.env
+/.env
 
 # virtualenv
 venv/
 ENV/
 
 # Spyder project settings
 .spyderproject
```

### Comparing `project-structure-0.8.28b0/.env.in` & `project-structure-0.8.28b3/.env.in`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 # SPDX-License-Identifier: MIT
 
 # Make non-default `./docker-compose*.yml` files the default
 # https://pscheit.medium.com/docker-compose-advanced-configuration-541356d121de#9aa6
 COMPOSE_PATH_SEPARATOR=:
 COMPOSE_FILE=./docker-compose.yml:./gitlab-runner/docker-compose.yml:./docker-compose.override.yml
 
-# Capture local values specific to this checkout
+# Capture local values specific to this checkout:
 TZ=${TZ}
 PUID=${PUID}
 PGID=${PGID}
-# Absolute path of the git repo checkout, useful where relative paths can't be used
+# Absolute path of the git repo checkout, useful where relative paths can't be used:
 CHECKOUT_DIR=${CHECKOUT_DIR}
-# Build host variables
+# Build host variables:
 DOCKER_GID=${DOCKER_GID}
-# Release variables
+
+# Release variables:
 DOCKER_USER=${DOCKER_USER}
 # Best to create and use a token.  Note that the token must have the `admin`/"Read,
 # Write, Delete" scope, aka "ACCESS PERMISSIONS":
 # https://hub.docker.com/settings/security?generateToken=true
 DOCKER_PASS=${DOCKER_PASS}
+
 # Project host credentials used here and in CI/CD to support local testing/debugging:
 CI_REGISTRY_PASSWORD=${CI_REGISTRY_PASSWORD}
 PROJECT_GITHUB_PAT=${PROJECT_GITHUB_PAT}
```

### Comparing `project-structure-0.8.28b0/.github/workflows/build-test.yml` & `project-structure-0.8.28b3/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/.gitignore` & `project-structure-0.8.28b3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 # pyenv
 .python-version
 
 # celery beat schedule file
 celerybeat-schedule
 
 # dotenv
-.env
+/.env
 
 # virtualenv
 venv/
 ENV/
 
 # Spyder project settings
 .spyderproject
```

### Comparing `project-structure-0.8.28b0/.gitlab-ci.yml` & `project-structure-0.8.28b3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/.pre-commit-config.yaml` & `project-structure-0.8.28b3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/.prospector.yaml` & `project-structure-0.8.28b3/.prospector.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   run: false
 # Deprecated in favor of PyFlakes:
 # https://github.com/timothycrosley/deprecated.frosted#important-note-frosted-is-deprecated-long-live-flake8
 # frosted:
 #   run: true
 # FIXME: I confirmed the package is installed but couldn't get to work:
 #     Cannot run tool pyroma as support was not installed.
-#     Please install by running 'pip install prospector[with_pyroma]'
+#     Please install by running 'pip3 install prospector[with_pyroma]'
 # pyroma:
 #   run: true
 
 pyflakes:
   disable:
     # Redundant with `pylint - unused-import`.
     # If a line disables that error with a `  # pylint: disable=unused-import` comment,
```

### Comparing `project-structure-0.8.28b0/.reuse/dep5` & `project-structure-0.8.28b3/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/CONTRIBUTING.rst` & `project-structure-0.8.28b3/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
   $ make
 
 If there's not already `an issue/ticket`_ for the changes you'll be making, create one.
 Regardless, take note of the issue/ticket number, e.g. ``#123``.  Then create a
 branch/fork off of the ``develop`` branch::
 
-  $ git switch -c feat-123-foo-bar origin/develop
+  $ git switch -c feat-123-foo-bar --track origin/develop
 
 This project uses `towncrier`_ to manage it's release notes, AKA changelog and thus
 requires at least one `news fragment`_ before merging back into ``develop``.  The VCS
 hooks enforce this when pushing to ``develop`` or ``main``::
 
   $ towncrier create 123.feature
```

### Comparing `project-structure-0.8.28b0/Dockerfile.devel` & `project-structure-0.8.28b3/Dockerfile`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,120 @@
 # SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 #
 # SPDX-License-Identifier: MIT
 
-## Container image for use by developers
 
-# Stay as close to the end user image as possible for build cache efficiency.
-# Then add everything that might contribute to efficient development
+## Image layers shared between all variants.
+
+# Stay as close to a vanilla Python environment as possible
 ARG PYTHON_MINOR=3.10
-FROM python:${PYTHON_MINOR}
+FROM python:${PYTHON_MINOR} AS base
+# Defensive shell options:
+SHELL ["/bin/bash", "-eu", "-o", "pipefail", "-c"]
+
+# Least volatile layers first:
+# https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
+LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/project-structure"
+LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/project-structure"
+LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/project-structure"
+LABEL org.opencontainers.image.title="Project Structure"
+LABEL org.opencontainers.image.description="Project structure foundation or template"
+LABEL org.opencontainers.image.licenses="MIT"
+LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
+LABEL org.opencontainers.image.vendor="rpatterson.net"
+LABEL org.opencontainers.image.base.name="docker.io/library/python:${PYTHON_MINOR}"
+
+# Find the same home directory even when run as another user, e.g. `root`.
+ENV HOME="/home/project-structure"
+ENTRYPOINT [ "entrypoint" ]
+CMD [ "project-structure" ]
+
+# Put the `ENTRYPOINT` on the `$PATH`
+COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
 
+# Install OS packages needed for the image `ENDPOINT`:
 RUN \
     rm -f /etc/apt/apt.conf.d/docker-clean && \
     echo 'Binary::apt::APT::Keep-Downloaded-Packages "true";' \
     >"/etc/apt/apt.conf.d/keep-cache"
 RUN --mount=type=cache,target=/var/cache/apt,sharing=locked \
     --mount=type=cache,target=/var/lib/apt,sharing=locked \
     apt-get update && \
-    apt-get install --no-install-recommends -y gosu=1.12-1+b6
-# Put the `ENTRYPOINT` on the `$PATH`
-COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
+    apt-get install --no-install-recommends -y "gosu=1.12-1+b6"
 
 WORKDIR "/usr/local/src/project-structure/"
 # Install dependencies with fixed versions in a separate layer to optimize build times
 # because this step takes the most time and changes the least frequently.
 ARG PYTHON_ENV=py310
 COPY [ "./requirements/${PYTHON_ENV}/user.txt", "./requirements/${PYTHON_ENV}/" ]
 # hadolint ignore=DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
-    pip install -r "./requirements/${PYTHON_ENV}/user.txt"
-# End of layers shared with the end-user `./Dockerfile` image.
+    pip3 install -r "./requirements/${PYTHON_ENV}/user.txt"
 
-# Match local development tool chain and avoid time consuming redundant package
-# installs.  Initialize the `$ tox -e py3##` Python virtual environment to install this
-# package and all the development tools into the image.
-ARG PYTHON_ENV=py310
-COPY [ "./build-host/requirements-${PYTHON_ENV}.txt", "./build-host/" ]
-# hadolint ignore=DL3042
-RUN --mount=type=cache,target=/root/.cache,sharing=locked \
-    pip install -r "./build-host/requirements-${PYTHON_ENV}.txt"
-COPY [ "./requirements/${PYTHON_ENV}/devel.txt", "./requirements/${PYTHON_ENV}/" ]
-COPY [ "./tox.ini", "./" ]
+# Build-time `LABEL`s
+ARG VERSION=
+LABEL org.opencontainers.image.version=${VERSION}
+
+
+## Container image for use by end users.
+
+# Stay as close to a vanilla environment as possible:
+FROM base AS user
+# Defensive shell options:
+SHELL ["/bin/bash", "-eu", "-o", "pipefail", "-c"]
+
+# Least volatile layers first:
+WORKDIR "/home/project-structure/"
+
+# Install this package in the most common/standard Python way while still being able to
+# build the image locally.
+ARG PYTHON_WHEEL
+COPY [ "${PYTHON_WHEEL}", "${PYTHON_WHEEL}" ]
+# hadolint ignore=DL3013,DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
-    tox --skip-pkg-install --notest -e "${PYTHON_ENV}"
+    pip3 install "${PYTHON_WHEEL}" && \
+    rm -rfv "./dist/"
+
+
+## Container image for use by developers.
+
+# Stay as close to the end user image as possible for build cache efficiency:
+FROM base AS devel
+# Defensive shell options:
+SHELL ["/bin/bash", "-eu", "-o", "pipefail", "-c"]
+
+# Least volatile layers first:
+LABEL org.opencontainers.image.title="Project Structure Development"
+LABEL org.opencontainers.image.description="Project structure foundation or template, development image"
+
 # Activate the Python virtual environment
 ENV VIRTUAL_ENV="/usr/local/src/project-structure/.tox/${PYTHON_ENV}"
 ENV PATH="${VIRTUAL_ENV}/bin:${PATH}"
-
-# Remain in the checkout `WORKDIR` and make the primary testing tool for the default
+# Remain in the checkout `WORKDIR` and make the build tools the default
 # command to run.
-ENV HOME="/home/project-structure"
-ENV PYTHON_ENV="${PYTHON_ENV}"
-ENTRYPOINT [ "entrypoint" ]
+WORKDIR "/usr/local/src/project-structure/"
 # Have to use the shell form of `CMD` because we need variable substitution:
 # hadolint ignore=DL3025
 CMD tox -e "${PYTHON_ENV}"
 
-# https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
-LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/project-structure"
-LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/project-structure"
-LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/project-structure"
-LABEL org.opencontainers.image.title="Project Structure Development"
-LABEL org.opencontainers.image.description="Project structure foundation or template, development image"
-LABEL org.opencontainers.image.licenses="MIT"
-LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
-LABEL org.opencontainers.image.vendor="rpatterson.net"
-LABEL org.opencontainers.image.base.name="docker.io/library/python:${PYTHON_MINOR}"
-# Build-time `LABEL`s
-ARG VERSION=
-LABEL org.opencontainers.image.version=${VERSION}
+# Then add everything that might contribute to efficient development.
+
+# Simulate the parts of the host install process from `./Makefile` needed for
+# development in the image:
+COPY [ "./build-host/requirements.txt.in", "./build-host/" ]
+# hadolint ignore=DL3042
+RUN --mount=type=cache,target=/root/.cache,sharing=locked \
+    mkdir -pv "${HOME}/.local/var/log/" && \
+    pip3 install -r "./build-host/requirements.txt.in" | \
+        tee -a "${HOME}/.local/var/log/project-structure-host-install.log"
+
+# Match local development tool chain and avoid time consuming redundant package
+# installs.  Initialize the `$ tox -e py3##` Python virtual environment to install this
+# package and all the development tools into the image:
+COPY [ \
+    "./requirements/${PYTHON_ENV}/test.txt", \
+    "./requirements/${PYTHON_ENV}/devel.txt", \
+    "./requirements/${PYTHON_ENV}/" \
+]
+COPY [ "./tox.ini", "./" ]
+RUN --mount=type=cache,target=/root/.cache,sharing=locked \
+    tox --no-recreate-pkg --skip-pkg-install --notest -e "${PYTHON_ENV}"
```

### Comparing `project-structure-0.8.28b0/LICENSES/MIT.txt` & `project-structure-0.8.28b3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/Makefile` & `project-structure-0.8.28b3/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 export TZ
 export DOCKER_GID=$(shell getent group "docker" | cut -d ":" -f 3)
 
 # Values concerning supported Python versions:
 # Use the same Python version tox would as a default.
 # https://tox.wiki/en/latest/config.html#base_python
 PYTHON_HOST_MINOR:=$(shell \
-    pip --version | sed -nE 's|.* \(python ([0-9]+.[0-9]+)\)$$|\1|p;q')
+    pip3 --version | sed -nE 's|.* \(python ([0-9]+.[0-9]+)\)$$|\1|p;q')
 export PYTHON_HOST_ENV=py$(subst .,,$(PYTHON_HOST_MINOR))
 # Determine the latest installed Python version of the supported versions
 PYTHON_BASENAMES=$(PYTHON_SUPPORTED_MINORS:%=python%)
 PYTHON_AVAIL_EXECS:=$(foreach \
     PYTHON_BASENAME,$(PYTHON_BASENAMES),$(shell which $(PYTHON_BASENAME)))
 PYTHON_LATEST_EXEC=$(firstword $(PYTHON_AVAIL_EXECS))
 PYTHON_LATEST_BASENAME=$(notdir $(PYTHON_LATEST_EXEC))
@@ -82,23 +82,24 @@
 # Fallback to the latest installed supported Python version
 PYTHON_MINOR=$(PYTHON_LATEST_BASENAME:python%=%)
 endif
 PYTHON_LATEST_MINOR=$(firstword $(PYTHON_SUPPORTED_MINORS))
 PYTHON_LATEST_ENV=py$(subst .,,$(PYTHON_LATEST_MINOR))
 PYTHON_MINORS=$(PYTHON_SUPPORTED_MINORS)
 ifeq ($(PYTHON_MINOR),)
-export PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
+PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
 else ifeq ($(findstring $(PYTHON_MINOR),$(PYTHON_MINORS)),)
-export PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
+PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
 endif
 export PYTHON_MINOR
 export PYTHON_ENV=py$(subst .,,$(PYTHON_MINOR))
 PYTHON_SHORT_MINORS=$(subst .,,$(PYTHON_MINORS))
 PYTHON_ENVS=$(PYTHON_SHORT_MINORS:%=py%)
 PYTHON_ALL_ENVS=$(PYTHON_ENVS) build
+PYTHON_EXTRAS=test devel
 export PYTHON_WHEEL=
 
 # Values derived from VCS/git:
 VCS_LOCAL_BRANCH:=$(shell git branch --show-current)
 CI_COMMIT_BRANCH=
 GITHUB_REF_TYPE=
 GITHUB_REF_NAME=
@@ -258,16 +259,20 @@
 endif
 # Values used to run built images in containers:
 DOCKER_COMPOSE_RUN_ARGS=
 DOCKER_COMPOSE_RUN_ARGS+= --rm
 ifeq ($(shell tty),not a tty)
 DOCKER_COMPOSE_RUN_ARGS+= -T
 endif
+export DOCKER_PASS
 
 # Values derived from or overridden by CI environments:
+ifeq ($(CI),true)
+TEMPLATE_IGNORE_EXISTING=true
+endif
 GITHUB_REPOSITORY_OWNER=$(CI_UPSTREAM_NAMESPACE)
 # Determine if this checkout is a fork of the upstream project:
 CI_IS_FORK=false
 ifeq ($(GITLAB_CI),true)
 USER_EMAIL=$(USER_NAME)@runners-manager.gitlab.com
 ifneq ($(VCS_BRANCH),develop)
 ifneq ($(VCS_BRANCH),main)
@@ -358,61 +363,69 @@
 export CI_PROJECT_ID
 CI_JOB_TOKEN=
 export CI_JOB_TOKEN
 CI_REGISTRY_PASSWORD=
 export CI_REGISTRY_PASSWORD
 GH_TOKEN=
 
+# Override variable values if present in `./.env` and if not overridden on the CLI:
+include $(wildcard .env)
+
 # Done with `$(shell ...)`, echo recipe commands going forward
 .SHELLFLAGS+= -x
 
 
-## Makefile "functions":
-#
-# Snippets whose output is frequently used including across recipes.  Used for output
-# only, not actually making any changes.
-# https://www.gnu.org/software/make/manual/html_node/Call-Function.html
-
-# Return the most recently built package:
-current_pkg = $(shell ls -t ./dist/*$(1) | head -n 1)
-
-
 ## Top-level targets:
 
 .PHONY: all
 ### The default target.
 all: build
 
 .PHONY: start
 ### Run the local development end-to-end stack services in the background as daemons.
-start: build-docker-$(PYTHON_MINOR) ./.env
+start: build-docker-$(PYTHON_MINOR) ./.env.~out~
 	docker compose down
 	docker compose up -d
 
 .PHONY: run
 ### Run the local development end-to-end stack services in the foreground for debugging.
-run: build-docker-$(PYTHON_MINOR) ./.env
+run: build-docker-$(PYTHON_MINOR) ./.env.~out~
 	docker compose down
 	docker compose up
 
 
 ## Build Targets:
 #
 # Recipes that make artifacts needed for by end-users, development tasks, other recipes.
 
 .PHONY: build
 ### Set up everything for development from a checkout, local and in containers.
-build: ./.git/hooks/pre-commit \
+build: ./.git/hooks/pre-commit ./.env.~out~ \
 		$(HOME)/.local/var/log/project-structure-host-install.log \
 		build-docker
 
+.PHONY: $(PYTHON_ENVS:%=build-requirements-%)
+### Compile fixed/pinned dependency versions if necessary.
+$(PYTHON_ENVS:%=build-requirements-%):
+# Avoid parallel tox recreations stomping on each other
+	$(MAKE) -e "$(@:build-requirements-%=./.tox/%/bin/pip-compile)"
+	targets="./requirements/$(@:build-requirements-%=%)/user.txt \
+	    $(PYTHON_EXTRAS:%=./requirements/$(@:build-requirements-%=%)/%.txt) \
+	    ./requirements/$(@:build-requirements-%=%)/build.txt \
+	    ./build-host/requirements-$(@:build-requirements-%=%).txt"
+# Workaround race conditions in pip's HTTP file cache:
+# https://github.com/pypa/pip/issues/6970#issuecomment-527678672
+	$(MAKE) -e -j $${targets} ||
+	    $(MAKE) -e -j $${targets} ||
+	    $(MAKE) -e -j $${targets}
+
 .PHONY: build-requirements-compile
 ### Compile the requirements for one Python version and one type/extra.
 build-requirements-compile:
-	$(MAKE) -e "./var/log/tox/$(PYTHON_ENV)/build.log"
+	$(MAKE) -e "./.tox/$(PYTHON_ENV)/bin/pip-compile"
 	pip_compile_opts="--resolver backtracking --upgrade"
 ifneq ($(PIP_COMPILE_EXTRA),)
 	pip_compile_opts+=" --extra $(PIP_COMPILE_EXTRA)"
 endif
 	./.tox/$(PYTHON_ENV)/bin/pip-compile $${pip_compile_opts} \
 	    --output-file "$(PIP_COMPILE_OUT)" "$(PIP_COMPILE_SRC)"
 
@@ -434,40 +447,26 @@
 # Also build the source distribution:
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
 	    tox run -e "$(PYTHON_ENV)" --override "testenv.package=sdist" --pkg-only
 	cp -lfv "$$(
 	    ls -t ./var-docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.tar.gz | head -n 1
 	)" "./dist/"
 
-.PHONY: $(PYTHON_ENVS:%=build-requirements-%)
-### Compile fixed/pinned dependency versions if necessary.
-$(PYTHON_ENVS:%=build-requirements-%):
-# Avoid parallel tox recreations stomping on each other
-	$(MAKE) -e "$(@:build-requirements-%=./var/log/tox/%/build.log)"
-	targets="./requirements/$(@:build-requirements-%=%)/user.txt \
-	    ./requirements/$(@:build-requirements-%=%)/devel.txt \
-	    ./requirements/$(@:build-requirements-%=%)/build.txt \
-	    ./build-host/requirements-$(@:build-requirements-%=%).txt"
-# Workaround race conditions in pip's HTTP file cache:
-# https://github.com/pypa/pip/issues/6970#issuecomment-527678672
-	$(MAKE) -e -j $${targets} ||
-	    $(MAKE) -e -j $${targets} ||
-	    $(MAKE) -e -j $${targets}
-
 ## Docker Build Targets:
 #
 # Strive for as much consistency as possible in development tasks between the local host
 # and inside containers.  To that end, most of the `*-docker` container target recipes
 # should run the corresponding `*-local` local host target recipes inside the
 # development container.  Top level targets, like `test`, should run as much as possible
 # inside the development container.
 
 .PHONY: build-docker
 ### Set up for development in Docker containers.
-build-docker: build-pkgs ./var/log/tox/build/build.log
+build-docker: build-pkgs ./var-docker/$(PYTHON_ENV)/log/build-user.log
+	tox run $(TOX_EXEC_OPTS) --notest -e "build"
 	$(MAKE) -e -j PYTHON_WHEEL="$(call current_pkg,.whl)" \
 	    DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --progress plain" \
 	    $(PYTHON_MINORS:%=build-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=build-docker-%)
 ### Set up for development in a Docker container for one Python version.
 $(PYTHON_MINORS:%=build-docker-%):
@@ -481,21 +480,20 @@
 ### Print the list of image tags for the current registry and variant.
 build-docker-tags:
 	$(MAKE) -e $(DOCKER_REGISTRIES:%=build-docker-tags-%)
 
 .PHONY: $(DOCKER_REGISTRIES:%=build-docker-tags-%)
 ### Print the list of image tags for the current registry and variant.
 $(DOCKER_REGISTRIES:%=build-docker-tags-%): \
-		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		./var/log/tox/build/build.log
+		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)
 	docker_image=$(DOCKER_IMAGE_$(@:build-docker-tags-%=%))
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)
 ifeq ($(VCS_BRANCH),main)
 # Only update tags end users may depend on to be stable from the `main` branch
-	VERSION=$$(./.tox/build/bin/cz version --project)
+	VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
 	major_version=$$(echo $${VERSION} | sed -nE 's|([0-9]+).*|\1|p')
 	minor_version=$$(
 	    echo $${VERSION} | sed -nE 's|([0-9]+\.[0-9]+).*|\1|p'
 	)
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-v$${minor_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-v$${major_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)
@@ -512,16 +510,16 @@
 	echo $${docker_image}:$(DOCKER_VARIANT)
 endif
 endif
 endif
 
 .PHONY: build-docker-build
 ### Run the actual commands used to build the Docker container image.
-build-docker-build: $(HOME)/.local/var/log/docker-multi-platform-host-install.log \
-		./var/log/tox/build/build.log \
+build-docker-build: ./Dockerfile \
+		$(HOME)/.local/var/log/docker-multi-platform-host-install.log \
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/docker-login-DOCKER.log
 # Workaround broken interactive session detection:
 	docker pull "python:$(PYTHON_MINOR)"
 	docker_build_caches=""
 ifeq ($(GITLAB_CI),true)
 # Don't cache when building final releases on `main`
@@ -540,32 +538,39 @@
 	if $(MAKE) -e pull-docker
 	then
 	    docker_build_caches+=" --cache-from $(DOCKER_IMAGE_GITHUB):\
 	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 	fi
 endif
 endif
-	docker_image_tags=""
+	docker_build_args=""
 	for image_tag in $$(
 	    $(MAKE) -e --no-print-directory build-docker-tags
 	)
 	do
-	    docker_image_tags+="--tag $${image_tag} "
+	    docker_build_args+=" --tag $${image_tag}"
 	done
+ifeq ($(DOCKER_VARIANT),)
+	docker_build_args+=" --target user"
+else
+	docker_build_args+=" --target $(DOCKER_VARIANT)"
+endif
 # https://github.com/moby/moby/issues/39003#issuecomment-879441675
 	docker buildx build $(DOCKER_BUILD_ARGS) \
 	    --build-arg BUILDKIT_INLINE_CACHE="1" \
 	    --build-arg PYTHON_MINOR="$(PYTHON_MINOR)" \
 	    --build-arg PYTHON_ENV="$(PYTHON_ENV)" \
-	    --build-arg VERSION="$$(./.tox/build/bin/cz version --project)" \
-	    $${docker_image_tags} $${docker_build_caches} --file "$(DOCKER_FILE)" "./"
+	    --build-arg VERSION="$$(
+	        $(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project
+	    )" \
+	    $${docker_build_args} $${docker_build_caches} --file "$(<)" "./"
 
 .PHONY: $(PYTHON_MINORS:%=build-docker-requirements-%)
 ### Pull container images and compile fixed/pinned dependency versions if necessary.
-$(PYTHON_MINORS:%=build-docker-requirements-%): ./.env
+$(PYTHON_MINORS:%=build-docker-requirements-%): ./.env.~out~
 	export PYTHON_MINOR="$(@:build-docker-requirements-%=%)"
 	export PYTHON_ENV="py$(subst .,,$(@:build-docker-requirements-%=%))"
 	$(MAKE) -e "./var-docker/$${PYTHON_ENV}/log/build-devel.log"
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
 	    make -e PYTHON_MINORS="$(@:build-docker-requirements-%=%)" \
 	    PIP_COMPILE_ARGS="$(PIP_COMPILE_ARGS)" \
 	    build-requirements-py$(subst .,,$(@:build-docker-requirements-%=%))
@@ -581,21 +586,23 @@
 
 .PHONY: test-local
 ### Run the full suite of tests, coverage checks, and linters on the local host.
 test-local:
 	tox $(TOX_RUN_ARGS) -e "$(TOX_ENV_LIST)"
 
 .PHONY: test-debug
-### Run tests in the host environment and invoke the debugger on errors/failures.
-test-debug: ./var/log/tox/$(PYTHON_ENV)/editable.log
+### Run tests directly on the host and invoke the debugger on errors/failures.
+test-debug: ./.tox/$(PYTHON_ENV)/log/editable.log
 	$(TOX_EXEC_ARGS) -- pytest --pdb
 
 .PHONY: test-docker
 ### Run the full suite of tests, coverage checks, and code linters in containers.
-test-docker: build-pkgs ./var/log/tox/build/build.log ./var/log/codecov-install.log
+test-docker: build-pkgs $(HOME)/.local/var/log/project-structure-host-install.log \
+		build-docker ./var/log/codecov-install.log
+	tox run $(TOX_EXEC_OPTS) --notest -e "build"
 	$(MAKE) -e -j PYTHON_WHEEL="$(call current_pkg,.whl)" \
 	    DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --progress plain" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=test-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=test-docker-%)
 ### Run the full suite of tests inside a docker container for one Python version.
@@ -604,15 +611,17 @@
 	    PYTHON_MINORS="$(@:test-docker-%=%)" \
 	    PYTHON_MINOR="$(@:test-docker-%=%)" \
 	    PYTHON_ENV="py$(subst .,,$(@:test-docker-%=%))" \
 	    test-docker-pyminor
 
 .PHONY: test-docker-pyminor
 ### Run the full suite of tests inside a docker container for this Python version.
-test-docker-pyminor: build-docker-$(PYTHON_MINOR) ./var/log/codecov-install.log
+test-docker-pyminor: build-docker-$(PYTHON_MINOR) \
+		$(HOME)/.local/var/log/project-structure-host-install.log \
+		./var/log/codecov-install.log
 	docker_run_args="--rm"
 	if [ ! -t 0 ]
 	then
 # No fancy output when running in parallel
 	    docker_run_args+=" -T"
 	fi
 # Ensure the dist/package has been correctly installed in the image
@@ -636,27 +645,25 @@
 	false
 endif
 endif
 endif
 
 .PHONY: test-docker-lint
 ### Check the style and content of the `./Dockerfile*` files.
-test-docker-lint: ./.env ./var/log/docker-login-DOCKER.log
+test-docker-lint: ./.env.~out~ ./var/log/docker-login-DOCKER.log
 	docker compose pull --quiet hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
-	    hadolint "./Dockerfile.devel"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
 .PHONY: test-push
 ### Perform any checks that should only be run before pushing.
 test-push: $(VCS_FETCH_TARGETS) \
 		$(HOME)/.local/var/log/project-structure-host-install.log \
-		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env.~out~
 	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)"
 ifeq ($(CI),true)
 ifneq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 # Don't waste CI time, only check for the canonical version:
 	exit
 endif
 ifeq ($(VCS_COMPARE_BRANCH),main)
@@ -707,16 +714,17 @@
 .PHONY: release
 ### Publish installable Python packages and container images as required by commits.
 release: release-pkgs release-docker
 
 .PHONY: release-pkgs
 ### Publish installable Python packages to PyPI if conventional commits require.
 release-pkgs: $(HOME)/.local/var/log/project-structure-host-install.log \
-		./var/log/tox/build/build.log ./var/log/git-remotes.log \
-		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) ~/.pypirc ./.env
+		./var/log/git-remotes.log \
+		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) ~/.pypirc.~out~ \
+		./.env.~out~
 # Only release from the `main` or `develop` branches:
 ifeq ($(RELEASE_PUBLISH),true)
 # Import the private signing key from CI secrets
 	$(MAKE) -e ./var/log/gpg-import.log
 # Bump the version and build the final release packages:
 	$(MAKE) -e build-pkgs
 # https://twine.readthedocs.io/en/latest/#using-twine
@@ -724,15 +732,15 @@
 # The VCS remote should reflect the release before the release is published to ensure
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
 	./.tox/build/bin/twine upload -s -r "$(PYPI_REPO)" \
 	    ./dist/project?structure-*
-	export VERSION=$$(./.tox/build/bin/cz version --project)
+	export VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
 # Create a GitLab release
 	./.tox/build/bin/twine upload -s -r "gitlab" \
 	    ./dist/project?structure-*
 	release_cli_args="--description ./NEWS-VERSION.rst"
 	release_cli_args+=" --tag-name v$${VERSION}"
 	release_cli_args+=" --assets-link {\
 	\"name\":\"PyPI\",\
@@ -774,58 +782,58 @@
 # previously built native images into the manifests.
 	DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --push"
 ifneq ($(DOCKER_PLATFORMS),)
 	DOCKER_BUILD_ARGS+=" --platform $(subst $(EMPTY) ,$(COMMA),$(DOCKER_PLATFORMS))"
 else
 endif
 	export DOCKER_BUILD_ARGS
-# Push the development manifest and images:
-	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
-	    build-docker-build
 # Push the end-user manifest and images:
 	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
 	$(MAKE) -e DOCKER_BUILD_ARGS="$${DOCKER_BUILD_ARGS}\
 	    --build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build
-# Update Docker Hub `README.md` from the official/canonical Python version:
+# Push the development manifest and images:
+	$(MAKE) -e DOCKER_VARIANT="devel" build-docker-build
+# Update Docker Hub `README.md` using the `./README.rst` reStructuredText version using
+# the official/canonical Python version:
 ifeq ($(VCS_BRANCH),main)
 	if [ "$${PYTHON_ENV}" == "$(PYTHON_HOST_ENV)" ]
 	then
 	    $(MAKE) -e "./var/log/docker-login-DOCKER.log"
 	    docker compose pull --quiet pandoc docker-pushrm
 	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
 	fi
 endif
 
 .PHONY: release-bump
 ### Bump the package version if on a branch that should trigger a release.
 release-bump: ~/.gitconfig $(VCS_RELEASE_FETCH_TARGETS) \
-		./var/log/git-remotes.log ./var/log/tox/build/build.log \
+		./var/log/git-remotes.log \
 		$(HOME)/.local/var/log/project-structure-host-install.log \
-		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env.~out~
 	if ! git diff --cached --exit-code
 	then
 	    set +x
 	    echo "CRITICAL: Cannot bump version with staged changes"
 	    false
 	fi
 # Ensure the local branch is updated to the forthcoming version bump commit:
-	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)" --
+	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)"
 # Check if a release is required:
 	exit_code=0
 	if [ "$(VCS_BRANCH)" = "main" ] &&
-	    ./.tox/build/bin/python ./bin/get-base-version $$(
-	        ./.tox/build/bin/cz version --project
+	    $(TOX_EXEC_BUILD_ARGS) -qq -- python ./bin/get-base-version $$(
+	        $(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project
 	    )
 	then
 # Release a previous pre-release as final regardless of whether commits since then
 # require a release:
 	    true
 	else
 # Is a release required by conventional commits:
-	    ./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
+	    $(TOX_EXEC_BUILD_ARGS) -qq -- python ./bin/cz-check-bump || exit_code=$$?
 	    if (( $$exit_code == 3 || $$exit_code == 21 ))
 	    then
 # No commits require a release:
 	        exit
 	    elif (( $$exit_code != 0 ))
 	    then
 	        exit $$exit_code
@@ -867,15 +875,15 @@
 ifeq ($(VCS_BRANCH),main)
 # Merge the bumped version back into `develop`:
 	$(MAKE) VCS_BRANCH="main" VCS_MERGE_BRANCH="develop" \
 	    VCS_REMOTE="$(VCS_COMPARE_REMOTE)" VCS_MERGE_BRANCH="develop" devel-merge
 ifeq ($(CI),true)
 	git push --no-verify "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
 endif
-	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)" --
+	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)"
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
 # Ensure the tag is available for creating the GitHub release below but push *before* to
 # GitLab to avoid a race with repository mirrorying:
 	git push --no-verify "github" tag "v$${next_version}"
 endif
@@ -901,17 +909,16 @@
 	$(TOX_EXEC_ARGS) -- autopep8 -v -i -r "./src/projectstructure/"
 	$(TOX_EXEC_ARGS) -- black "./src/projectstructure/"
 	$(TOX_EXEC_ARGS) -- reuse addheader -r --skip-unrecognised \
 	    --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "./"
 
 .PHONY: devel-upgrade
 ### Update all fixed/pinned dependencies to their latest available versions.
-devel-upgrade: ./.env $(HOME)/.local/var/log/project-structure-host-install.log \
-		./var-docker/$(PYTHON_ENV)/log/build-devel.log \
-		./var/log/tox/build/build.log
+devel-upgrade: ./.env.~out~ $(HOME)/.local/var/log/project-structure-host-install.log \
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log
 	touch "./setup.cfg" "./requirements/build.txt.in" \
 	    "./build-host/requirements.txt.in"
 # Ensure the network is create first to avoid race conditions
 	docker compose create project-structure-devel
 	$(MAKE) -e -j PIP_COMPILE_ARGS="--upgrade" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=build-docker-requirements-%)
@@ -924,15 +931,15 @@
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/git-remotes.log
 	remote_branch_exists=false
 	if git fetch "$(VCS_REMOTE)" "$(VCS_BRANCH)-upgrade"
 	then
 	    remote_branch_exists=true
 	fi
-	git switch -C "$(VCS_BRANCH)-upgrade" --track "$(VCS_BRANCH)" --
+	git switch -C "$(VCS_BRANCH)-upgrade"
 	now=$$(date -u)
 	$(MAKE) -e devel-upgrade
 	if $(MAKE) -e "test-clean"
 	then
 # No changes from upgrade, exit successfully but push nothing
 	    exit
 	fi
@@ -986,31 +993,35 @@
 ### Restore the checkout to a state as close to an initial clone as possible.
 clean:
 	docker compose down --remove-orphans --rmi "all" -v || true
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit uninstall \
 	    --hook-type "pre-commit" --hook-type "commit-msg" --hook-type "pre-push" \
 	    || true
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit clean || true
-	git clean -dfx -e "var/" -e ".env"
+	git clean -dfx -e "/var" -e "var-docker/" -e "/.env" -e "*~"
 	git clean -dfx "./var-docker/py*/.tox/" \
 	    "./var-docker/py*/project_structure.egg-info/"
 	rm -rfv "./var/log/" "./var-docker/py*/log/"
 
 
 ## Real Targets:
 #
 # Recipes that make actual changes and create and update files for the target.
 
 # Manage fixed/pinned versions in `./requirements/**.txt` files.  Has to be run for each
 # python version in the virtual environment for that Python version:
 # https://github.com/jazzband/pip-tools#cross-environment-usage-of-requirementsinrequirementstxt-and-pip-compile
-$(PYTHON_ENVS:%=./requirements/%/devel.txt): ./pyproject.toml ./setup.cfg ./tox.ini
+python_combine_requirements=$(PYTHON_ENVS:%=./requirements/%/$(1).txt)
+$(foreach extra,$(PYTHON_EXTRAS),$(call python_combine_requirements,$(extra))): \
+		./pyproject.toml ./setup.cfg ./tox.ini
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e PYTHON_ENV="$(@:requirements/%/devel.txt=%)" \
-	    PIP_COMPILE_EXTRA="devel" PIP_COMPILE_SRC="$(<)" PIP_COMPILE_OUT="$(@)" \
+	extra_basename="$$(basename "$(@)")"
+	$(MAKE) -e PYTHON_ENV="$$(basename "$$(dirname "$(@)")")" \
+	    PIP_COMPILE_EXTRA="$${extra_basename%.txt}" \
+	    PIP_COMPILE_SRC="$(<)" PIP_COMPILE_OUT="$(@)" \
 	    build-requirements-compile
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./requirements/%/user.txt): ./pyproject.toml ./setup.cfg ./tox.ini
 	true DEBUG Updated prereqs: $(?)
 	$(MAKE) -e PYTHON_ENV="$(@:requirements/%/user.txt=%)" PIP_COMPILE_SRC="$(<)" \
 	    PIP_COMPILE_OUT="$(@)" build-requirements-compile
@@ -1022,17 +1033,17 @@
 	    PIP_COMPILE_SRC="$(<)" PIP_COMPILE_OUT="$(@)" build-requirements-compile
 # Only update the installed tox version for the latest/host/main/default Python version
 	if [ "$(@:build-host/requirements-%.txt=%)" = "$(PYTHON_ENV)" ]
 	then
 # Don't install tox into one of it's own virtual environments
 	    if [ -n "$${VIRTUAL_ENV:-}" ]
 	    then
-	        pip_bin="$$(which -a pip | grep -v "^$${VIRTUAL_ENV}/bin/" | head -n 1)"
+	        pip_bin="$$(which -a pip3 | grep -v "^$${VIRTUAL_ENV}/bin/" | head -n 1)"
 	    else
-	        pip_bin="pip"
+	        pip_bin="pip3"
 	    fi
 	    "$${pip_bin}" install -r "$(@)"
 	fi
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./requirements/%/build.txt): ./requirements/build.txt.in
 	true DEBUG Updated prereqs: $(?)
@@ -1040,53 +1051,59 @@
 	    PIP_COMPILE_OUT="$(@)" build-requirements-compile
 
 # Targets used as pre-requisites to ensure virtual environments managed by tox have been
 # created and can be used directly to save time on Tox's overhead when we don't need
 # Tox's logic about when to update/recreate them, e.g.:
 #     $ ./.tox/build/bin/cz --help
 # Mostly useful for build/release tools.
-$(PYTHON_ALL_ENVS:%=./var/log/tox/%/build.log):
+$(PYTHON_ALL_ENVS:%=./.tox/%/bin/pip-compile):
 	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
-	mkdir -pv "$(dir $(@))"
-	tox run $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/build.log=%)" --notest |&
-	    tee -a "$(@)"
+	tox run $(TOX_EXEC_OPTS) -e "$(@:.tox/%/bin/pip-compile=%)" --notest
 # Workaround tox's `usedevelop = true` not working with `./pyproject.toml`.  Use as a
 # prerequisite when using Tox-managed virtual environments directly and changes to code
 # need to take effect immediately.
-$(PYTHON_ENVS:%=./var/log/tox/%/editable.log):
+$(PYTHON_ENVS:%=./.tox/%/log/editable.log):
 	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
 	mkdir -pv "$(dir $(@))"
-	tox exec $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/editable.log=%)" -- \
-	    pip install -e "./" |& tee -a "$(@)"
+	tox exec $(TOX_EXEC_OPTS) -e "$(@:./.tox/%/log/editable.log=%)" -- \
+	    pip3 install -e "./" |& tee -a "$(@)"
 
 ## Docker real targets:
 
 # Build the development image:
-./var-docker/$(PYTHON_ENV)/log/build-devel.log: \
-		./Dockerfile.devel ./.dockerignore ./bin/entrypoint \
+./var-docker/$(PYTHON_ENV)/log/build-devel.log: ./Dockerfile ./.dockerignore \
+		./bin/entrypoint ./build-host/requirements.txt.in \
+		./var-docker/$(PYTHON_ENV)/log/rebuild.log \
 		./pyproject.toml ./setup.cfg ./tox.ini \
-		./build-host/requirements.txt.in ./docker-compose.yml \
-		./docker-compose.override.yml ./.env \
-		./var-docker/$(PYTHON_ENV)/log/rebuild.log
+		./docker-compose.yml ./docker-compose.override.yml ./.env.~out~ \
+		./bin/host-install
 	true DEBUG Updated prereqs: $(?)
 	mkdir -pv "$(dir $(@))"
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
 	    touch "$(@)" "./var-docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
-	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
-	        project-structure-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
-	        "./var/log/tox/$(PYTHON_ENV)/build.log"
+	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	        tox run $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" --notest
 	    exit
 	fi
 endif
-	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
-	    DOCKER_BUILD_ARGS="--load" build-docker-build >>"$(@)"
+	$(MAKE) -e DOCKER_VARIANT="devel" DOCKER_BUILD_ARGS="--load" \
+	    build-docker-build | tee -a "$(@)"
+# Represent that host install is baked into the image in the `${HOME}` bind volume:
+	docker compose run --rm -T --workdir "/home/project-structure/" \
+	    --entrypoint "mkdir" project-structure-devel -pv "./.local/var/log/"
+	docker run --rm --workdir "/home/project-structure/" --entrypoint "cat" \
+	    "$$(docker compose config --images project-structure-devel | head -n 1)" \
+	    "./.local/var/log/project-structure-host-install.log" |
+	    docker compose run --rm -T --workdir "/home/project-structure/" \
+	        --entrypoint "tee" project-structure-devel -a \
+	        "./.local/var/log/project-structure-host-install.log" >"/dev/null"
 # Update the pinned/frozen versions, if needed, using the container.  If changed, then
 # we may need to re-build the container image again to ensure it's current and correct.
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
 	    make -e PYTHON_MINORS="$(PYTHON_MINOR)" build-requirements-$(PYTHON_ENV)
 ifeq ($(CI),true)
 # On CI, any changes from compiling requirements is a failure so no need to waste time
 # rebuilding images:
@@ -1094,14 +1111,15 @@
 else
 	$(MAKE) -e "$(@)"
 endif
 
 # Build the end-user image:
 ./var-docker/$(PYTHON_ENV)/log/build-user.log: \
 		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
+		./.dockerignore ./bin/entrypoint ./build-host/requirements.txt.in \
 		./var-docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
 ifeq ($(PYTHON_WHEEL),)
 	$(MAKE) -e "build-pkgs"
 	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
 endif
 # Build the end-user image now that all required artifacts are built"
@@ -1113,57 +1131,26 @@
 
 # Marker file used to trigger the rebuild of the image for just one Python version.
 # Useful to workaround async timestamp issues when running jobs in parallel:
 ./var-docker/$(PYTHON_ENV)/log/rebuild.log:
 	mkdir -pv "$(dir $(@))"
 	date >>"$(@)"
 
-# Local environment variables from a template:
-./.env: ./.env.in
-	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
+# Local environment variables and secrets from a template:
+./.env.~out~: ./.env.in
+	$(call expand_template,$(<),$(@))
 
 # Install all tools required by recipes that have to be installed externally on the
 # host.  Use a target file outside this checkout to support multiple checkouts.  Use a
 # target specific to this project so that other projects can use the same approach but
 # with different requirements.
-$(HOME)/.local/var/log/project-structure-host-install.log:
+$(HOME)/.local/var/log/project-structure-host-install.log: ./bin/host-install \
+		./build-host/requirements.txt.in
 	mkdir -pv "$(dir $(@))"
-	(
-	    if ! which pip
-	    then
-	        if which apk
-	        then
-	            sudo apk update
-	            sudo apk add \
-# We need `$ envsubst` in the `expand-template:` target recipe:
-	                "gettext" \
-# We need `$ pip3` to install the project's Python tools:
-	                "py3-pip" \
-# Needed for dependencies we can't get current versions for locally:
-	                "docker-cli-compose" \
-# Needed for publishing releases from CI/CD:
-	                "gnupg" "github-cli" "curl"
-	        elif which apt-get
-	        then
-	            sudo apt-get update
-	            sudo apt-get install -y "gettext-base" "python3-pip" \
-	                "docker-compose-plugin" "gnupg" "gh" "curl"
-	        else
-	            set +x
-	            echo "ERROR: OS not supported for installing host dependencies"
-	            false
-	        fi
-	    fi
-	    if [ -e ./build-host/requirements-$(PYTHON_HOST_ENV).txt ]
-	    then
-	        pip install -r "./build-host/requirements-$(PYTHON_HOST_ENV).txt"
-	    else
-	        pip install -r "./build-host/requirements.txt.in"
-	    fi
-	) |& tee -a "$(@)"
+	"$(<)" |& tee -a "$(@)"
 
 # https://docs.docker.com/build/building/multi-platform/#building-multi-platform-images
 $(HOME)/.local/var/log/docker-multi-platform-host-install.log:
 	mkdir -pv "$(dir $(@))"
 	if ! docker context inspect "multi-platform" |& tee -a "$(@)"
 	then
 	    docker context create "multi-platform" |& tee -a "$(@)"
@@ -1233,16 +1220,16 @@
 
 # Capture any project initialization tasks for reference.  Not actually usable.
 ./pyproject.toml:
 	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
 	$(TOX_EXEC_BUILD_ARGS) -- cz init
 
 # Tell Emacs where to find checkout-local tools needed to check the code.
-./.dir-locals.el: ./.dir-locals.el.in
-	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
+./.dir-locals.el.~out~: ./.dir-locals.el.in
+	$(call expand_template,$(<),$(@))
 
 # Ensure minimal VCS configuration, mostly useful in automation such as CI.
 ~/.gitconfig:
 	git config --global user.name "$(USER_FULL_NAME)"
 	git config --global user.email "$(USER_EMAIL)"
 
 ./var/log/git-remotes.log:
@@ -1274,60 +1261,51 @@
 endif
 endif
 	set -x
 # Fail fast if there's still no push access
 	git push --no-verify "origin" "HEAD:$(VCS_BRANCH)" | tee -a "$(@)"
 
 # Ensure release publishing authentication, mostly useful in automation such as CI.
-~/.pypirc: ./home/.pypirc.in
-	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
+~/.pypirc.~out~: ./home/.pypirc.in
+	$(call expand_template,$(<),$(@))
 
-./var/log/docker-login-DOCKER.log: ./.env
+./var/log/docker-login-DOCKER.log:
+	$(MAKE) "./.env.~out~"
 	mkdir -pv "$(dir $(@))"
-	set +x
-	source "./.env"
-	export DOCKER_PASS
 	if [ -n "$${DOCKER_PASS}" ]
 	then
-	    set -x
 	    printenv "DOCKER_PASS" | docker login -u "merpatterson" --password-stdin
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: DOCKER_PASS missing from ./.env or CI secrets"
 	    false
 	fi
 	date | tee -a "$(@)"
 # TEMPLATE: Add a cleanup rule for the GitLab container registry under the project
 # settings.
-./var/log/docker-login-GITLAB.log: ./.env
+./var/log/docker-login-GITLAB.log:
+	$(MAKE) "./.env.~out~"
 	mkdir -pv "$(dir $(@))"
-	set +x
-	source "./.env"
-	export CI_REGISTRY_PASSWORD
 	if [ -n "$${CI_REGISTRY_PASSWORD}" ]
 	then
-	    set -x
 	    printenv "CI_REGISTRY_PASSWORD" |
 	        docker login -u "$(CI_REGISTRY_USER)" --password-stdin "$(CI_REGISTRY)"
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: CI_REGISTRY_PASSWORD missing from ./.env or CI secrets"
 	    false
 	fi
 	date | tee -a "$(@)"
 # TEMPLATE: Connect the GitHub container registry to the repository using the `Connect`
 # button at the bottom of the container registry's web UI.
-./var/log/docker-login-GITHUB.log: ./.env
+./var/log/docker-login-GITHUB.log:
+	$(MAKE) "./.env.~out~"
 	mkdir -pv "$(dir $(@))"
-	set +x
-	source "./.env"
-	export PROJECT_GITHUB_PAT
 	if [ -n "$${PROJECT_GITHUB_PAT}" ]
 	then
-	    set -x
 	    printenv "PROJECT_GITHUB_PAT" |
 	        docker login -u "$(GITHUB_REPOSITORY_OWNER)" --password-stdin "ghcr.io"
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	    false
 	fi
@@ -1394,73 +1372,58 @@
 # prerequisite, apply the appropriate changes and then  run using `$ docker compose up
 # gitlab-runner`.  Particularly useful to conserve shared runner minutes:
 ./var/gitlab-runner/config/config.toml: ./gitlab-runner/config/config.toml.in
 	docker compose run --rm gitlab-runner register \
 	    --url "https://gitlab.com/" --docker-image "docker" --executor "docker"
 
 
-## Utility Targets:
+## Makefile "functions":
 #
-# Recipes used to make similar changes across targets where using Make's basic syntax
-# can't be used.
-
-.PHONY: expand-template
-## Create a file from a template replacing environment variables
-expand-template:
-	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
-	set +x
-	if [ -e "$(target)" ]
-	then
-ifeq ($(TEMPLATE_IGNORE_EXISTING),true)
-	    exit
-else
-	    envsubst <"$(template)" | diff -u "$(target)" "-" || true
-	    echo "ERROR: Template $(template) has been updated:"
-	    echo "       Reconcile changes and \`$$ touch $(target)\`:"
-	    false
-endif
-	fi
-	envsubst <"$(template)" >"$(target)"
-
-.PHONY: pull-docker
-### Pull an existing image best to use as a cache for building new images
-pull-docker: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		./var/log/tox/build/build.log
-	export VERSION=$$(./.tox/build/bin/cz version --project)
-	for vcs_branch in $(VCS_BRANCHES)
-	do
-	    docker_tag="$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${vcs_branch}"
-	    for docker_image in $(DOCKER_IMAGES)
-	    do
-	        if docker pull "$${docker_image}:$${docker_tag}"
-	        then
-	            docker tag "$${docker_image}:$${docker_tag}" \
-	                "$(DOCKER_IMAGE_DOCKER):$${docker_tag}"
-	            exit
-	        fi
-	    done
-	done
-	set +x
-	echo "ERROR: Could not pull any existing docker image"
-	false
+# Snippets whose output is frequently used including across recipes:
+# https://www.gnu.org/software/make/manual/html_node/Call-Function.html
 
-# TEMPLATE: Run this once for your project.  See the `./var/log/docker-login*.log`
-# targets for the authentication environment variables that need to be set or just login
-# to those container registries manually and touch these targets.
-.PHONY: bootstrap-project
-### Run any tasks needed to be run once for a given project by a maintainer
-bootstrap-project: \
-		./var/log/docker-login-GITLAB.log \
-		./var/log/docker-login-GITHUB.log
-# Initially seed the build host Docker image to bootstrap CI/CD environments
-# GitLab CI/CD:
-	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITLAB)" release
-# GitHub Actions:
-	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITHUB)" release
+# Return the most recently built package:
+current_pkg=$(shell ls -t ./dist/*$(1) | head -n 1)
 
+# Have to use a placeholder `*.~out~` as the target instead of the real expanded
+# template because we can't disable `.DELETE_ON_ERROR` on a per-target basis.
+#
+# Short-circuit/repeat the host-install recipe here because expanded templates should
+# *not* be updated when `./bin/host-install` is, so we can't use it as a prerequisite,
+# *but* it is required to expand templates.  We can't use a sub-make because any
+# expanded templates we use in `include ...` directives, such as `./.env`, are updated
+# as targets when reading the `./Makefile` leading to endless recursion.
+define expand_template=
+if ! which envsubst
+then
+    mkdir -pv "$(HOME)/.local/var/log/"
+    ./bin/host-install >"$(HOME)/.local/var/log/project-structure-host-install.log"
+fi
+is_target_newer="0"
+test "$(2:%.~out~=%)" -nt "$(1)" || is_target_newer="$${?}"
+touch "$(2:%.~out~=%)"
+if [ "$(CI)" != "true" ]
+then
+    envsubst <"$(1)" | diff -u "$(2:%.~out~=%)" "-" || true
+fi
+set +x
+echo "WARNING:Template $(1) has been updated."
+echo "        Reconcile changes and \`$$ touch $(2:%.~out~=%)\`."
+set -x
+if [ ! -s "$(2:%.~out~=%)" ]
+then
+    envsubst <"$(1)" >"$(2:%.~out~=%)"
+fi
+if [ "$(TEMPLATE_IGNORE_EXISTING)" == "true" ] || (( "$${is_target_newer}" == 0 ))
+then
+    envsubst <"$(1)" >"$(2)"
+    exit
+fi
+exit 1
+endef
 
 ## Makefile Development:
 #
 # Development primarily requires a balance of 2 priorities:
 #
 # - Ensure the correctness of the code and build artifacts
 # - Minimize iteration time overhead in the inner loop of development
@@ -1531,7 +1494,48 @@
 #   Overriding variables on the command-line when invoking make as "options"
 #
 # We want to avoid, however, using many more features of Make, particularly the more
 # "magical" features, to keep it readable, discover-able, and otherwise accessible to
 # developers who may not have significant familiarity with Make.  If there's a good,
 # pragmatic reason to add use of further features feel free to make the case but avoid
 # them if possible.
+
+
+## Maintainer targets:
+#
+# Recipes not used during the normal course of development.
+
+.PHONY: pull-docker
+### Pull an existing image best to use as a cache for building new images
+pull-docker: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
+		$(HOME)/.local/var/log/project-structure-host-install.log
+	export VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
+	for vcs_branch in $(VCS_BRANCHES)
+	do
+	    docker_tag="$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${vcs_branch}"
+	    for docker_image in $(DOCKER_IMAGES)
+	    do
+	        if docker pull "$${docker_image}:$${docker_tag}"
+	        then
+	            docker tag "$${docker_image}:$${docker_tag}" \
+	                "$(DOCKER_IMAGE_DOCKER):$${docker_tag}"
+	            exit
+	        fi
+	    done
+	done
+	set +x
+	echo "ERROR: Could not pull any existing docker image"
+	false
+
+# TEMPLATE: Run this once for your project.  See the `./var/log/docker-login*.log`
+# targets for the authentication environment variables that need to be set or just login
+# to those container registries manually and touch these targets.
+.PHONY: bootstrap-project
+### Run any tasks needed to be run once for a given project by a maintainer
+bootstrap-project: \
+		./var/log/docker-login-GITLAB.log \
+		./var/log/docker-login-GITHUB.log
+# Initially seed the build host Docker image to bootstrap CI/CD environments
+# GitLab CI/CD:
+	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITLAB)" release
+# GitHub Actions:
+	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITHUB)" release
```

### Comparing `project-structure-0.8.28b0/NEWS.rst` & `project-structure-0.8.28b3/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+project-structure 0.8.28b3 (2023-05-08)
+=======================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+project-structure 0.8.28b2 (2023-05-08)
+=======================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+project-structure 0.8.28b1 (2023-05-08)
+=======================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Sun May  7 09:27:36 AM UTC 2023.
+
+
 project-structure 0.8.28b0 (2023-05-05)
 =======================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `project-structure-0.8.28b0/PKG-INFO` & `project-structure-0.8.28b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.28b0
+Version: 0.8.28b3
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: devel
 
 .. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 ..
 .. SPDX-License-Identifier: MIT
 
 ########################################################################################
```

### Comparing `project-structure-0.8.28b0/README.rst` & `project-structure-0.8.28b3/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/TODO.rst` & `project-structure-0.8.28b3/TODO.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/bin/cz-check-bump` & `project-structure-0.8.28b3/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/bin/entrypoint` & `project-structure-0.8.28b3/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/bin/get-base-version` & `project-structure-0.8.28b3/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/Dockerfile` & `project-structure-0.8.28b3/build-host/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Find the same home directory even when run as another user, e.g. `root`.
 ENV HOME="/home/runner"
 # Add user installs to PATH
 ENV PATH="${HOME}/.local/bin:${PATH}"
 
 COPY [ "./requirements-py310.txt", "${HOME}/.local/lib/" ]
 RUN mkdir -pv "${HOME}/.local/var/log/" && \
-    pip install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
+    pip3 install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
     >"${HOME}/.local/var/log/project-structure-host-install.log"
 
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
 ENTRYPOINT [ "docker-entrypoint.sh", "entrypoint" ]
 CMD [ "make", "-e", "build-docker" ]
 
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
```

### Comparing `project-structure-0.8.28b0/build-host/Makefile` & `project-structure-0.8.28b3/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/README.rst` & `project-structure-0.8.28b3/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/bin/entrypoint` & `project-structure-0.8.28b3/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/requirements-py310.txt` & `project-structure-0.8.28b3/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/requirements-py311.txt` & `project-structure-0.8.28b3/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/requirements-py37.txt` & `project-structure-0.8.28b3/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/requirements-py38.txt` & `project-structure-0.8.28b3/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/build-host/requirements-py39.txt` & `project-structure-0.8.28b3/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/docker-compose.override.yml` & `project-structure-0.8.28b3/docker-compose.override.yml`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   project-structure:
     image: "\
       ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/project-structure\
       :${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "project-structure-checkout"
     build:
       context: "${CHECKOUT_DIR:-.}/"
+      target: "user"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     volumes:
       # Preserve caches caches between container runs
       - "${CHECKOUT_DIR:-.}/home/:/home/project-structure/"
@@ -33,15 +34,15 @@
       ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/project-structure\
       :devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "project-structure-devel"
     profiles:
       - "test"
     build:
       context: "${CHECKOUT_DIR:-.}/"
-      dockerfile: "${CHECKOUT_DIR:-.}/Dockerfile.devel"
+      target: "devel"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env`
```

### Comparing `project-structure-0.8.28b0/docker-compose.yml` & `project-structure-0.8.28b3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/gitlab-runner/config/config.toml.in` & `project-structure-0.8.28b3/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/gitlab-runner/docker-compose.yml` & `project-structure-0.8.28b3/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/pyproject.toml` & `project-structure-0.8.28b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/requirements/build.txt.in` & `project-structure-0.8.28b3/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/requirements/py310/build.txt` & `project-structure-0.8.28b3/requirements/py310/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
```

### Comparing `project-structure-0.8.28b0/requirements/py310/devel.txt` & `project-structure-0.8.28b3/requirements/py37/devel.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py310/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py37/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via project-structure (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
@@ -24,30 +24,28 @@
     # via project-structure (pyproject.toml)
 boolean-py==4.0
     # via
     #   license-expression
     #   reuse
 build==0.10.0
     # via
-    #   pip-tools
     #   project-structure (pyproject.toml)
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 chardet==5.1.0
     # via
     #   binaryornot
     #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
@@ -60,16 +58,14 @@
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -78,19 +74,26 @@
     # via gitpython
 gitpython==3.1.31
     # via
     #   bandit
     #   prospector
 idna==3.4
     # via requests
+importlib-metadata==4.13.0
+    # via
+    #   argcomplete
+    #   build
+    #   click
+    #   pydocstyle
+    #   rstcheck
+    #   rstcheck-core
+    #   stevedore
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
-isort==5.12.0
+isort==5.11.5
     # via pylint
 jinja2==3.1.2
     # via
     #   reuse
     #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
@@ -113,32 +116,27 @@
     #   mypy
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via project-structure (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-pluggy==1.0.0
-    # via pytest
 prospector[with_everything]==1.9.0
     # via project-structure (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -150,15 +148,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -173,16 +171,14 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via project-structure (pyproject.toml)
 python-debian==0.1.49
     # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   xenon
@@ -213,15 +209,15 @@
     # via typer
 six==1.16.0
     # via mando
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
-stevedore==5.0.0
+stevedore==3.5.2
     # via bandit
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
 tomli==2.0.1
@@ -229,38 +225,49 @@
     #   autoflake
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
-    #   pytest
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via project-structure (pyproject.toml)
 trove-classifiers==2023.5.2
     # via pyroma
+typed-ast==1.5.4
+    # via
+    #   astroid
+    #   black
+    #   mypy
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.9
     # via rstcheck-core
 typing-extensions==4.5.0
     # via
     #   astroid
+    #   black
+    #   gitpython
+    #   importlib-metadata
     #   mypy
+    #   platformdirs
     #   pydantic
+    #   pylint
+    #   rich
+    #   rstcheck
+    #   rstcheck-core
 urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via project-structure (pyproject.toml)
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `project-structure-0.8.28b0/requirements/py311/build.txt` & `project-structure-0.8.28b3/requirements/py311/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
```

### Comparing `project-structure-0.8.28b0/requirements/py311/devel.txt` & `project-structure-0.8.28b3/requirements/py38/devel.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py311/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py38/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via project-structure (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
@@ -24,30 +24,28 @@
     # via project-structure (pyproject.toml)
 boolean-py==4.0
     # via
     #   license-expression
     #   reuse
 build==0.10.0
     # via
-    #   pip-tools
     #   project-structure (pyproject.toml)
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 chardet==5.1.0
     # via
     #   binaryornot
     #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
@@ -78,16 +76,14 @@
     # via
     #   bandit
     #   prospector
 idna==3.4
     # via requests
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via
     #   reuse
     #   towncrier
 lazy-object-proxy==1.9.0
@@ -111,32 +107,27 @@
     #   mypy
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via project-structure (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-pluggy==1.0.0
-    # via pytest
 prospector[with_everything]==1.9.0
     # via project-structure (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -148,15 +139,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -171,16 +162,14 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via project-structure (pyproject.toml)
 python-debian==0.1.49
     # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   xenon
@@ -218,35 +207,46 @@
 stevedore==5.0.0
     # via bandit
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
+tomli==2.0.1
+    # via
+    #   autoflake
+    #   autopep8
+    #   black
+    #   build
+    #   mypy
+    #   pylint
+    #   pyproject-hooks
+    #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via project-structure (pyproject.toml)
 trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.9
     # via rstcheck-core
 typing-extensions==4.5.0
     # via
+    #   astroid
+    #   black
     #   mypy
     #   pydantic
+    #   pylint
+    #   rich
 urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via project-structure (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `project-structure-0.8.28b0/requirements/py37/build.txt` & `project-structure-0.8.28b3/requirements/py37/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
```

### Comparing `project-structure-0.8.28b0/requirements/py37/devel.txt` & `project-structure-0.8.28b3/requirements/py310/devel.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py37/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py310/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via project-structure (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
@@ -24,30 +24,28 @@
     # via project-structure (pyproject.toml)
 boolean-py==4.0
     # via
     #   license-expression
     #   reuse
 build==0.10.0
     # via
-    #   pip-tools
     #   project-structure (pyproject.toml)
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 chardet==5.1.0
     # via
     #   binaryornot
     #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
@@ -60,16 +58,14 @@
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -78,30 +74,17 @@
     # via gitpython
 gitpython==3.1.31
     # via
     #   bandit
     #   prospector
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
-    # via
-    #   argcomplete
-    #   build
-    #   click
-    #   pluggy
-    #   pydocstyle
-    #   pytest
-    #   rstcheck
-    #   rstcheck-core
-    #   stevedore
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
-isort==5.11.5
+isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via
     #   reuse
     #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
@@ -124,32 +107,27 @@
     #   mypy
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via project-structure (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-pluggy==1.0.0
-    # via pytest
 prospector[with_everything]==1.9.0
     # via project-structure (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -161,15 +139,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -184,16 +162,14 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via project-structure (pyproject.toml)
 python-debian==0.1.49
     # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   xenon
@@ -224,15 +200,15 @@
     # via typer
 six==1.16.0
     # via mando
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
-stevedore==3.5.2
+stevedore==5.0.0
     # via bandit
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
 tomli==2.0.1
@@ -240,53 +216,34 @@
     #   autoflake
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
-    #   pytest
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via project-structure (pyproject.toml)
 trove-classifiers==2023.5.2
     # via pyroma
-typed-ast==1.5.4
-    # via
-    #   astroid
-    #   black
-    #   mypy
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.9
     # via rstcheck-core
 typing-extensions==4.5.0
     # via
     #   astroid
-    #   black
-    #   gitpython
-    #   importlib-metadata
     #   mypy
-    #   platformdirs
     #   pydantic
-    #   pylint
-    #   rich
-    #   rstcheck
-    #   rstcheck-core
 urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via project-structure (pyproject.toml)
-zipp==3.15.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `project-structure-0.8.28b0/requirements/py38/build.txt` & `project-structure-0.8.28b3/requirements/py38/build.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
```

### Comparing `project-structure-0.8.28b0/requirements/py38/devel.txt` & `project-structure-0.8.28b3/requirements/py39/devel.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py38/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via project-structure (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
@@ -24,30 +24,28 @@
     # via project-structure (pyproject.toml)
 boolean-py==4.0
     # via
     #   license-expression
     #   reuse
 build==0.10.0
     # via
-    #   pip-tools
     #   project-structure (pyproject.toml)
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 chardet==5.1.0
     # via
     #   binaryornot
     #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
@@ -60,16 +58,14 @@
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -80,16 +76,14 @@
     # via
     #   bandit
     #   prospector
 idna==3.4
     # via requests
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via
     #   reuse
     #   towncrier
 lazy-object-proxy==1.9.0
@@ -113,32 +107,27 @@
     #   mypy
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via project-structure (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-pluggy==1.0.0
-    # via pytest
 prospector[with_everything]==1.9.0
     # via project-structure (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -150,15 +139,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -173,16 +162,14 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via project-structure (pyproject.toml)
 python-debian==0.1.49
     # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   xenon
@@ -229,15 +216,14 @@
     #   autoflake
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
-    #   pytest
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via project-structure (pyproject.toml)
 trove-classifiers==2023.5.2
     # via pyroma
@@ -248,22 +234,18 @@
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
-    #   rich
 urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via project-structure (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `project-structure-0.8.28b0/requirements/py39/build.txt` & `project-structure-0.8.28b3/requirements/py39/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
```

### Comparing `project-structure-0.8.28b0/requirements/py39/devel.txt` & `project-structure-0.8.28b3/requirements/py311/devel.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py311/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via project-structure (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
@@ -24,30 +24,28 @@
     # via project-structure (pyproject.toml)
 boolean-py==4.0
     # via
     #   license-expression
     #   reuse
 build==0.10.0
     # via
-    #   pip-tools
     #   project-structure (pyproject.toml)
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 chardet==5.1.0
     # via
     #   binaryornot
     #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
@@ -60,16 +58,14 @@
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -80,16 +76,14 @@
     # via
     #   bandit
     #   prospector
 idna==3.4
     # via requests
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via
     #   reuse
     #   towncrier
 lazy-object-proxy==1.9.0
@@ -113,32 +107,27 @@
     #   mypy
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via project-structure (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-pluggy==1.0.0
-    # via pytest
 prospector[with_everything]==1.9.0
     # via project-structure (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -150,15 +139,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -173,16 +162,14 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via project-structure (pyproject.toml)
 python-debian==0.1.49
     # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   xenon
@@ -220,49 +207,32 @@
 stevedore==5.0.0
     # via bandit
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
-tomli==2.0.1
-    # via
-    #   autoflake
-    #   autopep8
-    #   black
-    #   build
-    #   mypy
-    #   pylint
-    #   pyproject-hooks
-    #   pytest
-    #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via project-structure (pyproject.toml)
 trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
 types-docutils==0.19.1.9
     # via rstcheck-core
 typing-extensions==4.5.0
     # via
-    #   astroid
-    #   black
     #   mypy
     #   pydantic
-    #   pylint
 urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via project-structure (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `project-structure-0.8.28b0/setup.cfg` & `project-structure-0.8.28b3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -37,25 +37,26 @@
 where = src
 
 [options.entry_points]
 console_scripts = 
 	project-structure = projectstructure:main
 
 [options.extras_require]
-devel = 
+test = 
 	pytest
+	pip-tools
+devel = 
 	coverage
 	prospector[with_everything]
 	xenon
 	rstcheck
 	reuse<1.1.0
 	black
 	autoflake
 	autopep8
-	pip-tools
 	towncrier
 	build
 
 [tool:pytest]
 testpaths = src/projectstructure
 
 [coverage:run]
```

### Comparing `project-structure-0.8.28b0/src/project_structure.egg-info/PKG-INFO` & `project-structure-0.8.28b3/src/project_structure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.28b0
+Version: 0.8.28b3
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: devel
 
 .. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 ..
 .. SPDX-License-Identifier: MIT
 
 ########################################################################################
```

### Comparing `project-structure-0.8.28b0/src/project_structure.egg-info/SOURCES.txt` & `project-structure-0.8.28b3/src/project_structure.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .env.in
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 .prospector.yaml
 CONTRIBUTING.rst
 Dockerfile
-Dockerfile.devel
 Makefile
 NEWS-VERSION.rst
 NEWS.rst
 README.rst
 TODO.rst
 docker-compose.override.yml
 docker-compose.yml
@@ -24,14 +23,15 @@
 .reuse/dep5
 .tox/.gitignore
 LICENSES/MIT.txt
 bin/cz-check-bump
 bin/entrypoint
 bin/get-base-version
 bin/hadolint
+bin/host-install
 build-host/Dockerfile
 build-host/Makefile
 build-host/README.rst
 build-host/requirements-py310.txt
 build-host/requirements-py311.txt
 build-host/requirements-py37.txt
 build-host/requirements-py38.txt
@@ -43,26 +43,31 @@
 gitlab-runner/config/config.toml.in
 home/.gitignore
 home/.pypirc.in
 newsfragments/.gitignore
 requirements/build.txt.in
 requirements/py310/build.txt
 requirements/py310/devel.txt
+requirements/py310/test.txt
 requirements/py310/user.txt
 requirements/py311/build.txt
 requirements/py311/devel.txt
+requirements/py311/test.txt
 requirements/py311/user.txt
 requirements/py37/build.txt
 requirements/py37/devel.txt
+requirements/py37/test.txt
 requirements/py37/user.txt
 requirements/py38/build.txt
 requirements/py38/devel.txt
+requirements/py38/test.txt
 requirements/py38/user.txt
 requirements/py39/build.txt
 requirements/py39/devel.txt
+requirements/py39/test.txt
 requirements/py39/user.txt
 src/project_structure.egg-info/.gitignore
 src/project_structure.egg-info/PKG-INFO
 src/project_structure.egg-info/SOURCES.txt
 src/project_structure.egg-info/dependency_links.txt
 src/project_structure.egg-info/entry_points.txt
 src/project_structure.egg-info/requires.txt
```

### Comparing `project-structure-0.8.28b0/src/projectstructure/__init__.py` & `project-structure-0.8.28b3/src/projectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/src/projectstructure/tests/test_cli.py` & `project-structure-0.8.28b3/src/projectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b0/tox.ini` & `project-structure-0.8.28b3/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,34 @@
 [tox]
 # https://devguide.python.org/versions/#supported-versions
 envlist = py{310,311,39,38,37}
 # https://tox.wiki/en/latest/example/package.html#setuptools
 isolated_build = True
 
 [testenv]
-description = Run tests and checks for code and content
+description = Run the project test suite
 package = wheel
 wheel_build_env = .pkg
-extras = devel
-deps = -rrequirements/{envname}/devel.txt
+passenv =
+    HOME
+    PYTHON_HOST_ENV
+    DEBUG
+extras = test
+deps = -rrequirements/{envname}/test.txt
+commands =
+    pytest --junit-xml="./build/{envname}/pytest-junit.xml" -s
+
+[testenv:py310]
+description = Run the project test suite with coverage and checks for code and content
+extras =
+    test
+    devel
+deps =
+    -rrequirements/{envname}/test.txt
+    -rrequirements/{envname}/devel.txt
 commands =
 # Create a directory for artifacts not managed by `$ tox`:
     python -c 'import pathlib; \
         pathlib.Path("./build/{envname}").mkdir(parents=True, exist_ok=True)'
 # Fail fast.  Run quick tests and checks first to save time in the inner loop of
 # development iteration.
     pyroma --min="10" "./"
@@ -48,16 +63,15 @@
         "./newsfragments/"
 # Check copyright and licensing:
     reuse lint
 # Ensure this package is correctly installed into this environment.
     python -m "projectstructure" --help
     project-structure --help
 # Run more time consuming tests and checks last.
-    coverage run --data-file="./build/{envname}/.coverage" -m pytest \
-        --junit-xml="./build/{envname}/pytest-junit.xml" -s
+    coverage run --data-file="./build/{envname}/.coverage" -m {[testenv]commands}
     coverage json --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage.json"
     coverage lcov --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage-lcov.info"
     coverage xml --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage.xml"
     coverage html --fail-under=0 --data-file="./build/{envname}/.coverage" \
```

