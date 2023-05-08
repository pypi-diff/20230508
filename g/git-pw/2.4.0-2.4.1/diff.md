# Comparing `tmp/git-pw-2.4.0.tar.gz` & `tmp/git-pw-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-pw-2.4.0.tar", last modified: Tue Dec  6 13:17:11 2022, max compression
+gzip compressed data, was "git-pw-2.4.1.tar", last modified: Mon May  8 11:21:11 2023, max compression
```

## Comparing `git-pw-2.4.0.tar` & `git-pw-2.4.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.714744 git-pw-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-06 13:16:58.000000 git-pw-2.4.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.702744 git-pw-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.706744 git-pw-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2022-12-06 13:16:58.000000 git-pw-2.4.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-06 13:16:58.000000 git-pw-2.4.0/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-06 13:16:58.000000 git-pw-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-06 13:17:11.000000 git-pw-2.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2022-12-06 13:17:11.000000 git-pw-2.4.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-06 13:16:58.000000 git-pw-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-06 13:17:11.714744 git-pw-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2022-12-06 13:16:58.000000 git-pw-2.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.706744 git-pw-2.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2022-12-06 13:16:58.000000 git-pw-2.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-06 13:16:58.000000 git-pw-2.4.0/docs/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-06 13:16:58.000000 git-pw-2.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-06 13:16:58.000000 git-pw-2.4.0/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-06 13:16:58.000000 git-pw-2.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-06 13:16:58.000000 git-pw-2.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.706744 git-pw-2.4.0/git_pw/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2022-12-06 13:16:58.000000 git-pw-2.4.0/git_pw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.706744 git-pw-2.4.0/git_pw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-06 13:17:11.000000 git-pw-2.4.0/git_pw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.710744 git-pw-2.4.0/man/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-add.1
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-apply.1
--rw-r--r--   0 runner    (1001) docker     (123)      616 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-create.1
--rw-r--r--   0 runner    (1001) docker     (123)      442 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-delete.1
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-download.1
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-list.1
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-remove.1
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-show.1
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle-update.1
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-bundle.1
--rw-r--r--   0 runner    (1001) docker     (123)      683 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-patch-apply.1
--rw-r--r--   0 runner    (1001) docker     (123)      619 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-patch-download.1
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-patch-list.1
--rw-r--r--   0 runner    (1001) docker     (123)      426 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-patch-show.1
--rw-r--r--   0 runner    (1001) docker     (123)      975 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-patch-update.1
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-patch.1
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-series-apply.1
--rw-r--r--   0 runner    (1001) docker     (123)      631 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-series-download.1
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-series-list.1
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-series-show.1
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw-series.1
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2022-12-06 13:16:58.000000 git-pw-2.4.0/man/git-pw.1
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-06 13:16:58.000000 git-pw-2.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.710744 git-pw-2.4.0/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.714744 git-pw-2.4.0/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/add-yaml-format-support-5cd6b9028e6d2d8e.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/api-v1-1-5c804713ef435739.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/bundle-crud-47aadae6eb7a20ad.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/drop-pypy-support-f670deb05ef527fe.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/drop-python-35-36-support-add-python-310-7d364b9ba71bf5ba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/drop-python34-support-5e01360fff605972.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/enforce-filtering-by-project-59ed29c4b7edc0a5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/filter-item-list-by-user-id-4f4e7d6dc402093b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/filter-multiple-matches-197ff839f6b578da.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/handle-error-codes-d72c575fb2d9b452.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/initial-release-0aad09064615d023.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-24-60a9fa796f666f35.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-29-884269fdf35f64b2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-40-add82959d7442cfa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-43-c2c166e1fa23fe76.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-44-66b78577e9534f16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-46-50933643cd5c8db0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-47-a9ac87642050d289.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-48-694495f722119fed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-49-865c4f1657b97fce.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/issue-55-bfcf05e02ad305b1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/passthrough-git-am-arguments-23cd0b292304d648.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/patch-apply-applyPatchDeps-option-9a8fed887af313d5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/patch-states-b88240569f8474f1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/python-2-deprecation-c87e311384eab29b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/python-311-support-de330cb1ff9da396.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/random-fixes-3da473a63c253f2d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/remove-python-3-2-3-3-support-8987031bed2c0333.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/require-server-version-93ac0818c293b85e.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/save-patches-before-applying-c5e786156d47d752.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/update-multiple-patches-ed515cd53964c203.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/use-bundle-names-b1b3ee5c2858c96b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      443 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/use-git-pager-settings-ec6555d8311a8bec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2022-12-06 13:16:58.000000 git-pw-2.4.0/releasenotes/notes/warn-on-multiple-filters-a4e01fdb5cf6e459.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-06 13:16:58.000000 git-pw-2.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.714744 git-pw-2.4.0/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2022-12-06 13:16:58.000000 git-pw-2.4.0/rpm/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2022-12-06 13:16:58.000000 git-pw-2.4.0/rpm/git-pw.spec
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2022-12-06 13:17:11.714744 git-pw-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-06 13:16:58.000000 git-pw-2.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-06 13:16:58.000000 git-pw-2.4.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:17:11.714744 git-pw-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 13:16:58.000000 git-pw-2.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2022-12-06 13:16:58.000000 git-pw-2.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19501 2022-12-06 13:16:58.000000 git-pw-2.4.0/tests/test_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2022-12-06 13:16:58.000000 git-pw-2.4.0/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2022-12-06 13:16:58.000000 git-pw-2.4.0/tests/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2022-12-06 13:16:58.000000 git-pw-2.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-06 13:16:58.000000 git-pw-2.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 11:21:01.000000 git-pw-2.4.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.320402 git-pw-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.320402 git-pw-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-08 11:21:01.000000 git-pw-2.4.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 11:21:01.000000 git-pw-2.4.1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 11:21:01.000000 git-pw-2.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-08 11:21:11.000000 git-pw-2.4.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-08 11:21:11.000000 git-pw-2.4.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-08 11:21:01.000000 git-pw-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 11:21:11.332403 git-pw-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-08 11:21:01.000000 git-pw-2.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.324402 git-pw-2.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.324402 git-pw-2.4.1/git_pw/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.324402 git-pw-2.4.1/git_pw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.328403 git-pw-2.4.1/man/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-add.1
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-apply.1
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-create.1
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-delete.1
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-download.1
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-list.1
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-remove.1
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-show.1
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-update.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle.1
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-apply.1
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-download.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-list.1
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-show.1
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-update.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch.1
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-apply.1
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-download.1
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-list.1
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-show.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series.1
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw.1
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:21:01.000000 git-pw-2.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.328403 git-pw-2.4.1/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/add-yaml-format-support-5cd6b9028e6d2d8e.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/api-v1-1-5c804713ef435739.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/bundle-crud-47aadae6eb7a20ad.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/drop-pypy-support-f670deb05ef527fe.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/drop-python-35-36-support-add-python-310-7d364b9ba71bf5ba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/drop-python34-support-5e01360fff605972.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/enforce-filtering-by-project-59ed29c4b7edc0a5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/filter-item-list-by-user-id-4f4e7d6dc402093b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/filter-multiple-matches-197ff839f6b578da.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/handle-error-codes-d72c575fb2d9b452.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/initial-release-0aad09064615d023.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-24-60a9fa796f666f35.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-29-884269fdf35f64b2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-40-add82959d7442cfa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-43-c2c166e1fa23fe76.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-44-66b78577e9534f16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-46-50933643cd5c8db0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-47-a9ac87642050d289.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-48-694495f722119fed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-49-865c4f1657b97fce.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-55-bfcf05e02ad305b1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/passthrough-git-am-arguments-23cd0b292304d648.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/patch-apply-applyPatchDeps-option-9a8fed887af313d5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/patch-states-b88240569f8474f1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/python-2-deprecation-c87e311384eab29b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/python-311-support-de330cb1ff9da396.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/random-fixes-3da473a63c253f2d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/remove-python-3-2-3-3-support-8987031bed2c0333.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/require-server-version-93ac0818c293b85e.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/save-patches-before-applying-c5e786156d47d752.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/update-multiple-patches-ed515cd53964c203.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/use-bundle-names-b1b3ee5c2858c96b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/use-git-pager-settings-ec6555d8311a8bec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/warn-on-multiple-filters-a4e01fdb5cf6e459.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:21:01.000000 git-pw-2.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-08 11:21:01.000000 git-pw-2.4.1/rpm/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-08 11:21:01.000000 git-pw-2.4.1/rpm/git-pw.spec
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-08 11:21:11.332403 git-pw-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 11:21:01.000000 git-pw-2.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 11:21:01.000000 git-pw-2.4.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19499 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 11:21:01.000000 git-pw-2.4.1/tox.ini
```

### Comparing `git-pw-2.4.0/.github/workflows/ci.yaml` & `git-pw-2.4.1/.github/workflows/ci.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -74,34 +74,40 @@
         uses: actions/setup-python@v4
         with:
           python-version: '3.11'
       - name: Install dependencies
         run: python -m pip install build
       - name: Build a binary wheel and a source tarball
         run: python -m build --sdist --wheel --outdir dist/ .
