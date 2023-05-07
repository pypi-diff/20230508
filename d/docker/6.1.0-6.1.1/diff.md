# Comparing `tmp/docker-6.1.0.tar.gz` & `tmp/docker-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-6.1.0.tar", last modified: Fri May  5 15:55:56 2023, max compression
+gzip compressed data, was "docker-6.1.1.tar", last modified: Sun May  7 23:54:11 2023, max compression
```

## Comparing `docker-6.1.0.tar` & `docker-6.1.1.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.653294 docker-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 15:55:45.000000 docker-6.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 15:55:45.000000 docker-6.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 15:55:45.000000 docker-6.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.633294 docker-6.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-05 15:55:45.000000 docker-6.1.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.633294 docker-6.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-05 15:55:45.000000 docker-6.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-05 15:55:45.000000 docker-6.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-05 15:55:45.000000 docker-6.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-05 15:55:45.000000 docker-6.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-05 15:55:45.000000 docker-6.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 15:55:45.000000 docker-6.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 15:55:45.000000 docker-6.1.0/Dockerfile-docs
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-05 15:55:45.000000 docker-6.1.0/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-05 15:55:45.000000 docker-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-05 15:55:45.000000 docker-6.1.0/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 15:55:45.000000 docker-6.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-05 15:55:45.000000 docker-6.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-05 15:55:56.653294 docker-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-05 15:55:45.000000 docker-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.637294 docker-6.1.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 15:55:45.000000 docker-6.1.0/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 15:55:56.000000 docker-6.1.0/docker/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.637294 docker-6.1.0/docker/api/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    52445 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/exec_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-05 15:55:45.000000 docker-6.1.0/docker/api/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-05 15:55:45.000000 docker-6.1.0/docker/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-05 15:55:45.000000 docker-6.1.0/docker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-05 15:55:45.000000 docker-6.1.0/docker/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.637294 docker-6.1.0/docker/context/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 15:55:45.000000 docker-6.1.0/docker/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-05 15:55:45.000000 docker-6.1.0/docker/context/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-05 15:55:45.000000 docker-6.1.0/docker/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-05 15:55:45.000000 docker-6.1.0/docker/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.637294 docker-6.1.0/docker/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 15:55:45.000000 docker-6.1.0/docker/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-05 15:55:45.000000 docker-6.1.0/docker/credentials/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-05 15:55:45.000000 docker-6.1.0/docker/credentials/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-05 15:55:45.000000 docker-6.1.0/docker/credentials/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 15:55:45.000000 docker-6.1.0/docker/credentials/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-05 15:55:45.000000 docker-6.1.0/docker/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.641294 docker-6.1.0/docker/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45992 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-05 15:55:45.000000 docker-6.1.0/docker/models/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-05 15:55:45.000000 docker-6.1.0/docker/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.641294 docker-6.1.0/docker/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 15:55:45.000000 docker-6.1.0/docker/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 15:55:45.000000 docker-6.1.0/docker/transport/basehttpadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-05 15:55:45.000000 docker-6.1.0/docker/transport/npipeconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-05 15:55:45.000000 docker-6.1.0/docker/transport/npipesocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-05 15:55:45.000000 docker-6.1.0/docker/transport/sshconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-05 15:55:45.000000 docker-6.1.0/docker/transport/ssladapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-05 15:55:45.000000 docker-6.1.0/docker/transport/unixconn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.641294 docker-6.1.0/docker/types/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    33158 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-05 15:55:45.000000 docker-6.1.0/docker/types/swarm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.641294 docker-6.1.0/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/fnmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-05-05 15:55:45.000000 docker-6.1.0/docker/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 15:55:45.000000 docker-6.1.0/docker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.637294 docker-6.1.0/docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-05 15:55:56.000000 docker-6.1.0/docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-05 15:55:56.000000 docker-6.1.0/docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:55:56.000000 docker-6.1.0/docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:55:56.000000 docker-6.1.0/docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 15:55:56.000000 docker-6.1.0/docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 15:55:56.000000 docker-6.1.0/docker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.645294 docker-6.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.645294 docker-6.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 15:55:45.000000 docker-6.1.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.645294 docker-6.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 15:55:45.000000 docker-6.1.0/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-05 15:55:45.000000 docker-6.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    75067 2023-05-05 15:55:45.000000 docker-6.1.0/docs/change-log.md
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-05 15:55:45.000000 docker-6.1.0/docs/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-05 15:55:45.000000 docker-6.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-05 15:55:45.000000 docker-6.1.0/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-05 15:55:45.000000 docker-6.1.0/docs/containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-05 15:55:45.000000 docker-6.1.0/docs/favicon_whale.png
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-05 15:55:45.000000 docker-6.1.0/docs/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-05 15:55:45.000000 docker-6.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-05 15:55:45.000000 docker-6.1.0/docs/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 15:55:45.000000 docker-6.1.0/docs/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 15:55:45.000000 docker-6.1.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-05 15:55:45.000000 docker-6.1.0/docs/secrets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-05 15:55:45.000000 docker-6.1.0/docs/services.rst
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-05 15:55:45.000000 docker-6.1.0/docs/swarm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-05 15:55:45.000000 docker-6.1.0/docs/tls.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.645294 docker-6.1.0/docs/user_guides/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 15:55:45.000000 docker-6.1.0/docs/user_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-05 15:55:45.000000 docker-6.1.0/docs/user_guides/multiplex.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-05 15:55:45.000000 docker-6.1.0/docs/user_guides/swarm_services.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 15:55:45.000000 docker-6.1.0/docs/volumes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 15:55:45.000000 docker-6.1.0/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 15:55:45.000000 docker-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 15:55:45.000000 docker-6.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 15:55:45.000000 docker-6.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.645294 docker-6.1.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-05-05 15:55:45.000000 docker-6.1.0/scripts/release.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2186 2023-05-05 15:55:45.000000 docker-6.1.0/scripts/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 15:55:56.653294 docker-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-05 15:55:45.000000 docker-6.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 15:55:45.000000 docker-6.1.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.645294 docker-6.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-05 15:55:45.000000 docker-6.1.0/tests/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-05 15:55:45.000000 docker-6.1.0/tests/Dockerfile-dind-certs
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 15:55:45.000000 docker-6.1.0/tests/Dockerfile-ssh-dind
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.645294 docker-6.1.0/tests/gpg-keys/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 15:55:45.000000 docker-6.1.0/tests/gpg-keys/ownertrust
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 15:55:45.000000 docker-6.1.0/tests/gpg-keys/secret
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-05 15:55:45.000000 docker-6.1.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.649294 docker-6.1.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    56459 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_healthcheck_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18933 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_secret_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    62334 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/context_api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.649294 docker-6.1.0/tests/integration/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/credentials/create_gpg_key.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/credentials/store_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/credentials/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_nodes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/models_volumes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/regression_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.633294 docker-6.1.0/tests/integration/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.649294 docker-6.1.0/tests/integration/testdata/dummy-plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/testdata/dummy-plugin/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.633294 docker-6.1.0/tests/integration/testdata/dummy-plugin/rootfs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.649294 docker-6.1.0/tests/integration/testdata/dummy-plugin/rootfs/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.649294 docker-6.1.0/tests/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.633294 docker-6.1.0/tests/ssh/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.649294 docker-6.1.0/tests/ssh/config/client/
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/config/client/id_rsa
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/config/client/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.649294 docker-6.1.0/tests/ssh/config/server/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/config/server/known_ed25519
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/config/server/known_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/config/server/sshd_config
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/config/server/unknown_ed25519
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/config/server/unknown_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 15:55:45.000000 docker-6.1.0/tests/ssh/connect_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.653294 docker-6.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    58724 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28287 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/context_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/dockertypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/fake_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/fake_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/fake_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    24231 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/models_secrets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/sshadapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/ssladapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/swarm_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.633294 docker-6.1.0/tests/unit/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:56.653294 docker-6.1.0/tests/unit/testdata/certs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/testdata/certs/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/testdata/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/testdata/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/types_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16046 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/utils_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/utils_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/utils_json_stream_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/utils_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23196 2023-05-05 15:55:45.000000 docker-6.1.0/tests/unit/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-05 15:55:45.000000 docker-6.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.693834 docker-6.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-07 23:54:04.000000 docker-6.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 23:54:04.000000 docker-6.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-07 23:54:04.000000 docker-6.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-07 23:54:04.000000 docker-6.1.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-07 23:54:04.000000 docker-6.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 23:54:04.000000 docker-6.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-07 23:54:04.000000 docker-6.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-07 23:54:04.000000 docker-6.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-07 23:54:04.000000 docker-6.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-07 23:54:04.000000 docker-6.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-07 23:54:04.000000 docker-6.1.1/Dockerfile-docs
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-07 23:54:04.000000 docker-6.1.1/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-07 23:54:04.000000 docker-6.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-07 23:54:04.000000 docker-6.1.1/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 23:54:04.000000 docker-6.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-07 23:54:04.000000 docker-6.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-07 23:54:11.693834 docker-6.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-07 23:54:04.000000 docker-6.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 23:54:04.000000 docker-6.1.1/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 23:54:11.000000 docker-6.1.1/docker/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52534 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/exec_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-07 23:54:04.000000 docker-6.1.1/docker/api/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-07 23:54:04.000000 docker-6.1.1/docker/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-07 23:54:04.000000 docker-6.1.1/docker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-07 23:54:04.000000 docker-6.1.1/docker/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/context/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-07 23:54:04.000000 docker-6.1.1/docker/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 23:54:04.000000 docker-6.1.1/docker/credentials/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-07 23:54:04.000000 docker-6.1.1/docker/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46077 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-07 23:54:04.000000 docker-6.1.1/docker/models/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-07 23:54:04.000000 docker-6.1.1/docker/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.677834 docker-6.1.1/docker/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/basehttpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/npipeconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/npipesocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/sshconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/ssladapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-07 23:54:04.000000 docker-6.1.1/docker/transport/unixconn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docker/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27481 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33158 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-07 23:54:04.000000 docker-6.1.1/docker/types/swarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/fnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-05-07 23:54:04.000000 docker-6.1.1/docker/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-07 23:54:04.000000 docker-6.1.1/docker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.673833 docker-6.1.1/docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 23:54:11.000000 docker-6.1.1/docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-07 23:54:04.000000 docker-6.1.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 23:54:04.000000 docker-6.1.1/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-07 23:54:04.000000 docker-6.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    75067 2023-05-07 23:54:04.000000 docker-6.1.1/docs/change-log.md
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-07 23:54:04.000000 docker-6.1.1/docs/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-07 23:54:04.000000 docker-6.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-07 23:54:04.000000 docker-6.1.1/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-07 23:54:04.000000 docker-6.1.1/docs/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-07 23:54:04.000000 docker-6.1.1/docs/favicon_whale.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-07 23:54:04.000000 docker-6.1.1/docs/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-07 23:54:04.000000 docker-6.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-07 23:54:04.000000 docker-6.1.1/docs/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-07 23:54:04.000000 docker-6.1.1/docs/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-07 23:54:04.000000 docker-6.1.1/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-07 23:54:04.000000 docker-6.1.1/docs/secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-07 23:54:04.000000 docker-6.1.1/docs/services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 23:54:04.000000 docker-6.1.1/docs/swarm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-07 23:54:04.000000 docker-6.1.1/docs/tls.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.681834 docker-6.1.1/docs/user_guides/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-07 23:54:04.000000 docker-6.1.1/docs/user_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-07 23:54:04.000000 docker-6.1.1/docs/user_guides/multiplex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-07 23:54:04.000000 docker-6.1.1/docs/user_guides/swarm_services.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-07 23:54:04.000000 docker-6.1.1/docs/volumes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 23:54:04.000000 docker-6.1.1/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-07 23:54:04.000000 docker-6.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 23:54:04.000000 docker-6.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-07 23:54:04.000000 docker-6.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-05-07 23:54:04.000000 docker-6.1.1/scripts/release.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2186 2023-05-07 23:54:04.000000 docker-6.1.1/scripts/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 23:54:11.693834 docker-6.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-07 23:54:04.000000 docker-6.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 23:54:04.000000 docker-6.1.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-07 23:54:04.000000 docker-6.1.1/tests/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-07 23:54:04.000000 docker-6.1.1/tests/Dockerfile-dind-certs
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 23:54:04.000000 docker-6.1.1/tests/Dockerfile-ssh-dind
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/gpg-keys/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-07 23:54:04.000000 docker-6.1.1/tests/gpg-keys/ownertrust
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 23:54:04.000000 docker-6.1.1/tests/gpg-keys/secret
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-07 23:54:04.000000 docker-6.1.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56459 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_healthcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18933 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_secret_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62334 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/context_api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.685834 docker-6.1.1/tests/integration/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/create_gpg_key.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/store_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/credentials/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_nodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/models_volumes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/regression_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/integration/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/integration/testdata/dummy-plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/testdata/dummy-plugin/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/integration/testdata/dummy-plugin/rootfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/integration/testdata/dummy-plugin/rootfs/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/ssh/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/ssh/config/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/client/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/client/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.689834 docker-6.1.1/tests/ssh/config/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/known_ed25519
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/known_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/sshd_config
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/unknown_ed25519
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/config/server/unknown_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 23:54:04.000000 docker-6.1.1/tests/ssh/connect_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.693834 docker-6.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59084 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28287 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/dockertypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/fake_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/fake_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/fake_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24231 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_secrets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/sshadapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/ssladapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/swarm_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.669834 docker-6.1.1/tests/unit/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:11.693834 docker-6.1.1/tests/unit/testdata/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/testdata/certs/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/testdata/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/testdata/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/types_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16046 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_json_stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23196 2023-05-07 23:54:04.000000 docker-6.1.1/tests/unit/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-07 23:54:04.000000 docker-6.1.1/tox.ini
```

### Comparing `docker-6.1.0/.github/workflows/ci.yml` & `docker-6.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/.github/workflows/release.yml` & `docker-6.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/CONTRIBUTING.md` & `docker-6.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/Jenkinsfile` & `docker-6.1.1/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/LICENSE` & `docker-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/MAINTAINERS` & `docker-6.1.1/MAINTAINERS`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/Makefile` & `docker-6.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/PKG-INFO` & `docker-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 6.1.0
+Version: 6.1.1
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-6.1.0/README.md` & `docker-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/build.py` & `docker-6.1.1/docker/api/build.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/client.py` & `docker-6.1.1/docker/api/client.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/config.py` & `docker-6.1.1/docker/api/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/container.py` & `docker-6.1.1/docker/api/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -674,15 +674,16 @@
         """
         Inspect changes on a container's filesystem.
 
         Args:
             container (str): The container to diff
 
         Returns:
-            (str)
+            (list) A list of dictionaries containing the attributes `Path`
+                and `Kind`.
 
         Raises:
             :py:class:`docker.errors.APIError`
                 If the server returns an error.
         """
         return self._result(
             self._get(self._url("/containers/{0}/changes", container)), True
@@ -1159,16 +1160,17 @@
             params['one-shot'] = one_shot
         if stream:
             if one_shot:
                 raise errors.InvalidArgument(
                     'one_shot is only available in conjunction with '
                     'stream=False'
                 )
-            return self._stream_helper(self._get(url, params=params),
-                                       decode=decode)
+            return self._stream_helper(
+                self._get(url, stream=True, params=params), decode=decode
+            )
         else:
             if decode:
                 raise errors.InvalidArgument(
                     "decode is only available in conjunction with stream=True"
                 )
             return self._result(self._get(url, params=params), json=True)
```

