# Comparing `tmp/hikari-yuyo-1.9.0a1.tar.gz` & `tmp/hikari-yuyo-1.9.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-yuyo-1.9.0a1.tar", last modified: Mon Feb 27 17:47:06 2023, max compression
+gzip compressed data, was "hikari-yuyo-1.9.1a1.tar", last modified: Tue Mar  7 15:46:17 2023, max compression
```

## Comparing `hikari-yuyo-1.9.0a1.tar` & `hikari-yuyo-1.9.1a1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0      320 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.codeclimate.yml
--rw-r--r--   0        0        0       19 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.gitattributes
--rw-r--r--   0        0        0       26 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/FUNDING.yml
--rw-r--r--   0        0        0      459 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/dependabot.yml
--rw-r--r--   0        0        0      147 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/docs.in
--rw-r--r--   0        0        0      524 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1144 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0     1034 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1516 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/pr-docs.yml
--rw-r--r--   0        0        0      872 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2335 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/py-test.yml
--rw-r--r--   0        0        0      980 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1265 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/release-docs.yml
--rw-r--r--   0        0        0     1025 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      836 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1110 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1221 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1060 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0      854 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.github/workflows/verify-types.yml
--rw-r--r--   0        0        0     1734 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.gitignore
--rw-r--r--   0        0        0       85 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/.gitmodules
--rw-r--r--   0        0        0    19314 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     6160 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1520 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/LICENSE
--rw-r--r--   0        0        0     1274 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/README.md
--rw-r--r--   0        0        0      145 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/dev-requirements/constraints.in
--rw-r--r--   0        0        0    44557 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/dev-requirements/constraints.txt
--rw-r--r--   0        0        0       56 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/dev-requirements/flake8.txt
--rw-r--r--   0        0        0      125 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/dev-requirements/tests.in
--rw-r--r--   0        0        0    52707 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/dev-requirements/tests.txt
--rw-r--r--   0        0        0      173 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    65198 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0       17 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/changelog.md
--rw-r--r--   0        0        0       14 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/index.md
--rw-r--r--   0        0        0       27 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/asgi.md
--rw-r--r--   0        0        0       33 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/backoff.md
--rw-r--r--   0        0        0       45 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/chunk_tracker.md
--rw-r--r--   0        0        0       39 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/components.md
--rw-r--r--   0        0        0       17 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/index.md
--rw-r--r--   0        0        0       29 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/links.md
--rw-r--r--   0        0        0       41 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/list_status.md
--rw-r--r--   0        0        0       31 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/modals.md
--rw-r--r--   0        0        0       39 2023-02-27 17:46:52.559098 hikari-yuyo-1.9.0a1/docs/reference/pagination.md
--rw-r--r--   0        0        0       37 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/docs/reference/reactions.md
--rw-r--r--   0        0        0       39 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/docs/reference/to_builder.md
--rw-r--r--   0        0        0       22 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/docs/usage.md
--rw-r--r--   0        0        0       64 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/examples/__init__.py
--rw-r--r--   0        0        0     1643 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/examples/components.py
--rw-r--r--   0        0        0     1745 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/mkdocs.yml
--rw-r--r--   0        0        0     1714 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/noxfile.py
--rw-r--r--   0        0        0       14 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.gitattributes
--rw-r--r--   0        0        0      458 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/dependabot.yml
--rw-r--r--   0        0        0     1240 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0      959 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/lint.yml
--rw-r--r--   0        0        0      976 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1032 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      832 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1106 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1217 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1114 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0     1751 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/.gitignore
--rw-r--r--   0        0        0     1520 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/LICENSE
--rw-r--r--   0        0        0      138 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/README.md
--rw-r--r--   0        0        0       50 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/bot/.env.example
--rw-r--r--   0        0        0      612 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/bot/Dockerfile
--rw-r--r--   0        0        0    30730 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/bot/main.py
--rw-r--r--   0        0        0       10 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/bot/other-requirements.txt
--rw-r--r--   0        0        0      193 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/bot/requirements.in
--rw-r--r--   0        0        0    19200 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/bot/requirements.txt
--rw-r--r--   0        0        0      933 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/dev-requirements/flake8.in
--rw-r--r--   0        0        0    20621 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/dev-requirements/flake8.txt
--rw-r--r--   0        0        0       10 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/dev-requirements/other-type-checking.txt
--rw-r--r--   0        0        0      112 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    29031 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0      250 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/docker-compose.yml
--rw-r--r--   0        0        0       26 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/FUNDING.yml
--rw-r--r--   0        0        0      764 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/clippy.yml
--rw-r--r--   0        0        0     1133 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/freeze-for-pr.yml
--rw-r--r--   0        0        0     1271 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/lint.yml
--rw-r--r--   0        0        0     1577 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/pr-docs.yml
--rw-r--r--   0        0        0      964 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/publish.yml
--rw-r--r--   0        0        0     2399 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/py-test.yml
--rw-r--r--   0        0        0     1013 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/reformat.yml
--rw-r--r--   0        0        0     1375 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/release-docs.yml
--rw-r--r--   0        0        0     1075 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/resync-piped.yml
--rw-r--r--   0        0        0     1223 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/rustfmt.yml
--rw-r--r--   0        0        0      869 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/type-check.yml
--rw-r--r--   0        0        0     1115 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/update-licence.yml
--rw-r--r--   0        0        0     1226 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/upgrade-locks.yml
--rw-r--r--   0        0        0     1130 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/verify-locks.yml
--rw-r--r--   0        0        0      887 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/actions/verify-types.yml
--rw-r--r--   0        0        0      550 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/dependabot.yml
--rw-r--r--   0        0        0      524 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/github/pull_request_template.md
--rw-r--r--   0        0        0     1713 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/noxfile.py
--rw-r--r--   0        0        0     4230 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/pyproject.toml
--rw-r--r--   0        0        0      141 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/docs.in
--rw-r--r--   0        0        0    32100 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/docs.txt
--rw-r--r--   0        0        0       90 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/flake8.in
--rw-r--r--   0        0        0     1671 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/flake8.txt
--rw-r--r--   0        0        0       32 2023-02-27 17:46:53.163105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/freeze-locks.in
--rw-r--r--   0        0        0    52180 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/freeze-locks.txt
--rw-r--r--   0        0        0     1072 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/library-flake8.in
--rw-r--r--   0        0        0    27936 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/library-flake8.txt
--rw-r--r--   0        0        0       58 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/lint.in
--rw-r--r--   0        0        0     5198 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/lint.txt
--rw-r--r--   0        0        0       60 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/nox.in
--rw-r--r--   0        0        0    10580 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/nox.txt
--rw-r--r--   0        0        0       12 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/publish.in
--rw-r--r--   0        0        0     9682 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/publish.txt
--rw-r--r--   0        0        0       78 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/reformat.in
--rw-r--r--   0        0        0    15631 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/reformat.txt
--rw-r--r--   0        0        0       44 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/tests.in
--rw-r--r--   0        0        0     7307 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/tests.txt
--rw-r--r--   0        0        0       29 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/type-checking.in
--rw-r--r--   0        0        0     3965 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/base-requirements/type-checking.txt
--rw-r--r--   0        0        0    24254 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/noxfile.py
--rw-r--r--   0        0        0     1714 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/noxfile.template.py
--rw-r--r--   0        0        0     4737 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/piped_shared/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/piped_shared/py.typed
--rw-r--r--   0        0        0      334 2023-02-27 17:46:53.167105 hikari-yuyo-1.9.0a1/piped/python/pyproject.toml
--rw-r--r--   0        0        0     6287 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/pyproject.toml
--rw-r--r--   0        0        0     1596 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/__init__.py
--rw-r--r--   0        0        0     5036 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test__internal.py
--rw-r--r--   0        0        0    62452 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_asgi.py
--rw-r--r--   0        0        0     5523 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_chunk_tracker.py
--rw-r--r--   0        0        0    13464 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_components.py
--rw-r--r--   0        0        0    25280 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_links.py
--rw-r--r--   0        0        0    40207 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_list_status.py
--rw-r--r--   0        0        0    18338 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_modals.py
--rw-r--r--   0        0        0     5981 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_pagination.py
--rw-r--r--   0        0        0     2556 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_reactions.py
--rw-r--r--   0        0        0    37058 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/tests/test_to_builder.py
--rw-r--r--   0        0        0     3752 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/__init__.py
--rw-r--r--   0        0        0     4328 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/_internal.py
--rw-r--r--   0        0        0    32386 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/asgi.py
--rw-r--r--   0        0        0    14071 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/backoff.py
--rw-r--r--   0        0        0    24090 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/chunk_tracker.py
--rw-r--r--   0        0        0   162526 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/components.py
--rw-r--r--   0        0        0    16862 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/links.py
--rw-r--r--   0        0        0    35386 2023-02-27 17:46:52.563098 hikari-yuyo-1.9.0a1/yuyo/list_status.py
--rw-r--r--   0        0        0    52519 2023-02-27 17:46:52.567098 hikari-yuyo-1.9.0a1/yuyo/modals.py
--rw-r--r--   0        0        0    12991 2023-02-27 17:46:52.567098 hikari-yuyo-1.9.0a1/yuyo/pagination.py
--rw-r--r--   0        0        0        0 2023-02-27 17:46:52.567098 hikari-yuyo-1.9.0a1/yuyo/py.typed
--rw-r--r--   0        0        0    33047 2023-02-27 17:46:52.567098 hikari-yuyo-1.9.0a1/yuyo/reactions.py
--rw-r--r--   0        0        0    15230 2023-02-27 17:46:52.567098 hikari-yuyo-1.9.0a1/yuyo/to_builder.py
--rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 hikari-yuyo-1.9.0a1/PKG-INFO
+-rw-r--r--   0        0        0      320 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.codeclimate.yml
+-rw-r--r--   0        0        0       19 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.gitattributes
+-rw-r--r--   0        0        0       26 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      459 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.github/dependabot.yml
+-rw-r--r--   0        0        0      147 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.github/docs.in
+-rw-r--r--   0        0        0      524 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1144 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1034 2023-03-07 15:46:02.235737 hikari-yuyo-1.9.1a1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1516 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/pr-docs.yml
+-rw-r--r--   0        0        0      872 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2335 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/py-test.yml
+-rw-r--r--   0        0        0      980 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1265 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/release-docs.yml
+-rw-r--r--   0        0        0     1025 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      836 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1110 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1221 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1060 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0      854 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.github/workflows/verify-types.yml
+-rw-r--r--   0        0        0     1734 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.gitignore
+-rw-r--r--   0        0        0       85 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/.gitmodules
+-rw-r--r--   0        0        0    19994 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     6160 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1520 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/LICENSE
+-rw-r--r--   0        0        0     1274 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/README.md
+-rw-r--r--   0        0        0      145 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/dev-requirements/constraints.in
+-rw-r--r--   0        0        0    43452 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/dev-requirements/constraints.txt
+-rw-r--r--   0        0        0       56 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0      125 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/dev-requirements/tests.in
+-rw-r--r--   0        0        0    51602 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/dev-requirements/tests.txt
+-rw-r--r--   0        0        0      173 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    64093 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0       17 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/changelog.md
+-rw-r--r--   0        0        0       14 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/index.md
+-rw-r--r--   0        0        0       27 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/asgi.md
+-rw-r--r--   0        0        0       33 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/backoff.md
+-rw-r--r--   0        0        0       45 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/chunk_tracker.md
+-rw-r--r--   0        0        0       39 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/components.md
+-rw-r--r--   0        0        0       17 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/index.md
+-rw-r--r--   0        0        0       29 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/links.md
+-rw-r--r--   0        0        0       41 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/list_status.md
+-rw-r--r--   0        0        0       31 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/modals.md
+-rw-r--r--   0        0        0       39 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/pagination.md
+-rw-r--r--   0        0        0       37 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/reactions.md
+-rw-r--r--   0        0        0       39 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/reference/to_builder.md
+-rw-r--r--   0        0        0       22 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/docs/usage.md
+-rw-r--r--   0        0        0       64 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/examples/__init__.py
+-rw-r--r--   0        0        0     1643 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/examples/components.py
+-rw-r--r--   0        0        0     1745 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/mkdocs.yml
+-rw-r--r--   0        0        0     1714 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/noxfile.py
+-rw-r--r--   0        0        0       14 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.gitattributes
+-rw-r--r--   0        0        0      458 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/dependabot.yml
+-rw-r--r--   0        0        0     1240 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0      959 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      976 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1032 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      832 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1106 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1217 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1114 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0     1751 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/.gitignore
+-rw-r--r--   0        0        0     1520 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/LICENSE
+-rw-r--r--   0        0        0      138 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/README.md
+-rw-r--r--   0        0        0       50 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/bot/.env.example
+-rw-r--r--   0        0        0      612 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/bot/Dockerfile
+-rw-r--r--   0        0        0    30730 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/bot/main.py
+-rw-r--r--   0        0        0       10 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/bot/other-requirements.txt
+-rw-r--r--   0        0        0      192 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/bot/requirements.in
+-rw-r--r--   0        0        0    19199 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/bot/requirements.txt
+-rw-r--r--   0        0        0      933 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/dev-requirements/flake8.in
+-rw-r--r--   0        0        0    20621 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0       10 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/dev-requirements/other-type-checking.txt
+-rw-r--r--   0        0        0      112 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    29030 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0      250 2023-03-07 15:46:02.743744 hikari-yuyo-1.9.1a1/piped/docker-compose.yml
+-rw-r--r--   0        0        0       26 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/FUNDING.yml
+-rw-r--r--   0        0        0      764 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/clippy.yml
+-rw-r--r--   0        0        0     1133 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1271 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/lint.yml
+-rw-r--r--   0        0        0     1577 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/pr-docs.yml
+-rw-r--r--   0        0        0      964 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/publish.yml
+-rw-r--r--   0        0        0     2399 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/py-test.yml
+-rw-r--r--   0        0        0     1013 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/reformat.yml
+-rw-r--r--   0        0        0     1375 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/release-docs.yml
+-rw-r--r--   0        0        0     1075 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/resync-piped.yml
+-rw-r--r--   0        0        0     1223 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/rustfmt.yml
+-rw-r--r--   0        0        0      869 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/type-check.yml
+-rw-r--r--   0        0        0     1115 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/update-licence.yml
+-rw-r--r--   0        0        0     1226 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/upgrade-locks.yml
+-rw-r--r--   0        0        0     1130 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/verify-locks.yml
+-rw-r--r--   0        0        0      887 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/actions/verify-types.yml
+-rw-r--r--   0        0        0      550 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/dependabot.yml
+-rw-r--r--   0        0        0      524 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/github/pull_request_template.md
+-rw-r--r--   0        0        0     1713 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/noxfile.py
+-rw-r--r--   0        0        0     4853 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/docs.in
+-rw-r--r--   0        0        0    32100 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/docs.txt
+-rw-r--r--   0        0        0       90 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/flake8.in
+-rw-r--r--   0        0        0     1671 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/flake8.txt
+-rw-r--r--   0        0        0       32 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/freeze-locks.in
+-rw-r--r--   0        0        0    52429 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/freeze-locks.txt
+-rw-r--r--   0        0        0     1072 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/library-flake8.in
+-rw-r--r--   0        0        0    27936 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/library-flake8.txt
+-rw-r--r--   0        0        0       58 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/lint.in
+-rw-r--r--   0        0        0     5368 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/lint.txt
+-rw-r--r--   0        0        0       60 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/nox.in
+-rw-r--r--   0        0        0    10580 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/nox.txt
+-rw-r--r--   0        0        0       12 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/publish.in
+-rw-r--r--   0        0        0     9682 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/publish.txt
+-rw-r--r--   0        0        0       78 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/reformat.in
+-rw-r--r--   0        0        0    15801 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/reformat.txt
+-rw-r--r--   0        0        0       44 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/tests.in
+-rw-r--r--   0        0        0     7307 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/tests.txt
+-rw-r--r--   0        0        0       29 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/type-checking.in
+-rw-r--r--   0        0        0     3965 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/base-requirements/type-checking.txt
+-rw-r--r--   0        0        0    24254 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/noxfile.py
+-rw-r--r--   0        0        0     1714 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/noxfile.template.py
+-rw-r--r--   0        0        0     4737 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/piped_shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/piped_shared/py.typed
+-rw-r--r--   0        0        0      334 2023-03-07 15:46:02.747743 hikari-yuyo-1.9.1a1/piped/python/pyproject.toml
+-rw-r--r--   0        0        0     6910 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1596 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/tests/__init__.py
+-rw-r--r--   0        0        0     5036 2023-03-07 15:46:02.239737 hikari-yuyo-1.9.1a1/tests/test__internal.py
+-rw-r--r--   0        0        0    62445 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_asgi.py
+-rw-r--r--   0        0        0     5523 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_chunk_tracker.py
+-rw-r--r--   0        0        0    13464 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_components.py
+-rw-r--r--   0        0        0    25280 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_links.py
+-rw-r--r--   0        0        0    40207 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_list_status.py
+-rw-r--r--   0        0        0    18338 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_modals.py
+-rw-r--r--   0        0        0     5981 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_pagination.py
+-rw-r--r--   0        0        0     2556 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_reactions.py
+-rw-r--r--   0        0        0    37058 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/tests/test_to_builder.py
+-rw-r--r--   0        0        0     3752 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/__init__.py
+-rw-r--r--   0        0        0     4328 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/_internal.py
+-rw-r--r--   0        0        0    32562 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/asgi.py
+-rw-r--r--   0        0        0    14071 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/backoff.py
+-rw-r--r--   0        0        0    24090 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/chunk_tracker.py
+-rw-r--r--   0        0        0   163774 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/components.py
+-rw-r--r--   0        0        0    16862 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/links.py
+-rw-r--r--   0        0        0    35386 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/list_status.py
+-rw-r--r--   0        0        0    52778 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/modals.py
+-rw-r--r--   0        0        0    12991 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/pagination.py
+-rw-r--r--   0        0        0        0 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/py.typed
+-rw-r--r--   0        0        0    33120 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/reactions.py
+-rw-r--r--   0        0        0    15230 2023-03-07 15:46:02.243737 hikari-yuyo-1.9.1a1/yuyo/to_builder.py
+-rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 hikari-yuyo-1.9.1a1/PKG-INFO
```

### Comparing `hikari-yuyo-1.9.0a1/.github/pull_request_template.md` & `hikari-yuyo-1.9.1a1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/freeze-for-pr.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/lint.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/pr-docs.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/pr-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/publish.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/py-test.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/py-test.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/reformat.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/release-docs.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/release-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/resync-piped.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/type-check.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/update-licence.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/upgrade-locks.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/verify-locks.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.github/workflows/verify-types.yml` & `hikari-yuyo-1.9.1a1/.github/workflows/verify-types.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/.gitignore` & `hikari-yuyo-1.9.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/CHANGELOG.md` & `hikari-yuyo-1.9.1a1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [1.9.1a1] - 2023-03-07
+### Added
+- Re-exposed `yuyo.reactions.EventT` as [yuyo.reactions.ReactionEventT][].
+
+### Changed
+- `token_type` now defaults to `"Bot"` when a string token is passed for
+  [AsgiBot.\_\_init\_\_][yuyo.asgi.AsgiBot.__init__].
+
+### Fixed
+- [yuyo.modals.modal][] and [yuyo.modals.as_modal][] no-longer lead to Alluka's type-hint introspection
+  raising an exception.
+- Handling of defaulting empty modal text inputs.
+- Add `type` property to [yuyo.components.ActionRowExecutor][] and
+  [yuyo.components.ChildActionRowExecutor][] to fix compatibility with `Hikari>=2.0.0.dev117`.
+
 ## [1.9.0a1] - 2023-02-27
 ### Added
 - `from_tanjun` convenience classmethods for initialising from a Tanjun client to
   [ComponentClient][yuyo.modals.ModalClient], [ModalClient][yuyo.modals.ModalClient],
   [ReactionClient][yuyo.reactions.ReactionClient], and [ServiceManager][yuyo.list_status.ServiceManager].
 - `alluka` keyword-argument to to `from_gateway_bot` and `from_rest_bot` methods on
   [ComponentClient][yuyo.modals.ModalClient], [ModalClient][yuyo.modals.ModalClient], and