+      - name: Publish distribution to Test PyPI
+        if: ${{ github.ref_type != 'tag' }}
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository-url: https://test.pypi.org/legacy/
       - name: Publish distribution to PyPI
-        if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        if: ${{ github.ref_type == 'tag' }}
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Create release on GitHub
         id: create_release
-        if: startsWith(github.ref, 'refs/tags')
+        if: ${{ github.ref_type == 'tag' }}
         uses: actions/create-release@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
-          tag_name: ${{ github.ref }}
-          release_name: ${{ github.ref }}
+          tag_name: ${{ github.ref_name }}
+          release_name: ${{ github.ref_name }}
           draft: false
           prerelease: false
       - name: Add sdist to release
         id: upload-release-asset
-        if: startsWith(github.ref, 'refs/tags')
+        if: ${{ github.ref_type == 'tag' }}
         uses: actions/upload-release-asset@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           upload_url: ${{ steps.create_release.outputs.upload_url }}
-          asset_path: ./dist/git-pw-${{ github.ref }}.tar.gz
-          asset_name: git-pw-${{ github.ref }}.tar.gz
+          asset_path: ./dist/git-pw-${{ github.ref_name }}.tar.gz
+          asset_name: git-pw-${{ github.ref_name }}.tar.gz
           asset_content_type: application/gzip
