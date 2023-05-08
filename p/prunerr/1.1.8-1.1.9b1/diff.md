# Comparing `tmp/prunerr-1.1.8.tar.gz` & `tmp/prunerr-1.1.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prunerr-1.1.8.tar", last modified: Thu Apr 27 19:15:36 2023, max compression
+gzip compressed data, was "prunerr-1.1.9b1.tar", last modified: Fri May  5 23:14:29 2023, max compression
```

## Comparing `prunerr-1.1.8.tar` & `prunerr-1.1.9b1.tar`

### file list

```diff
@@ -1,1374 +1,1419 @@
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.269576 prunerr-1.1.8/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-27 18:36:00.000000 prunerr-1.1.8/.dir-locals.el.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-27 18:36:00.000000 prunerr-1.1.8/.dockerignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1261 2023-04-27 18:36:00.000000 prunerr-1.1.8/.env.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/.github/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/.github/workflows/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-27 18:36:00.000000 prunerr-1.1.8/.github/workflows/build-test.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1557 2023-04-27 18:36:00.000000 prunerr-1.1.8/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4351 2023-04-27 18:36:00.000000 prunerr-1.1.8/.gitlab-ci.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      777 2023-04-27 18:36:00.000000 prunerr-1.1.8/.pre-commit-config.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-27 18:36:00.000000 prunerr-1.1.8/.prospector.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4109 2023-04-27 18:36:00.000000 prunerr-1.1.8/CONTRIBUTING.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2429 2023-04-27 18:36:00.000000 prunerr-1.1.8/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3224 2023-04-27 18:36:00.000000 prunerr-1.1.8/Dockerfile.devel
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-27 18:36:00.000000 prunerr-1.1.8/LICENSE
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    58281 2023-04-27 18:36:00.000000 prunerr-1.1.8/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      161 2023-04-27 18:52:20.000000 prunerr-1.1.8/NEWS-VERSION.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5500 2023-04-27 18:52:20.000000 prunerr-1.1.8/NEWS.rst
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    18069 2023-04-27 19:15:36.269576 prunerr-1.1.8/PKG-INFO
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17084 2023-04-27 18:36:00.000000 prunerr-1.1.8/README.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5038 2023-04-27 18:36:00.000000 prunerr-1.1.8/TODO.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2759 2023-04-27 18:36:00.000000 prunerr-1.1.8/bin/cz-check-bump
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-27 18:36:00.000000 prunerr-1.1.8/bin/entrypoint
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-27 18:36:00.000000 prunerr-1.1.8/bin/get-base-version
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-27 18:36:00.000000 prunerr-1.1.8/bin/hadolint
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/build-host/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-27 18:36:00.000000 prunerr-1.1.8/build-host/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-27 18:36:00.000000 prunerr-1.1.8/build-host/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-27 18:36:00.000000 prunerr-1.1.8/build-host/README.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/build-host/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-27 18:36:00.000000 prunerr-1.1.8/build-host/bin/entrypoint
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      730 2023-04-27 18:50:41.000000 prunerr-1.1.8/build-host/requirements-py310.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      673 2023-04-27 18:50:41.000000 prunerr-1.1.8/build-host/requirements-py311.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      947 2023-04-27 18:50:41.000000 prunerr-1.1.8/build-host/requirements-py37.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      728 2023-04-27 18:50:41.000000 prunerr-1.1.8/build-host/requirements-py38.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      728 2023-04-27 18:50:41.000000 prunerr-1.1.8/build-host/requirements-py39.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-27 18:36:56.000000 prunerr-1.1.8/build-host/requirements.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/dist/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-27 18:36:00.000000 prunerr-1.1.8/dist/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-27 18:36:00.000000 prunerr-1.1.8/docker-compose-servarr.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5132 2023-04-27 18:36:00.000000 prunerr-1.1.8/docker-compose.override.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4047 2023-04-27 18:36:00.000000 prunerr-1.1.8/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/gitlab-runner/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/gitlab-runner/config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-27 18:36:00.000000 prunerr-1.1.8/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      566 2023-04-27 18:36:00.000000 prunerr-1.1.8/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/home/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-27 18:36:00.000000 prunerr-1.1.8/home/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-27 18:36:00.000000 prunerr-1.1.8/home/.pypirc.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3005 2023-04-27 18:52:20.000000 prunerr-1.1.8/pyproject.toml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/requirements/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      668 2023-04-27 18:36:56.000000 prunerr-1.1.8/requirements/build.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/requirements/py310/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     2567 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py310/build.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     5141 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py310/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-27 18:37:14.000000 prunerr-1.1.8/requirements/py310/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/requirements/py311/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     2529 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py311/build.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     4915 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py311/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-27 18:38:04.000000 prunerr-1.1.8/requirements/py311/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/requirements/py37/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     2840 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py37/build.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     5960 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py37/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-27 18:38:38.000000 prunerr-1.1.8/requirements/py37/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/requirements/py38/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     2668 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py38/build.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     5459 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py38/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-27 18:38:20.000000 prunerr-1.1.8/requirements/py38/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/requirements/py39/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     2565 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py39/build.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)     5446 2023-04-27 18:50:41.000000 prunerr-1.1.8/requirements/py39/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-27 18:38:31.000000 prunerr-1.1.8/requirements/py39/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/s6/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/s6/etc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/s6/etc/s6-overlay/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/s6/etc/s6-overlay/s6-rc.d/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.237576 prunerr-1.1.8/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-27 18:36:00.000000 prunerr-1.1.8/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1748 2023-04-27 19:15:36.269576 prunerr-1.1.8/setup.cfg
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8429 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/__main__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/downloaditem.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/home/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10134 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/home/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/newsfragments/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/newsfragments/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/servarr.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/example-5s.mkv
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/home/daemon/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/home/daemon/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/home/download-client-only/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/home/download-clients/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/home/download-clients/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/home/download-items/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/home/download-items/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/empty/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/home/empty/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/home/empty/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/move-exec/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/home/move-exec/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/home/move-exec/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/home/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/home/review-edge-cases/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:14:25.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.205576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:14:25.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.209576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.245576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.213576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.249576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.217576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.253576 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.221576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.257576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.225576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:14:25.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.261576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.229576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:14:25.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:14:25.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.233576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.265576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.269576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.269576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.269576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.269576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.269576 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_cli.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_daemon.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_downloaditem.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_free_space.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_move.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_review.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_servarr.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/tests/test_verify.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-27 18:36:00.000000 prunerr-1.1.8/src/prunerr/utils.py
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      160 2023-04-27 19:15:36.000000 prunerr-1.1.8/src/prunerr/version.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-27 19:15:36.241576 prunerr-1.1.8/src/prunerr.egg-info/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    18069 2023-04-27 19:15:36.000000 prunerr-1.1.8/src/prunerr.egg-info/PKG-INFO
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64656 2023-04-27 19:15:36.000000 prunerr-1.1.8/src/prunerr.egg-info/SOURCES.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-27 19:15:36.000000 prunerr-1.1.8/src/prunerr.egg-info/dependency_links.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-27 19:15:36.000000 prunerr-1.1.8/src/prunerr.egg-info/entry_points.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      312 2023-04-27 19:15:36.000000 prunerr-1.1.8/src/prunerr.egg-info/requires.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-27 19:15:36.000000 prunerr-1.1.8/src/prunerr.egg-info/top_level.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3327 2023-04-27 18:36:00.000000 prunerr-1.1.8/tox.ini
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      677 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.cz.toml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      643 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.dir-locals.el.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1776 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.dockerignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1361 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.env.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/.github/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/.github/workflows/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3998 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1776 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4449 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.gitlab-ci.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      877 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2548 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.prospector.yaml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/.reuse/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      995 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.reuse/dep5
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/.tox/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/.tox/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2529 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3324 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/Dockerfile.devel
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/LICENSES/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1071 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/LICENSES/MIT.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    57970 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      141 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/NEWS-VERSION.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5811 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/NEWS.rst
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    18085 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/PKG-INFO
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17085 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/README.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5141 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/TODO.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2860 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/bin/cz-check-bump
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1022 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/bin/entrypoint
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1202 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/bin/get-base-version
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      422 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/bin/hadolint
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/build-host/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2094 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1564 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      849 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/README.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/build-host/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2142 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      730 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      673 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      947 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      728 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      104 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/build-host/requirements.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/dist/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      222 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/dist/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1497 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/docker-compose-servarr.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5435 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/docker-compose.override.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4147 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/gitlab-runner/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/gitlab-runner/config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1423 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      666 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/home/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      246 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/home/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      427 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/home/.pypirc.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      187 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/newsfragments/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2398 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/pyproject.toml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/requirements/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      679 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/build.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/requirements/py310/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2383 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py310/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5472 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      857 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py310/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/requirements/py311/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2383 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py311/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5246 2023-05-05 23:08:05.000000 prunerr-1.1.9b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      857 2023-05-05 23:07:46.000000 prunerr-1.1.9b1/requirements/py311/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/requirements/py37/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2660 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py37/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     6291 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1396 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py37/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/requirements/py38/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2503 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py38/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5790 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1156 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py38/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/requirements/py39/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2381 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py39/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5777 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1156 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/requirements/py39/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/s6/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/s6/etc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/s6/etc/s6-overlay/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/s6/etc/s6-overlay/s6-rc.d/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      343 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1785 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/setup.cfg
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/src/prunerr/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8530 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      303 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/__main__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15538 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11477 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/downloaditem.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/src/prunerr/home/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10234 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/home/.config/prunerr.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8037 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19164 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11515 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/servarr.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1011 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22119 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/example-5s.mkv
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/home/daemon/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3304 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/home/daemon/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/home/download-client-only/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      190 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/home/download-clients/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3057 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/home/download-clients/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/home/download-items/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      190 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/home/download-items/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/empty/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/home/empty/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      103 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/home/empty/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/move-exec/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/home/move-exec/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      188 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/home/move-exec/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/home/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/home/review-edge-cases/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      920 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:13:17.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.752513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:13:17.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.780513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.756513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.784513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.760513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.764513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.788513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.768513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:13:17.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:13:17.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:13:17.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.792513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.772513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-27 18:36:00.000000 prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4830 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_cli.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3006 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_daemon.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8922 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3845 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_downloaditem.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11450 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_free_space.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17308 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_move.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8174 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13210 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_review.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1568 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1671 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_servarr.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1304 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/tests/test_verify.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1474 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr/utils.py
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      162 2023-05-05 23:14:29.000000 prunerr-1.1.9b1/src/prunerr/version.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/src/prunerr.egg-info/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/src/prunerr.egg-info/.gitignore
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    18085 2023-05-05 23:14:29.000000 prunerr-1.1.9b1/src/prunerr.egg-info/PKG-INFO
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    65331 2023-05-05 23:14:29.000000 prunerr-1.1.9b1/src/prunerr.egg-info/SOURCES.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-05-05 23:14:29.000000 prunerr-1.1.9b1/src/prunerr.egg-info/dependency_links.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-05-05 23:14:29.000000 prunerr-1.1.9b1/src/prunerr.egg-info/entry_points.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      324 2023-05-05 23:14:29.000000 prunerr-1.1.9b1/src/prunerr.egg-info/requires.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-05-05 23:14:29.000000 prunerr-1.1.9b1/src/prunerr.egg-info/top_level.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      262 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/towncrier.toml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3258 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/tox.ini
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      229 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.776513 prunerr-1.1.9b1/var-docker/media/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/media/Library/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/media/Library/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py310/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py310/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py310/.tox/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py310/.tox/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py310/prunerr.egg-info/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py310/prunerr.egg-info/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py311/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py311/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py311/.tox/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py311/.tox/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py311/prunerr.egg-info/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py311/prunerr.egg-info/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py37/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py37/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py37/.tox/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py37/.tox/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py37/prunerr.egg-info/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py37/prunerr.egg-info/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py38/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py38/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py38/.tox/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py38/.tox/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py38/prunerr.egg-info/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py38/prunerr.egg-info/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py39/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py39/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py39/.tox/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py39/.tox/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-05-05 23:14:29.796513 prunerr-1.1.9b1/var-docker/py39/prunerr.egg-info/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      192 2023-05-05 23:01:26.000000 prunerr-1.1.9b1/var-docker/py39/prunerr.egg-info/.gitignore
```

### Comparing `prunerr-1.1.8/.dockerignore` & `prunerr-1.1.9b1/.dockerignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Backup files
 *~
 **/*~
 *.rej
 **/*.rej
 
 # Byte-compiled / optimized / DLL files