### Comparing `docker-6.1.0/docker/api/daemon.py` & `docker-6.1.1/docker/api/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/exec_api.py` & `docker-6.1.1/docker/api/exec_api.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/image.py` & `docker-6.1.1/docker/api/image.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/network.py` & `docker-6.1.1/docker/api/network.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/plugin.py` & `docker-6.1.1/docker/api/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/secret.py` & `docker-6.1.1/docker/api/secret.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/service.py` & `docker-6.1.1/docker/api/service.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/swarm.py` & `docker-6.1.1/docker/api/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/api/volume.py` & `docker-6.1.1/docker/api/volume.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/auth.py` & `docker-6.1.1/docker/auth.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/client.py` & `docker-6.1.1/docker/client.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/constants.py` & `docker-6.1.1/docker/constants.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/context/api.py` & `docker-6.1.1/docker/context/api.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/context/config.py` & `docker-6.1.1/docker/context/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/context/context.py` & `docker-6.1.1/docker/context/context.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/credentials/errors.py` & `docker-6.1.1/docker/credentials/errors.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/credentials/store.py` & `docker-6.1.1/docker/credentials/store.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/errors.py` & `docker-6.1.1/docker/errors.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/configs.py` & `docker-6.1.1/docker/models/configs.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/containers.py` & `docker-6.1.1/docker/models/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,16 @@
         return self.client.images.get(resp['Id'])
 
     def diff(self):
         """
         Inspect changes on a container's filesystem.
 
         Returns:
-            (str)
+            (list) A list of dictionaries containing the attributes `Path`
+                and `Kind`.
 
         Raises:
             :py:class:`docker.errors.APIError`
                 If the server returns an error.
         """
         return self.client.api.diff(self.id)