```

### Comparing `git-pw-2.4.0/.pre-commit-config.yaml` & `git-pw-2.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/ChangeLog` & `git-pw-2.4.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 CHANGES
 =======
 
+2.4.1
+-----
+
+* Release 2.4.1
+* CI: Address deprecation warning
+* CI: Use modern contexts
+* CI: Reintroduce publishing to Test PyPI
+* utils: Correct type
+* Fix black issues
+* Remove '[testenv] basepython'
+* CI: Switch to pypa/gh-action-pypi-publish@release/v1
+
 2.4.0
 -----
 
 * Release 2.4.0
 * Replace implicit optional typedefs
 * Add Python 3.11 support
 * docs: Actually configure reno to use the main branch
```

### Comparing `git-pw-2.4.0/LICENSE` & `git-pw-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/PKG-INFO` & `git-pw-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-pw
-Version: 2.4.0
+Version: 2.4.1
 Summary: Git-Patchwork integration tool
 Home-page: https://github.com/getpatchwork/git-pw
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/getpatchwork/git-pw/issues
 Project-URL: Source Code, https://github.com/getpatchwork/git-pw
```

### Comparing `git-pw-2.4.0/README.rst` & `git-pw-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/docs/conf.py` & `git-pw-2.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/git_pw/api.py` & `git-pw-2.4.1/git_pw/api.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/git_pw/bundle.py` & `git-pw-2.4.1/git_pw/bundle.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/git_pw/config.py` & `git-pw-2.4.1/git_pw/config.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/git_pw/patch.py` & `git-pw-2.4.1/git_pw/patch.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/git_pw/series.py` & `git-pw-2.4.1/git_pw/series.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/git_pw/shell.py` & `git-pw-2.4.1/git_pw/shell.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/git_pw/utils.py` & `git-pw-2.4.1/git_pw/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     out = _tabulate(output, headers, fmt)
 
     pager = os.environ.get('GIT_PAGER', None)
     if pager:
         _echo_via_pager(pager, out)
         return
 
-    pager = git_config('core.parser')
+    pager = git_config('core.pager')
     if pager:
         _echo_via_pager(pager, out)
         return
 
     pager = os.environ.get('PAGER', None)
     if pager:
         _echo_via_pager(pager, out)