@@ -12,27 +16,37 @@
 *$py.class
 **/*$py.class
 
 # C extensions
 *.so
 **/.so
 
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
-var/
+/var
+/var-docker
+/README.md
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
```

### Comparing `prunerr-1.1.8/.env.in` & `prunerr-1.1.9b1/.env.in`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Make non-default `./docker-compose*.yml` files the default
 # https://pscheit.medium.com/docker-compose-advanced-configuration-541356d121de#9aa6
 COMPOSE_PATH_SEPARATOR=:
 COMPOSE_FILE=./docker-compose.yml:./gitlab-runner/docker-compose.yml:./docker-compose-servarr.yml:./docker-compose.override.yml
 
 # Capture local values specific to this checkout
 TZ=${TZ}
```

### Comparing `prunerr-1.1.8/.github/workflows/build-test.yml` & `prunerr-1.1.9b1/.github/workflows/build-test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 name: "Build and Test"
 
 on:
   # Only run on branches, not tags:
   # https://github.com/orgs/community/discussions/25615#discussioncomment-3397691
   push:
     branches:
@@ -74,32 +78,32 @@
       # Upload build artifacts:
       # https://github.com/actions/upload-artifact#usage
       - name: "Archive test suite reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "test-suite-reports"
           path: |
-            ./build/*/pytest*
+            ./build/*test*
       # https://github.com/marketplace/actions/test-reporter#example
       - name: "Publish test suite report"
         uses: "dorny/test-reporter@main"
         # run this step even if previous step failed
         if: >-
           (success() || failure())
           && (
             (! github.event.pull_request)
             || ! (
               (github.repository_owner == 'rpatterson')
               && (github.event.pull_request.head.repo.owner.login != 'rpatterson')
             )
           )
         with:
-          name: "PyTest Test Suite (python${{ matrix.PYTHON_MINORS }})"
+          name: "Test Suite Reports"
           path: >-
-            ./build/*/pytest-junit.xml,
+            ./build/*/*test-junit.xml,
             ./build/*/prospector-xunit.xml
           reporter: "java-junit"
       - name: "Archive code coverage reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "code-coverage-reports"
           path: |
@@ -107,9 +111,9 @@
             ./build/*/coverage*
             ./build/*/htmlcov*
       - name: "Archive linter reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "linter-reports"
           path: |
+            ./build/*/*lint*
             ./build/*/prospector*
-            ./build/*/pylint*
```

### Comparing `prunerr-1.1.8/.gitignore` & `prunerr-1.1.9b1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Backup files
 *~
 **/*~
 *.rej
 **/*.rej
 
 # Byte-compiled / optimized / DLL files
@@ -12,27 +16,37 @@
 *$py.class
 **/*$py.class
 
 # C extensions
 *.so
 **/.so
 
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
-var/
+/var
+/var-docker
+/README.md
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
```

### Comparing `prunerr-1.1.8/.gitlab-ci.yml` & `prunerr-1.1.9b1/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # https://gitlab.com/gitlab-org/gitlab/-/blob/master/lib/gitlab/ci/templates/Docker.gitlab-ci.yml
 
 default:
   image:
     name: "$CI_TEMPLATE_REGISTRY_HOST/rpatterson/$CI_PROJECT_NAME:build-host"
     entrypoint:
       - "docker-entrypoint.sh"
@@ -99,15 +103,15 @@
             && $CI_COMMIT_TITLE =~
         /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+$/
           )
         )
         && $CI_PROJECT_NAMESPACE == "rpatterson"
   script:
     - >-
-      entrypoint make -e release-python test-clean
+      entrypoint make -e release-pkgs test-clean
   artifacts:
     paths:
       - "./dist/prunerr-*"
 
 merge-upgrade:
   stage: "merge-upgrade"
   needs: ["build-test"]
```

### Comparing `prunerr-1.1.8/.pre-commit-config.yaml` & `prunerr-1.1.9b1/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Run all test, linters and other code checks before committing and pushing.
 fail_fast: true
 repos:
 # Check commit message format and style before pushing to a remote
   - repo: "https://github.com/commitizen-tools/commitizen"
-    rev: "3.1.0"
+    rev: "3.2.1"
     hooks:
       - id: "commitizen"
 # Checks defined in the `./Makefile`
   - repo: "local"
     hooks:
 # Fail fast, run quicker checks first
     - id: "test-push"
       name: "test-push"
       stages: ["push"]
       entry: "make -e test-push"
-      language: "python"
+      language: "system"
       pass_filenames: false
 # Only run the longer running test check after everything else
     - id: "test"
       name: "test"
       stages: ["commit", "merge-commit", "push", "manual"]
       entry: "make -e test"
-      language: "python"
+      language: "system"
       pass_filenames: false
```

### Comparing `prunerr-1.1.8/.prospector.yaml` & `prunerr-1.1.9b1/.prospector.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # https://prospector.landscape.io/en/master/profiles.html#global-configuration-options
 strictness: "veryhigh"
 test-warnings: true
 doc-warnings: true
 member-warnings: true
 autodetect: false
 inherits:
```

### Comparing `prunerr-1.1.8/CONTRIBUTING.rst` & `prunerr-1.1.9b1/CONTRIBUTING.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
+
 ########################################################################################
 Contributing
 ########################################################################################
 
 Development requires fairly standard development tools, but ``git`` and ``make`` to
 bootstrap the local development environment.  Once installed, clone the repository::
 
@@ -37,16 +41,32 @@
   $ make test-local
 
 You can also inspect test failures and errors in `Python's post-mortem debugger`_.  This
 also runs locally directly on your development host::
 
   $ make test-debug
 
-The ``$ make test`` target also runs the ``$ make format`` target to format code
-according to this project's guidelines and rules.
+The linters make various decisions on style, formatting, and conventions for you so you
+don't have to think about them and no one has to debate them.  They're enforced by ``$
+make test`` and the VCS hooks.  You may also use the same tools to apply all fixes and
+formatting that can be automated to format code according to this project's guidelines
+and rules::
+
+  $ make devel-format
+
+This project also uses `Reuse`_ to manage licenses and copyright.  If you add files,
+you'll need to put an `SPDX header comment`_ in each added file.  For those file types
+recognized by the `reuse-tool`_, you can use ``$ make devel-format`` to add such headers
+automatically.  Otherwise you may have to use ``$ reuse addheader`` manually specifying
+the appropriate ``--style`` option.  See ``$ reuse addheader --help`` for the available
+``${COMMENT_STYLE}`` values.  You can use ``--style "python"`` for unrecognized file
+types that support the common ``#`` comment style::
+
+  $ tox exec -e build -- reuse addheader --style "${COMMENT_STYLE:?}" \
+  --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "${PATH:?}"
 
 Contributions should be pushed to feature branches or forks off of the upstream
 ``develop`` branch.  Once work is finished and all the tests are passing locally, open a
 merge/pull request (MR) against the upstream ``develop`` branch.  Address any issues
 revealed by any failed CI/CD jobs for your MR.  Once all CI/CD checks are green, project
 maintainers can merge your work where CI/CD will publish a pre-release for your changes
 including container images and PyPI packages.  Contributors should then test the
@@ -74,13 +94,17 @@
 the `Makefile`_ for guidance on making contributions there.
 
 
 .. _`Python's post-mortem debugger`:
    https://docs.python.org/3/library/pdb.html#pdb.post_mortem
 
 .. _`towncrier`: https://towncrier.readthedocs.io/en/stable/#philosophy
-.. _`news fragment`: https://towncrier.readthedocs.io/en/stable/quickstart.html#creating-news-fragments
+.. _`news fragment`:
+   https://towncrier.readthedocs.io/en/stable/quickstart.html#creating-news-fragments
+.. _`Reuse`: https://reuse.software/tutorial/#step-2
+.. _`SPDX header comment`: https://spdx.dev/specifications/#current-version
+.. _`reuse-tool`: https://github.com/fsfe/reuse-tool#usage
 
 .. _`an issue/ticket`: https://gitlab.com/rpatterson/prunerr/-/issues
 
 .. _Makefile: ./Makefile
 .. _`the ./TODO.rst file`: ./TODO.rst
```

### Comparing `prunerr-1.1.8/Dockerfile` & `prunerr-1.1.9b1/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Container image for use by end users
 
 # Stay as close to a vanilla Python environment as possible
 ARG PYTHON_MINOR=3.10
 FROM python:${PYTHON_MINOR}
 
 RUN \
```

### Comparing `prunerr-1.1.8/Dockerfile.devel` & `prunerr-1.1.9b1/Dockerfile.devel`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Container image for use by developers
 
 # Stay as close to the end user image as possible for build cache efficiency.
 # Then add everything that might contribute to efficient development
 ARG PYTHON_MINOR=3.10
 FROM python:${PYTHON_MINOR}
```

### Comparing `prunerr-1.1.8/LICENSE` & `prunerr-1.1.9b1/LICENSES/MIT.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-The MIT License (MIT)
+MIT License
 
 Copyright (c) 2020 Ross Patterson
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `prunerr-1.1.8/Makefile` & `prunerr-1.1.9b1/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Development, build and maintenance tasks:
 #
 # To ease discovery for new contributors, variables that act as options affecting
 # behavior are at the top.  Then skip to `## Top-level targets:` below to find targets
 # intended for use by developers.  The real work, however, is in the recipes for real
 # targets that follow.  If making changes here, please start by reading the philosophy
 # commentary at the bottom of this file.
 
 # Variables used as options to control behavior:
 export TEMPLATE_IGNORE_EXISTING=false
 # https://devguide.python.org/versions/#supported-versions
-PYTHON_SUPPORTED_MINORS=3.11 3.10 3.9 3.8 3.7
-# Project-specific variables
+PYTHON_SUPPORTED_MINORS=3.10 3.11 3.9 3.8 3.7
 export DOCKER_USER=merpatterson
 GPG_SIGNING_KEYID=2EFF7CCE6828E359
 CI_UPSTREAM_NAMESPACE=rpatterson
 CI_PROJECT_NAME=prunerr
 # Project-specific options:
-export DOWNLOAD_VOLUME=$(CHECKOUT_DIR)/var/media/Library/
+export DOWNLOAD_VOLUME=$(CHECKOUT_DIR)/var-docker/media/Library/
 PRUNERR_CMD=exec
 PRUNERR_ARGS=$(PRUNERR_CMD)
 
 
 ## "Private" Variables:
 
 # Variables that aren't likely to be of concern those just using and reading top-level
@@ -200,28 +203,28 @@
 VCS_BRANCHES+=develop
 endif
 VCS_BRANCHES+=main
 endif
 
 # Values used to run Tox:
 TOX_ENV_LIST=$(subst $(EMPTY) ,$(COMMA),$(PYTHON_ENVS))
+TOX_RUN_ARGS=run-parallel --parallel auto --parallel-live
 ifeq ($(words $(PYTHON_MINORS)),1)
 TOX_RUN_ARGS=run
-else
-TOX_RUN_ARGS=run-parallel --parallel auto --parallel-live
 endif
 ifneq ($(PYTHON_WHEEL),)
 TOX_RUN_ARGS+= --installpkg "$(PYTHON_WHEEL)"
 endif
 export TOX_RUN_ARGS
 # The options that allow for rapid execution of arbitrary commands in the venvs managed
 # by tox
 TOX_EXEC_OPTS=--no-recreate-pkg --skip-pkg-install
 TOX_EXEC_ARGS=tox exec $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)"
 TOX_EXEC_BUILD_ARGS=tox exec $(TOX_EXEC_OPTS) -e "build"
+PIP_COMPILE_EXTRA=
 
 # Values used to build Docker images:
 DOCKER_FILE=./Dockerfile
 export DOCKER_BUILD_ARGS=
 export DOCKER_BUILD_PULL=false
 # Values used to tag built images:
 export DOCKER_VARIANT=
@@ -253,20 +256,14 @@
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITLAB)
 else ifeq ($(GITHUB_ACTIONS),true)
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITHUB)
 else
 DOCKER_IMAGES+=$(DOCKER_IMAGE_DOCKER)
 endif
 # Values used to run built images in containers:
-DOCKER_VOLUMES=\
-./var/docker/$(PYTHON_ENV)/ \
-./src/prunerr.egg-info/ \
-./var/docker/$(PYTHON_ENV)/prunerr.egg-info/ \
-./.tox/ ./var/docker/$(PYTHON_ENV)/.tox/ \
-./var/media/Library/
 DOCKER_COMPOSE_RUN_ARGS=
 DOCKER_COMPOSE_RUN_ARGS+= --rm
 ifeq ($(shell tty),not a tty)
 DOCKER_COMPOSE_RUN_ARGS+= -T
 endif
 
 # Values derived from or overridden by CI environments:
@@ -325,14 +322,15 @@
 # external changes, such as new PyPI releases, don't turn CI/CD red spuriously and
 # unrelated to the contributor's actual changes.
 PIP_COMPILE_ARGS=
 endif
 GITHUB_RELEASE_ARGS=--prerelease
 # Only publish releases from the `main` or `develop` branches and only under the
 # canonical CI/CD platform:
+DOCKER_PLATFORMS=
 ifeq ($(GITLAB_CI),true)
 ifeq ($(VCS_BRANCH),main)
 RELEASE_PUBLISH=true
 GITHUB_RELEASE_ARGS=
 else ifeq ($(VCS_BRANCH),develop)
 # Publish pre-releases from the `develop` branch:
 RELEASE_PUBLISH=true
@@ -382,55 +380,66 @@
 
 .PHONY: all
 ### The default target.
 all: build
 
 .PHONY: start
 ### Run the local development end-to-end stack services in the background as daemons.
-start: build-docker-volumes-$(PYTHON_ENV) build-docker-$(PYTHON_MINOR) ./.env
+start: build-docker-$(PYTHON_MINOR) ./.env
 	docker compose down
 	docker compose up -d
 
 .PHONY: run
 ### Run the local development end-to-end stack services in the foreground for debugging.
-run: build-docker-volumes-$(PYTHON_ENV) build-docker-$(PYTHON_MINOR) ./.env
+run: build-docker-$(PYTHON_MINOR) ./.env
 	docker compose down
 	docker compose up
 
 
 ## Build Targets:
 #
 # Recipes that make artifacts needed for by end-users, development tasks, other recipes.
 
 .PHONY: build
 ### Set up everything for development from a checkout, local and in containers.
 build: ./.git/hooks/pre-commit \
 		$(HOME)/.local/var/log/prunerr-host-install.log \
 		build-docker
 
+.PHONY: build-requirements-compile
+### Compile the requirements for one Python version and one type/extra.
+build-requirements-compile:
+	$(MAKE) -e "./var/log/tox/$(PYTHON_ENV)/build.log"
+	pip_compile_opts="--resolver backtracking --upgrade"
+ifneq ($(PIP_COMPILE_EXTRA),)
+	pip_compile_opts+=" --extra $(PIP_COMPILE_EXTRA)"
+endif
+	./.tox/$(PYTHON_ENV)/bin/pip-compile $${pip_compile_opts} \
+	    --output-file "$(PIP_COMPILE_OUT)" "$(PIP_COMPILE_SRC)"
+
 .PHONY: build-pkgs
 ### Ensure the built package is current when used outside of tox.
 build-pkgs: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log build-docker-volumes-$(PYTHON_ENV)
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log
 # Defined as a .PHONY recipe so that multiple targets can depend on this as a
 # pre-requisite and it will only be run once per invocation.
 	rm -vf ./dist/*
 # Build Python packages/distributions from the development Docker container for
 # consistency/reproducibility.
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
 	    tox run -e "$(PYTHON_ENV)" --pkg-only
 # Copy the wheel to a location accessible to all containers:
 	cp -lfv "$$(
-	    ls -t ./var/docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.whl | head -n 1
+	    ls -t ./var-docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.whl | head -n 1
 	)" "./dist/"
 # Also build the source distribution:
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
 	    tox run -e "$(PYTHON_ENV)" --override "testenv.package=sdist" --pkg-only
 	cp -lfv "$$(
-	    ls -t ./var/docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.tar.gz | head -n 1
+	    ls -t ./var-docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.tar.gz | head -n 1
 	)" "./dist/"
 
 .PHONY: $(PYTHON_ENVS:%=build-requirements-%)
 ### Compile fixed/pinned dependency versions if necessary.
 $(PYTHON_ENVS:%=build-requirements-%):
 # Avoid parallel tox recreations stomping on each other
 	$(MAKE) -e "$(@:build-requirements-%=./var/log/tox/%/build.log)"
@@ -462,15 +471,15 @@
 .PHONY: $(PYTHON_MINORS:%=build-docker-%)
 ### Set up for development in a Docker container for one Python version.
 $(PYTHON_MINORS:%=build-docker-%):
 	$(MAKE) -e \
 	    PYTHON_MINORS="$(@:build-docker-%=%)" \
 	    PYTHON_MINOR="$(@:build-docker-%=%)" \
 	    PYTHON_ENV="py$(subst .,,$(@:build-docker-%=%))" \
-	    "./var/docker/py$(subst .,,$(@:build-docker-%=%))/log/build-user.log"
+	    "./var-docker/py$(subst .,,$(@:build-docker-%=%))/log/build-user.log"
 
 .PHONY: build-docker-tags
 ### Print the list of image tags for the current registry and variant.
 build-docker-tags:
 	$(MAKE) -e $(DOCKER_REGISTRIES:%=build-docker-tags-%)
 
 .PHONY: $(DOCKER_REGISTRIES:%=build-docker-tags-%)
@@ -551,42 +560,31 @@
 	    $${docker_image_tags} $${docker_build_caches} --file "$(DOCKER_FILE)" "./"
 
 .PHONY: $(PYTHON_MINORS:%=build-docker-requirements-%)
 ### Pull container images and compile fixed/pinned dependency versions if necessary.
 $(PYTHON_MINORS:%=build-docker-requirements-%): ./.env
 	export PYTHON_MINOR="$(@:build-docker-requirements-%=%)"
 	export PYTHON_ENV="py$(subst .,,$(@:build-docker-requirements-%=%))"
-	$(MAKE) -e build-docker-volumes-$${PYTHON_ENV} \
-	    "./var/docker/$${PYTHON_ENV}/log/build-devel.log"
+	$(MAKE) -e "./var-docker/$${PYTHON_ENV}/log/build-devel.log"
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
 	    make -e PYTHON_MINORS="$(@:build-docker-requirements-%=%)" \
 	    PIP_COMPILE_ARGS="$(PIP_COMPILE_ARGS)" \
 	    build-requirements-py$(subst .,,$(@:build-docker-requirements-%=%))
 
-.PHONY: $(PYTHON_ENVS:%=build-docker-volumes-%)
-### Ensure access permissions to build artifacts in Python version container volumes.
-# If created by `# dockerd`, they end up owned by `root`.
-$(PYTHON_ENVS:%=build-docker-volumes-%): \
-		./src/prunerr.egg-info/ ./.tox/ ./var/media/Library/
-	$(MAKE) -e \
-	    $(@:build-docker-volumes-%=./var/docker/%/) \
-	    $(@:build-docker-volumes-%=./var/docker/%/prunerr.egg-info/) \
-	    $(@:build-docker-volumes-%=./var/docker/%/.tox/)
-
 
 ## Test Targets:
 #
 # Recipes that run the test suite.
 
 .PHONY: test
 ### Format the code and run the full suite of tests, coverage checks, and linters.
 test: test-docker-lint test-docker
 
 .PHONY: test-local
-### Run the full suite of tests on the local host.
+### Run the full suite of tests, coverage checks, and linters on the local host.
 test-local:
 	tox $(TOX_RUN_ARGS) -e "$(TOX_ENV_LIST)"
 
 .PHONY: test-debug
 ### Run tests in the host environment and invoke the debugger on errors/failures.
 test-debug: ./var/log/tox/$(PYTHON_ENV)/editable.log
 	$(TOX_EXEC_ARGS) -- pytest --pdb
@@ -608,16 +606,15 @@
 	    PYTHON_MINORS="$(@:test-docker-%=%)" \
 	    PYTHON_MINOR="$(@:test-docker-%=%)" \
 	    PYTHON_ENV="py$(subst .,,$(@:test-docker-%=%))" \
 	    test-docker-pyminor
 
 .PHONY: test-docker-pyminor
 ### Run the full suite of tests inside a docker container for this Python version.
-test-docker-pyminor: build-docker-volumes-$(PYTHON_ENV) build-docker-$(PYTHON_MINOR) \
-		./var/log/codecov-install.log
+test-docker-pyminor: build-docker-$(PYTHON_MINOR) ./var/log/codecov-install.log
 	docker_run_args="--rm"
 	if [ ! -t 0 ]
 	then
 # No fancy output when running in parallel
 	    docker_run_args+=" -T"
 	fi
 # Ensure the dist/package has been correctly installed in the image
@@ -641,29 +638,27 @@
 	false
 endif
 endif
 endif
 
 .PHONY: test-docker-lint
 ### Check the style and content of the `./Dockerfile*` files.
-test-docker-lint: ./.env build-docker-volumes-$(PYTHON_ENV) \
-		./var/log/docker-login-DOCKER.log
+test-docker-lint: ./.env ./var/log/docker-login-DOCKER.log
 	docker compose pull --quiet hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./Dockerfile.devel"
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
 .PHONY: test-push
 ### Perform any checks that should only be run before pushing.
 test-push: $(VCS_FETCH_TARGETS) \
 		$(HOME)/.local/var/log/prunerr-host-install.log \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
-		build-docker-volumes-$(PYTHON_ENV) ./.env
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env
 	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)"
 ifeq ($(CI),true)
 ifneq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 # Don't waste CI time, only check for the canonical version:
 	exit
 endif
 ifeq ($(VCS_COMPARE_BRANCH),main)
@@ -709,21 +704,21 @@
 ## Release Targets:
 #
 # Recipes that make an changes needed for releases and publish built artifacts to
 # end-users.
 
 .PHONY: release
 ### Publish installable Python packages and container images as required by commits.
-release: release-python release-docker
+release: release-pkgs release-docker
 
-.PHONY: release-python
-### Publish installable Python packages to PyPI.
-release-python: ./var/log/tox/build/build.log ./var/log/git-remotes.log \
-		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		~/.pypirc ./.env build-docker-volumes-$(PYTHON_ENV)
+.PHONY: release-pkgs
+### Publish installable Python packages to PyPI if conventional commits require.
+release-pkgs: $(HOME)/.local/var/log/prunerr-host-install.log \
+		./var/log/tox/build/build.log ./var/log/git-remotes.log \
+		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) ~/.pypirc ./.env
 # Only release from the `main` or `develop` branches:
 ifeq ($(RELEASE_PUBLISH),true)
 # Import the private signing key from CI secrets
 	$(MAKE) -e ./var/log/gpg-import.log
 # Bump the version and build the final release packages:
 	$(MAKE) -e build-pkgs
 # https://twine.readthedocs.io/en/latest/#using-twine
@@ -763,16 +758,15 @@
 # Create a GitHub release
 	gh release create "v$${VERSION}" $(GITHUB_RELEASE_ARGS) \
 	    --notes-file "./NEWS-VERSION.rst" ./dist/prunerr-*
 endif
 
 .PHONY: release-docker
 ### Publish all container images to all container registries.
-release-docker: build-docker-volumes-$(PYTHON_ENV) build-docker \
-		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
+release-docker: build-docker $(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	$(MAKE) -e -j DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=release-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=release-docker-%)
 ### Publish the container images for one Python version to all container registries.
 $(PYTHON_MINORS:%=release-docker-%): \
 		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log) \
@@ -803,16 +797,16 @@
 	fi
 endif
 
 .PHONY: release-bump
 ### Bump the package version if on a branch that should trigger a release.
 release-bump: ~/.gitconfig $(VCS_RELEASE_FETCH_TARGETS) \
 		./var/log/git-remotes.log ./var/log/tox/build/build.log \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
-		./.env build-docker-volumes-$(PYTHON_ENV)
+		$(HOME)/.local/var/log/prunerr-host-install.log \
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env
 	if ! git diff --cached --exit-code
 	then
 	    set +x
 	    echo "CRITICAL: Cannot bump version with staged changes"
 	    false
 	fi
 # Ensure the local branch is updated to the forthcoming version bump commit:
@@ -852,20 +846,20 @@
 # Capture the release notes for *just this* release for creating the GitHub release.
 # Have to run before the real `$ towncrier build` run without the `--draft` option
 # because after that the `newsfragments` will have been deleted.
 	next_version=$$(
 	    $(TOX_EXEC_BUILD_ARGS) -qq -- cz bump $${cz_bump_args} --yes --dry-run |
 	    sed -nE 's|.* ([^ ]+) *→ *([^ ]+).*|\2|p;q'
 	) || true
-# Build and stage the release notes to be commited by `$ cz bump`
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
 	    $(TOX_EXEC_ARGS) -qq -- \
 	    towncrier build --version "$${next_version}" --draft --yes \
 	    >"./NEWS-VERSION.rst"
 	git add -- "./NEWS-VERSION.rst"
+# Build and stage the release notes to be commited by `$ cz bump`:
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
 	    $(TOX_EXEC_ARGS) -- towncrier build --version "$${next_version}" --yes
 # Increment the version in VCS
 	$(TOX_EXEC_BUILD_ARGS) -- cz bump $${cz_bump_args}
 # Ensure the container image reflects the version bump but we don't need to update the
 # requirements again.
 	touch \
@@ -903,19 +897,21 @@
 ### Automatically correct code in this checkout according to linters and style checkers.
 devel-format: $(HOME)/.local/var/log/prunerr-host-install.log
 	$(TOX_EXEC_ARGS) -- autoflake -r -i --remove-all-unused-imports \
 		--remove-duplicate-keys --remove-unused-variables \
 		--remove-unused-variables "./src/prunerr/"
 	$(TOX_EXEC_ARGS) -- autopep8 -v -i -r "./src/prunerr/"
 	$(TOX_EXEC_ARGS) -- black "./src/prunerr/"
+	$(TOX_EXEC_ARGS) -- reuse addheader -r --skip-unrecognised \
+	    --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "./"
 
 .PHONY: devel-upgrade
 ### Update all fixed/pinned dependencies to their latest available versions.
-devel-upgrade: ./.env build-docker-volumes-$(PYTHON_ENV) \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
+devel-upgrade: ./.env $(HOME)/.local/var/log/prunerr-host-install.log \
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log \
 		./var/log/tox/build/build.log
 	touch "./setup.cfg" "./requirements/build.txt.in" \
 	    "./build-host/requirements.txt.in"
 # Ensure the network is create first to avoid race conditions
 	docker compose create prunerr-devel
 	$(MAKE) -e -j PIP_COMPILE_ARGS="--upgrade" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
@@ -939,18 +935,18 @@
 	if $(MAKE) -e "test-clean"
 	then
 # No changes from upgrade, exit successfully but push nothing
 	    exit
 	fi
 # Commit the upgrade changes
 	echo "Upgrade all requirements to the latest versions as of $${now}." \
-	    >"./src/prunerr/newsfragments/+upgrade-requirements.bugfix.rst"
+	    >"./newsfragments/+upgrade-requirements.bugfix.rst"
 	git add --update './build-host/requirements-*.txt' './requirements/*/*.txt' \
 	    "./.pre-commit-config.yaml"