@@ -357,15 +372,16 @@
 - Renamed module pagnation to pagination.
 - Move the reaction handling logic over to "reactions.py"
 - Renamed string_patinator functions to paginate_string
 
 ### Fixed
 - Iffy behaviour around "locking" the reaction executor which lead to some requests just being ignored.
 
-[Unreleased]: https://github.com/FasterSpeeding/Yuyo/compare/v1.9.0a1...HEAD
+[Unreleased]: https://github.com/FasterSpeeding/Yuyo/compare/v1.9.1a1...HEAD
+[1.9.1a1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.9.0a1...v1.9.1a1
 [1.9.0a1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.8.0a1.post1...v1.9.0a1
 [1.8.0a1.post1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.8.0a1...v1.8.0a1.post1
 [1.8.0a1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.7.0a1...v1.8.0a1
 [1.7.0a1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.6.1a1...v1.7.0a1
 [1.6.1a1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.6.0a1...v1.6.1a1
 [1.6.0a1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.5.0a1...v1.6.0a1
 [1.5.0a1]:https://github.com/FasterSpeeding/Yuyo/compare/v1.4.0a1.post1...v1.5.0a1
```

### Comparing `hikari-yuyo-1.9.0a1/CODE_OF_CONDUCT.md` & `hikari-yuyo-1.9.1a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/CONTRIBUTING.md` & `hikari-yuyo-1.9.1a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/LICENSE` & `hikari-yuyo-1.9.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/README.md` & `hikari-yuyo-1.9.1a1/README.md`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/dev-requirements/constraints.txt` & `hikari-yuyo-1.9.1a1/dev-requirements/constraints.txt`

 * *Files 3% similar despite different names*

```diff
@@ -168,103 +168,90 @@
     --hash=sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4 \
     --hash=sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e \
     --hash=sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9 \
     --hash=sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6 \
     --hash=sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b \
     --hash=sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01 \
     --hash=sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0
-charset-normalizer==3.0.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b \
-    --hash=sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42 \
-    --hash=sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d \
-    --hash=sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b \
-    --hash=sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a \
-    --hash=sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59 \
-    --hash=sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154 \
-    --hash=sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1 \
-    --hash=sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c \
-    --hash=sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a \
-    --hash=sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d \
-    --hash=sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6 \
-    --hash=sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b \
-    --hash=sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b \
-    --hash=sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783 \
-    --hash=sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5 \
-    --hash=sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918 \
-    --hash=sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555 \
-    --hash=sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639 \
-    --hash=sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786 \
-    --hash=sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e \
-    --hash=sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed \
-    --hash=sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820 \
-    --hash=sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8 \
-    --hash=sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3 \
-    --hash=sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541 \
-    --hash=sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14 \
-    --hash=sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be \
-    --hash=sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e \
-    --hash=sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76 \
-    --hash=sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b \
-    --hash=sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c \
-    --hash=sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b \
-    --hash=sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3 \
-    --hash=sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc \
-    --hash=sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6 \
-    --hash=sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59 \
-    --hash=sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4 \
-    --hash=sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d \
-    --hash=sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d \
-    --hash=sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3 \
-    --hash=sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a \
-    --hash=sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea \
-    --hash=sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6 \
-    --hash=sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e \
-    --hash=sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603 \
-    --hash=sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24 \
-    --hash=sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a \
-    --hash=sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58 \
-    --hash=sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678 \
-    --hash=sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a \
-    --hash=sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c \
-    --hash=sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6 \
-    --hash=sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18 \
-    --hash=sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174 \
-    --hash=sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317 \
-    --hash=sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f \
-    --hash=sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc \
-    --hash=sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837 \
-    --hash=sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41 \
-    --hash=sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c \
-    --hash=sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579 \
-    --hash=sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753 \
-    --hash=sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8 \
-    --hash=sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291 \
-    --hash=sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087 \
-    --hash=sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866 \
-    --hash=sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3 \
-    --hash=sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d \
-    --hash=sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1 \
-    --hash=sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca \
-    --hash=sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e \
-    --hash=sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db \
-    --hash=sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72 \
-    --hash=sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d \
-    --hash=sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc \
-    --hash=sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539 \
-    --hash=sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d \
-    --hash=sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af \
-    --hash=sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b \
-    --hash=sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602 \
-    --hash=sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f \
-    --hash=sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478 \
-    --hash=sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c \
-    --hash=sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e \
-    --hash=sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479 \
-    --hash=sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7 \
-    --hash=sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8
+charset-normalizer==3.1.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
+    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
+    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
+    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
+    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
+    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
+    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
+    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
+    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
+    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
+    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
+    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
+    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
+    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
+    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
+    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
+    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
+    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
+    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
+    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
+    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
+    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
+    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
+    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
+    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
+    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
+    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
+    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
+    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
+    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
+    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
+    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
+    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
+    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
+    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
+    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
+    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
+    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
+    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
+    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
+    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
+    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
+    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
+    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
+    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
+    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
+    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
+    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
+    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
+    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
+    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
+    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
+    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
+    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
+    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
+    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
+    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
+    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
+    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
+    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
+    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
+    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
+    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
+    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
+    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
+    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
+    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
+    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
+    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
+    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
+    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
+    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
+    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
+    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
+    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
 colorama==0.4.6 ; python_full_version >= "3.9.0" and python_version < "3.12" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 colorlog==6.7.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:0d33ca236784a1ba3ff9c532d4964126d8a2c44f1f0cb1d2b0728196f512f662 \
     --hash=sha256:bd94bd21c1e13fac7bd3153f4bc3a7dc0eb0974b8bc2fdf1a989e474f6e582e5
 frozenlist==1.3.3 ; python_full_version >= "3.9.0" and python_version < "3.12" \
@@ -344,20 +331,20 @@
     --hash=sha256:ff8bf625fe85e119553b5383ba0fb6aa3d0ec2ae980295aaefa552374926b3f4
 hikari-sake==1.0.7 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:7f163acc889869df0a423e7804a7a5686ccc028ec33afdee4b8fdaf305a1c286 \
     --hash=sha256:9a941706192c2d769601c5f2665c26233960c552807e8f12411640f0b0a61316
 hikari-tanjun==2.11.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:3616cbf238b006b88daa3916932947993124344ae013fb523785673d4542c267 \
     --hash=sha256:8ff718f11c4e5ae5958e1a719fa84773db7e4c88e09a8e2faf84d920b70c44af
-hikari==2.0.0.dev116 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:0e1d0bdfe777a6c16cdda7807b49d93c0a0da39ab369683955491d3d10963c90 \
-    --hash=sha256:f78f5f828eff4c44484ca251555a19f0424366aa87a0092dbaceae9b039e0ab4
-hikari==2.0.0.dev116 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:0e1d0bdfe777a6c16cdda7807b49d93c0a0da39ab369683955491d3d10963c90 \
-    --hash=sha256:f78f5f828eff4c44484ca251555a19f0424366aa87a0092dbaceae9b039e0ab4
+hikari==2.0.0.dev117 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:1d1828d1b16687badac1c882ac40d6ead2299c16ca7937065b8fced0fd4ef028 \
+    --hash=sha256:4f2c30d60ebbff37635a80ac788a2c9715ee6f2df626239180e96e65815d9958
+hikari==2.0.0.dev117 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:1d1828d1b16687badac1c882ac40d6ead2299c16ca7937065b8fced0fd4ef028 \
+    --hash=sha256:4f2c30d60ebbff37635a80ac788a2c9715ee6f2df626239180e96e65815d9958
 idna==3.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
 multidict==6.0.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9 \
     --hash=sha256:0b1a97283e0c85772d613878028fec909f003993e1007eafa715b24b377cb9b8 \
     --hash=sha256:0dfad7a5a1e39c53ed00d2dd0c2e36aed4650936dc18fd9a1826a5ae1cad6f03 \
```

### Comparing `hikari-yuyo-1.9.0a1/dev-requirements/tests.txt` & `hikari-yuyo-1.9.1a1/dev-requirements/tests.txt`

 * *Files 3% similar despite different names*

```diff
@@ -168,103 +168,90 @@
     --hash=sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4 \
     --hash=sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e \
     --hash=sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9 \
     --hash=sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6 \
     --hash=sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b \
     --hash=sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01 \
     --hash=sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0
-charset-normalizer==3.0.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b \
-    --hash=sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42 \
-    --hash=sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d \
-    --hash=sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b \
-    --hash=sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a \
-    --hash=sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59 \
-    --hash=sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154 \
-    --hash=sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1 \
-    --hash=sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c \
-    --hash=sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a \
-    --hash=sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d \
-    --hash=sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6 \
-    --hash=sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b \
-    --hash=sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b \
-    --hash=sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783 \
-    --hash=sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5 \
-    --hash=sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918 \
-    --hash=sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555 \
-    --hash=sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639 \
-    --hash=sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786 \
-    --hash=sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e \
-    --hash=sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed \
-    --hash=sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820 \
-    --hash=sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8 \
-    --hash=sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3 \
-    --hash=sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541 \
-    --hash=sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14 \
-    --hash=sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be \
-    --hash=sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e \
-    --hash=sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76 \
-    --hash=sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b \
-    --hash=sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c \
-    --hash=sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b \
-    --hash=sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3 \
-    --hash=sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc \
-    --hash=sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6 \
-    --hash=sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59 \
-    --hash=sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4 \
-    --hash=sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d \
-    --hash=sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d \
-    --hash=sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3 \
-    --hash=sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a \
-    --hash=sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea \
-    --hash=sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6 \
-    --hash=sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e \
-    --hash=sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603 \
-    --hash=sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24 \
-    --hash=sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a \
-    --hash=sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58 \
-    --hash=sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678 \
-    --hash=sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a \
-    --hash=sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c \
-    --hash=sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6 \
-    --hash=sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18 \
-    --hash=sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174 \
-    --hash=sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317 \
-    --hash=sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f \
-    --hash=sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc \
-    --hash=sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837 \
-    --hash=sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41 \
-    --hash=sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c \
-    --hash=sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579 \
-    --hash=sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753 \
-    --hash=sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8 \
-    --hash=sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291 \
-    --hash=sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087 \
-    --hash=sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866 \
-    --hash=sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3 \
-    --hash=sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d \
-    --hash=sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1 \
-    --hash=sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca \
-    --hash=sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e \
-    --hash=sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db \
-    --hash=sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72 \
-    --hash=sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d \
-    --hash=sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc \
-    --hash=sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539 \
-    --hash=sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d \
-    --hash=sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af \
-    --hash=sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b \
-    --hash=sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602 \
-    --hash=sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f \
-    --hash=sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478 \
-    --hash=sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c \
-    --hash=sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e \
-    --hash=sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479 \
-    --hash=sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7 \
-    --hash=sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8
+charset-normalizer==3.1.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
+    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
+    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
+    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
+    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
+    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
+    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
+    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
+    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
+    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
+    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
+    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
+    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
+    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
+    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
+    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
+    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
+    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
+    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
+    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
+    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
+    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
+    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
+    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
+    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
+    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
+    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
+    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
+    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
+    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
+    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
+    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
+    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
+    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
+    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
+    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
+    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
+    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
+    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
+    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
+    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
+    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
+    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
+    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
+    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
+    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
+    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
+    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
+    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
+    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
+    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
+    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
+    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
+    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
+    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
+    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
+    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
+    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
+    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
+    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
+    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
+    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
+    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
+    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
+    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
+    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
+    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
+    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
+    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
+    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
+    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
+    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
+    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
+    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
+    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
 colorama==0.4.6 ; python_full_version >= "3.9.0" and python_version < "3.12" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 colorlog==6.7.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:0d33ca236784a1ba3ff9c532d4964126d8a2c44f1f0cb1d2b0728196f512f662 \
     --hash=sha256:bd94bd21c1e13fac7bd3153f4bc3a7dc0eb0974b8bc2fdf1a989e474f6e582e5
 coverage[toml]==7.2.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
@@ -405,20 +392,20 @@
     --hash=sha256:ff8bf625fe85e119553b5383ba0fb6aa3d0ec2ae980295aaefa552374926b3f4
 hikari-sake==1.0.7 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:7f163acc889869df0a423e7804a7a5686ccc028ec33afdee4b8fdaf305a1c286 \
     --hash=sha256:9a941706192c2d769601c5f2665c26233960c552807e8f12411640f0b0a61316
 hikari-tanjun==2.11.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:3616cbf238b006b88daa3916932947993124344ae013fb523785673d4542c267 \
     --hash=sha256:8ff718f11c4e5ae5958e1a719fa84773db7e4c88e09a8e2faf84d920b70c44af
-hikari==2.0.0.dev116 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:0e1d0bdfe777a6c16cdda7807b49d93c0a0da39ab369683955491d3d10963c90 \
-    --hash=sha256:f78f5f828eff4c44484ca251555a19f0424366aa87a0092dbaceae9b039e0ab4
-hikari[server]==2.0.0.dev116 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:0e1d0bdfe777a6c16cdda7807b49d93c0a0da39ab369683955491d3d10963c90 \
-    --hash=sha256:f78f5f828eff4c44484ca251555a19f0424366aa87a0092dbaceae9b039e0ab4
+hikari==2.0.0.dev117 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:1d1828d1b16687badac1c882ac40d6ead2299c16ca7937065b8fced0fd4ef028 \
+    --hash=sha256:4f2c30d60ebbff37635a80ac788a2c9715ee6f2df626239180e96e65815d9958
+hikari[server]==2.0.0.dev117 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:1d1828d1b16687badac1c882ac40d6ead2299c16ca7937065b8fced0fd4ef028 \
+    --hash=sha256:4f2c30d60ebbff37635a80ac788a2c9715ee6f2df626239180e96e65815d9958
 idna==3.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
 iniconfig==2.0.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
 multidict==6.0.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
@@ -524,17 +511,17 @@
     --hash=sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470
 pytest-sugar==0.9.6 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:30e5225ed2b3cc988a8a672f8bda0fc37bcd92d62e9273937f061112b3f2186d \
     --hash=sha256:c4793495f3c32e114f0f5416290946c316eb96ad5a3684dcdadda9267e59b2b8
 pytest-xdist==3.2.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:336098e3bbd8193276867cc87db8b22903c3927665dff9d1ac8684c02f597b68 \
     --hash=sha256:fa10f95a2564cd91652f2d132725183c3b590d9fdcdec09d3677386ecf4c1ce9
-pytest==7.2.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5 \
-    --hash=sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42
+pytest==7.2.2 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e \
+    --hash=sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4
 python-dateutil==2.8.2 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
 redis==4.5.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:1eec3741cda408d3a5f84b78d089c8b8d895f21b3b050988351e925faf202864 \
     --hash=sha256:5deb072d26e67d2be1712603bfb7947ec3431fb0eec9c578994052e33035af6d
 six==1.16.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
```

### Comparing `hikari-yuyo-1.9.0a1/dev-requirements/type-checking.txt` & `hikari-yuyo-1.9.1a1/dev-requirements/type-checking.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,17 @@
     --hash=sha256:fe7ba4a51f33ab275515f66b0a236bcde4fb5561498fe8f898d4e549b2e4509f
 aiosignal==1.3.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:54cd96e15e1649b75d6c87526a6ff0b6c1b0dd3459f43d9ca11d48c339b68cfc \
     --hash=sha256:f8376fb07dd1e86a584e4fcdec80b36b7f81aac666ebc724e2c090300dd83b17
 alluka==0.1.3 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:5bc3f13b74b4706a99f1eaee0dd64f709aac1a67a88999b86f2eca6a2adf1c8a \
     --hash=sha256:c2d67315764f72d7789256676fa81fda093c10fbe4137e66ff4f9dab631f408e
-argcomplete==2.0.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:6372ad78c89d662035101418ae253668445b391755cfe94ea52f1b9d22425b20 \
-    --hash=sha256:cffa11ea77999bb0dd27bb25ff6dc142a6796142f68d45b1a26b11f58724561e
+argcomplete==2.0.6 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:6c2170b3e0ab54683cb28d319b65261bde1f11388be688b68118b7d281e34c94 \
+    --hash=sha256:dc33528d96727882b576b24bc89ed038f3c6abbb6855ff9bb6be23384afff9d6
 asgiref==3.6.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:71e68008da809b957b7ee4b43dbccff33d1b23519fb8344e33f049897077afac \
     --hash=sha256:9567dfe7bd8d3c8c892227827c41cce860b368104c3431da67a0c5a65a949506
 async-timeout==4.0.2 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15 \
     --hash=sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c
 attrs==22.2.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
@@ -171,103 +171,90 @@
     --hash=sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4 \
     --hash=sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e \
     --hash=sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9 \
     --hash=sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6 \
     --hash=sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b \
     --hash=sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01 \
     --hash=sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0
-charset-normalizer==3.0.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b \
-    --hash=sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42 \
-    --hash=sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d \
-    --hash=sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b \
-    --hash=sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a \
-    --hash=sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59 \
-    --hash=sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154 \
-    --hash=sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1 \
-    --hash=sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c \
-    --hash=sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a \
-    --hash=sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d \
-    --hash=sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6 \
-    --hash=sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b \
-    --hash=sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b \
-    --hash=sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783 \
-    --hash=sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5 \
-    --hash=sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918 \
-    --hash=sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555 \
-    --hash=sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639 \
-    --hash=sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786 \
-    --hash=sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e \
-    --hash=sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed \
-    --hash=sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820 \
-    --hash=sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8 \
-    --hash=sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3 \
-    --hash=sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541 \
-    --hash=sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14 \
-    --hash=sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be \
-    --hash=sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e \
-    --hash=sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76 \
-    --hash=sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b \
-    --hash=sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c \
-    --hash=sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b \
-    --hash=sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3 \
-    --hash=sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc \
-    --hash=sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6 \
-    --hash=sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59 \
-    --hash=sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4 \
-    --hash=sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d \
-    --hash=sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d \
-    --hash=sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3 \
-    --hash=sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a \
-    --hash=sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea \
-    --hash=sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6 \
-    --hash=sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e \
-    --hash=sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603 \
-    --hash=sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24 \
-    --hash=sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a \
-    --hash=sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58 \
-    --hash=sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678 \
-    --hash=sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a \
-    --hash=sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c \
-    --hash=sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6 \
-    --hash=sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18 \
-    --hash=sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174 \
-    --hash=sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317 \
-    --hash=sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f \
-    --hash=sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc \
-    --hash=sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837 \
-    --hash=sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41 \
-    --hash=sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c \
-    --hash=sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579 \
-    --hash=sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753 \
-    --hash=sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8 \
-    --hash=sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291 \
-    --hash=sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087 \
-    --hash=sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866 \
-    --hash=sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3 \
-    --hash=sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d \
-    --hash=sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1 \
-    --hash=sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca \
-    --hash=sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e \
-    --hash=sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db \
-    --hash=sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72 \
-    --hash=sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d \
-    --hash=sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc \
-    --hash=sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539 \
-    --hash=sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d \
-    --hash=sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af \
-    --hash=sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b \
-    --hash=sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602 \
-    --hash=sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f \
-    --hash=sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478 \
-    --hash=sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c \
-    --hash=sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e \
-    --hash=sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479 \
-    --hash=sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7 \
-    --hash=sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8
+charset-normalizer==3.1.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
+    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
+    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
+    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
+    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
+    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
+    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
+    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
+    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
+    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
+    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
+    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
+    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
+    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
+    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
+    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
+    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
+    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
+    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
+    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
+    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
+    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
+    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
+    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
+    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
+    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
+    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
+    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
+    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
+    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
+    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
+    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
+    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
+    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
+    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
+    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
+    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
+    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
+    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
+    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
+    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
+    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
+    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
+    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
+    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
+    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
+    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
+    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
+    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
+    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
+    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
+    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
+    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
+    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
+    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
+    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
+    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
+    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
+    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
+    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
+    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
+    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
+    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
+    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
+    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
+    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
+    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
+    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
+    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
+    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
+    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
+    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
+    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
+    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
+    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
 colorama==0.4.6 ; python_full_version >= "3.9.0" and python_version < "3.12" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 colorlog==6.7.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:0d33ca236784a1ba3ff9c532d4964126d8a2c44f1f0cb1d2b0728196f512f662 \
     --hash=sha256:bd94bd21c1e13fac7bd3153f4bc3a7dc0eb0974b8bc2fdf1a989e474f6e582e5
 coverage[toml]==7.2.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
@@ -414,20 +401,20 @@
     --hash=sha256:ff8bf625fe85e119553b5383ba0fb6aa3d0ec2ae980295aaefa552374926b3f4
 hikari-sake==1.0.7 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:7f163acc889869df0a423e7804a7a5686ccc028ec33afdee4b8fdaf305a1c286 \
     --hash=sha256:9a941706192c2d769601c5f2665c26233960c552807e8f12411640f0b0a61316
 hikari-tanjun==2.11.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:3616cbf238b006b88daa3916932947993124344ae013fb523785673d4542c267 \
     --hash=sha256:8ff718f11c4e5ae5958e1a719fa84773db7e4c88e09a8e2faf84d920b70c44af
-hikari==2.0.0.dev116 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:0e1d0bdfe777a6c16cdda7807b49d93c0a0da39ab369683955491d3d10963c90 \
-    --hash=sha256:f78f5f828eff4c44484ca251555a19f0424366aa87a0092dbaceae9b039e0ab4
-hikari[server]==2.0.0.dev116 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:0e1d0bdfe777a6c16cdda7807b49d93c0a0da39ab369683955491d3d10963c90 \
-    --hash=sha256:f78f5f828eff4c44484ca251555a19f0424366aa87a0092dbaceae9b039e0ab4
+hikari==2.0.0.dev117 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:1d1828d1b16687badac1c882ac40d6ead2299c16ca7937065b8fced0fd4ef028 \
+    --hash=sha256:4f2c30d60ebbff37635a80ac788a2c9715ee6f2df626239180e96e65815d9958
+hikari[server]==2.0.0.dev117 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:1d1828d1b16687badac1c882ac40d6ead2299c16ca7937065b8fced0fd4ef028 \
+    --hash=sha256:4f2c30d60ebbff37635a80ac788a2c9715ee6f2df626239180e96e65815d9958
 idna==3.4 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
 iniconfig==2.0.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
 jinja2==3.1.2 ; python_full_version >= "3.9.0" and python_version < "3.12" \
@@ -594,17 +581,17 @@
     --hash=sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b
 nox==2022.11.21 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:0e41a990e290e274cb205a976c4c97ee3c5234441a8132c8c3fd9ea3c22149eb \
     --hash=sha256:e21c31de0711d1274ca585a2c5fde36b1aa962005ba8e9322bf5eeed16dcd684
 packaging==23.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2 \
     --hash=sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97
-platformdirs==3.0.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9 \
-    --hash=sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567
+platformdirs==3.1.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:13b08a53ed71021350c9e300d4ea8668438fb0046ab3937ac9a29913a1a1350a \
+    --hash=sha256:accc3665857288317f32c7bebb5a8e482ba717b474f3fc1d18ca7f9214be0cef
 pluggy==1.0.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
 pycparser==2.21 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
     --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
 pydantic==1.10.5 ; python_full_version >= "3.9.0" and python_version < "3.12" \
@@ -666,41 +653,41 @@
     --hash=sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470
 pytest-sugar==0.9.6 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:30e5225ed2b3cc988a8a672f8bda0fc37bcd92d62e9273937f061112b3f2186d \
     --hash=sha256:c4793495f3c32e114f0f5416290946c316eb96ad5a3684dcdadda9267e59b2b8
 pytest-xdist==3.2.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:336098e3bbd8193276867cc87db8b22903c3927665dff9d1ac8684c02f597b68 \
     --hash=sha256:fa10f95a2564cd91652f2d132725183c3b590d9fdcdec09d3677386ecf4c1ce9
-pytest==7.2.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5 \
-    --hash=sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42
+pytest==7.2.2 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e \
+    --hash=sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4
 python-dateutil==2.8.2 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
 redis==4.5.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:1eec3741cda408d3a5f84b78d089c8b8d895f21b3b050988351e925faf202864 \
     --hash=sha256:5deb072d26e67d2be1712603bfb7947ec3431fb0eec9c578994052e33035af6d
-setuptools==67.4.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:e5fd0a713141a4a105412233c63dc4e17ba0090c8e8334594ac790ec97792330 \
-    --hash=sha256:f106dee1b506dee5102cc3f3e9e68137bbad6d47b616be7991714b0c62204251
+setuptools==67.5.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:15136a251127da2d2e77ac7a1bc231eb504654f7e3346d93613a13f2e2787535 \
+    --hash=sha256:1c39d42bda4cb89f7fdcad52b6762e3c309ec8f8715b27c684176b7d71283242
 six==1.16.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
 termcolor==2.2.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:91ddd848e7251200eac969846cbae2dacd7d71c2871e92733289e7e3666f48e7 \
     --hash=sha256:dfc8ac3f350788f23b2947b3e6cfa5a53b630b612e6cd8965a015a776020b99a
 tomli==2.0.1 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
 typing-extensions==4.5.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
-virtualenv==20.19.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
-    --hash=sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590 \
-    --hash=sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1
+virtualenv==20.20.0 ; python_full_version >= "3.9.0" and python_version < "3.12" \
+    --hash=sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45 \
+    --hash=sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4
 yarl==1.8.2 ; python_full_version >= "3.9.0" and python_version < "3.12" \
     --hash=sha256:009a028127e0a1755c38b03244c0bea9d5565630db9c4cf9572496e947137a87 \
     --hash=sha256:0414fd91ce0b763d4eadb4456795b307a71524dbacd015c657bb2a39db2eab89 \
     --hash=sha256:0978f29222e649c351b173da2b9b4665ad1feb8d1daa9d971eb90df08702668a \
     --hash=sha256:0ef8fb25e52663a1c85d608f6dd72e19bd390e2ecaf29c17fb08f730226e3a08 \
     --hash=sha256:10b08293cda921157f1e7c2790999d903b3fd28cd5c208cf8826b3b508026996 \
     --hash=sha256:1684a9bd9077e922300ecd48003ddae7a7474e0412bea38d4631443a91d61077 \
```

### Comparing `hikari-yuyo-1.9.0a1/examples/components.py` & `hikari-yuyo-1.9.1a1/examples/components.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/mkdocs.yml` & `hikari-yuyo-1.9.1a1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/noxfile.py` & `hikari-yuyo-1.9.1a1/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/freeze-for-pr.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/lint.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/reformat.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/resync-piped.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/type-check.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/update-licence.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/upgrade-locks.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.github/workflows/verify-locks.yml` & `hikari-yuyo-1.9.1a1/piped/.github/workflows/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/.gitignore` & `hikari-yuyo-1.9.1a1/piped/.gitignore`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/LICENSE` & `hikari-yuyo-1.9.1a1/piped/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/bot/Dockerfile` & `hikari-yuyo-1.9.1a1/piped/bot/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.11.1
+FROM python:3.11.2
 
 ARG app_id
 ARG client_secret
 ARG private_key
 ARG webhook_secret
 ENV CLIENT_ID=app_id
 ENV CLIENT_SECRET=client_secret
```

### Comparing `hikari-yuyo-1.9.0a1/piped/bot/main.py` & `hikari-yuyo-1.9.1a1/piped/bot/main.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/bot/requirements.txt` & `hikari-yuyo-1.9.1a1/piped/bot/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -173,17 +173,17 @@
     --hash=sha256:ca9075ab3de9e48b75fa8ccb897c34ccc1519177ad8841d99f7fd74cf43be5bf \
     --hash=sha256:f582cac9d11c227c652d3ce8ee223d94eb06f4228b52a8adaafa9fa62e73d5c9 \
     --hash=sha256:f5bee6c523d13944a1fdc6f0525bc86dbbd94372f17b83fa6331aabacc8fd08e \
     --hash=sha256:f836444b4c5ece128b23ec36a446c9ab7f9b0f7981d0d27e13a7c366ee163f8a
 python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-python-dotenv==0.21.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1c93de8f636cde3ce377292818d0e440b6e45a82f215c3744979151fa8151c49 \
-    --hash=sha256:41e12e0318bebc859fcc4d97d4db8d20ad21721a6aa5047dd59f090391cb549a
+python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a8df96034aae6d2d50a4ebe8216326c61c3eb64836776504fcca410e5937a3ba \
+    --hash=sha256:f5971a9226b701070a4bf2c38c89e5a3f0d64de8debda981d1db98583009122a
 rfc3986[idna2008]==1.5.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835 \
     --hash=sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
 sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
```

### Comparing `hikari-yuyo-1.9.0a1/piped/dev-requirements/flake8.in` & `hikari-yuyo-1.9.1a1/piped/dev-requirements/flake8.in`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/dev-requirements/flake8.txt` & `hikari-yuyo-1.9.1a1/piped/dev-requirements/flake8.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     --hash=sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104
 click==8.1.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-eradicate==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8bfaca181db9227dc88bdbce4d051a9627604c2243e7d85324f6d6ce0fd08bb2 \
-    --hash=sha256:aac7384ab25b1bf21c4c012de9b4bf8398945a14c98c911545b2ea50ab558014
+eradicate==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:751813c315a48ce7e3d0483410991015342d380a956e86e0265c61bfb875bcbc \
+    --hash=sha256:c329a05def6a4b558dab58bb1b694f5209706b7c99ba174d226dfdb69a5ba0da
 flake8-bandit==4.1.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:068e09287189cbfd7f986e92605adea2067630b75380c6b5733dab7d87f9a84e \
     --hash=sha256:4c8a53eb48f23d4ef1e59293657181a3c989d0077c9952717e98a0eace43e06d
 flake8-black==0.3.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0dfbca3274777792a5bcb2af887a4cad72c72d0e86c94e08e3a3de151bb41c34 \
     --hash=sha256:fe8ea2eca98d8a504f22040d9117347f6b367458366952862ac3586e7d4eeaca
 flake8-broken-line==0.6.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -95,17 +95,17 @@
     --hash=sha256:aa0cac02a62c7739e370ce6b9c31743edac904bae4b157274511fc8a19c75bbc
 flake8-mutable==1.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:38fd9dadcbcda6550a916197bc40ed76908119dabb37fbcca30873666c31d2d5 \
     --hash=sha256:ee9b77111b867d845177bbc289d87d541445ffcc6029a0c5c65865b42b18c6a6
 flake8-pep3101==2.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1d818e1f53c6d26e875714f2f041ec15fbb23c17e2268dbbb024e9c3383541cd \
     --hash=sha256:ae2ee1758734a473ca971b4bf9ff09c961b6099916db91fdb6b9718328dfcacb
-flake8-pep585==0.1.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:67feae956ccf7ef20c5cfe57bb63f5342e4f7898fd1cb1d3a8a8a52e26393fd2 \
-    --hash=sha256:8b7bccfa760c40baedb28dc48b1b514907867b3551a7aec87552d115355a6def
+flake8-pep585==0.1.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:363f9413aa12849ee9bfdc437c4e79cc4e0fb3af4abbb61cfed79860e349e0e0 \
+    --hash=sha256:d5c7a5858382d6ca8c56554bd8bed090e12c378b98f6d7c6502abed9a40a658e
 flake8-pep604==1.1.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6e0c4ef8bfa6377eed47df382bde1519a1ddde6508d18b32281846f5a3f77301 \
     --hash=sha256:e533659d0eda50fa83cbca9dde4f3a3fc0b1593d8cd7134e494ccd71102d3fb4
 flake8-plugin-utils==1.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1fe43e3e9acf3a7c0f6b88f5338cad37044d2f156c43cb6b080b5f9da8a76f06 \
     --hash=sha256:20fa2a8ca2decac50116edb42e6af0a1253ef639ad79941249b840531889c65a
 flake8-print==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -136,26 +136,26 @@
     --hash=sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7
 gitpython==3.1.31 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573 \
     --hash=sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d
 isort==5.12.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504 \
     --hash=sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6
-markdown-it-py==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:93de681e5c021a432c63147656fe21790bc01231e0cd2da73626f1aa3ac0fe27 \
-    --hash=sha256:cf7e59fed14b5ae17c0006eff14a2d9a00ed5f3a846148153899a0224e2c07da
+markdown-it-py==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
+    --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
 mccabe==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
 mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
-more-itertools==9.0.0 ; python_version == "3.9" \
-    --hash=sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41 \
-    --hash=sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab
+more-itertools==9.1.0 ; python_version == "3.9" \
+    --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
+    --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
 mr-proper==0.0.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:03b517b19e617537f711ce418b125e5f2efd82ec881539cdee83195c78c14a02 \
     --hash=sha256:74a1b60240c46f10ba518707ef72811a01e5c270da0a78b5dd2dd923d99fdb14
 mypy-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
 packaging==23.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -225,17 +225,17 @@
     --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
     --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
     --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
     --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
 rich==13.3.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:125d96d20c92b946b983d0d392b84ff945461e5a06d3867e9f9e575f8697b67f \
     --hash=sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9
-setuptools==67.3.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9d3de8591bd6f6522594406fa46a6418eabd0562dacb267f8556675762801514 \
-    --hash=sha256:ed4e75fafe103c79b692f217158ba87edf38d31004b9dbc1913debb48793c828
+setuptools==67.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:e5fd0a713141a4a105412233c63dc4e17ba0090c8e8334594ac790ec97792330 \
+    --hash=sha256:f106dee1b506dee5102cc3f3e9e68137bbad6d47b616be7991714b0c62204251
 smmap==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94 \
     --hash=sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936
 stdlib-list==0.8.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2ae0712a55b68f3fbbc9e58d6fa1b646a062188f49745b495f94d3310a9fdd3e \
     --hash=sha256:a1e503719720d71e2ed70ed809b385c60cd3fb555ba7ec046b96360d30b16d9f
 stevedore==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
```

### Comparing `hikari-yuyo-1.9.0a1/piped/dev-requirements/type-checking.txt` & `hikari-yuyo-1.9.1a1/piped/dev-requirements/type-checking.txt`

 * *Files 2% similar despite different names*

```diff
@@ -278,29 +278,29 @@
     --hash=sha256:bd46a0e6296346c477e59a954da57beaf9c538da37b9df482e50f836e4a7d4bb \
     --hash=sha256:c428c0f64a86661fb4873495c4fac430ec7a7cef2b8c1c28f3d1a7277f9ea5ab \
     --hash=sha256:c9e5b778b6842f135902e2d82624008c6a79710207e28e86966cd136c621bfee \
     --hash=sha256:ca9075ab3de9e48b75fa8ccb897c34ccc1519177ad8841d99f7fd74cf43be5bf \
     --hash=sha256:f582cac9d11c227c652d3ce8ee223d94eb06f4228b52a8adaafa9fa62e73d5c9 \
     --hash=sha256:f5bee6c523d13944a1fdc6f0525bc86dbbd94372f17b83fa6331aabacc8fd08e \
     --hash=sha256:f836444b4c5ece128b23ec36a446c9ab7f9b0f7981d0d27e13a7c366ee163f8a
-pyright==1.1.294 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5b27e28a1cfc60cea707fd3b644769fa6dd0b194481cdcc2399cf2a51cc5a846 \
-    --hash=sha256:fea5fed3d6a3f02259e622c901e86a7b8bcf237d35e1cdfe01d0e0723768dcb6
+pyright==1.1.296 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:51cc5f05807b1fb53f9f0e14736b8f772b500a3ba4e0edeb99727e68e700d9ea \
+    --hash=sha256:6c3cd394473e55a516ebe443d02b83e63456ef29f052dcf8e64e7875c1418fa6
 python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-python-dotenv==0.21.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1c93de8f636cde3ce377292818d0e440b6e45a82f215c3744979151fa8151c49 \
-    --hash=sha256:41e12e0318bebc859fcc4d97d4db8d20ad21721a6aa5047dd59f090391cb549a
+python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a8df96034aae6d2d50a4ebe8216326c61c3eb64836776504fcca410e5937a3ba \
+    --hash=sha256:f5971a9226b701070a4bf2c38c89e5a3f0d64de8debda981d1db98583009122a
 rfc3986[idna2008]==1.5.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835 \
     --hash=sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97
-setuptools==67.3.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9d3de8591bd6f6522594406fa46a6418eabd0562dacb267f8556675762801514 \
-    --hash=sha256:ed4e75fafe103c79b692f217158ba87edf38d31004b9dbc1913debb48793c828
+setuptools==67.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:e5fd0a713141a4a105412233c63dc4e17ba0090c8e8334594ac790ec97792330 \
+    --hash=sha256:f106dee1b506dee5102cc3f3e9e68137bbad6d47b616be7991714b0c62204251
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
 sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101 \
     --hash=sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384
 starlette==0.25.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -342,10 +342,10 @@
     --hash=sha256:c092a2c1e736086d59ac8e41f9c98f26bbf9b9222a76f21af9dfe949b99b2eb9 \
     --hash=sha256:c686a47d57ca910a2572fddfe9912819880b8765e2f01dc0dd12a9bf8573e539 \
     --hash=sha256:cbbe908fda687e39afd6ea2a2f14c2c3e43f2ca88e3a11964b297822358d0e6c \
     --hash=sha256:ce9f61938d7155f79d3cb2ffa663147d4a76d16e08f65e2c66b77bd41b356718 \
     --hash=sha256:dbbaf9da2ee98ee2531e0c780455f2841e4675ff580ecf93fe5c48fe733b5667 \
     --hash=sha256:f1e507c9ee39c61bfddd79714e4f85900656db1aec4d40c6de55648e85c2799c \
     --hash=sha256:ff3d00b70ce95adce264462c930fbaecb29718ba6563db354608f37e49e09024
-virtualenv==20.19.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590 \
-    --hash=sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1
+virtualenv==20.20.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45 \
+    --hash=sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4
```

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/clippy.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/clippy.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/freeze-for-pr.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/freeze-for-pr.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/lint.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/lint.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/pr-docs.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/pr-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/publish.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/publish.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/py-test.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/py-test.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/reformat.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/reformat.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/release-docs.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/release-docs.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/resync-piped.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/resync-piped.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/rustfmt.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/rustfmt.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/type-check.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/type-check.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/update-licence.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/update-licence.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/upgrade-locks.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/upgrade-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/verify-locks.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/verify-locks.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/actions/verify-types.yml` & `hikari-yuyo-1.9.1a1/piped/github/actions/verify-types.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/dependabot.yml` & `hikari-yuyo-1.9.1a1/piped/github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/github/pull_request_template.md` & `hikari-yuyo-1.9.1a1/piped/github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/noxfile.py` & `hikari-yuyo-1.9.1a1/piped/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/pyproject.toml` & `hikari-yuyo-1.9.1a1/piped/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -104,17 +104,27 @@
 
 [tool.pyright]
 include = ["bot/main.py", "noxfile.py", "python"]
 
 # TODO: only the bot logic is 3.11+, everything else is 3.8+
 pythonVersion = "3.11"
 typeCheckingMode = "strict"
-reportMissingModuleSource = "error"
-reportMissingTypeStubs = "error"
+reportMissingModuleSource = "error"  # Is only "warning" on strict mode.
 
+# Error code which are disabled even when general strict.
+reportShadowedImports = "error"
+reportCallInDefaultInitializer = "none"  # Ended up just complaining about cases where this was fine (e.g. timedeltas).
+reportImplicitStringConcatenation = "none"  # Conflicts with flake8 config.
+reportMissingSuperCall = "none"  # Way too strict (requires calls to `object.__init__`).
+reportPropertyTypeMismatch = "error"
+reportUninitializedInstanceVariable = "error"
+reportUnnecessaryTypeIgnoreComment = "error"
+reportUnusedCallResult = "none"  # Enforces doing `_ = ...`.
+
+# Error codes which lead to too many false-positives.
 reportIncompatibleMethodOverride = "warning"    # This relies on ordering for key-word only arguments
                                                 # which is more annoying than it's worth
 reportUnknownMemberType = "warning"             # This messes with instance checking generic objects
 reportUnknownArgumentType = "warning"           # Pretty much the same as reportUnknownMemberType
 reportUnknownLambdaType = "warning"
 reportImportCycles = "warning"                  # This isn't necessarily an issue if it's type checking only.
 reportUnknownVariableType = "warning"           # Lotta false-positives, might fix/change later.
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/docs.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/docs.txt`

 * *Files 4% similar despite different names*

```diff
@@ -179,17 +179,17 @@
     --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
 mkdocs-autorefs==0.4.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:70748a7bd025f9ecd6d6feeba8ba63f8e891a1af55f48e366d6d6e78493aba84 \
     --hash=sha256:a2248a9501b29dc0cc8ba4c09f4f47ff121945f6ce33d760f145d6f89d313f5b
 mkdocs-material-extensions==1.1.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93 \
     --hash=sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945
-mkdocs-material==9.0.13 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:06e51eba6a090de070a3489890cf1e491d52c04c6ff2b06dd4586c6cdd974a3f \
-    --hash=sha256:a62696610899d01df091b4d5ad23f9811f878a1f34307d7cea677baf4854c84f
+mkdocs-material==9.0.15 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:734bcf6af9759888385ee15952c2e8a475d8568ded20965da321f0d8117dfe8f \
+    --hash=sha256:d856bc67bc0115b1f258ca012724e17b72a9aea9b8b4d287c38460704f14eeb4
 mkdocs==1.4.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:8947af423a6d0facf41ea1195b8e1e8c85ad94ac95ae307fe11232e0424b11c5 \
     --hash=sha256:c8856a832c1e56702577023cd64cc5f84948280c1c0fcc6af4cd39006ea6aa8c
 mkdocstrings-python==0.8.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4e6e1cd6f37a785de0946ced6eb846eb2f5d891ac1cc2c7b832943d3529087a7 \
     --hash=sha256:9ae473f6dc599339b09eee17e4d2b05d6ac0ec29860f3fc9b7512d940fc61adf
 mkdocstrings==0.20.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -348,39 +348,39 @@
     --hash=sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
 urllib3==1.26.14 ; python_version >= "3.9" and python_version < "4" \
     --hash=sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72 \
     --hash=sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1
-watchdog==2.2.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:102a60093090fc3ff76c983367b19849b7cc24ec414a43c0333680106e62aae1 \
-    --hash=sha256:17f1708f7410af92ddf591e94ae71a27a13974559e72f7e9fde3ec174b26ba2e \
-    --hash=sha256:195ab1d9d611a4c1e5311cbf42273bc541e18ea8c32712f2fb703cfc6ff006f9 \
-    --hash=sha256:4cb5ecc332112017fbdb19ede78d92e29a8165c46b68a0b8ccbd0a154f196d5e \
-    --hash=sha256:5100eae58133355d3ca6c1083a33b81355c4f452afa474c2633bd2fbbba398b3 \
-    --hash=sha256:61fdb8e9c57baf625e27e1420e7ca17f7d2023929cd0065eb79c83da1dfbeacd \
-    --hash=sha256:6ccd8d84b9490a82b51b230740468116b8205822ea5fdc700a553d92661253a3 \
-    --hash=sha256:6e01d699cd260d59b84da6bda019dce0a3353e3fcc774408ae767fe88ee096b7 \
-    --hash=sha256:748ca797ff59962e83cc8e4b233f87113f3cf247c23e6be58b8a2885c7337aa3 \
-    --hash=sha256:83a7cead445008e880dbde833cb9e5cc7b9a0958edb697a96b936621975f15b9 \
-    --hash=sha256:8586d98c494690482c963ffb24c49bf9c8c2fe0589cec4dc2f753b78d1ec301d \
-    --hash=sha256:8b5cde14e5c72b2df5d074774bdff69e9b55da77e102a91f36ef26ca35f9819c \
-    --hash=sha256:8c28c23972ec9c524967895ccb1954bc6f6d4a557d36e681a36e84368660c4ce \
-    --hash=sha256:967636031fa4c4955f0f3f22da3c5c418aa65d50908d31b73b3b3ffd66d60640 \
-    --hash=sha256:96cbeb494e6cbe3ae6aacc430e678ce4b4dd3ae5125035f72b6eb4e5e9eb4f4e \
-    --hash=sha256:978a1aed55de0b807913b7482d09943b23a2d634040b112bdf31811a422f6344 \
-    --hash=sha256:a09483249d25cbdb4c268e020cb861c51baab2d1affd9a6affc68ffe6a231260 \
-    --hash=sha256:a480d122740debf0afac4ddd583c6c0bb519c24f817b42ed6f850e2f6f9d64a8 \
-    --hash=sha256:adaf2ece15f3afa33a6b45f76b333a7da9256e1360003032524d61bdb4c422ae \
-    --hash=sha256:bc43c1b24d2f86b6e1cc15f68635a959388219426109233e606517ff7d0a5a73 \
-    --hash=sha256:c27d8c1535fd4474e40a4b5e01f4ba6720bac58e6751c667895cbc5c8a7af33c \
-    --hash=sha256:cdcc23c9528601a8a293eb4369cbd14f6b4f34f07ae8769421252e9c22718b6f \
-    --hash=sha256:cece1aa596027ff56369f0b50a9de209920e1df9ac6d02c7f9e5d8162eb4f02b \
-    --hash=sha256:d0f29fd9f3f149a5277929de33b4f121a04cf84bb494634707cfa8ea8ae106a8 \
-    --hash=sha256:d6b87477752bd86ac5392ecb9eeed92b416898c30bd40c7e2dd03c3146105646 \
-    --hash=sha256:e038be858425c4f621900b8ff1a3a1330d9edcfeaa1c0468aeb7e330fb87693e \
-    --hash=sha256:e618a4863726bc7a3c64f95c218437f3349fb9d909eb9ea3a1ed3b567417c661 \
-    --hash=sha256:f8ac23ff2c2df4471a61af6490f847633024e5aa120567e08d07af5718c9d092
-zipp==3.14.0 ; python_version >= "3.9" and python_version < "3.10" \
-    --hash=sha256:188834565033387710d046e3fe96acfc9b5e86cbca7f39ff69cf21a4128198b7 \
-    --hash=sha256:9e5421e176ef5ab4c0ad896624e87a7b2f07aca746c9b2aa305952800cb8eecb
+watchdog==2.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:03f342a9432fe08107defbe8e405a2cb922c5d00c4c6c168c68b633c64ce6190 \
+    --hash=sha256:0d9878be36d2b9271e3abaa6f4f051b363ff54dbbe7e7df1af3c920e4311ee43 \
+    --hash=sha256:0e1dd6d449267cc7d6935d7fe27ee0426af6ee16578eed93bacb1be9ff824d2d \
+    --hash=sha256:2caf77ae137935c1466f8cefd4a3aec7017b6969f425d086e6a528241cba7256 \
+    --hash=sha256:3d2dbcf1acd96e7a9c9aefed201c47c8e311075105d94ce5e899f118155709fd \
+    --hash=sha256:4109cccf214b7e3462e8403ab1e5b17b302ecce6c103eb2fc3afa534a7f27b96 \
+    --hash=sha256:4cd61f98cb37143206818cb1786d2438626aa78d682a8f2ecee239055a9771d5 \
+    --hash=sha256:53f3e95081280898d9e4fc51c5c69017715929e4eea1ab45801d5e903dd518ad \
+    --hash=sha256:564e7739abd4bd348aeafbf71cc006b6c0ccda3160c7053c4a53b67d14091d42 \
+    --hash=sha256:5b848c71ef2b15d0ef02f69da8cc120d335cec0ed82a3fa7779e27a5a8527225 \
+    --hash=sha256:5defe4f0918a2a1a4afbe4dbb967f743ac3a93d546ea4674567806375b024adb \
+    --hash=sha256:6f5d0f7eac86807275eba40b577c671b306f6f335ba63a5c5a348da151aba0fc \
+    --hash=sha256:7a1876f660e32027a1a46f8a0fa5747ad4fcf86cb451860eae61a26e102c8c79 \
+    --hash=sha256:7a596f9415a378d0339681efc08d2249e48975daae391d58f2e22a3673b977cf \
+    --hash=sha256:85bf2263290591b7c5fa01140601b64c831be88084de41efbcba6ea289874f44 \
+    --hash=sha256:8a4d484e846dcd75e96b96d80d80445302621be40e293bfdf34a631cab3b33dc \
+    --hash=sha256:8f2df370cd8e4e18499dd0bfdef476431bcc396108b97195d9448d90924e3131 \
+    --hash=sha256:91fd146d723392b3e6eb1ac21f122fcce149a194a2ba0a82c5e4d0ee29cd954c \
+    --hash=sha256:95ad708a9454050a46f741ba5e2f3468655ea22da1114e4c40b8cbdaca572565 \
+    --hash=sha256:964fd236cd443933268ae49b59706569c8b741073dbfd7ca705492bae9d39aab \
+    --hash=sha256:9da7acb9af7e4a272089bd2af0171d23e0d6271385c51d4d9bde91fe918c53ed \
+    --hash=sha256:a073c91a6ef0dda488087669586768195c3080c66866144880f03445ca23ef16 \
+    --hash=sha256:a74155398434937ac2780fd257c045954de5b11b5c52fc844e2199ce3eecf4cf \
+    --hash=sha256:aa8b028750b43e80eea9946d01925168eeadb488dfdef1d82be4b1e28067f375 \
+    --hash=sha256:d1f1200d4ec53b88bf04ab636f9133cb703eb19768a39351cee649de21a33697 \
+    --hash=sha256:d9f9ed26ed22a9d331820a8432c3680707ea8b54121ddcc9dc7d9f2ceeb36906 \
+    --hash=sha256:ea5d86d1bcf4a9d24610aa2f6f25492f441960cf04aed2bd9a97db439b643a7b \
+    --hash=sha256:efe3252137392a471a2174d721e1037a0e6a5da7beb72a021e662b7000a9903f
+zipp==3.15.0 ; python_version >= "3.9" and python_version < "3.10" \
+    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
+    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/flake8.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/flake8.txt`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/freeze-locks.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/freeze-locks.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/freeze-locks.in --output-file python/base-requirements/freeze-locks.txt --min-python-version 3.9
 #
 attrs==22.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836 \
     --hash=sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99
+build==0.10.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
+    --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
 cachecontrol[filecache]==0.12.11 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2c75d6a8938cb1933c75c50184549ad42728a27e9f6b92fd677c3151aa72555b \
     --hash=sha256:a5b9fcc986b184db101aa280b42ecdcdfc524892596f606858e0b7a8b4d9e144
 certifi==2022.12.7 ; python_version >= "3.9" and python_version < "4" \
     --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
     --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
 cffi==1.15.1 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" or python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
@@ -166,14 +169,17 @@
     --hash=sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e \
     --hash=sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479 \
     --hash=sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7 \
     --hash=sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8
 cleo==2.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6eb133670a3ed1f3b052d53789017b6e50fca66d1287e6e6696285f4cb8ea448 \
     --hash=sha256:eb4b2e1f3063c11085cebe489a6e9124163c226575a3c3be69b2e51af4a15ec5
+colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt" \
+    --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
+    --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 crashtest==0.4.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:80d7b1f316ebfbd429f648076d6275c877ba30ba48979de4191714a75266f0ce \
     --hash=sha256:8d23eac5fa660409f57472e3851dab7ac18aba459a8d19cbbba86d3d5aecd2a5
 cryptography==39.0.1 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
     --hash=sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4 \
     --hash=sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f \
     --hash=sha256:4789d1e3e257965e960232345002262ede4d094d1a19f4d3b52e48d4d8f3b885 \
@@ -193,93 +199,89 @@
     --hash=sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6 \
     --hash=sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336 \
     --hash=sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0 \
     --hash=sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c \
     --hash=sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106 \
     --hash=sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a \
     --hash=sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8
-distlib==0.3.6 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32" or python_version > "3.9" and python_version < "4.0" or sys_platform == "win32" and python_version == "3.9" \
+distlib==0.3.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
-dulwich==0.20.50 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:06775c5713cfeda778c7c67d4422b5e7554d3a7f644f1dde646cdf486a30285a \
-    --hash=sha256:0c61c193d02c0e1e0d758cdd57ae76685c368d09a01f00d704ba88bd96767cfe \
-    --hash=sha256:0e4862f318d99cc8a500e3622a89613a88c07d957a0f628cdc2ed86addff790f \
-    --hash=sha256:0f9c4f2455f966cad94648278fa9972e4695b35d04f82792fa58e1ea15dd83f0 \
-    --hash=sha256:11b180b80363b4fc70664197028181a17ae4c52df9965a29b62a6c52e40c2dbe \
-    --hash=sha256:2644466270267270f2157ea6f1c0aa224f6f3bf06a307fc39954e6b4b3d82bae \
-    --hash=sha256:2aa2a4a84029625bf9c63771f8a628db1f3be2d2ea3cb8b17942cd4317797152 \
-    --hash=sha256:322ff8ff6aa4d6d36294cd36de1c84767eb1903c7db3e7b4475ad091febf5363 \
-    --hash=sha256:3b1964fa80cafd5a1fd71615b0313daf6f3295c6ab05656ea0c1d2423539904a \
-    --hash=sha256:3fb35cedb1243bc420d885ef5b4afd642c6ac8f07ddfc7fdbca1becf9948bf7e \
-    --hash=sha256:4842e22ed863a776b36ef8ffe9ed7b772eb452b42c8d02975c29d27e3bc50ab4 \
-    --hash=sha256:49f66f1c057c18d7d60363f461f4ab8329320fbe1f02a7a33c255864a7d3c942 \
-    --hash=sha256:4aa1d0861517ebbbe0e0084cc9ab4f7ab720624a3eda2bd10e45f774ab858db8 \
-    --hash=sha256:4bb23a9cec63e16c0e432335f068169b73dd44fa9318dd7cd7a4ca83607ff367 \
-    --hash=sha256:4e541cd690a5e3d55082ed51732d755917e933cddeb4b0204f2a5ec5d5d7b60b \
-    --hash=sha256:50a941796b2c675be39be728d540c16b5b7ce77eb9e1b3f855650ece6832d2be \
-    --hash=sha256:519b627d49d273e2fd01c79d09e578675ca6cd05193c1787e9ef165c9a1d66ea \
-    --hash=sha256:5267619b34ddaf8d9a6b841492cd17a971fd25bf9a5657f2de928385c3a08b94 \
-    --hash=sha256:5411d0f1092152e1c0bb916ae490fe181953ae1b8d13f4e68661253e10b78dbb \
-    --hash=sha256:57bff9bde0b6b05b00c6acbb1a94357caddb2908ed7026a48c715ff50d220335 \
-    --hash=sha256:583c6bbc27f13fe2e41a19f6987a42681c6e4f6959beae0a6e5bb033b8b081a8 \
-    --hash=sha256:5d3290a45651c8e534f8e83ae2e30322aefdd162f0f338bae2e79a6ee5a87513 \
-    --hash=sha256:6343569f998ce429e2a5d813c56768ac51b496522401db950f0aa44240bfa901 \
-    --hash=sha256:6a75cab01b909c4c683c2083e060e378bc01701b7366b5a7d9846ef6d3b9e3d5 \
-    --hash=sha256:6d409a282f8848fd6c8d7c7545ad2f75c16de5d5977de202642f1d50fdaac554 \
-    --hash=sha256:7301773e5cc16d521bc6490e73772a86a4d1d0263de506f08b54678cc4e2f061 \
-    --hash=sha256:731e7f319b34251fadeb362ada1d52cc932369d9cdfa25c0e41150cda28773d0 \
-    --hash=sha256:78c388ad421199000fb7b5ed5f0c7b509b3e31bd7cad303786a4d0bf89b82f60 \
-    --hash=sha256:790e4a641284a7fb4d56ebdaf8b324a5826fbbb9c54307c06f586f9f6a5e56db \
-    --hash=sha256:7aaabb8e4beadd53f75f853a981caaadef3ef130e5645c902705704eaf136daa \
-    --hash=sha256:80ab07131a6e68594441f5c4767e9e44e87fceafc3e347e541c928a18c679bd8 \
-    --hash=sha256:80e8750ee2fa0ab2784a095956077758e5f6107de27f637c4b9d18406652c22c \
-    --hash=sha256:8cc6092a4f0bbbff2e553e87a9c6325955b64ea43fca21297c8182e19ae8a43c \
-    --hash=sha256:8f3af857f94021cae1322d86925bfc0dd31e501e885ab5db275473bfac0bb39d \
-    --hash=sha256:9091f1d53a3c0747cbf0bd127c64e7f09b770264d8fb53e284383fcdf69154e7 \
-    --hash=sha256:9163fbb021a8ad9c35a0814a5eedf45a8eb3a0b764b865d7016d901fc5a947fc \
-    --hash=sha256:97f02f8d500d4af08dc022d697c56e8539171acc3f575c2fe9acf3b078e5c8c9 \
-    --hash=sha256:a24a3893108f3b97beb958670d5f3f2a3bec73a1fe18637a572a85abd949a1c4 \
-    --hash=sha256:a344230cadfc5d315752add6ce9d4cfcfc6c85e36bbf57fce9444bcc7c6ea8fb \
-    --hash=sha256:a405cd236766060894411614a272cfb86fe86cde5ca73ef264fc4fa5a715fff4 \
-    --hash=sha256:a6ec7c8fea2b44187a3b545e6c11ab9947ffb122647b07abcdb7cc3aaa770c0e \
-    --hash=sha256:af4adac92fb95671ea3a24f2f8e5e5e8f638711ce9c33a3ca6cd68bf1ff7d99f \
-    --hash=sha256:b4d11d44176e5d2fa8271fc86ad1e0a8731b9ad8f77df64c12846b30e16135eb \
-    --hash=sha256:b70106580ed11f45f4c32d2831d0c9c9f359bc2415fff4a6be443e3a36811398 \
-    --hash=sha256:c075f69c2de19d9fd97e3b70832d2b42c6a4a5d909b3ffd1963b67d86029f95f \
-    --hash=sha256:c2edbff3053251985f10702adfafbee118298d383ef5b5b432a5f22d1f1915df \
-    --hash=sha256:c3dc9f97ec8d3db08d9723b9fd06f3e52c15b84c800d153cfb59b0a3dc8b8d40 \
-    --hash=sha256:c7542a72c5640dd0620862d6df8688f02a6c336359b5af9b3fcfe11b7fa6652f \
-    --hash=sha256:c83e7840d9d0a94d7033bc109efe0c22dfcdcd816bcd4469085e42809e3bf5ba \
-    --hash=sha256:c96e3fb9d48c0454dc242c7accc7819780c9a7f29e441a9eff12361ed0fa35f9 \
-    --hash=sha256:cb194c53109131bcbcd1ca430fcd437cdaf2d33e204e45fbe121c47eaa43e9af \
-    --hash=sha256:d2f7df39bd1378d3b0bfb3e7fc930fd0191924af1f0ef587bcd9946afe076c06 \
-    --hash=sha256:d3ee45001411b638641819b7b3b33f31f13467c84066e432256580fcab7d8815 \
-    --hash=sha256:d4629635a97e3af1b5da48071e00c8e70fad85f3266fadabe1f5a8f49172c507 \
-    --hash=sha256:dd9fa00971ecf059bb358085a942ecac5be4ff71acdf299f44c8cbc45c18659f \
-    --hash=sha256:df3562dde3079d57287c233d45b790bc967c5aae975c9a7b07ca30e60e055512 \
-    --hash=sha256:e1ae18d5805f0c0c5dac65795f8d48660437166b12ee2c0ffea95bfdbf9c1051 \
-    --hash=sha256:e29a3c2037761fa816aa556e78364dfc8e3f44b873db2d17aed96f9b06ac83a3 \
-    --hash=sha256:ea8ffe26d91dbcd5580dbd5a07270a12ea57b091604d77184da0a0d9fad50ed3 \
-    --hash=sha256:ee0f9b02019c0ea84cdd31c00a0c283669b771c85612997a911715cf84e33d99 \
-    --hash=sha256:eefe786a6010f8546baac4912113eeed4e397ddb8c433a345b548a04d4176496 \
-    --hash=sha256:f08406b6b789dea5c95ba1130a0801d8748a67f18be940fe7486a8b481fde875 \
-    --hash=sha256:fbb6368f18451dc44c95c55e1a609d1a01d3821f7ed480b22b2aea1baca0f4a7
-filelock==3.9.0 ; python_version < "4.0" and python_version >= "3.9" \
+dulwich==0.21.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:026427b5ef0f1fe138ed22078e49b00175b58b11e5c18e2be00f06ee0782603b \
+    --hash=sha256:03ed9448f2944166e28aa8d3f4c8feeceb5c6880e9ffe5ab274869d45abd9589 \
+    --hash=sha256:058aaba18aefe18fcd84b216fd34d032ad453967dcf3dee263278951cd43e2d4 \
+    --hash=sha256:075c8e9d2694ff16fc6e8a5ec0c771b7c33be12e4ebecc346fd74315d3d84605 \
+    --hash=sha256:08ee426b609dab552839b5c7394ae9af2112c164bb727b7f85a69980eced9251 \
+    --hash=sha256:092829f27a2c87cdf6b6523216822859ecf01d281ddfae0e58cad1f44adafff6 \
+    --hash=sha256:0b541bd58426a30753ab12cc024ba29b6699d197d9d0d9f130b9768ab20e0e6a \
+    --hash=sha256:0cd83f84e58aa59fb9d85cf15e74be83a5be876ac5876d5030f60fcce7ab36f1 \
+    --hash=sha256:1799c04bd53ec404ebd2c82c1d66197a31e5f0549c95348bb7d3f57a28c94241 \
+    --hash=sha256:1cf246530b8d574b33a9614da76881b96c190c0fe78f76ab016c88082c0da051 \
+    --hash=sha256:208d01a9cda1bae16c92e8c54e806701a16969346aba44b8d6921c6c227277a9 \
+    --hash=sha256:21ee962211839bb6e52d41f363ce9dbb0638d341a1c02263e163d69012f58b25 \
+    --hash=sha256:250ec581682af846cb85844f8032b7642dd278006b1c3abd5e8e718eba0b1b00 \
+    --hash=sha256:25376efc6ea2ee9daa868a120d4f9c905dcb7774f68931be921fba41a657f58a \
+    --hash=sha256:2bf2be68fddfc0adfe43be99ab31f6b0f16b9ef1e40464679ba831ff615ad4a3 \
+    --hash=sha256:33f73e8f902c6397cc73a727db1f6e75add8ce894bfbb1a15daa2f7a4138a744 \
+    --hash=sha256:3b048f84c94c3284f29bf228f1094ccc48763d76ede5c35632153bd7f697b846 \
+    --hash=sha256:40f8f461eba87ef2e8ce0005ca2c12f1b4fdbbafd3a717b8570060d7cd35ee0c \
+    --hash=sha256:512bb4b04e403a38860f7eb22abeeaefba3c4a9c08bc7beec8885494c5828034 \
+    --hash=sha256:5a1137177b62eec949c0f1564eef73920f842af5ebfc260c20d9cd47e8ecd519 \
+    --hash=sha256:6618e35268d116bffddd6dbec360a40c54b3164f8af0513d95d8698f36e2eacc \
+    --hash=sha256:67dbf4dd7586b2d437f539d5dc930ebceaf74a4150720644d6ea7e5ffc1cb2ff \
+    --hash=sha256:6f8d45f5fcdb52c60c902a951f549faad9979314e7e069f4fa3d14eb409b16a0 \
+    --hash=sha256:73f9feba3da1ae66f0b521d7c2727db7f5025a83facdc73f4f39abe2b6d4f00d \
+    --hash=sha256:7aaf5c4528e83e3176e7dbb01dcec34fb41c93279a8f8527cf33e5df88bfb910 \
+    --hash=sha256:7c69c95d5242171d07396761f759a8a4d566e9a01bf99612f9b9e309e70a80fc \
+    --hash=sha256:7ca3b453d767eb83b3ec58f0cfcdc934875a341cdfdb0dc55c1431c96608cf83 \
+    --hash=sha256:7f2cb11fe789b72feeae7cdf6e27375c33ed6915f8ca5ea7ce81b5e234c75a9e \
+    --hash=sha256:89af4ee347f361338bad5c27b023f9d19e7aed17aa75cb519f28e6cf1658a0ba \
+    --hash=sha256:8ad7de37c9ff817bc5d26f89100f87b7f1a5cc25e5eaaa54f11dc66cca9652e4 \
+    --hash=sha256:8ba1fe3fb415fd34cae5ca090fb82030b6e8423d6eb2c4c9c4fbf50b15c7664c \
+    --hash=sha256:9213a114dd19cfca19715088f12f143e918c5e1b4e26f7acf1a823d7da9e1413 \
+    --hash=sha256:9f08e5cc10143d3da2a2cf735d8b932ef4e4e1d74b0c74ce66c52eab02068be8 \
+    --hash=sha256:a275b3a579dfd923d6330f6e5c2886dbdb5da4e004c5abecb107eb347d301412 \
+    --hash=sha256:a2e6270923bf5ec0e9f720d689579a904f401c62193222d000d8cb8e880684e9 \
+    --hash=sha256:a98989ff1ed20825728495ffb859cd700a120850074184d2e1ec08a0b1ab8ab3 \
+    --hash=sha256:ae38c6d24d7aff003a241c8f1dd268eb1c6f7625d91e3435836ff5a5eed05ce5 \
+    --hash=sha256:af7a417e19068b1abeb9addd3c045a2d6e40d15365af6aa3cbe2d47305b5bb11 \
+    --hash=sha256:b09b6166876d2cba8f331a548932b09e11c9386db0525c9ca15c399b666746fc \
+    --hash=sha256:b9fc609a3d4009ee31212f435f5a75720ef24280f6d23edfd53f77b562a79c5b \
+    --hash=sha256:ba3d42cd83d7f89b9c1b2f76df971e8ab58815f8060da4dc67b9ae9dba1b34cc \
+    --hash=sha256:baf5b3b901272837bee2311ecbd28fdbe960d288a070dc72bdfdf48cfcbb8090 \
+    --hash=sha256:bb54fe45deb55e4caae4ea2c1dba93ee79fb5c377287b14056d4c30fb156920e \
+    --hash=sha256:be0801ae3f9017c6437bcd23a4bf2b2aa88e465f7efeed4b079944d07e3df994 \
+    --hash=sha256:c349431f5c8aa99b8744550d0bb4615f63e73450584202ac5db0e5d7da4d82ff \
+    --hash=sha256:c80ade5cdb0ea447e7f43b32abc2f4a628dcdfa64dc8ee5ab4262987e5e0814f \
+    --hash=sha256:c8d1837c3d2d8e56aacc13a91ec7540b3baadc1b254fbdf225a2d15b72b654c3 \
+    --hash=sha256:c97561c22fc05d0f6ba370d9bd67f86c313c38f31a1793e0ee9acb78ee28e4b8 \
+    --hash=sha256:cf1f6edc968619a4355481c29d5571726723bc12924e2b25bd3348919f9bc992 \
+    --hash=sha256:cf7af6458cf6343a2a0632ae2fc5f04821b2ffefc7b8a27f4eacb726ef89c682 \
+    --hash=sha256:d0ac29adf468a838884e1507d81e872096238c76fe7da7f3325507e4390b6867 \
+    --hash=sha256:d7ad871d044a96f794170f2434e832c6b42804d0b53721377d03f865245cd273 \
+    --hash=sha256:ddb790f2fdc22984fba643866b21d04733c5cf7c3ace2a1e99e0c1c1d2336aab \
+    --hash=sha256:e3b686b49adeb7fc45791dfae96ffcffeba1038e8b7603f369d6661f59e479fc \
+    --hash=sha256:e7b8cb38a93de87b980f882f0dcd19f2e3ad43216f34e06916315cb3a03e6964 \
+    --hash=sha256:f4f8ff776ca38ce272d9c164a7f77db8a54a8cad6d9468124317adf8732be07d
+filelock==3.9.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de \
     --hash=sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d
 html5lib==1.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0d78f8fde1c230e99fe37986a60526d7049ed4bf8a9fadbad5f00e22e58e041d \
     --hash=sha256:b2e5b40261e20f354d198eae92afc10d750afb487ed5e50f9c4eaf07c184146f
 idna==3.4 ; python_version >= "3.9" and python_version < "4" \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
-importlib-metadata==4.13.0 ; python_version >= "3.9" and python_version < "3.12" \
-    --hash=sha256:8a8a81bcf996e74fee46f0d16bd3eaa382a7eb20fd82445c3ad11f4090334116 \
-    --hash=sha256:dd0173e8f150d6815e098fd354f6414b0f079af4644ddfe90c71e2fc6174346d
+importlib-metadata==6.0.0 ; python_version >= "3.9" and python_version < "3.12" \
+    --hash=sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad \
+    --hash=sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d
+installer==0.6.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:ae7c62d1d6158b5c096419102ad0d01fdccebf857e784cee57f94165635fe038 \
+    --hash=sha256:f3bd36cd261b440a88a1190b1becca0578fee90b4b62decc796932fdd5ae8839
 jaraco-classes==3.2.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158 \
     --hash=sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a
 jeepney==0.8.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
     --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
 jsonschema==4.17.3 ; python_version >= "3.9" and python_version < "4.0" \
@@ -287,17 +289,17 @@
     --hash=sha256:a870ad254da1a8ca84b6a2905cac29d265f805acc57af304784962a2aa6508f6
 keyring==23.13.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd \
     --hash=sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678
 lockfile==0.12.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6aed02de03cba24efabcd600b30540140634fc06cfa603822d508d5361e9f799 \
     --hash=sha256:6c3cb24f344923d30b2785d5ad75182c8ea7ac1b6171b08657258ec7429d50fa
-more-itertools==9.0.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41 \
-    --hash=sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab
+more-itertools==9.1.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
+    --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
 msgpack==1.0.4 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:002b5c72b6cd9b4bafd790f364b8480e859b4712e91f43014fe01e4f957b8467 \
     --hash=sha256:0a68d3ac0104e2d3510de90a1091720157c319ceeb90d74f7b5295a6bee51bae \
     --hash=sha256:0df96d6eaf45ceca04b3f3b4b111b86b33785683d682c655063ef8057d61fd92 \
     --hash=sha256:0dfe3947db5fb9ce52aaea6ca28112a170db9eae75adf9339a1aec434dc954ef \
     --hash=sha256:0e3590f9fb9f7fbc36df366267870e77269c03172d086fa76bb4eba8b2b46624 \
     --hash=sha256:11184bc7e56fd74c00ead4f9cc9a3091d62ecb96e97653add7a879a14b003227 \
@@ -358,35 +360,38 @@
     --hash=sha256:a6d50dcab8d375889302bebeef22da83a439d2a0da327cb65e1ff60c1197d1d7
 pip-requirements-parser==32.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4659bc2a667783e7a15d190f6fccf8b2486685b6dba4c19c3876314769c57526 \
     --hash=sha256:b4fa3a7a0be38243123cf9d1f3518da10c51bdb165a2b2985566247f9155a7d3
 pkginfo==1.9.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
     --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
-platformdirs==2.6.2 ; python_version < "4.0" and python_version >= "3.9" \
+platformdirs==2.6.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490 \
     --hash=sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2
-poetry-core==1.4.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:514bd33c30e0bf56b0ed44ee15e120d7e47b61ad908b2b1011da68c48a84ada9 \
-    --hash=sha256:5559ab80384ac021db329ef317086417e140ee1176bcfcb3a3838b544e213c8e
+poetry-core==1.5.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:41887261358863f25831fa0ad1fe7e451fc32d1c81fcf7710ba5174cc0047c6d \
+    --hash=sha256:b1900dea81eb18feb7323d404e5f10430205541a4a683a912893f9d2b5807797
 poetry-plugin-export==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:61ae5ec1db233aba947a48e1ce54c6ff66afd0e1c87195d6bce64c73a5ae658c \
     --hash=sha256:6e5919bf84afcb08cdd419a03f909f490d8671f00633a3c6df8ba09b0820dc2f
-poetry==1.3.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:26ded25f0cf67943243ca4f0aafd47ec4668bdb62845dbb8c2b0e3d9cd280bf4 \
-    --hash=sha256:41980d557954b1418fa503de7a8fb25f19c03c0223a171666b305f05a45fc206
+poetry==1.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:151ad741e163a329c8b13ea602dde979b7616fc350cfcff74b604e93263934a8 \
+    --hash=sha256:f88a7a812a5d8c1f5a378e0924f898926b2ac10c3b5c03f7282f2182f90d8507
 ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35 \
     --hash=sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220
 pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" or python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
     --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
     --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
 pyparsing==3.0.9 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb \
     --hash=sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc
+pyproject-hooks==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
+    --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
 pyrsistent==0.19.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:016ad1afadf318eb7911baa24b049909f7f3bb2c5b1ed7b6a8f21db21ea3faa8 \
     --hash=sha256:1a2994773706bbb4995c31a97bc94f1418314923bd1048c6d964837040376440 \
     --hash=sha256:20460ac0ea439a3e79caa1dbd560344b64ed75e85d8703943e0b66c2a6150e4a \
     --hash=sha256:3311cb4237a341aa52ab8448c27e3a9931e2ee09561ad150ba94e4cfd3fc888c \
     --hash=sha256:3a8cb235fa6d3fd7aae6a4f1429bbb1fec1577d978098da1252f0489937786f3 \
     --hash=sha256:3ab2204234c0ecd8b9368dbd6a53e83c3d4f3cab10ecaf6d0e772f456c442393 \
@@ -530,17 +535,17 @@
     --hash=sha256:de61417c958b06fd4923b2e26d4e70dd7ffc691d5435bcd7ed78d061278885f1
 urllib3==1.26.14 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72 \
     --hash=sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1
 virtualenv==20.16.5 ; sys_platform == "win32" and python_version == "3.9" \
     --hash=sha256:227ea1b9994fdc5ea31977ba3383ef296d7472ea85be9d6732e42a91c04e80da \
     --hash=sha256:d07dfc5df5e4e0dbc92862350ad87a36ed505b978f6c39609dc489eadd5b0d27
-virtualenv==20.19.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32" or python_version > "3.9" and python_version < "4.0" \
-    --hash=sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590 \
-    --hash=sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1
+virtualenv==20.20.0 ; sys_platform != "win32" and python_version >= "3.9" and python_version < "4.0" or python_version > "3.9" and python_version < "4.0" \
+    --hash=sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45 \
+    --hash=sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4
 webencodings==0.5.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78 \
     --hash=sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923
 xattr==0.10.1 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" \
     --hash=sha256:042ad818cda6013162c0bfd3816f6b74b7700e73c908cde6768da824686885f8 \
     --hash=sha256:0aedf55b116beb6427e6f7958ccd80a8cbc80e82f87a4cd975ccb61a8d27b2ee \
     --hash=sha256:0e14bd5965d3db173d6983abdc1241c22219385c22df8b0eb8f1846c15ce1fee \
@@ -609,10 +614,10 @@
     --hash=sha256:e8c014c371391f28f8cd27d73ea59f42b30772cd640b5a2538ad4f440fd9190b \
     --hash=sha256:ec0956a8ab0f0d3f9011ba480f1e1271b703d11542375ef73eb8695a6bd4b78b \
     --hash=sha256:f1be6e733e9698f645dbb98565bb8df9b75e80e15a21eb52787d7d96800e823b \
     --hash=sha256:f24a7c04ff666d0fe905dfee0a84bc899d624aeb6dccd1ea86b5c347f15c20c1 \
     --hash=sha256:f55a2dd73a12a1ae5113c5d9cd4b4ab6bf7950f4d76d0a1a0c0c4264d50da61d \
     --hash=sha256:fc354f086f926a1c7f04886f97880fed1a26d20e3bc338d0d965fd161dbdb8ab \
     --hash=sha256:ffcb57ca1be338d69edad93cf59aac7c6bb4dbb92fd7bf8d456c69ea42f7e6d2
-zipp==3.14.0 ; python_version >= "3.9" and python_version < "3.12" \
-    --hash=sha256:188834565033387710d046e3fe96acfc9b5e86cbca7f39ff69cf21a4128198b7 \
-    --hash=sha256:9e5421e176ef5ab4c0ad896624e87a7b2f07aca746c9b2aa305952800cb8eecb
+zipp==3.15.0 ; python_version >= "3.9" and python_version < "3.12" \
+    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
+    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/library-flake8.in` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/library-flake8.in`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/library-flake8.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/library-flake8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     --hash=sha256:dbbc264b70a470ed8c6c95976a11dfb8b7f63df44ed1af87328bbed2663f5161
 click==8.1.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-eradicate==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8bfaca181db9227dc88bdbce4d051a9627604c2243e7d85324f6d6ce0fd08bb2 \
-    --hash=sha256:aac7384ab25b1bf21c4c012de9b4bf8398945a14c98c911545b2ea50ab558014
+eradicate==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:751813c315a48ce7e3d0483410991015342d380a956e86e0265c61bfb875bcbc \
+    --hash=sha256:c329a05def6a4b558dab58bb1b694f5209706b7c99ba174d226dfdb69a5ba0da
 flake8-async==22.11.14 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:317cf0f882a2f4a09c2250c451acff8358d7faec8a0aa54521b6e69336fe9d0b \
     --hash=sha256:b4db2d55883653b47d4bfd946fdf506e8958bb4ca35974790b8c3e620fc1abff
 flake8-bandit==4.1.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:068e09287189cbfd7f986e92605adea2067630b75380c6b5733dab7d87f9a84e \
     --hash=sha256:4c8a53eb48f23d4ef1e59293657181a3c989d0077c9952717e98a0eace43e06d
 flake8-black==0.3.6 ; python_version >= "3.9" and python_version < "4.0" \
@@ -113,17 +113,17 @@
     --hash=sha256:ee9b77111b867d845177bbc289d87d541445ffcc6029a0c5c65865b42b18c6a6
 flake8-no-pep420==2.3.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1b965a18508ac7842de288740aa43627d3a5bb2be64f7d5d70d55cb691c3de84 \
     --hash=sha256:ccba3efa05c50b1c2712d78807cca81e563ab571d6b3bcb90228e87388704cf5
 flake8-pep3101==2.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1d818e1f53c6d26e875714f2f041ec15fbb23c17e2268dbbb024e9c3383541cd \
     --hash=sha256:ae2ee1758734a473ca971b4bf9ff09c961b6099916db91fdb6b9718328dfcacb
-flake8-pep585==0.1.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:67feae956ccf7ef20c5cfe57bb63f5342e4f7898fd1cb1d3a8a8a52e26393fd2 \
-    --hash=sha256:8b7bccfa760c40baedb28dc48b1b514907867b3551a7aec87552d115355a6def
+flake8-pep585==0.1.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:363f9413aa12849ee9bfdc437c4e79cc4e0fb3af4abbb61cfed79860e349e0e0 \
+    --hash=sha256:d5c7a5858382d6ca8c56554bd8bed090e12c378b98f6d7c6502abed9a40a658e
 flake8-plugin-utils==1.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1fe43e3e9acf3a7c0f6b88f5338cad37044d2f156c43cb6b080b5f9da8a76f06 \
     --hash=sha256:20fa2a8ca2decac50116edb42e6af0a1253ef639ad79941249b840531889c65a
 flake8-print==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:76915a2a389cc1c0879636c219eb909c38501d3a43cc8dae542081c9ba48bdf9 \
     --hash=sha256:84a1a6ea10d7056b804221ac5e62b1cee1aefc897ce16f2e5c42d3046068f5d8
 flake8-printf-formatting==1.1.2 ; python_version >= "3.9" and python_version < "4.0" \
@@ -166,17 +166,17 @@
     --hash=sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d
 isort==5.12.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504 \
     --hash=sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6
 jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
-markdown-it-py==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:93de681e5c021a432c63147656fe21790bc01231e0cd2da73626f1aa3ac0fe27 \
-    --hash=sha256:cf7e59fed14b5ae17c0006eff14a2d9a00ed5f3a846148153899a0224e2c07da
+markdown-it-py==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
+    --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
 markupsafe==2.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
     --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
     --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
     --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
     --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
     --hash=sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0 \
@@ -226,17 +226,17 @@
     --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
 mccabe==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
 mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
-more-itertools==9.0.0 ; python_version == "3.9" \
-    --hash=sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41 \
-    --hash=sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab
+more-itertools==9.1.0 ; python_version == "3.9" \
+    --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
+    --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
 mr-proper==0.0.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:03b517b19e617537f711ce418b125e5f2efd82ec881539cdee83195c78c14a02 \
     --hash=sha256:74a1b60240c46f10ba518707ef72811a01e5c270da0a78b5dd2dd923d99fdb14
 mypy-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
 packaging==23.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -309,17 +309,17 @@
     --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
     --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
     --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
     --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
 rich==13.3.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:125d96d20c92b946b983d0d392b84ff945461e5a06d3867e9f9e575f8697b67f \
     --hash=sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9
-setuptools==67.3.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9d3de8591bd6f6522594406fa46a6418eabd0562dacb267f8556675762801514 \
-    --hash=sha256:ed4e75fafe103c79b692f217158ba87edf38d31004b9dbc1913debb48793c828
+setuptools==67.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:e5fd0a713141a4a105412233c63dc4e17ba0090c8e8334594ac790ec97792330 \
+    --hash=sha256:f106dee1b506dee5102cc3f3e9e68137bbad6d47b616be7991714b0c62204251
 smmap==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94 \
     --hash=sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936
 snowballstemmer==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
 stdlib-list==0.8.0 ; python_version >= "3.9" and python_version < "4.0" \
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/lint.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/lint.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,20 +41,22 @@
     --hash=sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b \
     --hash=sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b \
     --hash=sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640 \
     --hash=sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7 \
     --hash=sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a \
     --hash=sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71 \
     --hash=sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8 \
+    --hash=sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122 \
     --hash=sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7 \
     --hash=sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80 \
     --hash=sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e \
     --hash=sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab \
     --hash=sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0 \
-    --hash=sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646
+    --hash=sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646 \
+    --hash=sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38
 ruamel-yaml==0.17.21 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7 \
     --hash=sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af
 slotscheck==0.16.4 ; python_version >= "3.9" and python_version < "4" \
     --hash=sha256:2a4f63debc66578e281f87bb581929f416788005a9260c2da4520a0f82a3b860 \
     --hash=sha256:3ceed3cb325dccffe93a24ffb472c3193b75bc3f5cf613dcacbdb3114ba1f941
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/nox.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/nox.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,10 +121,10 @@
     --hash=sha256:f836444b4c5ece128b23ec36a446c9ab7f9b0f7981d0d27e13a7c366ee163f8a
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
 typing-extensions==4.5.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
-virtualenv==20.19.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590 \
-    --hash=sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1
+virtualenv==20.20.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3c22fa5a7c7aa106ced59934d2c20a2ecb7f49b4130b8bf444178a16b880fa45 \
+    --hash=sha256:a8a4b8ca1e28f864b7514a253f98c1d62b64e31e77325ba279248c65fb4fcef4
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/publish.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/publish.txt`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/reformat.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/reformat.txt`

 * *Files 1% similar despite different names*

```diff
@@ -154,20 +154,22 @@
     --hash=sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b \
     --hash=sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b \
     --hash=sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640 \
     --hash=sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7 \
     --hash=sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a \
     --hash=sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71 \
     --hash=sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8 \
+    --hash=sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122 \
     --hash=sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7 \
     --hash=sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80 \
     --hash=sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e \
     --hash=sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab \
     --hash=sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0 \
-    --hash=sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646
+    --hash=sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646 \
+    --hash=sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38
 ruamel-yaml==0.17.21 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7 \
     --hash=sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af
 sort-all==1.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1eb6a91cc61f36bd48d697f687377c6eb67b4ef98e2850fc65130502bae945d8 \
     --hash=sha256:ccc0fc7191a486ff826cb4d21c2b67d93f9d9cb5eb72e8d572d017d50d4eca88
 tokenize-rt==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/tests.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/tests.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,66 +6,66 @@
 #
 attrs==22.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836 \
     --hash=sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-coverage[toml]==7.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:04481245ef966fbd24ae9b9e537ce899ae584d521dfbe78f89cad003c38ca2ab \
-    --hash=sha256:0c45948f613d5d18c9ec5eaa203ce06a653334cf1bd47c783a12d0dd4fd9c851 \
-    --hash=sha256:10188fe543560ec4874f974b5305cd1a8bdcfa885ee00ea3a03733464c4ca265 \
-    --hash=sha256:218fe982371ac7387304153ecd51205f14e9d731b34fb0568181abaf7b443ba0 \
-    --hash=sha256:29571503c37f2ef2138a306d23e7270687c0efb9cab4bd8038d609b5c2393a3a \
-    --hash=sha256:2a60d6513781e87047c3e630b33b4d1e89f39836dac6e069ffee28c4786715f5 \
-    --hash=sha256:2bf1d5f2084c3932b56b962a683074a3692bce7cabd3aa023c987a2a8e7612f6 \
-    --hash=sha256:3164d31078fa9efe406e198aecd2a02d32a62fecbdef74f76dad6a46c7e48311 \
-    --hash=sha256:32df215215f3af2c1617a55dbdfb403b772d463d54d219985ac7cd3bf124cada \
-    --hash=sha256:33d1ae9d4079e05ac4cc1ef9e20c648f5afabf1a92adfaf2ccf509c50b85717f \
-    --hash=sha256:33ff26d0f6cc3ca8de13d14fde1ff8efe1456b53e3f0273e63cc8b3c84a063d8 \
-    --hash=sha256:38da2db80cc505a611938d8624801158e409928b136c8916cd2e203970dde4dc \
-    --hash=sha256:3b155caf3760408d1cb903b21e6a97ad4e2bdad43cbc265e3ce0afb8e0057e73 \
-    --hash=sha256:3b946bbcd5a8231383450b195cfb58cb01cbe7f8949f5758566b881df4b33baf \
-    --hash=sha256:3baf5f126f30781b5e93dbefcc8271cb2491647f8283f20ac54d12161dff080e \
-    --hash=sha256:4b14d5e09c656de5038a3f9bfe5228f53439282abcab87317c9f7f1acb280352 \
-    --hash=sha256:51b236e764840a6df0661b67e50697aaa0e7d4124ca95e5058fa3d7cbc240b7c \
-    --hash=sha256:63ffd21aa133ff48c4dff7adcc46b7ec8b565491bfc371212122dd999812ea1c \
-    --hash=sha256:6a43c7823cd7427b4ed763aa7fb63901ca8288591323b58c9cd6ec31ad910f3c \
-    --hash=sha256:755e89e32376c850f826c425ece2c35a4fc266c081490eb0a841e7c1cb0d3bda \
-    --hash=sha256:7a726d742816cb3a8973c8c9a97539c734b3a309345236cd533c4883dda05b8d \
-    --hash=sha256:7c7c0d0827e853315c9bbd43c1162c006dd808dbbe297db7ae66cd17b07830f0 \
-    --hash=sha256:7ed681b0f8e8bcbbffa58ba26fcf5dbc8f79e7997595bf071ed5430d8c08d6f3 \
-    --hash=sha256:7ee5c9bb51695f80878faaa5598040dd6c9e172ddcf490382e8aedb8ec3fec8d \
-    --hash=sha256:8361be1c2c073919500b6601220a6f2f98ea0b6d2fec5014c1d9cfa23dd07038 \
-    --hash=sha256:8ae125d1134bf236acba8b83e74c603d1b30e207266121e76484562bc816344c \
-    --hash=sha256:9817733f0d3ea91bea80de0f79ef971ae94f81ca52f9b66500c6a2fea8e4b4f8 \
-    --hash=sha256:98b85dd86514d889a2e3dd22ab3c18c9d0019e696478391d86708b805f4ea0fa \
-    --hash=sha256:9ccb092c9ede70b2517a57382a601619d20981f56f440eae7e4d7eaafd1d1d09 \
-    --hash=sha256:9d58885215094ab4a86a6aef044e42994a2bd76a446dc59b352622655ba6621b \
-    --hash=sha256:b643cb30821e7570c0aaf54feaf0bfb630b79059f85741843e9dc23f33aaca2c \
-    --hash=sha256:bc7c85a150501286f8b56bd8ed3aa4093f4b88fb68c0843d21ff9656f0009d6a \
-    --hash=sha256:beeb129cacea34490ffd4d6153af70509aa3cda20fdda2ea1a2be870dfec8d52 \
-    --hash=sha256:c31b75ae466c053a98bf26843563b3b3517b8f37da4d47b1c582fdc703112bc3 \
-    --hash=sha256:c4e4881fa9e9667afcc742f0c244d9364d197490fbc91d12ac3b5de0bf2df146 \
-    --hash=sha256:c5b15ed7644ae4bee0ecf74fee95808dcc34ba6ace87e8dfbf5cb0dc20eab45a \
-    --hash=sha256:d12d076582507ea460ea2a89a8c85cb558f83406c8a41dd641d7be9a32e1274f \
-    --hash=sha256:d248cd4a92065a4d4543b8331660121b31c4148dd00a691bfb7a5cdc7483cfa4 \
-    --hash=sha256:d47dd659a4ee952e90dc56c97d78132573dc5c7b09d61b416a9deef4ebe01a0c \
-    --hash=sha256:d4a5a5879a939cb84959d86869132b00176197ca561c664fc21478c1eee60d75 \
-    --hash=sha256:da9b41d4539eefd408c46725fb76ecba3a50a3367cafb7dea5f250d0653c1040 \
-    --hash=sha256:db61a79c07331e88b9a9974815c075fbd812bc9dbc4dc44b366b5368a2936063 \
-    --hash=sha256:ddb726cb861c3117a553f940372a495fe1078249ff5f8a5478c0576c7be12050 \
-    --hash=sha256:ded59300d6330be27bc6cf0b74b89ada58069ced87c48eaf9344e5e84b0072f7 \
-    --hash=sha256:e2617759031dae1bf183c16cef8fcfb3de7617f394c813fa5e8e46e9b82d4222 \
-    --hash=sha256:e5cdbb5cafcedea04924568d990e20ce7f1945a1dd54b560f879ee2d57226912 \
-    --hash=sha256:ec8e767f13be637d056f7e07e61d089e555f719b387a7070154ad80a0ff31801 \
-    --hash=sha256:ef382417db92ba23dfb5864a3fc9be27ea4894e86620d342a116b243ade5d35d \
-    --hash=sha256:f2cba5c6db29ce991029b5e4ac51eb36774458f0a3b8d3137241b32d1bb91f06 \
-    --hash=sha256:f5b4198d85a3755d27e64c52f8c95d6333119e49fd001ae5798dac872c95e0f8 \
-    --hash=sha256:ffeeb38ee4a80a30a6877c5c4c359e5498eec095878f1581453202bfacc8fbc2
+coverage[toml]==7.2.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0339dc3237c0d31c3b574f19c57985fcbe494280153bbcad33f2cdf469f4ac3e \
+    --hash=sha256:09643fb0df8e29f7417adc3f40aaf379d071ee8f0350ab290517c7004f05360b \
+    --hash=sha256:0bd7e628f6c3ec4e7d2d24ec0e50aae4e5ae95ea644e849d92ae4805650b4c4e \
+    --hash=sha256:0cf557827be7eca1c38a2480484d706693e7bb1929e129785fe59ec155a59de6 \
+    --hash=sha256:0f8318ed0f3c376cfad8d3520f496946977abde080439d6689d7799791457454 \
+    --hash=sha256:1b7fb13850ecb29b62a447ac3516c777b0e7a09ecb0f4bb6718a8654c87dfc80 \
+    --hash=sha256:22c308bc508372576ffa3d2dbc4824bb70d28eeb4fcd79d4d1aed663a06630d0 \
+    --hash=sha256:3004765bca3acd9e015794e5c2f0c9a05587f5e698127ff95e9cfba0d3f29339 \
+    --hash=sha256:3a209d512d157379cc9ab697cbdbb4cfd18daa3e7eebaa84c3d20b6af0037384 \
+    --hash=sha256:436313d129db7cf5b4ac355dd2bd3f7c7e5294af077b090b85de75f8458b8616 \
+    --hash=sha256:49567ec91fc5e0b15356da07a2feabb421d62f52a9fff4b1ec40e9e19772f5f8 \
+    --hash=sha256:4dd34a935de268a133e4741827ae951283a28c0125ddcdbcbba41c4b98f2dfef \
+    --hash=sha256:570c21a29493b350f591a4b04c158ce1601e8d18bdcd21db136fbb135d75efa6 \
+    --hash=sha256:5928b85416a388dd557ddc006425b0c37e8468bd1c3dc118c1a3de42f59e2a54 \
+    --hash=sha256:5d2b9b5e70a21474c105a133ba227c61bc95f2ac3b66861143ce39a5ea4b3f84 \
+    --hash=sha256:617a94ada56bbfe547aa8d1b1a2b8299e2ec1ba14aac1d4b26a9f7d6158e1273 \
+    --hash=sha256:6a034480e9ebd4e83d1aa0453fd78986414b5d237aea89a8fdc35d330aa13bae \
+    --hash=sha256:6fce673f79a0e017a4dc35e18dc7bb90bf6d307c67a11ad5e61ca8d42b87cbff \
+    --hash=sha256:78d2c3dde4c0b9be4b02067185136b7ee4681978228ad5ec1278fa74f5ca3e99 \
+    --hash=sha256:7f099da6958ddfa2ed84bddea7515cb248583292e16bb9231d151cd528eab657 \
+    --hash=sha256:80559eaf6c15ce3da10edb7977a1548b393db36cbc6cf417633eca05d84dd1ed \
+    --hash=sha256:834c2172edff5a08d78e2f53cf5e7164aacabeb66b369f76e7bb367ca4e2d993 \
+    --hash=sha256:861cc85dfbf55a7a768443d90a07e0ac5207704a9f97a8eb753292a7fcbdfcfc \
+    --hash=sha256:8649371570551d2fd7dee22cfbf0b61f1747cdfb2b7587bb551e4beaaa44cb97 \
+    --hash=sha256:87dc37f16fb5e3a28429e094145bf7c1753e32bb50f662722e378c5851f7fdc6 \
+    --hash=sha256:8a6450da4c7afc4534305b2b7d8650131e130610cea448ff240b6ab73d7eab63 \
+    --hash=sha256:8d3843ca645f62c426c3d272902b9de90558e9886f15ddf5efe757b12dd376f5 \
+    --hash=sha256:8dca3c1706670297851bca1acff9618455122246bdae623be31eca744ade05ec \
+    --hash=sha256:97a3189e019d27e914ecf5c5247ea9f13261d22c3bb0cfcfd2a9b179bb36f8b1 \
+    --hash=sha256:99f4dd81b2bb8fc67c3da68b1f5ee1650aca06faa585cbc6818dbf67893c6d58 \
+    --hash=sha256:9e872b082b32065ac2834149dc0adc2a2e6d8203080501e1e3c3c77851b466f9 \
+    --hash=sha256:a81dbcf6c6c877986083d00b834ac1e84b375220207a059ad45d12f6e518a4e3 \
+    --hash=sha256:abacd0a738e71b20e224861bc87e819ef46fedba2fb01bc1af83dfd122e9c319 \
+    --hash=sha256:ae82c988954722fa07ec5045c57b6d55bc1a0890defb57cf4a712ced65b26ddd \
+    --hash=sha256:b0c0d46de5dd97f6c2d1b560bf0fcf0215658097b604f1840365296302a9d1fb \
+    --hash=sha256:b1991a6d64231a3e5bbe3099fb0dd7c9aeaa4275ad0e0aeff4cb9ef885c62ba2 \
+    --hash=sha256:b2167d116309f564af56f9aa5e75ef710ef871c5f9b313a83050035097b56820 \
+    --hash=sha256:bd5a12239c0006252244f94863f1c518ac256160cd316ea5c47fb1a11b25889a \
+    --hash=sha256:bdd3f2f285ddcf2e75174248b2406189261a79e7fedee2ceeadc76219b6faa0e \
+    --hash=sha256:c77f2a9093ccf329dd523a9b2b3c854c20d2a3d968b6def3b820272ca6732242 \
+    --hash=sha256:cb5f152fb14857cbe7f3e8c9a5d98979c4c66319a33cad6e617f0067c9accdc4 \
+    --hash=sha256:cca7c0b7f5881dfe0291ef09ba7bb1582cb92ab0aeffd8afb00c700bf692415a \
+    --hash=sha256:d2ef6cae70168815ed91388948b5f4fcc69681480a0061114db737f957719f03 \
+    --hash=sha256:d9256d4c60c4bbfec92721b51579c50f9e5062c21c12bec56b55292464873508 \
+    --hash=sha256:e191a63a05851f8bce77bc875e75457f9b01d42843f8bd7feed2fc26bbe60833 \
+    --hash=sha256:e2b50ebc2b6121edf352336d503357321b9d8738bb7a72d06fc56153fd3f4cd8 \
+    --hash=sha256:e3ea04b23b114572b98a88c85379e9e9ae031272ba1fb9b532aa934c621626d4 \
+    --hash=sha256:e4d70c853f0546855f027890b77854508bdb4d6a81242a9d804482e667fff6e6 \
+    --hash=sha256:f29351393eb05e6326f044a7b45ed8e38cb4dcc38570d12791f271399dc41431 \
+    --hash=sha256:f3d07edb912a978915576a776756069dede66d012baa503022d3a0adba1b6afa \
+    --hash=sha256:fac6343bae03b176e9b58104a9810df3cdccd5cfed19f99adfa807ffbf43cf9b
 exceptiongroup==1.1.0 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e \
     --hash=sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23
 iniconfig==2.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
 packaging==23.0 ; python_version >= "3.9" and python_version < "4.0" \
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/base-requirements/type-checking.txt` & `hikari-yuyo-1.9.1a1/piped/python/base-requirements/type-checking.txt`

 * *Files 10% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     --hash=sha256:e60d0b09f62ae97a94605c3f73fd952395286cf3e3b9e7b97f60b01ddfbbda88 \
     --hash=sha256:e64f48c6176e243ad015e995de05af7f22bbe370dbb5b32bd6988438ec873919 \
     --hash=sha256:e831662208055b006eef68392a768ff83596035ffd6d846786578ba1714ba8f6 \
     --hash=sha256:eda5c8b9949ed411ff752b9a01adda31afe7eae1e53e946dbdf9db23865e66c4
 nodeenv==1.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e \
     --hash=sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b
-pyright==1.1.294 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5b27e28a1cfc60cea707fd3b644769fa6dd0b194481cdcc2399cf2a51cc5a846 \
-    --hash=sha256:fea5fed3d6a3f02259e622c901e86a7b8bcf237d35e1cdfe01d0e0723768dcb6
-setuptools==67.3.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9d3de8591bd6f6522594406fa46a6418eabd0562dacb267f8556675762801514 \
-    --hash=sha256:ed4e75fafe103c79b692f217158ba87edf38d31004b9dbc1913debb48793c828
+pyright==1.1.296 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:51cc5f05807b1fb53f9f0e14736b8f772b500a3ba4e0edeb99727e68e700d9ea \
+    --hash=sha256:6c3cd394473e55a516ebe443d02b83e63456ef29f052dcf8e64e7875c1418fa6
+setuptools==67.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:e5fd0a713141a4a105412233c63dc4e17ba0090c8e8334594ac790ec97792330 \
+    --hash=sha256:f106dee1b506dee5102cc3f3e9e68137bbad6d47b616be7991714b0c62204251
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
 typing-extensions==4.5.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
```

### Comparing `hikari-yuyo-1.9.0a1/piped/python/noxfile.py` & `hikari-yuyo-1.9.1a1/piped/python/noxfile.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/python/noxfile.template.py` & `hikari-yuyo-1.9.1a1/piped/python/noxfile.template.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/piped/python/piped_shared/__init__.py` & `hikari-yuyo-1.9.1a1/piped/python/piped_shared/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/pyproject.toml` & `hikari-yuyo-1.9.1a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.3,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "hikari-yuyo"
-version = "1.9.0a1"
+version = "1.9.1a1"
 readme = "README.md"
 requires-python = ">=3.9.0,<3.12"
 license = {file = "LICENSE"}
 authors = [ {name = "Faster Speeding", email="lucina@lmbyrne.dev"} ]
 keywords= ["hikari"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -166,17 +166,27 @@
 [tool.piped.github_actions.verify_types]
 
 [tool.pyright]
 include = ["examples", "noxfile.py", "tests", "yuyo"]
 
 pythonVersion = "3.9"
 typeCheckingMode = "strict"
-reportMissingModuleSource = "error"
-reportMissingTypeStubs = "error"
+reportMissingModuleSource = "error"  # Is only "warning" on strict mode.
 
+# Error code which are disabled even when general strict.
+reportShadowedImports = "error"
+reportCallInDefaultInitializer = "none"  # Ended up just complaining about cases where this was fine (e.g. timedeltas).
+reportImplicitStringConcatenation = "none"  # Conflicts with flake8 config.
+reportMissingSuperCall = "none"  # Way too strict (requires calls to `object.__init__`).
+reportPropertyTypeMismatch = "error"
+reportUninitializedInstanceVariable = "error"
+reportUnnecessaryTypeIgnoreComment = "error"
+reportUnusedCallResult = "none"  # Enforces doing `_ = ...`.
+
+# Error codes which lead to too many false-positives.
 reportIncompatibleMethodOverride = "warning"    # This relies on ordering for key-word only arguments
                                                 # which is more annoying than it's worth
 reportUnknownMemberType = "warning"             # This messes with instance checking generic objects
 reportUnknownArgumentType = "warning"           # Pretty much the same as reportUnknownMemberType
 reportUnknownLambdaType = "warning"
 reportImportCycles = "warning"                  # This isn't necessarily an issue if it's type checking only.
 reportUnknownVariableType = "warning"           # Lotta false-positives, might fix/change later.
```

### Comparing `hikari-yuyo-1.9.0a1/tests/__init__.py` & `hikari-yuyo-1.9.1a1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test__internal.py` & `hikari-yuyo-1.9.1a1/tests/test__internal.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_asgi.py` & `hikari-yuyo-1.9.1a1/tests/test_asgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1186,15 +1186,15 @@
                 max_retries=3,
             )
 
         assert bot.proxy_settings is mock_settings
 
     def test_rest_property(self):
         with mock.patch.object(hikari.impl, "RESTClientImpl") as mock_rest_client_impl:
-            bot = yuyo.AsgiBot("token", "Bot")
+            bot = yuyo.AsgiBot("token")
 
             mock_rest_client_impl.assert_called_once_with(  # noqa: S106
                 cache=None,
                 entity_factory=bot.entity_factory,
                 executor=None,
                 http_settings=bot.http_settings,
                 max_rate_limit=300.0,
```

### Comparing `hikari-yuyo-1.9.0a1/tests/test_chunk_tracker.py` & `hikari-yuyo-1.9.1a1/tests/test_chunk_tracker.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_components.py` & `hikari-yuyo-1.9.1a1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_links.py` & `hikari-yuyo-1.9.1a1/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_list_status.py` & `hikari-yuyo-1.9.1a1/tests/test_list_status.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_modals.py` & `hikari-yuyo-1.9.1a1/tests/test_modals.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_pagination.py` & `hikari-yuyo-1.9.1a1/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_reactions.py` & `hikari-yuyo-1.9.1a1/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/tests/test_to_builder.py` & `hikari-yuyo-1.9.1a1/tests/test_to_builder.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/__init__.py` & `hikari-yuyo-1.9.1a1/yuyo/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/_internal.py` & `hikari-yuyo-1.9.1a1/yuyo/_internal.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/asgi.py` & `hikari-yuyo-1.9.1a1/yuyo/asgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
     ) -> None:
         ...
 
     @typing.overload
     def __init__(
         self,
         token: str,
-        token_type: typing.Union[str, hikari.TokenType],
+        token_type: typing.Union[str, hikari.TokenType] = hikari.TokenType.BOT,
         public_key: typing.Union[bytes, str, None] = None,
         *,
         asgi_managed: bool = True,
         executor: typing.Optional[concurrent.futures.Executor] = None,
         http_settings: typing.Optional[hikari.impl.HTTPSettings] = None,
         max_body_size: int = 1024**2,
         max_rate_limit: float = 300.0,
@@ -544,15 +544,15 @@
         ----------
         token
             The bot or bearer token. If no token is to be used,
             this can be undefined.
         token_type
             The type of token in use. This should only be passed when `str`
             is passed for `token`, can be `"Bot"` or `"Bearer"` and will be
-            defaulted to `"Bearer"` in this situation.
+            defaulted to `"Bot"` in this situation.
 
             This should be left as [None][] when either
             [hikari.api.rest.TokenStrategy][] or [None][] is passed for
             `token`.
         asgi_managed
             Whether this bot's internal components should be automatically
             started and stopped based on the Asgi lifespan events.
@@ -613,14 +613,20 @@
         ValueError
             * If `token_type` is provided when a token strategy is passed for `token`.
             * if `token_type` is left as [None][] when a string is passed for `token`.
         """
         if isinstance(public_key, str):
             public_key = bytes.fromhex(public_key)
 
+        if isinstance(token, str):
+            token = token.strip()
+
+            if token_type is None:
+                token_type = hikari.TokenType.BOT
+
         self._entity_factory = hikari.impl.EntityFactoryImpl(self)
         self._executor = executor
         self._http_settings = http_settings or hikari.impl.HTTPSettings()
         self._is_alive = False
         self._join_event: typing.Optional[asyncio.Event] = None
         self._on_shutdown: dict[
             collections.Callable[[Self], collections.Coroutine[typing.Any, typing.Any, typing.Any]],
```

### Comparing `hikari-yuyo-1.9.0a1/yuyo/backoff.py` & `hikari-yuyo-1.9.1a1/yuyo/backoff.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/chunk_tracker.py` & `hikari-yuyo-1.9.1a1/yuyo/chunk_tracker.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/components.py` & `hikari-yuyo-1.9.1a1/yuyo/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -2313,14 +2313,18 @@
         For buttons the limit is 5. For other sub-components the limit is 1.
         """
         if self._components and isinstance(self._components[0], hikari.api.ButtonBuilder):
             return len(self._components) >= 5
 
         return bool(self._components)
 
+    @property
+    def type(self) -> typing.Literal[hikari.ComponentType.ACTION_ROW]:
+        return hikari.ComponentType.ACTION_ROW
+
     def _assert_can_add_type(self, type_: hikari.ComponentType, /) -> Self:
         if self._stored_type is not None and self._stored_type != type_:
             raise ValueError(f"{type_} component type cannot be added to a container which already holds {type_}")
 
         self._stored_type = type_
         return self
 
@@ -2519,14 +2523,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         Self
             The action row to enable chained calls.
         """
         if custom_id is None:
@@ -2575,14 +2581,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         Self
             The action row to enable chained calls.
         """
         if custom_id is None:
@@ -2625,14 +2633,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         hikari.api.special_endpoints.TextSelectMenuBuilder
             Builder for the added text select menu.
 
             [TextSelectMenuBuilder.add_option][hikari.api.special_endpoints.TextSelectMenuBuilder.add_option]
@@ -3093,14 +3103,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         Self
             The action column to enable chained calls.
         """
         _append_row(self._rows).add_select_menu(
@@ -3143,14 +3155,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         type[Self]
             The action column class to enable chained calls.
 
         Raises
@@ -3202,14 +3216,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         CallbackSig
             The decorated callback.
 
         Raises
@@ -3259,14 +3275,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         Self
             The action column to enable chained calls.
         """
         _append_row(self._rows).add_channel_select(
@@ -3307,14 +3325,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         type[Self]
             The action column class to enable chained calls.
 
         Raises
@@ -3364,14 +3384,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         CallbackSig
             The decorated callback.
 
         Raises
@@ -3416,14 +3438,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         hikari.api.special_endpoints.TextSelectMenuBuilder
             Builder for the added text select menu.
 
             [TextSelectMenuBuilder.add_option][hikari.api.special_endpoints.TextSelectMenuBuilder.add_option]
@@ -3463,14 +3487,16 @@
             The select menu's custom ID.
         placeholder
             Placeholder text to show when no entries have been selected.
         min_values
             The minimum amount of entries which need to be selected.
         max_values
             The maximum amount of entries which can be selected.
+        is_disabled
+            Whether this select menu should be marked as disabled.
 
         Returns
         -------
         hikari.api.special_endpoints.TextSelectMenuBuilder
             Builder for the added text select menu.
 
             [TextSelectMenuBuilder.add_option][hikari.api.special_endpoints.TextSelectMenuBuilder.add_option]
@@ -3619,14 +3645,16 @@
         The select menu's custom ID.
     placeholder
         Placeholder text to show when no entries have been selected.
     min_values
         The minimum amount of entries which need to be selected.
     max_values
         The maximum amount of entries which can be selected.
+    is_disabled
+        Whether this select menu should be marked as disabled.
 
     Returns
     -------
     type[Self]
         The decorated action column class.
     """
     return lambda executor: executor.add_static_select_menu(
@@ -3665,14 +3693,16 @@
         The select menu's custom ID.
     placeholder
         Placeholder text to show when no entries have been selected.
     min_values
         The minimum amount of entries which need to be selected.
     max_values
         The maximum amount of entries which can be selected.
+    is_disabled
+        Whether this select menu should be marked as disabled.
 
     Returns
     -------
     type[Self]
         The decorated action column class.
     """
     return lambda executor: executor.add_static_channel_select(
```

### Comparing `hikari-yuyo-1.9.0a1/yuyo/links.py` & `hikari-yuyo-1.9.1a1/yuyo/links.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/list_status.py` & `hikari-yuyo-1.9.1a1/yuyo/list_status.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/modals.py` & `hikari-yuyo-1.9.1a1/yuyo/modals.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,28 +57,29 @@
 import hikari
 import typing_extensions
 
 from . import _internal
 from . import components as components_
 
 _P = typing_extensions.ParamSpec("_P")
+_T = typing.TypeVar("_T")
 
 if typing.TYPE_CHECKING:
     import types
 
     import tanjun
     from typing_extensions import Self
 
-    _T = typing.TypeVar("_T")
     _ModalT = typing.TypeVar("_ModalT", bound="Modal")
-    _CoroT = collections.Coroutine[typing.Any, typing.Any, _T]
     __SelfishSig = typing_extensions.Concatenate[_T, _P]
     _SelfishSig = __SelfishSig[_T, ...]
 
 
+_CoroT = collections.Coroutine[typing.Any, typing.Any, _T]
+
 _ModalResponseT = typing.Union[hikari.api.InteractionMessageBuilder, hikari.api.InteractionDeferredBuilder]
 """Type hint of the builder response types allows for modal interactions."""
 
 
 class _NoDefaultEnum(enum.Enum):
     VALUE = object()
 
@@ -1222,15 +1223,18 @@
         for field in self._tracked_fields:
             if field.prefix_match:
                 component = compiled_prefixes.get(field.custom_id)
 
             else:
                 component = components.get(field.custom_id)
 
-            if not component:
+            # Discord still provides text components when no input was given just with
+            # an empty string for `value` but we also want to support possible future
+            # cases where they just just don't provide the component.
+            if not component or not component.value:
                 if field.default is NO_DEFAULT:
                     raise RuntimeError(f"Missing required component `{field.custom_id}`")
 
                 fields[field.parameter] = field.default
                 continue
 
             if component.type is not field.type:
```

### Comparing `hikari-yuyo-1.9.0a1/yuyo/pagination.py` & `hikari-yuyo-1.9.1a1/yuyo/pagination.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/yuyo/reactions.py` & `hikari-yuyo-1.9.1a1/yuyo/reactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,23 @@
 if typing.TYPE_CHECKING:
     import tanjun
     from hikari.api import event_manager as event_manager_api
     from typing_extensions import Self
 
     _CallbackSigT = typing.TypeVar("_CallbackSigT", bound="CallbackSig")
     _EventT = typing.TypeVar("_EventT", bound=hikari.Event)
-    _ReactionEventT = typing.Union[hikari.ReactionAddEvent, hikari.ReactionDeleteEvent]
 
     # This doesn't enforce ShardAware (unlike yuyo._internal.GatewayBotProto)
     class _GatewayBotProto(hikari.EventManagerAware, hikari.RESTAware, typing.Protocol):
         """Protocol of a cacheless Hikari Gateway bot."""
 
 
+ReactionEventT = typing.Union[hikari.ReactionAddEvent, hikari.ReactionDeleteEvent]
+"""Type hint of the event types [CallbackSig][yuyo.reactions.CallbackSig] takes as its first argument."""
+
 CallbackSig = collections.Callable[..., collections.Coroutine[typing.Any, typing.Any, None]]
 """Type-hint of a callback used to handle matching reactions events."""
 
 
 class HandlerClosed(Exception):
     """Error raised when a reaction handler has been closed."""
 
@@ -90,15 +92,15 @@
         ----------
         message
             The message to bind this handler to.
         """
 
     @abc.abstractmethod
     async def on_reaction_event(
-        self, event: _ReactionEventT, /, *, alluka: typing.Optional[alluka_.abc.Client] = None
+        self, event: ReactionEventT, /, *, alluka: typing.Optional[alluka_.abc.Client] = None
     ) -> None:
         """Handle a reaction event.
 
         Parameters
         ----------
         event
             The event to handle.
@@ -234,15 +236,15 @@
 
             self.set_callback(emoji_identifier, callback)
             return callback
 
         return decorator
 
     async def on_reaction_event(
-        self, event: _ReactionEventT, /, *, alluka: typing.Optional[alluka_.abc.Client] = None
+        self, event: ReactionEventT, /, *, alluka: typing.Optional[alluka_.abc.Client] = None
     ) -> None:
         # <<inherited docstring from AbstractReactionHandler>>.
         if self.has_expired:
             asyncio.create_task(self.close())
             raise
 
         if self._message is None or self._authors and event.user_id not in self._authors:
@@ -492,28 +494,28 @@
 
         try:
             await self._message.edit(**response.to_kwargs())
 
         except (hikari.NotFoundError, hikari.ForbiddenError) as exc:
             raise HandlerClosed() from exc
 
-    async def _on_disable(self, _: _ReactionEventT, /) -> None:
+    async def _on_disable(self, _: ReactionEventT, /) -> None:
         if message := self._message:
             self._message = None
             # We create a task here rather than awaiting this to ensure the instance is marked as ended as soon as
             # possible.
             asyncio.create_task(message.delete())
 
         raise HandlerClosed
 
-    async def _on_first(self, _: _ReactionEventT, /) -> None:
+    async def _on_first(self, _: ReactionEventT, /) -> None:
         if self._index != 0 and (first_entry := self._buffer[0] if self._buffer else await self.get_next_entry()):
             await self._edit_message(first_entry)
 
-    async def _on_last(self, _: _ReactionEventT, /) -> None:
+    async def _on_last(self, _: ReactionEventT, /) -> None:
         if self._iterator:
             self._buffer.extend(map(pagination.Page.from_entry, await _internal.collect_iterable(self._iterator)))
 
         if self._buffer:
             self._index = len(self._buffer) - 1
             await self._edit_message(self._buffer[-1])
 
@@ -535,19 +537,19 @@
             entry = pagination.Page.from_entry(entry)
             self._index += 1
             self._buffer.append(entry)
             return entry
 
         return None  # MyPy
 
-    async def _on_next(self, _: _ReactionEventT, /) -> None:
+    async def _on_next(self, _: ReactionEventT, /) -> None:
         if entry := await self.get_next_entry():
             await self._edit_message(entry)
 
-    async def _on_previous(self, _: _ReactionEventT, /) -> None:
+    async def _on_previous(self, _: ReactionEventT, /) -> None:
         if self._index > 0:
             self._index -= 1
             await self._edit_message(self._buffer[self._index])
 
     def add_author(self, user: hikari.SnowflakeishOr[hikari.User], /) -> Self:
         """Add a author/owner to this handler.
 
@@ -831,30 +833,28 @@
         await self.close()
 
     @property
     def is_closed(self) -> bool:
         """Whether this client is closed."""
         return self._gc_task is None
 
-    def set_handler(
-        self, message: hikari.SnowflakeishOr[hikari.Message], paginator: AbstractReactionHandler, /
-    ) -> Self:
+    def set_handler(self, message: hikari.SnowflakeishOr[hikari.Message], handler: AbstractReactionHandler, /) -> Self:
         """Add a reaction handler to this reaction client.
 
         !!! note
             This does not call [yuyo.reactions.AbstractReactionHandler.open][].
 
         Parameters
         ----------
         message
             The message ID to add register a reaction handler with.
-        paginator
-            The object of the opened paginator to register in this reaction client.
+        handler
+            The object of the opened handler to register in this reaction client.
         """
-        self._handlers[hikari.Snowflake(message)] = paginator
+        self._handlers[hikari.Snowflake(message)] = handler
         return self
 
     def get_handler(
         self, message: hikari.SnowflakeishOr[hikari.Message], /
     ) -> typing.Optional[AbstractReactionHandler]:
         """Get a reference to a paginator registered in this reaction client.
```

### Comparing `hikari-yuyo-1.9.0a1/yuyo/to_builder.py` & `hikari-yuyo-1.9.1a1/yuyo/to_builder.py`

 * *Files identical despite different names*

### Comparing `hikari-yuyo-1.9.0a1/PKG-INFO` & `hikari-yuyo-1.9.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-yuyo
-Version: 1.9.0a1
+Version: 1.9.1a1
 Summary: A collection of utility functions and classes designed to expand Hikari.
 Keywords: hikari
 Author-email: Faster Speeding <lucina@lmbyrne.dev>
 Requires-Python: >=3.9.0,<3.12
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