```

### Comparing `git-pw-2.4.0/git_pw.egg-info/PKG-INFO` & `git-pw-2.4.1/git_pw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-pw
-Version: 2.4.0
+Version: 2.4.1
 Summary: Git-Patchwork integration tool
 Home-page: https://github.com/getpatchwork/git-pw
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/getpatchwork/git-pw/issues
 Project-URL: Source Code, https://github.com/getpatchwork/git-pw
```

### Comparing `git-pw-2.4.0/git_pw.egg-info/SOURCES.txt` & `git-pw-2.4.1/git_pw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/man/git-pw-bundle-create.1` & `git-pw-2.4.1/man/git-pw-bundle-create.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE CREATE" "1" "2022-12-06" "2.4.0" "git-pw bundle create Manual"
+.TH "GIT-PW BUNDLE CREATE" "1" "2023-05-08" "2.4.1" "git-pw bundle create Manual"
 .SH NAME
 git-pw\-bundle\-create \- Create a bundle.
 .SH SYNOPSIS
 .B git-pw bundle create
 [OPTIONS] NAME PATCH_IDS...
 .SH DESCRIPTION
 Create a bundle.
```

### Comparing `git-pw-2.4.0/man/git-pw-bundle-list.1` & `git-pw-2.4.1/man/git-pw-bundle-list.1`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE LIST" "1" "2022-12-06" "2.4.0" "git-pw bundle list Manual"
+.TH "GIT-PW BUNDLE LIST" "1" "2023-05-08" "2.4.1" "git-pw bundle list Manual"
 .SH NAME
 git-pw\-bundle\-list \- List bundles.
 .SH SYNOPSIS
 .B git-pw bundle list
 [OPTIONS] [NAME]
 .SH DESCRIPTION
 List bundles.
```

### Comparing `git-pw-2.4.0/man/git-pw-bundle-remove.1` & `git-pw-2.4.1/man/git-pw-bundle-remove.1`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE REMOVE" "1" "2022-12-06" "2.4.0" "git-pw bundle remove Manual"
+.TH "GIT-PW BUNDLE REMOVE" "1" "2023-05-08" "2.4.1" "git-pw bundle remove Manual"
 .SH NAME
 git-pw\-bundle\-remove \- Remove one or more patches from a bundle.
 .SH SYNOPSIS
 .B git-pw bundle remove
 [OPTIONS] BUNDLE_ID PATCH_IDS...
 .SH DESCRIPTION
 Remove one or more patches from a bundle.
```

### Comparing `git-pw-2.4.0/man/git-pw-bundle.1` & `git-pw-2.4.1/man/git-pw-bundle.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE" "1" "2022-12-06" "2.4.0" "git-pw bundle Manual"
+.TH "GIT-PW BUNDLE" "1" "2023-05-08" "2.4.1" "git-pw bundle Manual"
 .SH NAME
 git-pw\-bundle \- Interact with bundles.
 .SH SYNOPSIS
 .B git-pw bundle
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 Interact with bundles.
```

### Comparing `git-pw-2.4.0/man/git-pw-patch-apply.1` & `git-pw-2.4.1/man/git-pw-patch-apply.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH APPLY" "1" "2022-12-06" "2.4.0" "git-pw patch apply Manual"
+.TH "GIT-PW PATCH APPLY" "1" "2023-05-08" "2.4.1" "git-pw patch apply Manual"
 .SH NAME
 git-pw\-patch\-apply \- Apply patch.
 .SH SYNOPSIS
 .B git-pw patch apply
 [OPTIONS] PATCH_ID [ARGS]...
 .SH DESCRIPTION
 Apply patch.
```

### Comparing `git-pw-2.4.0/man/git-pw-patch-download.1` & `git-pw-2.4.1/man/git-pw-patch-download.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH DOWNLOAD" "1" "2022-12-06" "2.4.0" "git-pw patch download Manual"
+.TH "GIT-PW PATCH DOWNLOAD" "1" "2023-05-08" "2.4.1" "git-pw patch download Manual"
 .SH NAME
 git-pw\-patch\-download \- Download patch in diff or mbox format.
 .SH SYNOPSIS
 .B git-pw patch download
 [OPTIONS] PATCH_ID [OUTPUT]
 .SH DESCRIPTION
 Download patch in diff or mbox format.