-	git add "./src/prunerr/newsfragments/+upgrade-requirements.bugfix.rst"
+	git add "./newsfragments/+upgrade-requirements.bugfix.rst"
 	git_commit_args="--all --gpg-sign"
 ifeq ($(CI),true)
 # Don't duplicate the CI run from the push below:
 	git_push_args+=" --no-verify"
 endif
 	git commit $${git_commit_args} -m \
 	    "fix(deps): Upgrade requirements latest versions"
@@ -992,45 +988,43 @@
 clean:
 	docker compose down --remove-orphans --rmi "all" -v || true
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit uninstall \
 	    --hook-type "pre-commit" --hook-type "commit-msg" --hook-type "pre-push" \
 	    || true
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit clean || true
 	git clean -dfx -e "var/" -e ".env"
-	rm -rfv "./var/log/"
-	rm -rf "./var/docker/"
+	git clean -dfx "./var-docker/py*/.tox/" \
+	    "./var-docker/py*/prunerr.egg-info/"
+	rm -rfv "./var/log/" "./var-docker/py*/log/"
 
 
 ## Real Targets:
 #
 # Recipes that make actual changes and create and update files for the target.
 
 # Manage fixed/pinned versions in `./requirements/**.txt` files.  Has to be run for each
 # python version in the virtual environment for that Python version:
 # https://github.com/jazzband/pip-tools#cross-environment-usage-of-requirementsinrequirementstxt-and-pip-compile
 $(PYTHON_ENVS:%=./requirements/%/devel.txt): ./pyproject.toml ./setup.cfg ./tox.ini
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:requirements/%/devel.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:requirements/%/devel.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --extra "devel" \
-	    --output-file "$(@)" "$(<)"
+	$(MAKE) -e PYTHON_ENV="$(@:requirements/%/devel.txt=%)" \
+	    PIP_COMPILE_EXTRA="devel" PIP_COMPILE_SRC="$(<)" PIP_COMPILE_OUT="$(@)" \
+	    build-requirements-compile
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./requirements/%/user.txt): ./pyproject.toml ./setup.cfg ./tox.ini
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:requirements/%/user.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:requirements/%/user.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --output-file "$(@)" "$(<)"
+	$(MAKE) -e PYTHON_ENV="$(@:requirements/%/user.txt=%)" PIP_COMPILE_SRC="$(<)" \
+	    PIP_COMPILE_OUT="$(@)" build-requirements-compile
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./build-host/requirements-%.txt): ./build-host/requirements.txt.in
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:build-host/requirements-%.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:build-host/requirements-%.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --output-file "$(@)" "$(<)"
+	$(MAKE) -e PYTHON_ENV="$(@:build-host/requirements-%.txt=%)" \
+	    PIP_COMPILE_SRC="$(<)" PIP_COMPILE_OUT="$(@)" build-requirements-compile
 # Only update the installed tox version for the latest/host/main/default Python version
 	if [ "$(@:build-host/requirements-%.txt=%)" = "$(PYTHON_ENV)" ]
 	then
 # Don't install tox into one of it's own virtual environments
 	    if [ -n "$${VIRTUAL_ENV:-}" ]
 	    then
 	        pip_bin="$$(which -a pip | grep -v "^$${VIRTUAL_ENV}/bin/" | head -n 1)"
@@ -1039,17 +1033,16 @@
 	    fi
 	    "$${pip_bin}" install -r "$(@)"
 	fi
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./requirements/%/build.txt): ./requirements/build.txt.in
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:requirements/%/build.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:requirements/%/build.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --output-file "$(@)" "$(<)"
+	$(MAKE) -e PYTHON_ENV="$(@:requirements/%/build.txt=%)" PIP_COMPILE_SRC="$(<)" \
+	    PIP_COMPILE_OUT="$(@)" build-requirements-compile
 
 # Targets used as pre-requisites to ensure virtual environments managed by tox have been
 # created and can be used directly to save time on Tox's overhead when we don't need
 # Tox's logic about when to update/recreate them, e.g.:
 #     $ ./.tox/build/bin/cz --help
 # Mostly useful for build/release tools.
 $(PYTHON_ALL_ENVS:%=./var/log/tox/%/build.log):
@@ -1065,28 +1058,27 @@
 	mkdir -pv "$(dir $(@))"
 	tox exec $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/editable.log=%)" -- \
 	    pip install -e "./" |& tee -a "$(@)"
 
 ## Docker real targets:
 
 # Build the development image:
-./var/docker/$(PYTHON_ENV)/log/build-devel.log: \
+./var-docker/$(PYTHON_ENV)/log/build-devel.log: \
 		./Dockerfile.devel ./.dockerignore ./bin/entrypoint \
 		./pyproject.toml ./setup.cfg ./tox.ini \
 		./build-host/requirements.txt.in ./docker-compose.yml \
 		./docker-compose.override.yml ./.env \
-		./var/docker/$(PYTHON_ENV)/log/rebuild.log
+		./var-docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e build-docker-volumes-$(PYTHON_ENV)
 	mkdir -pv "$(dir $(@))"
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
-	    touch "$(@)" "./var/docker/$(PYTHON_ENV)/log/rebuild.log"
+	    touch "$(@)" "./var-docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
 	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
 	        prunerr-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
 	        "./var/log/tox/$(PYTHON_ENV)/build.log"
 	    exit
 	fi
 endif
@@ -1101,66 +1093,68 @@
 # rebuilding images:
 	touch "$(@)"
 else
 	$(MAKE) -e "$(@)"
 endif
 
 # Build the end-user image:
-./var/docker/$(PYTHON_ENV)/log/build-user.log: \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
-		./var/docker/$(PYTHON_ENV)/log/rebuild.log
+./var-docker/$(PYTHON_ENV)/log/build-user.log: \
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
+		./var-docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
 ifeq ($(PYTHON_WHEEL),)
 	$(MAKE) -e "build-pkgs"
 	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
 endif
 # Build the end-user image now that all required artifacts are built"
 	mkdir -pv "$(dir $(@))"
 	$(MAKE) -e DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --load \
 	--build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build >>"$(@)"
 # The image installs the host requirements, reflect that in the bind mount volumes
 	date >>"$(@:%/build-user.log=%/host-install.log)"
 
-./var/ $(PYTHON_ENVS:%=./var/docker/%/) \
-./src/prunerr.egg-info/ \
-$(PYTHON_ENVS:%=./var/docker/%/prunerr.egg-info/) \
-./.tox/ $(PYTHON_ENVS:%=./var/docker/%/.tox/) \
-./var/media/Library/:
-	mkdir -pv "$(@)"
-
 # Marker file used to trigger the rebuild of the image for just one Python version.
 # Useful to workaround async timestamp issues when running jobs in parallel:
-./var/docker/$(PYTHON_ENV)/log/rebuild.log:
+./var-docker/$(PYTHON_ENV)/log/rebuild.log:
 	mkdir -pv "$(dir $(@))"
 	date >>"$(@)"
 
 # Local environment variables from a template:
 ./.env: ./.env.in
+	set +x
 	export TRANSMISSION_PASS="$$(apg -M ncl -n 1)"
+	set -x
 	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
 
 # Install all tools required by recipes that have to be installed externally on the
 # host.  Use a target file outside this checkout to support multiple checkouts.  Use a
 # target specific to this project so that other projects can use the same approach but
 # with different requirements.
 $(HOME)/.local/var/log/prunerr-host-install.log:
 	mkdir -pv "$(dir $(@))"