```

### Comparing `docker-6.1.0/docker/models/images.py` & `docker-6.1.1/docker/models/images.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/networks.py` & `docker-6.1.1/docker/models/networks.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/nodes.py` & `docker-6.1.1/docker/models/nodes.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/plugins.py` & `docker-6.1.1/docker/models/plugins.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/resource.py` & `docker-6.1.1/docker/models/resource.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/secrets.py` & `docker-6.1.1/docker/models/secrets.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/services.py` & `docker-6.1.1/docker/models/services.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/swarm.py` & `docker-6.1.1/docker/models/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/models/volumes.py` & `docker-6.1.1/docker/models/volumes.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/tls.py` & `docker-6.1.1/docker/tls.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/transport/npipeconn.py` & `docker-6.1.1/docker/transport/npipeconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/transport/npipesocket.py` & `docker-6.1.1/docker/transport/npipesocket.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/transport/sshconn.py` & `docker-6.1.1/docker/transport/sshconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/transport/ssladapter.py` & `docker-6.1.1/docker/transport/ssladapter.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/transport/unixconn.py` & `docker-6.1.1/docker/transport/unixconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/types/__init__.py` & `docker-6.1.1/docker/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/types/containers.py` & `docker-6.1.1/docker/types/containers.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/types/daemon.py` & `docker-6.1.1/docker/types/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/types/healthcheck.py` & `docker-6.1.1/docker/types/healthcheck.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/types/networks.py` & `docker-6.1.1/docker/types/networks.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/types/services.py` & `docker-6.1.1/docker/types/services.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/types/swarm.py` & `docker-6.1.1/docker/types/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/__init__.py` & `docker-6.1.1/docker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/build.py` & `docker-6.1.1/docker/utils/build.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/config.py` & `docker-6.1.1/docker/utils/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/decorators.py` & `docker-6.1.1/docker/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/fnmatch.py` & `docker-6.1.1/docker/utils/fnmatch.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/json_stream.py` & `docker-6.1.1/docker/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/ports.py` & `docker-6.1.1/docker/utils/ports.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/proxy.py` & `docker-6.1.1/docker/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/socket.py` & `docker-6.1.1/docker/utils/socket.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/utils/utils.py` & `docker-6.1.1/docker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker/version.py` & `docker-6.1.1/docker/version.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docker.egg-info/PKG-INFO` & `docker-6.1.1/docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 6.1.0
+Version: 6.1.1
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-6.1.0/docker.egg-info/SOURCES.txt` & `docker-6.1.1/docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/api.rst` & `docker-6.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/change-log.md` & `docker-6.1.1/docs/change-log.md`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/client.rst` & `docker-6.1.1/docs/client.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/conf.py` & `docker-6.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/containers.rst` & `docker-6.1.1/docs/containers.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/favicon_whale.png` & `docker-6.1.1/docs/favicon_whale.png`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/images.rst` & `docker-6.1.1/docs/images.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/index.rst` & `docker-6.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/networks.rst` & `docker-6.1.1/docs/networks.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/nodes.rst` & `docker-6.1.1/docs/nodes.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/plugins.rst` & `docker-6.1.1/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/services.rst` & `docker-6.1.1/docs/services.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/swarm.rst` & `docker-6.1.1/docs/swarm.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/tls.rst` & `docker-6.1.1/docs/tls.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/user_guides/multiplex.rst` & `docker-6.1.1/docs/user_guides/multiplex.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/user_guides/swarm_services.md` & `docker-6.1.1/docs/user_guides/swarm_services.md`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/docs/volumes.rst` & `docker-6.1.1/docs/volumes.rst`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/scripts/release.sh` & `docker-6.1.1/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/scripts/versions.py` & `docker-6.1.1/scripts/versions.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/setup.py` & `docker-6.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/Dockerfile` & `docker-6.1.1/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/Dockerfile-dind-certs` & `docker-6.1.1/tests/Dockerfile-dind-certs`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/gpg-keys/secret` & `docker-6.1.1/tests/gpg-keys/secret`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/helpers.py` & `docker-6.1.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_build_test.py` & `docker-6.1.1/tests/integration/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_client_test.py` & `docker-6.1.1/tests/integration/api_client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_config_test.py` & `docker-6.1.1/tests/integration/api_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_container_test.py` & `docker-6.1.1/tests/integration/api_container_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_exec_test.py` & `docker-6.1.1/tests/integration/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_healthcheck_test.py` & `docker-6.1.1/tests/integration/api_healthcheck_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_image_test.py` & `docker-6.1.1/tests/integration/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_network_test.py` & `docker-6.1.1/tests/integration/api_network_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_plugin_test.py` & `docker-6.1.1/tests/integration/api_plugin_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_secret_test.py` & `docker-6.1.1/tests/integration/api_secret_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_service_test.py` & `docker-6.1.1/tests/integration/api_service_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_swarm_test.py` & `docker-6.1.1/tests/integration/api_swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/api_volume_test.py` & `docker-6.1.1/tests/integration/api_volume_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/base.py` & `docker-6.1.1/tests/integration/base.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/client_test.py` & `docker-6.1.1/tests/integration/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/conftest.py` & `docker-6.1.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/context_api_test.py` & `docker-6.1.1/tests/integration/context_api_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/credentials/store_test.py` & `docker-6.1.1/tests/integration/credentials/store_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/errors_test.py` & `docker-6.1.1/tests/integration/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_containers_test.py` & `docker-6.1.1/tests/integration/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_images_test.py` & `docker-6.1.1/tests/integration/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_networks_test.py` & `docker-6.1.1/tests/integration/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_nodes_test.py` & `docker-6.1.1/tests/integration/models_nodes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_resources_test.py` & `docker-6.1.1/tests/integration/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_services_test.py` & `docker-6.1.1/tests/integration/models_services_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_swarm_test.py` & `docker-6.1.1/tests/integration/models_swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/models_volumes_test.py` & `docker-6.1.1/tests/integration/models_volumes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/integration/regression_test.py` & `docker-6.1.1/tests/integration/regression_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/ssh/api_build_test.py` & `docker-6.1.1/tests/ssh/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/ssh/base.py` & `docker-6.1.1/tests/ssh/base.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/ssh/config/client/id_rsa` & `docker-6.1.1/tests/ssh/config/client/id_rsa`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/ssh/config/client/id_rsa.pub` & `docker-6.1.1/tests/ssh/config/client/id_rsa.pub`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/ssh/connect_test.py` & `docker-6.1.1/tests/ssh/connect_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/api_build_test.py` & `docker-6.1.1/tests/unit/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/api_container_test.py` & `docker-6.1.1/tests/unit/api_container_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1524,18 +1524,29 @@
 
     def test_container_stats(self):
         self.client.stats(fake_api.FAKE_CONTAINER_ID)
 
         fake_request.assert_called_with(
             'GET',
             url_prefix + 'containers/' + fake_api.FAKE_CONTAINER_ID + '/stats',
+            stream=True,
             timeout=60,
             params={'stream': True}
         )
 