```

### Comparing `git-pw-2.4.0/man/git-pw-patch-list.1` & `git-pw-2.4.1/man/git-pw-patch-list.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH LIST" "1" "2022-12-06" "2.4.0" "git-pw patch list Manual"
+.TH "GIT-PW PATCH LIST" "1" "2023-05-08" "2.4.1" "git-pw patch list Manual"
 .SH NAME
 git-pw\-patch\-list \- List patches.
 .SH SYNOPSIS
 .B git-pw patch list
 [OPTIONS] [NAME]
 .SH DESCRIPTION
 List patches.
```

### Comparing `git-pw-2.4.0/man/git-pw-patch-update.1` & `git-pw-2.4.1/man/git-pw-patch-update.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH UPDATE" "1" "2022-12-06" "2.4.0" "git-pw patch update Manual"
+.TH "GIT-PW PATCH UPDATE" "1" "2023-05-08" "2.4.1" "git-pw patch update Manual"
 .SH NAME
 git-pw\-patch\-update \- Update one or more patches.
 .SH SYNOPSIS
 .B git-pw patch update
 [OPTIONS] PATCH_IDS...
 .SH DESCRIPTION
 Update one or more patches.
```

### Comparing `git-pw-2.4.0/man/git-pw-patch.1` & `git-pw-2.4.1/man/git-pw-patch.1`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH" "1" "2022-12-06" "2.4.0" "git-pw patch Manual"
+.TH "GIT-PW PATCH" "1" "2023-05-08" "2.4.1" "git-pw patch Manual"
 .SH NAME
 git-pw\-patch \- Interact with patches.
 .SH SYNOPSIS
 .B git-pw patch
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 Interact with patches.
```

### Comparing `git-pw-2.4.0/man/git-pw-series-download.1` & `git-pw-2.4.1/man/git-pw-series-download.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW SERIES DOWNLOAD" "1" "2022-12-06" "2.4.0" "git-pw series download Manual"
+.TH "GIT-PW SERIES DOWNLOAD" "1" "2023-05-08" "2.4.1" "git-pw series download Manual"
 .SH NAME
 git-pw\-series\-download \- Download series in mbox format.
 .SH SYNOPSIS
 .B git-pw series download
 [OPTIONS] SERIES_ID [OUTPUT]
 .SH DESCRIPTION
 Download series in mbox format.
```

### Comparing `git-pw-2.4.0/man/git-pw-series-list.1` & `git-pw-2.4.1/man/git-pw-series-list.1`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW SERIES LIST" "1" "2022-12-06" "2.4.0" "git-pw series list Manual"
+.TH "GIT-PW SERIES LIST" "1" "2023-05-08" "2.4.1" "git-pw series list Manual"
 .SH NAME
 git-pw\-series\-list \- List series.
 .SH SYNOPSIS
 .B git-pw series list
 [OPTIONS] [NAME]
 .SH DESCRIPTION
 List series.
```

### Comparing `git-pw-2.4.0/man/git-pw-series.1` & `git-pw-2.4.1/man/git-pw-series.1`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW SERIES" "1" "2022-12-06" "2.4.0" "git-pw series Manual"
+.TH "GIT-PW SERIES" "1" "2023-05-08" "2.4.1" "git-pw series Manual"
 .SH NAME
 git-pw\-series \- Interact with series.
 .SH SYNOPSIS
 .B git-pw series
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 Interact with series.
```

### Comparing `git-pw-2.4.0/man/git-pw.1` & `git-pw-2.4.1/man/git-pw.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW" "1" "2022-12-06" "2.4.0" "git-pw Manual"
+.TH "GIT-PW" "1" "2023-05-08" "2.4.1" "git-pw Manual"
 .SH NAME
 git-pw \- git-pw is a tool for integrating Git with...
 .SH SYNOPSIS
 .B git-pw
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 git-pw is a tool for integrating Git with Patchwork.
```

### Comparing `git-pw-2.4.0/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml` & `git-pw-2.4.1/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml` & `git-pw-2.4.1/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/rpm/README.rst` & `git-pw-2.4.1/rpm/README.rst`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/rpm/git-pw.spec` & `git-pw-2.4.1/rpm/git-pw.spec`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/setup.cfg` & `git-pw-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/tests/test_api.py` & `git-pw-2.4.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/tests/test_bundle.py` & `git-pw-2.4.1/tests/test_bundle.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,14 @@
             [('name', 'hello'), ('patches', (1, 2)), ('public', True)],
         )
 
     @mock.patch('git_pw.api.LOG')
     def test_create_api_v1_1(
         self, mock_log, mock_echo, mock_create, mock_version
     ):