-# Bootstrap the minimum Python environment
 	(
 	    if ! which pip
 	    then
 	        if which apk
 	        then
 	            sudo apk update
-	            sudo apk add "gettext" "py3-pip" "gnupg" "github-cli" "curl" "apg"
+	            sudo apk add \
+# We need `$ envsubst` in the `expand-template:` target recipe:
+	                "gettext" \
+# We need `$ pip3` to install the project's Python tools:
+	                "py3-pip" \
+# Needed for dependencies we can't get current versions for locally:
+	                "docker-cli-compose" \
+# Needed for publishing releases from CI/CD:
+	                "gnupg" "github-cli" "curl" "apg"
 	        elif which apt-get
 	        then
 	            sudo apt-get update
-	            sudo apt-get install -y \
-	                "gettext-base" "python3-pip" "gnupg" "gh" "curl" "apg"
+	            sudo apt-get install -y "gettext-base" "python3-pip" \
+	                "docker-compose-plugin" "gnupg" "gh" "curl" "apg"
 	        else
 	            set +x
 	            echo "ERROR: OS not supported for installing host dependencies"
 	            false
 	        fi
 	    fi
 	    if [ -e ./build-host/requirements-$(PYTHON_HOST_ENV).txt ]
```

### Comparing `prunerr-1.1.8/NEWS.rst` & `prunerr-1.1.9b1/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+prunerr 1.1.9b1 (2023-05-05)
+============================
+
+Bugfixes
+--------
+
+- Workaround the broken previous release not being published.
+
+
+prunerr 1.1.9b0 (2023-05-05)
+============================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Fri May  5 01:58:13 PM UTC 2023.
+
+
 prunerr 1.1.8 (2023-04-27)
 ==========================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Thu Apr 27 18:36:06 UTC 2023.
```

### Comparing `prunerr-1.1.8/PKG-INFO` & `prunerr-1.1.9b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.8
+Version: 1.1.9b1
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
-License-File: LICENSE
+
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
 
 ########################################################################################
 Prunerr
 ########################################################################################
 Perma-seed Servarr media libraries
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/prunerr.svg?logo=pypi&label=PyPI&logoColor=gold
           :alt: PyPI latest release version
           :target: https://pypi.org/project/prunerr/
-       .. figure:: https://img.shields.io/pypi/dm/prunerr.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-          :alt: PyPI downloads per month
-          :target: https://pypi.org/project/prunerr/
        .. figure:: https://img.shields.io/pypi/pyversions/prunerr.svg?logo=python&label=Python&logoColor=gold
           :alt: PyPI Python versions
           :target: https://pypi.org/project/prunerr/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
           :alt: Python code style
           :target: https://github.com/psf/black
+       .. figure:: https://api.reuse.software/badge/gitlab.com/rpatterson/prunerr
+          :alt: REUSE license status
+          :target: https://api.reuse.software/info/gitlab.com/rpatterson/prunerr
 
      - .. figure:: https://gitlab.com/rpatterson/prunerr/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/prunerr/-/releases
        .. figure:: https://gitlab.com/rpatterson/prunerr/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
           :target: https://gitlab.com/rpatterson/prunerr/-/commits/main
@@ -162,16 +166,14 @@
 See the `Usage`_ section below for full details.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
-Install and use either via a local, native installation or a Docker container image:
-
 Local/Native Installation
 ========================================================================================
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ pip3 install --user prunerr
 
@@ -184,30 +186,30 @@
 `the example ./docker-compose.yml file`_ for an example configuration.  Once you have
 your configuration, you can create and run the container::
 
   $ docker compose up
 
 Alternatively, you make use the image directly.  Pull `the Docker image`_::
 
-  $ docker pull "registry.gitlab.org/rpatterson/prunerr"
+  $ docker pull "registry.gitlab.com/rpatterson/prunerr"
 
 And then use the image to create and run a container::
 
-  $ docker run --rm -it "registry.gitlab.org/rpatterson/prunerr" ...
+  $ docker run --rm -it "registry.gitlab.com/rpatterson/prunerr" ...
 
 Images variant tags are published for the Python version, branch, and major/minor
 versions so that users can control when they get new images over time,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:py310-main``.  The canonical Python
-version is 3.10 which is the version used in tags without ``py###``,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:main``.  Pre-releases are from
+e.g. ``registry.gitlab.com/rpatterson/prunerr:py310-main``.  The canonical
+Python version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.com/rpatterson/prunerr:main``.  Pre-releases are from
 ``develop`` and final releases are from ``main`` which is also the default for tags
-without a branch, e.g. ``registry.gitlab.org/merpatterson/prunerr:py310``. The
+without a branch, e.g. ``registry.gitlab.com/rpatterson/prunerr:py310``. The
 major/minor version tags are only applied to the final release images and without the
 corresponding ``main`` branch tag,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:py310-v0.8``.
+e.g. ``registry.gitlab.com/rpatterson/prunerr:py310-v0.8``.
 
 Multi-platform Docker images are published containing images for the following
 platforms or architectures in the Python 3.10 ``py310`` variant:
 
 - ``linux/amd64``
 - ``linux/arm64``
 - ``linux/arm/v7``
```

### Comparing `prunerr-1.1.8/README.rst` & `prunerr-1.1.9b1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
+
 ########################################################################################
 Prunerr
 ########################################################################################
 Perma-seed Servarr media libraries
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/prunerr.svg?logo=pypi&label=PyPI&logoColor=gold
           :alt: PyPI latest release version
           :target: https://pypi.org/project/prunerr/
-       .. figure:: https://img.shields.io/pypi/dm/prunerr.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-          :alt: PyPI downloads per month
-          :target: https://pypi.org/project/prunerr/
        .. figure:: https://img.shields.io/pypi/pyversions/prunerr.svg?logo=python&label=Python&logoColor=gold
           :alt: PyPI Python versions
           :target: https://pypi.org/project/prunerr/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
           :alt: Python code style
           :target: https://github.com/psf/black
+       .. figure:: https://api.reuse.software/badge/gitlab.com/rpatterson/prunerr
+          :alt: REUSE license status
+          :target: https://api.reuse.software/info/gitlab.com/rpatterson/prunerr
 
      - .. figure:: https://gitlab.com/rpatterson/prunerr/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/prunerr/-/releases
        .. figure:: https://gitlab.com/rpatterson/prunerr/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
           :target: https://gitlab.com/rpatterson/prunerr/-/commits/main
@@ -135,16 +139,14 @@
 See the `Usage`_ section below for full details.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
-Install and use either via a local, native installation or a Docker container image:
-
 Local/Native Installation
 ========================================================================================
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ pip3 install --user prunerr
 
@@ -157,30 +159,30 @@
 `the example ./docker-compose.yml file`_ for an example configuration.  Once you have
 your configuration, you can create and run the container::
 
   $ docker compose up
 
 Alternatively, you make use the image directly.  Pull `the Docker image`_::
 
-  $ docker pull "registry.gitlab.org/rpatterson/prunerr"
+  $ docker pull "registry.gitlab.com/rpatterson/prunerr"
 
 And then use the image to create and run a container::
 
-  $ docker run --rm -it "registry.gitlab.org/rpatterson/prunerr" ...
+  $ docker run --rm -it "registry.gitlab.com/rpatterson/prunerr" ...
 
 Images variant tags are published for the Python version, branch, and major/minor
 versions so that users can control when they get new images over time,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:py310-main``.  The canonical Python
-version is 3.10 which is the version used in tags without ``py###``,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:main``.  Pre-releases are from
+e.g. ``registry.gitlab.com/rpatterson/prunerr:py310-main``.  The canonical
+Python version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.com/rpatterson/prunerr:main``.  Pre-releases are from
 ``develop`` and final releases are from ``main`` which is also the default for tags
-without a branch, e.g. ``registry.gitlab.org/merpatterson/prunerr:py310``. The
+without a branch, e.g. ``registry.gitlab.com/rpatterson/prunerr:py310``. The
 major/minor version tags are only applied to the final release images and without the
 corresponding ``main`` branch tag,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:py310-v0.8``.
+e.g. ``registry.gitlab.com/rpatterson/prunerr:py310-v0.8``.
 
 Multi-platform Docker images are published containing images for the following
 platforms or architectures in the Python 3.10 ``py310`` variant:
 
 - ``linux/amd64``
 - ``linux/arm64``
 - ``linux/arm/v7``
```

### Comparing `prunerr-1.1.8/TODO.rst` & `prunerr-1.1.9b1/TODO.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
+
 ########################################################################################
 Seeking Contributions
 ########################################################################################
 
 The following are known issues with Prunerr or features that are particularly desirable
 to implement in Prunerr.  IOW, contributions are particularly welcome for the following:
```

### Comparing `prunerr-1.1.8/bin/cz-check-bump` & `prunerr-1.1.9b1/bin/cz-check-bump`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python3
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Check if the conventional commits since the last release require a new release.
 
 Works around Commitizen's version handling when bumping from a pre-release:
 
 https://github.com/commitizen-tools/commitizen/issues/688#issue-1628052526
 """
```

### Comparing `prunerr-1.1.8/bin/entrypoint` & `prunerr-1.1.9b1/bin/entrypoint`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/bin/bash
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 #
 # Perform any required volatile run-time initialization
 
 set -eu -o pipefail
 shopt -s inherit_errexit
 if [ "${DEBUG:=false}" = "true" ]
 then
@@ -22,15 +27,15 @@
 	    false
 	fi
 	if ! id "${PUID}" >"/dev/null" 2>&1
 	then
 	    # Add a user to the `passwd` DB so that the `~prunerr/`
 	    # HOME directory can be looked up.
 	    adduser --uid "${PUID}" --disabled-password \
-		    --gecos "Prunerr,,," "prunerr" >"/dev/null"
+	        --gecos "Prunerr,,," "prunerr" >"/dev/null"
 	fi
 	# Fix the TTY ownership if the session is interactive
 	if tty_dev=$(tty)
 	then
 	    chown "${PUID}" "${tty_dev}"
 	fi
 	# Delegate the rest to the `CMD`
```

### Comparing `prunerr-1.1.8/bin/get-base-version` & `prunerr-1.1.9b1/bin/get-base-version`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Return the current version minus any pre-release suffix along with it's type.
 
 Useful to get the final/stable version when the previous pre-release has been blessed as
 ready for publishing as final.
 """  # pylint: disable=invalid-name
```

### Comparing `prunerr-1.1.8/build-host/Dockerfile` & `prunerr-1.1.9b1/build-host/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Container image in which to build, test, and release the project
 
 # I *want* something to break to let me know if something changes in the latest version
 # of the base image changes something:
 # hadolint ignore=DL3007
 FROM docker:latest
```

### Comparing `prunerr-1.1.8/build-host/Makefile` & `prunerr-1.1.9b1/build-host/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Build and publish an image in which to build, test, and release the project
 
 ### Defensive settings for make:
 #     https://tech.davis-hansson.com/p/make/
 SHELL:=bash
 .ONESHELL:
 .SHELLFLAGS:=-eu -o pipefail -c
```

### Comparing `prunerr-1.1.8/build-host/bin/entrypoint` & `prunerr-1.1.9b1/build-host/bin/entrypoint`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/bin/ash
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 #
 # Shared set up for local testing of CI/CD
 
 set -eu -o pipefail
 CHOWN_ARGS="-R"
 if [ "${DEBUG:=false}" = "true" ]
 then
```

### Comparing `prunerr-1.1.8/build-host/requirements-py310.txt` & `prunerr-1.1.9b1/build-host/requirements-py310.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,9 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `prunerr-1.1.8/build-host/requirements-py311.txt` & `prunerr-1.1.9b1/build-host/requirements-py311.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,9 +26,9 @@
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `prunerr-1.1.8/build-host/requirements-py37.txt` & `prunerr-1.1.9b1/build-host/requirements-py37.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,11 +40,11 @@
 tox==4.5.1
     # via -r build-host/requirements.txt.in
 typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   platformdirs
     #   tox
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `prunerr-1.1.8/build-host/requirements-py38.txt` & `prunerr-1.1.9b1/build-host/requirements-py38.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,9 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `prunerr-1.1.8/build-host/requirements-py39.txt` & `prunerr-1.1.9b1/build-host/requirements-py39.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,9 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `prunerr-1.1.8/docker-compose-servarr.yml` & `prunerr-1.1.9b1/docker-compose-servarr.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Example Servarr service to demonstrate the integration with Prunerr.
 #
 # In a separate file because integrating with Servarr is optional.  See the comment
 # above `COMPOSE_FILE` in `./.env.in` for an example of how to add this file.
 version: "3.8"
 
 services:
```

### Comparing `prunerr-1.1.8/docker-compose.override.yml` & `prunerr-1.1.9b1/docker-compose.override.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Override `$ docker compose ...` configuration for development or testing here in this
 # repo checkout.  Everything that may be used outside this checkout should be in
 # `./docker-compose.yml`.
 version: "3.8"
 
 services:
 
@@ -19,107 +23,109 @@
   # Configuration specific to development:
   prunerr-daemon:
     image: "\
       ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/prunerr\
       :${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "prunerr-daemon-checkout"
     build:
-      context: "${CHECKOUT_DIR}/"
+      context: "${CHECKOUT_DIR:-.}/"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     volumes:
       # Preserve caches caches between container runs
-      - "${CHECKOUT_DIR}/home/:/home/prunerr/"
+      - "${CHECKOUT_DIR:-.}/home/:/home/prunerr/"
 
   ## Contianers used for development and release:
 
   # Container for use by developers:
   prunerr-devel:
     image: "\
       ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/prunerr\
       :devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
     container_name: "prunerr-devel"
     profiles:
       - "test"
     build:
-      context: "${CHECKOUT_DIR}/"
-      dockerfile: "${CHECKOUT_DIR}/Dockerfile.devel"
+      context: "${CHECKOUT_DIR:-.}/"
+      dockerfile: "${CHECKOUT_DIR:-.}/Dockerfile.devel"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env`
       PUID: "${PUID:-1000}"
       PGID: "${PGID:-${PUID:-1000}}"
       # Variables from the environment we want to be passed through into the container:
       CI: "${CI:-false}"
       # DEBUG: "true"
     volumes:
       # Ensure local changes are reflected inside the container.
-      - "${CHECKOUT_DIR}/bin/entrypoint:/usr/local/bin/entrypoint"
-      - "${CHECKOUT_DIR}/:/usr/local/src/prunerr/"
+      - "${CHECKOUT_DIR:-.}/bin/entrypoint:/usr/local/bin/entrypoint"
+      - "${CHECKOUT_DIR:-.}/:/usr/local/src/prunerr/"
       # Preserve caches caches between container runs
-      - "${CHECKOUT_DIR}/home/:/home/prunerr/"
+      - "${CHECKOUT_DIR:-.}/home/:/home/prunerr/"
       # Avoid any clashes between image variants and/or the local host at both build and
       # run-time.
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/\
+      - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}/\
         :/usr/local/src/prunerr/var/"
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/.tox/\
+      - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}/.tox/\
         :/usr/local/src/prunerr/.tox/"
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}\
+      - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}\
         /prunerr.egg-info/\
         :/usr/local/src/prunerr/src/prunerr.egg-info/"
 
   # https://github.com/hadolint/hadolint#how-to-use
   hadolint:
     image: "ghcr.io/hadolint/hadolint"
     profiles:
       - "test"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
-      - "${CHECKOUT_DIR}/:/usr/local/src/prunerr/"
+      - "${CHECKOUT_DIR:-.}/:/usr/local/src/prunerr/"
     working_dir: "/usr/local/src/prunerr/"
     command: >-
       hadolint "./Dockerfile"
 
   pandoc:
     image: "pandoc/core"
     profiles:
       - "release"
     user: "${PUID:-1000}:${PGID:-${PUID:-1000}}"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
-      - "${CHECKOUT_DIR}/:/data/"
+      - "${CHECKOUT_DIR:-.}/:/data/"
     entrypoint: "ash"
-    # Strip reStructuredText directives unsupported in Markdown:
+    # Strip reStructuredText directives unsupported in Markdown before converting and
+    # converted Markdown that isn't widely supported, e.g. table of contents and tables
+    # respectively:
     command: >-
       -xeu -c '
         grep -Ev "^ *\.\. +(contents)::.*" "./README.rst" |
-        pandoc -f "rst" -t "markdown" -o "./var/README.md"
+        pandoc -f "rst" -t "gfm" | grep -Ev "^(\+-+\+|\|.*\|)$" >"./README.md"
       '
 
   docker-pushrm:
     image: "chko/docker-pushrm"
     depends_on:
       pandoc:
         condition: "service_completed_successfully"
     profiles:
       - "release"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       DOCKER_USER: "${DOCKER_USER:-merpatterson}"
       DOCKER_PASS: "${DOCKER_PASS}"
     volumes:
-      - "${CHECKOUT_DIR}/:/data/"
+      - "${CHECKOUT_DIR:-.}/:/data/"
     command: >-
       --file "/data/var/README.md"
       --short "Perma-seed Servarr media libraries"
       --debug "merpatterson/prunerr"
 
   gitlab-release-cli:
     image: "${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/gitlab-org/release-cli:latest"
@@ -136,28 +142,28 @@
   # The container in which CI/CD is run:
   build-host:
     image: "\
       ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/prunerr\
       :build-host"
     profiles:
       - "ci"
-    build: "${CHECKOUT_DIR}/build-host/"
+    build: "${CHECKOUT_DIR:-.}/build-host/"
     privileged: true
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
-      - "${CHECKOUT_DIR}/:${CHECKOUT_DIR}"
-      - "${CHECKOUT_DIR}/build-host/bin/entrypoint:/usr/local/bin/entrypoint"
+      - "${CHECKOUT_DIR:-.}/:${CHECKOUT_DIR:-.}"
+      - "${CHECKOUT_DIR:-.}/build-host/bin/entrypoint:/usr/local/bin/entrypoint"
       # Share local SSH authentication to repository remotes
       - "~/.ssh/:/home/runner/.ssh/"
     env_file: "./.env"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       PUID: "${PUID:-1000}"
       PGID: "${DOCKER_GID:-${PGID:-${PUID:-1000}}}"
       # DEBUG: "true"
-    working_dir: "${CHECKOUT_DIR}"
+    working_dir: "${CHECKOUT_DIR:-.}"
     command: >-
       make -e build-docker test-docker release
 
   gitlab-runner:
     profiles:
       - "ci"
```

### Comparing `prunerr-1.1.8/docker-compose.yml` & `prunerr-1.1.9b1/docker-compose.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Minimal `$ docker compose ...` configuration to demonstrate the requirements for
-# running Prunerr in containers.
+# running prunerr in containers.
 version: "3.8"
 
 services:
 
   transmission:
     image: "linuxserver/transmission"
     container_name: "transmission"
```

### Comparing `prunerr-1.1.8/gitlab-runner/config/config.toml.in` & `prunerr-1.1.9b1/gitlab-runner/config/config.toml.in`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Set to 2 times the number of parallel matrix jobs as a default.
 # Alternatively, set to the number of CPUs/cores or some multiple:
 concurrent = 10
 # Pick up jobs as soon as possible:
 check_interval = 1
 shutdown_timeout = 0
```

### Comparing `prunerr-1.1.8/pyproject.toml` & `prunerr-1.1.9b1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,23 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 [build-system]
 # https://setuptools.pypa.io/en/latest/build_meta.html#how-to-use-it
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # Use VCS tags as the sole authority on versions.  Dynamically determine the current
 # version from VCS tags:
 # https://github.com/pypa/setuptools_scm#pyprojecttoml-usage
 write_to = "src/prunerr/version.py"
 # Uncomment to test uploading to PyPI locally
 # local_scheme = "no-local-version"
-[tool.commitizen]
-# Parse commit messages according to conventional commits to decide wether the next
-# versin tag should be a major, minor or patch bump and create the VCS tag.  Also
-# provides VCS hooks to enforce that commit messages comply with conventional commits:
-# https://commitizen-tools.github.io/commitizen/
-name = "cz_conventional_commits"
-changelog_start_rev = "v0.0.0"
-version = "1.1.8"
-tag_format = "v$version"
-annotated_tag = true
-gpg_sign = true
-bump_message = """\
-build(release): Version $current_version → $new_version
-
-[actions skip]
-[ci release]
-"""
-[tool.towncrier]
-# https://towncrier.readthedocs.io/en/stable/#quick-start
-package = "prunerr"
-package_dir = "src"
-name = "prunerr"
 
 [tool.pylint.MASTER]
 # Ensure `duplicate-code` and any other errors that depend on not runnining in parallel
 # are reported:
 jobs = 1
 enable-all-extensions = true
 output-format = "colorized"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prunerr-1.1.8/requirements/py310/build.txt` & `prunerr-1.1.9b1/requirements/py310/build.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,31 +16,31 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
     #   commitizen
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
@@ -58,22 +58,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -83,45 +81,39 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
-typing-extensions==4.5.0
-    # via setuptools-scm
-urllib3==1.26.15
+urllib3==2.0.2
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `prunerr-1.1.8/requirements/py310/devel.txt` & `prunerr-1.1.9b1/requirements/py310/devel.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,33 @@
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
 autopep8==2.0.2
     # via prunerr (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via prunerr (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   pip-tools
     #   prunerr (pyproject.toml)
     #   pyroma
 certifi==2022.12.7
     # via requests
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
     #   pip-tools
@@ -42,15 +52,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.5
     # via prunerr (pyproject.toml)
 dill==0.3.6
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
@@ -77,17 +87,21 @@
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+license-expression==30.1.0
+    # via reuse
 main-wrapper==0.1.1
     # via service-logging
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
@@ -165,33 +179,38 @@
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
 pytest==7.3.1
     # via prunerr (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   prunerr (pyproject.toml)
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
+    #   reuse
     #   transmission-rpc
     #   xenon
 requests-mock==1.10.0
     # via prunerr (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
+reuse==1.0.0
+    # via prunerr (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via prunerr (pyproject.toml)
 rstcheck-core==1.0.3
@@ -235,29 +254,29 @@
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   astroid
     #   mypy
     #   pydantic
     #   transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `prunerr-1.1.8/requirements/py310/user.txt` & `prunerr-1.1.9b1/requirements/py38/user.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py310/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py38/user.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
+cli-exit-tools==1.2.3.2
+    # via
+    #   lib-detect-testenv
+    #   pathlib3x
+click==8.1.3
+    # via
+    #   cli-exit-tools
+    #   lib-detect-testenv
+    #   pathlib3x
 idna==3.4
     # via requests
+lib-detect-testenv==2.0.3
+    # via cli-exit-tools
 main-wrapper==0.1.1
     # via service-logging
+pathlib3x==2.0.2.1 ; python_version < "3.10"
+    # via prunerr (pyproject.toml)
 pyyaml==6.0
     # via prunerr (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   transmission-rpc
 service-logging==0.1.1
     # via prunerr (pyproject.toml)
 six==1.16.0
     # via main-wrapper
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
```

### Comparing `prunerr-1.1.8/requirements/py311/build.txt` & `prunerr-1.1.9b1/requirements/py38/build.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,35 +16,37 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
     #   commitizen
     #   keyring
     #   twine
+importlib-resources==5.12.0
+    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -58,22 +60,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -83,46 +83,46 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via setuptools-scm
-urllib3==1.26.15
+    # via rich
+urllib3==2.0.2
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `prunerr-1.1.8/requirements/py311/devel.txt` & `prunerr-1.1.9b1/requirements/py311/devel.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,33 @@
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
 autopep8==2.0.2
     # via prunerr (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via prunerr (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   pip-tools
     #   prunerr (pyproject.toml)
     #   pyroma
 certifi==2022.12.7
     # via requests
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
     #   pip-tools
@@ -42,15 +52,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.5
     # via prunerr (pyproject.toml)
 dill==0.3.6
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
@@ -75,17 +85,21 @@
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+license-expression==30.1.0
+    # via reuse
 main-wrapper==0.1.1
     # via service-logging
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
@@ -163,33 +177,38 @@
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
 pytest==7.3.1
     # via prunerr (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   prunerr (pyproject.toml)
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
+    #   reuse
     #   transmission-rpc
     #   xenon
 requests-mock==1.10.0
     # via prunerr (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
+reuse==1.0.0
+    # via prunerr (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via prunerr (pyproject.toml)
 rstcheck-core==1.0.3
@@ -222,28 +241,28 @@
     #   vulture
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   mypy
     #   pydantic
     #   transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `prunerr-1.1.8/requirements/py311/user.txt` & `prunerr-1.1.9b1/requirements/py311/user.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     # via requests
 idna==3.4
     # via requests
 main-wrapper==0.1.1
     # via service-logging
 pyyaml==6.0
     # via prunerr (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   transmission-rpc
 service-logging==0.1.1
     # via prunerr (pyproject.toml)
 six==1.16.0
     # via main-wrapper
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
```

### Comparing `prunerr-1.1.8/requirements/py37/build.txt` & `prunerr-1.1.9b1/requirements/py311/build.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,41 +16,35 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
-    #   argcomplete
     #   commitizen
     #   keyring
-    #   pre-commit
-    #   setuptools-scm
     #   twine
-    #   virtualenv
-importlib-resources==5.12.0
-    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -64,22 +58,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==2.21.0
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -89,56 +81,42 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
-typing-extensions==4.5.0
-    # via
-    #   commitizen
-    #   importlib-metadata
-    #   markdown-it-py
-    #   platformdirs
-    #   rich
-    #   setuptools-scm
-urllib3==1.26.15
+urllib3==2.0.2
     # via
     #   requests
     #   twine
-virtualenv==20.21.1
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `prunerr-1.1.8/requirements/py37/devel.txt` & `prunerr-1.1.9b1/requirements/py39/devel.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py37/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
 astroid==2.15.4
     # via
@@ -14,27 +14,35 @@
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
 autopep8==2.0.2
     # via prunerr (pyproject.toml)
-backports-cached-property==1.0.2 ; python_version < "3.8"
-    # via prunerr (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via prunerr (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   pip-tools
     #   prunerr (pyproject.toml)
     #   pyroma
 certifi==2022.12.7
     # via requests
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 cli-exit-tools==1.2.3.2
     # via
     #   lib-detect-testenv
     #   pathlib3x
 click==8.1.3
@@ -51,15 +59,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.5
     # via prunerr (pyproject.toml)
 dill==0.3.6
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
@@ -79,37 +87,30 @@
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
 iniconfig==2.0.0
     # via pytest
-isort==5.11.5
+isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
 lib-detect-testenv==2.0.3
     # via cli-exit-tools
+license-expression==30.1.0
+    # via reuse
 main-wrapper==0.1.1
     # via service-logging
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
@@ -189,33 +190,38 @@
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
 pytest==7.3.1
     # via prunerr (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   prunerr (pyproject.toml)
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
+    #   reuse
     #   transmission-rpc
     #   xenon
 requests-mock==1.10.0
     # via prunerr (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
+reuse==1.0.0
+    # via prunerr (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via prunerr (pyproject.toml)
 rstcheck-core==1.0.3
@@ -233,15 +239,15 @@
     #   main-wrapper
     #   mando
     #   requests-mock
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
-stevedore==3.5.2
+stevedore==5.0.0
     # via bandit
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
@@ -259,50 +265,37 @@
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.5.2
     # via pyroma
-typed-ast==1.5.4
-    # via
-    #   astroid
-    #   black
-    #   mypy
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
-    #   gitpython
-    #   importlib-metadata
     #   mypy
-    #   platformdirs
     #   pydantic
     #   pylint
-    #   rich
-    #   rstcheck
-    #   rstcheck-core
     #   transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via prunerr (pyproject.toml)
-zipp==3.15.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `prunerr-1.1.8/requirements/py37/user.txt` & `prunerr-1.1.9b1/requirements/py37/user.txt`

 * *Files 17% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     # via cli-exit-tools
 main-wrapper==0.1.1
     # via service-logging
 pathlib3x==2.0.2.1 ; python_version < "3.10"
     # via prunerr (pyproject.toml)
 pyyaml==6.0
     # via prunerr (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   transmission-rpc
 service-logging==0.1.1
     # via prunerr (pyproject.toml)
 six==1.16.0
     # via main-wrapper
@@ -49,11 +49,11 @@
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `prunerr-1.1.8/requirements/py38/build.txt` & `prunerr-1.1.9b1/requirements/py39/build.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,37 +16,35 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
     #   commitizen
     #   keyring
     #   twine
-importlib-resources==5.12.0
-    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -60,22 +58,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -85,52 +81,42 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
-typing-extensions==4.5.0
-    # via
-    #   rich
-    #   setuptools-scm
-urllib3==1.26.15
+urllib3==2.0.2
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `prunerr-1.1.8/requirements/py38/devel.txt` & `prunerr-1.1.9b1/requirements/py38/devel.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,23 +16,33 @@
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
 autopep8==2.0.2
     # via prunerr (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via prunerr (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   pip-tools
     #   prunerr (pyproject.toml)
     #   pyroma
 certifi==2022.12.7
     # via requests
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 cli-exit-tools==1.2.3.2
     # via
     #   lib-detect-testenv
     #   pathlib3x
 click==8.1.3
@@ -49,15 +59,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.5
     # via prunerr (pyproject.toml)
 dill==0.3.6
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
@@ -84,19 +94,23 @@
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
 lib-detect-testenv==2.0.3
     # via cli-exit-tools
+license-expression==30.1.0
+    # via reuse
 main-wrapper==0.1.1
     # via service-logging
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
@@ -176,33 +190,38 @@
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
 pytest==7.3.1
     # via prunerr (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   prunerr (pyproject.toml)
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
+    #   reuse
     #   transmission-rpc
     #   xenon
 requests-mock==1.10.0
     # via prunerr (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
+reuse==1.0.0
+    # via prunerr (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via prunerr (pyproject.toml)
 rstcheck-core==1.0.3
@@ -246,32 +265,32 @@
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
     #   rich
     #   transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `prunerr-1.1.8/requirements/py38/user.txt` & `prunerr-1.1.9b1/requirements/py39/user.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py39/user.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
 certifi==2022.12.7
     # via requests
@@ -27,23 +27,23 @@
     # via cli-exit-tools
 main-wrapper==0.1.1
     # via service-logging
 pathlib3x==2.0.2.1 ; python_version < "3.10"
     # via prunerr (pyproject.toml)
 pyyaml==6.0
     # via prunerr (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   transmission-rpc
 service-logging==0.1.1
     # via prunerr (pyproject.toml)
 six==1.16.0
     # via main-wrapper
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
```

### Comparing `prunerr-1.1.8/requirements/py39/build.txt` & `prunerr-1.1.9b1/requirements/py37/build.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,35 +16,40 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
+    #   argcomplete
     #   commitizen
     #   keyring
+    #   pre-commit
     #   twine
+    #   virtualenv
+importlib-resources==5.12.0
+    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -58,22 +63,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -83,48 +86,51 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via setuptools-scm
-urllib3==1.26.15
+    # via
+    #   commitizen
+    #   importlib-metadata
+    #   markdown-it-py
+    #   platformdirs
+    #   rich
+urllib3==2.0.2
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `prunerr-1.1.8/requirements/py39/devel.txt` & `prunerr-1.1.9b1/requirements/py37/devel.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=requirements/py39/devel.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py37/devel.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
 astroid==2.15.4
     # via
@@ -14,25 +14,37 @@
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
 autoflake==1.7.8
     # via prunerr (pyproject.toml)
 autopep8==2.0.2
     # via prunerr (pyproject.toml)
+backports-cached-property==1.0.2 ; python_version < "3.8"
+    # via prunerr (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via prunerr (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   pip-tools
     #   prunerr (pyproject.toml)
     #   pyroma
 certifi==2022.12.7
     # via requests
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 cli-exit-tools==1.2.3.2
     # via
     #   lib-detect-testenv
     #   pathlib3x
 click==8.1.3
@@ -49,15 +61,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.5
     # via prunerr (pyproject.toml)
 dill==0.3.6
     # via pylint
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
@@ -77,26 +89,41 @@
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
+    #   pluggy
+    #   pydocstyle
+    #   pytest
+    #   rstcheck
+    #   rstcheck-core
+    #   stevedore
 incremental==22.10.0
     # via towncrier
 iniconfig==2.0.0
     # via pytest
-isort==5.12.0
+isort==5.11.5
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
 lib-detect-testenv==2.0.3
     # via cli-exit-tools
+license-expression==30.1.0
+    # via reuse
 main-wrapper==0.1.1
     # via service-logging
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
@@ -176,33 +203,38 @@
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
 pytest==7.3.1
     # via prunerr (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   prospector
     #   prunerr (pyproject.toml)
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
+    #   reuse
     #   transmission-rpc
     #   xenon
 requests-mock==1.10.0
     # via prunerr (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
+reuse==1.0.0
+    # via prunerr (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via prunerr (pyproject.toml)
 rstcheck-core==1.0.3
@@ -220,15 +252,15 @@
     #   main-wrapper
     #   mando
     #   requests-mock
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
-stevedore==5.0.0
+stevedore==3.5.2
     # via bandit
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
@@ -246,37 +278,50 @@
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.5.2
     # via pyroma
+typed-ast==1.5.4
+    # via
+    #   astroid
+    #   black
+    #   mypy
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
+    #   gitpython
+    #   importlib-metadata
     #   mypy
+    #   platformdirs
     #   pydantic
     #   pylint
+    #   rich
+    #   rstcheck
+    #   rstcheck-core
     #   transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via prunerr (pyproject.toml)
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `prunerr-1.1.8/requirements/py39/user.txt` & `prunerr-1.1.9b1/requirements/py310/user.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py39/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py310/user.txt --resolver=backtracking pyproject.toml
 #
 argcomplete==3.0.8
     # via prunerr (pyproject.toml)
 arrapi==1.4.2
     # via prunerr (pyproject.toml)
 certifi==2022.12.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-cli-exit-tools==1.2.3.2
-    # via
-    #   lib-detect-testenv
-    #   pathlib3x
-click==8.1.3
-    # via
-    #   cli-exit-tools
-    #   lib-detect-testenv
-    #   pathlib3x
 idna==3.4
     # via requests
-lib-detect-testenv==2.0.3
-    # via cli-exit-tools
 main-wrapper==0.1.1
     # via service-logging
-pathlib3x==2.0.2.1 ; python_version < "3.10"
-    # via prunerr (pyproject.toml)
 pyyaml==6.0
     # via prunerr (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   transmission-rpc
 service-logging==0.1.1
     # via prunerr (pyproject.toml)
 six==1.16.0
     # via main-wrapper
 tenacity==8.2.2
     # via prunerr (pyproject.toml)
 transmission-rpc==3.4.2
     # via prunerr (pyproject.toml)
 typing-extensions==4.5.0
     # via transmission-rpc
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
```

### Comparing `prunerr-1.1.8/setup.cfg` & `prunerr-1.1.9b1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 	sonarr
 	radarr
 	transmission
 	bittorent
 	torrent
 classifiers = 
 	Development Status :: 4 - Beta
+	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: POSIX :: BSD
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.7
 	Topic :: Communications :: File Sharing
 	Topic :: Internet
 
 [options]
@@ -56,14 +57,15 @@
 devel = 
 	requests-mock
 	pytest
 	coverage
 	prospector[with_everything]
 	xenon
 	rstcheck
+	reuse<1.1.0
 	black
 	autoflake
 	autopep8
 	types-PyYAML
 	pip-tools
 	towncrier
 	build
```

### Comparing `prunerr-1.1.8/src/prunerr/__init__.py` & `prunerr-1.1.9b1/src/prunerr/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # PYTHON_ARGCOMPLETE_OK
+
 """
 Remove Servarr download client items to preserve disk space according to rules.
 """
 
 import sys
 import contextlib
 import logging
```

### Comparing `prunerr-1.1.8/src/prunerr/downloadclient.py` & `prunerr-1.1.9b1/src/prunerr/downloadclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Prunerr interaction with download clients.
 """
 
 import re
 import shutil
 import urllib.parse
```

### Comparing `prunerr-1.1.8/src/prunerr/downloaditem.py` & `prunerr-1.1.9b1/src/prunerr/downloaditem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Prunerr interaction with download clients.
 """
 
 import os
 import time
 import urllib.parse
```

### Comparing `prunerr-1.1.8/src/prunerr/home/.config/prunerr.yml` & `prunerr-1.1.9b1/src/prunerr/home/.config/prunerr.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 daemon:
   ## The number of seconds to wait between each execution of the order of operations.
   ## Default: 60
   # poll: 60
 servarrs:
   ## The Servarr application instances, such as Sonarr or Radarr, whose download client
   ## items should be pruned.  At least one Servarr instance must be configured.
```

### Comparing `prunerr-1.1.8/src/prunerr/operations.py` & `prunerr-1.1.9b1/src/prunerr/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Download item metadata operations used in Prunerr configuration.
 
 Used to determine item indexer priority, reviewing grabbed items, etc.
 """
 
 import re
```

### Comparing `prunerr-1.1.8/src/prunerr/runner.py` & `prunerr-1.1.9b1/src/prunerr/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Run Prunerr commands across multiple Servarr instances and download clients.
 """
 
 import gc
 import os
 import time
```

### Comparing `prunerr-1.1.8/src/prunerr/servarr.py` & `prunerr-1.1.9b1/src/prunerr/servarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Prunerr interaction with Servarr instances.
 """
 
 import dataclasses
 import time
 import urllib.parse
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/Makefile` & `prunerr-1.1.9b1/src/prunerr/tests/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Capture test fixture generation and other testing maintenance tasks
 
 ### Defensive settings for make:
 #     https://tech.davis-hansson.com/p/make/
 SHELL:=bash
 .ONESHELL:
 .SHELLFLAGS:=-xeu -o pipefail -c
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/__init__.py` & `prunerr-1.1.9b1/src/prunerr/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Tests for Prunerr.
 """
 
 import sys
 import os
 import functools
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/example-5s.mkv` & `prunerr-1.1.9b1/src/prunerr/tests/example-5s.mkv`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/home/daemon/.config/prunerr.yml` & `prunerr-1.1.9b1/src/prunerr/tests/home/daemon/.config/prunerr.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 daemon:
   # Cover the `time.sleep(1)` part of the `daemon` loop.
   poll: 1
 servarrs:
   Sonarr:
     url: "http://localhost:8989"
     api-key: ""
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/home/download-clients/.config/prunerr.yml` & `prunerr-1.1.9b1/src/prunerr/tests/home/download-clients/.config/prunerr.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 servarrs:
   Sonarr:
     url: "http://localhost:8989"
     api-key: ""
     type: "sonarr"
   Radarr:
     url: "http://localhost:7878"
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml` & `prunerr-1.1.9b1/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 servarrs:
   Sonarr:
     url: "http://localhost:8989"
     api-key: ""
     type: "sonarr"
   Radarr:
     url: "http://localhost:7878"
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json` & `prunerr-1.1.9b1/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_cli.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
-Test the Prunerr Command-Line Interface.
+Test the prunerr Command-Line Interface.
 """
 
 import sys
 import os
 import io
 import runpy
 import subprocess  # nosec B404
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_daemon.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_daemon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Tests covering the Prunerr `daemon` sub-command.
 """
 
 import os
 import pathlib
 import time
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_downloadclient.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_downloadclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test Prunerr's interaction with download clients.
 """
 # Aggregate download client configurations from Servarr and the configuration file.
 
 import os
 import pathlib
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_downloaditem.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_downloaditem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test Prunerr's interaction with download items.
 """
 
 import os
 import pathlib
 import logging
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_free_space.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_free_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Prunerr removes imported items to free space according to configured rules.
 """
 
 import os
 import shutil
 import logging
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_move.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_move.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test moving download items that Servarr has acted on.
 """
 
 import os
 import functools
 import pathlib
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_operations.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test Prunerr's configurable operations.
 """
 
 import os
 import logging
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_review.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Prunerr performs various configurable action on download items accorging to rules.
 """
 
 import os
 import functools
 import pathlib
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_runner.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Tests covering the `prunerr.runner` module.
 """
 
 import os
 import pathlib
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_servarr.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_servarr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test Prunerr's interaction with Servarr instances.
 """
 
 import os
 
 from unittest import mock
```

### Comparing `prunerr-1.1.8/src/prunerr/tests/test_verify.py` & `prunerr-1.1.9b1/src/prunerr/tests/test_verify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Prunerr verifies corrupt items and resumes them once verified.
 """
 
 import os
 
 from unittest import mock
```

### Comparing `prunerr-1.1.8/src/prunerr/utils.py` & `prunerr-1.1.9b1/src/prunerr/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Utility functions or other shared constants and values.
 
 Particularly useful to avoid circular imports.
 """
 
 import os
```

### Comparing `prunerr-1.1.8/src/prunerr.egg-info/PKG-INFO` & `prunerr-1.1.9b1/src/prunerr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.8
+Version: 1.1.9b1
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
-License-File: LICENSE
+
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
 
 ########################################################################################
 Prunerr
 ########################################################################################
 Perma-seed Servarr media libraries
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/prunerr.svg?logo=pypi&label=PyPI&logoColor=gold
           :alt: PyPI latest release version
           :target: https://pypi.org/project/prunerr/
-       .. figure:: https://img.shields.io/pypi/dm/prunerr.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-          :alt: PyPI downloads per month
-          :target: https://pypi.org/project/prunerr/
        .. figure:: https://img.shields.io/pypi/pyversions/prunerr.svg?logo=python&label=Python&logoColor=gold
           :alt: PyPI Python versions
           :target: https://pypi.org/project/prunerr/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
           :alt: Python code style
           :target: https://github.com/psf/black
+       .. figure:: https://api.reuse.software/badge/gitlab.com/rpatterson/prunerr
+          :alt: REUSE license status
+          :target: https://api.reuse.software/info/gitlab.com/rpatterson/prunerr
 
      - .. figure:: https://gitlab.com/rpatterson/prunerr/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/prunerr/-/releases
        .. figure:: https://gitlab.com/rpatterson/prunerr/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
           :target: https://gitlab.com/rpatterson/prunerr/-/commits/main
@@ -162,16 +166,14 @@
 See the `Usage`_ section below for full details.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
-Install and use either via a local, native installation or a Docker container image:
-
 Local/Native Installation
 ========================================================================================
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ pip3 install --user prunerr
 
@@ -184,30 +186,30 @@
 `the example ./docker-compose.yml file`_ for an example configuration.  Once you have
 your configuration, you can create and run the container::
 
   $ docker compose up
 
 Alternatively, you make use the image directly.  Pull `the Docker image`_::
 
-  $ docker pull "registry.gitlab.org/rpatterson/prunerr"
+  $ docker pull "registry.gitlab.com/rpatterson/prunerr"
 
 And then use the image to create and run a container::
 
-  $ docker run --rm -it "registry.gitlab.org/rpatterson/prunerr" ...
+  $ docker run --rm -it "registry.gitlab.com/rpatterson/prunerr" ...
 
 Images variant tags are published for the Python version, branch, and major/minor
 versions so that users can control when they get new images over time,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:py310-main``.  The canonical Python
-version is 3.10 which is the version used in tags without ``py###``,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:main``.  Pre-releases are from
+e.g. ``registry.gitlab.com/rpatterson/prunerr:py310-main``.  The canonical
+Python version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.com/rpatterson/prunerr:main``.  Pre-releases are from
 ``develop`` and final releases are from ``main`` which is also the default for tags
-without a branch, e.g. ``registry.gitlab.org/merpatterson/prunerr:py310``. The
+without a branch, e.g. ``registry.gitlab.com/rpatterson/prunerr:py310``. The
 major/minor version tags are only applied to the final release images and without the
 corresponding ``main`` branch tag,
-e.g. ``registry.gitlab.org/merpatterson/prunerr:py310-v0.8``.
+e.g. ``registry.gitlab.com/rpatterson/prunerr:py310-v0.8``.
 
 Multi-platform Docker images are published containing images for the following
 platforms or architectures in the Python 3.10 ``py310`` variant:
 
 - ``linux/amd64``
 - ``linux/arm64``
 - ``linux/arm/v7``
```

### Comparing `prunerr-1.1.8/src/prunerr.egg-info/SOURCES.txt` & `prunerr-1.1.9b1/src/prunerr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,34 @@
+.cz.toml
 .dir-locals.el.in
 .dockerignore
 .env.in
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 .prospector.yaml
 CONTRIBUTING.rst
 Dockerfile
 Dockerfile.devel
-LICENSE
 Makefile
 NEWS-VERSION.rst
 NEWS.rst
 README.rst
 TODO.rst
 docker-compose-servarr.yml
 docker-compose.override.yml
 docker-compose.yml
 pyproject.toml
 setup.cfg
+towncrier.toml
 tox.ini
 .github/workflows/build-test.yml
+.reuse/dep5
+.tox/.gitignore
+LICENSES/MIT.txt
 bin/cz-check-bump
 bin/entrypoint
 bin/get-base-version
 bin/hadolint
 build-host/Dockerfile
 build-host/Makefile
 build-host/README.rst
@@ -36,14 +40,15 @@
 build-host/requirements.txt.in
 build-host/bin/entrypoint
 dist/.gitignore
 gitlab-runner/docker-compose.yml
 gitlab-runner/config/config.toml.in
 home/.gitignore
 home/.pypirc.in
+newsfragments/.gitignore
 requirements/build.txt.in
 requirements/py310/build.txt
 requirements/py310/devel.txt
 requirements/py310/user.txt
 requirements/py311/build.txt
 requirements/py311/devel.txt
 requirements/py311/user.txt
@@ -62,22 +67,22 @@
 src/prunerr/downloadclient.py
 src/prunerr/downloaditem.py
 src/prunerr/operations.py
 src/prunerr/runner.py
 src/prunerr/servarr.py
 src/prunerr/utils.py
 src/prunerr/version.py
+src/prunerr.egg-info/.gitignore
 src/prunerr.egg-info/PKG-INFO
 src/prunerr.egg-info/SOURCES.txt
 src/prunerr.egg-info/dependency_links.txt
 src/prunerr.egg-info/entry_points.txt
 src/prunerr.egg-info/requires.txt
 src/prunerr.egg-info/top_level.txt
 src/prunerr/home/.config/prunerr.yml
-src/prunerr/newsfragments/.gitignore
 src/prunerr/tests/Makefile
 src/prunerr/tests/__init__.py
 src/prunerr/tests/example-5s.mkv
 src/prunerr/tests/test_cli.py
 src/prunerr/tests/test_daemon.py
 src/prunerr/tests/test_downloadclient.py
 src/prunerr/tests/test_downloaditem.py
@@ -541,8 +546,26 @@
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
-src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+var/.gitignore
+var-docker/.gitignore
+var-docker/media/Library/.gitignore
+var-docker/py310/.gitignore
+var-docker/py310/.tox/.gitignore
+var-docker/py310/prunerr.egg-info/.gitignore
+var-docker/py311/.gitignore
+var-docker/py311/.tox/.gitignore
+var-docker/py311/prunerr.egg-info/.gitignore
+var-docker/py37/.gitignore
+var-docker/py37/.tox/.gitignore
+var-docker/py37/prunerr.egg-info/.gitignore
+var-docker/py38/.gitignore
+var-docker/py38/.tox/.gitignore
+var-docker/py38/prunerr.egg-info/.gitignore
+var-docker/py39/.gitignore
+var-docker/py39/.tox/.gitignore
+var-docker/py39/prunerr.egg-info/.gitignore
```

### Comparing `prunerr-1.1.8/tox.ini` & `prunerr-1.1.9b1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+; SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+;
+; SPDX-License-Identifier: MIT
+
 [tox]
 # https://devguide.python.org/versions/#supported-versions
-envlist = py{37,38,39,310,311}
+envlist = py{310,311,39,38,37}
 # https://tox.wiki/en/latest/example/package.html#setuptools
 isolated_build = True
 
 [testenv]
 description = Run tests and checks for code and content
 package = wheel
 wheel_build_env = .pkg
-passenv =
-    HOME
-    PYTHON_HOST_ENV
-    DEBUG
 extras = devel
 deps = -rrequirements/{envname}/devel.txt
 commands =
 # Create a directory for artifacts not managed by `$ tox`:
     python -c 'import pathlib; \
         pathlib.Path("./build/{envname}").mkdir(parents=True, exist_ok=True)'
 # Fail fast.  Run quick tests and checks first to save time in the inner loop of
@@ -41,15 +41,17 @@
 # https://github.com/PyCQA/prospector/issues/599#issue-1600120419
     vulture "./src/prunerr/"
 # https://xenon.readthedocs.io/en/latest/#an-actual-example
     xenon --max-absolute "C" --max-modules "B" --max-average "A" \
         "./src/prunerr/"
 # Check documentation as much a possible:
     rstcheck -r "./README.rst" "./CONTRIBUTING.rst" "./TODO.rst" \
-        "./src/prunerr/" "./build-host/"
+        "./newsfragments/" "./build-host/"
+# Check copyright and licensing:
+    reuse lint
 # Ensure this package is correctly installed into this environment.
     python -m "prunerr" --help
     prunerr --help
 # Run more time consuming tests and checks last.
     coverage run --data-file="./build/{envname}/.coverage" -m pytest \
         --junit-xml="./build/{envname}/pytest-junit.xml" -s
     coverage json --fail-under=0 --data-file="./build/{envname}/.coverage" \
@@ -61,15 +63,12 @@
     coverage html --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -d "./build/{envname}/htmlcov"
     coverage report --data-file="./build/{envname}/.coverage"
 
 [testenv:build]
 description = Independent build, release, devel tools (requires PYTHON_HOST_ENV)
 skip_install = true
-# Workaround an issue with `skip_install` and passing in the `--installpkg` CLI option:
-# https://github.com/tox-dev/tox/issues/2442#issuecomment-1347549575
-package_env =
 deps = -rrequirements/{env:PYTHON_HOST_ENV:py310}/build.txt
 commands =
 
 [testenv:.pkg]
-deps = build
+deps = build
```