+    def test_container_stats_without_streaming(self):
+        self.client.stats(fake_api.FAKE_CONTAINER_ID, stream=False)
+
+        fake_request.assert_called_with(
+            'GET',
+            url_prefix + 'containers/' + fake_api.FAKE_CONTAINER_ID + '/stats',
+            timeout=60,
+            params={'stream': False}
+        )
+
     def test_container_stats_with_one_shot(self):
         self.client.stats(
             fake_api.FAKE_CONTAINER_ID, stream=False, one_shot=True)
 
         fake_request.assert_called_with(
             'GET',
             url_prefix + 'containers/' + fake_api.FAKE_CONTAINER_ID + '/stats',
```

### Comparing `docker-6.1.0/tests/unit/api_exec_test.py` & `docker-6.1.1/tests/unit/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/api_image_test.py` & `docker-6.1.1/tests/unit/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/api_network_test.py` & `docker-6.1.1/tests/unit/api_network_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/api_test.py` & `docker-6.1.1/tests/unit/api_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/api_volume_test.py` & `docker-6.1.1/tests/unit/api_volume_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/auth_test.py` & `docker-6.1.1/tests/unit/auth_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/client_test.py` & `docker-6.1.1/tests/unit/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/context_test.py` & `docker-6.1.1/tests/unit/context_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/dockertypes_test.py` & `docker-6.1.1/tests/unit/dockertypes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/errors_test.py` & `docker-6.1.1/tests/unit/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/fake_api.py` & `docker-6.1.1/tests/unit/fake_api.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/fake_api_client.py` & `docker-6.1.1/tests/unit/fake_api_client.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/fake_stat.py` & `docker-6.1.1/tests/unit/fake_stat.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/models_containers_test.py` & `docker-6.1.1/tests/unit/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/models_images_test.py` & `docker-6.1.1/tests/unit/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/models_networks_test.py` & `docker-6.1.1/tests/unit/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/models_resources_test.py` & `docker-6.1.1/tests/unit/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/models_services_test.py` & `docker-6.1.1/tests/unit/models_services_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/sshadapter_test.py` & `docker-6.1.1/tests/unit/sshadapter_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/ssladapter_test.py` & `docker-6.1.1/tests/unit/ssladapter_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/swarm_test.py` & `docker-6.1.1/tests/unit/swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/utils_build_test.py` & `docker-6.1.1/tests/unit/utils_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/utils_config_test.py` & `docker-6.1.1/tests/unit/utils_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/utils_json_stream_test.py` & `docker-6.1.1/tests/unit/utils_json_stream_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/utils_proxy_test.py` & `docker-6.1.1/tests/unit/utils_proxy_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.1.0/tests/unit/utils_test.py` & `docker-6.1.1/tests/unit/utils_test.py`

 * *Files identical despite different names*