-
         mock_version.return_value = (1, 1)
 
         runner = CLIRunner()
         result = runner.invoke(bundle.create_cmd, ['hello', '1', '2'])
 
         assert result.exit_code == 1, result
         assert mock_log.error.called
@@ -471,15 +470,14 @@
         self,
         mock_log,
         mock_echo,
         mock_detail,
         mock_update,
         mock_version,
     ):
-
         mock_version.return_value = (1, 1)
 
         runner = CLIRunner()
         result = runner.invoke(bundle.update_cmd, ['1', '--name', 'hello'])
 
         assert result.exit_code == 1, result
         assert mock_log.error.called
```

### Comparing `git-pw-2.4.0/tests/test_patch.py` & `git-pw-2.4.1/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/tests/test_series.py` & `git-pw-2.4.1/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.0/tests/test_utils.py` & `git-pw-2.4.1/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,39 +56,39 @@
 @mock.patch.object(utils, 'git_config', return_value='bar')
 @mock.patch.object(utils, '_tabulate')
 @mock.patch.object(utils, '_echo_via_pager')
 @mock.patch.dict(os.environ, {'PAGER': 'baz'})
 def test_echo_via_pager_config(mock_inner, mock_tabulate, mock_config):
     utils.echo_via_pager('test', ('foo',), None)
 
-    mock_config.assert_called_once_with('core.parser')
+    mock_config.assert_called_once_with('core.pager')
     mock_tabulate.assert_called_once_with('test', ('foo',), None)
     mock_inner.assert_called_once_with('bar', mock_tabulate.return_value)
 
 
 @mock.patch.object(utils, 'git_config', return_value=None)
 @mock.patch.object(utils, '_tabulate')
 @mock.patch.object(utils, '_echo_via_pager')
 @mock.patch.dict(os.environ, {'PAGER': 'baz'})
 def test_echo_via_pager_env_PAGER(mock_inner, mock_tabulate, mock_config):
     utils.echo_via_pager('test', ('foo',), None)
 
-    mock_config.assert_called_once_with('core.parser')
+    mock_config.assert_called_once_with('core.pager')
     mock_tabulate.assert_called_once_with('test', ('foo',), None)
     mock_inner.assert_called_once_with('baz', mock_tabulate.return_value)
 
 
 @mock.patch.object(utils, 'git_config', return_value=None)
 @mock.patch.object(utils, '_tabulate')
 @mock.patch.object(utils, '_echo_via_pager')
 @mock.patch.dict(os.environ, {'PAGER': ''})
 def test_echo_via_pager_env_default(mock_inner, mock_tabulate, mock_config):
     utils.echo_via_pager('test', ('foo',), None)
 
-    mock_config.assert_called_once_with('core.parser')
+    mock_config.assert_called_once_with('core.pager')
     mock_tabulate.assert_called_once_with('test', ('foo',), None)
     mock_inner.assert_called_once_with('less', mock_tabulate.return_value)
 
 
 def _test_tabulate(fmt):
     output = [(b'foo', 'bar', u'baz', '😀', None, 1)]
     headers = ('col1', 'colb', 'colIII', 'colX', 'colY', 'colZ')
```

### Comparing `git-pw-2.4.0/tox.ini` & `git-pw-2.4.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [tox]
 minversion = 3.1
 envlist = pep8,mypy,clean,py{37,38,39,310,311},report
-ignore_basepython_conflict = true
 
 [testenv]
-basepython = python3
 deps =
   -r{toxinidir}/test-requirements.txt
 commands =
   pytest -Wall --cov=git_pw --cov-report term-missing {posargs}
 
 [testenv:pep8]
 skip_install = true
```

