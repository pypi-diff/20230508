# Comparing `tmp/cercis-0.1.3.tar.gz` & `tmp/cercis-0.1.4.tar.gz`

## Comparing `cercis-0.1.3.tar` & `cercis-0.1.4.tar`

### file list

```diff
@@ -1,305 +1,307 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.3/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.3/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.3/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.3/.gitattributes
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.3/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.3/.prettierrc.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.3/.readthedocs.yaml
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cercis-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.3/Dockerfile
--rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 cercis-0.1.3/README.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.3/action.yml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.3/mypy.ini
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.3/test_requirements.txt
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.3/tox.ini
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/ISSUE_TEMPLATE/docs-issue.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/ISSUE_TEMPLATE/style_issue.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/check-changelog.yml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/upload_binary.yml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.3/.github/workflows/version-check.yml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.3/action/main.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.3/autoload/black.vim
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.3/gallery/Dockerfile
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.3/gallery/README.md
--rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.3/gallery/gallery.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.3/plugin/black.vim
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.3/scripts/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/scripts/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.3/scripts/check_version_and_changelog.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.3/scripts/diff_shades_gha_helper.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.3/scripts/fuzz.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.3/scripts/make_width_table.py
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.3/scripts/migrate-black.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.3/src/_cercis_version.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blackd/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blackd/__main__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blackd/middlewares.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/Grammar.txt
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/PatternGrammar.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/README
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/__init__.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pygram.py
--rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pytree.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/__init__.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/conv.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/driver.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/grammar.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/literals.py
--rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/parse.py
--rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/pgen.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/token.py
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.3/src/blib2to3/pgen2/tokenize.py
--rw-r--r--   0        0        0    49104 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/__main__.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/_width_table.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/brackets.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/cache.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/comments.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/concurrency.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/const.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/debug.py
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/files.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/handle_ipynb_magics.py
--rw-r--r--   0        0        0    62207 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/linegen.py
--rw-r--r--   0        0        0    38672 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/lines.py
--rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/mode.py
--rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/numerics.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/output.py
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/py.typed
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/rusty.py
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/strings.py
--rw-r--r--   0        0        0    91688 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/trans.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/utils_line_wrapping.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.3/src/cercis/utils_linegen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/optional.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test.toml
--rw-r--r--   0        0        0   101263 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test_black.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test_blackd.py
--rw-r--r--   0        0        0    11625 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test_format.py
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test_ipynb.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test_trans.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/test_utils_line_wrapping.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/edge_cases.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
--rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/pragma_comments/Black_default.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/pragma_comments/Cercis_default.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/single_quote/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/single_quote/docstring_preview.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/single_quote/more_quotes.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/single_quote/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/configurable_cases/single_quote/torture.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.3/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.3/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.3/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.3/LICENSE_ORIGINAL
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 cercis-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    17093 2020-02-02 00:00:00.000000 cercis-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.4/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.4/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.4/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.4/.gitattributes
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.4/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.4/.prettierrc.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 cercis-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.4/Dockerfile
+-rw-r--r--   0        0        0    15433 2020-02-02 00:00:00.000000 cercis-0.1.4/README.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.4/action.yml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.4/mypy.ini
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.4/test_requirements.txt
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.4/tox.ini
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/docs-issue.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/style_issue.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/check-changelog.yml
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/upload_binary.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/version-check.yml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.4/action/main.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.4/autoload/black.vim
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.4/gallery/Dockerfile
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.4/gallery/README.md
+-rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.4/gallery/gallery.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.4/plugin/black.vim
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/check_version_and_changelog.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/fuzz.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/migrate-black.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.4/src/_cercis_version.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blackd/middlewares.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/Grammar.txt
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/PatternGrammar.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/README
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0    49574 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/__main__.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/_width_table.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/brackets.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/cache.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/comments.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/concurrency.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/const.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/debug.py
+-rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/files.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/handle_ipynb_magics.py
+-rw-r--r--   0        0        0    62321 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/linegen.py
+-rw-r--r--   0        0        0    38672 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/lines.py
+-rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/mode.py
+-rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/numerics.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/output.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/py.typed
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/rusty.py
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/strings.py
+-rw-r--r--   0        0        0    91688 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/trans.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/utils_line_wrapping.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/utils_linegen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/optional.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test.toml
+-rw-r--r--   0        0        0   101263 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_black.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_blackd.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_format.py
+-rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_trans.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_utils_line_wrapping.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/edge_cases.py
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
+-rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Black_default.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Cercis_default.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring_preview.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/more_quotes.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/torture.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.4/LICENSE_ORIGINAL
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 cercis-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    18951 2020-02-02 00:00:00.000000 cercis-0.1.4/PKG-INFO
```

### Comparing `cercis-0.1.3/.pre-commit-config.yaml` & `cercis-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.pre-commit-hooks.yaml` & `cercis-0.1.4/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/CHANGELOG.md` & `cercis-0.1.4/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # Change Log
 
+## [0.1.4] - 2023-05-07
+
+- Added
+  - A new configurable option: `--closing-bracket-extra-indent`
+
 ## [0.1.3] - 2023-05-07
 
 - Added
+
   - A new configurable option: `--collapse-nested-brackets`
   - A new configurable option: `--wrap-pragma-comments`
   - Some Github workflow actions to make sure CHANGELOG.md is updated
 
 - Changed
+
   - Changed the default quote to single quote
   - Changed the default line length to 79 characters
 
 - Removed
   - Some unrelated documentation and config files
 
 ## [0.1.2] - 2023-05-04
```

### Comparing `cercis-0.1.3/Dockerfile` & `cercis-0.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/README.md` & `cercis-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,17 +85,18 @@
 Black doesn't. Configurability is our main motivation behind creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 1. [Line length](#31-line-length)
 2. [Single quote vs double quote](#32-single-quote-vs-double-quote)
 3. [Extra indentation at function definition](#33-extra-indentation-at-function-definition)
-4. ["Simple" lines with long strings](#34-simple-lines-with-long-strings)
-5. [Collapse nested brackets](#35-collapse-nested-brackets)
-6. [Wrap pragma comments](#36-wrapping-long-lines-ending-with-pragma-comments)
+4. [Extra indentation at closing brackets](#34-closing-bracket-indentation)
+5. ["Simple" lines with long strings](#35-simple-lines-with-long-strings)
+6. [Collapse nested brackets](#36-collapse-nested-brackets)
+7. [Wrap pragma comments](#37-wrapping-long-lines-ending-with-pragma-comments)
 
 The next section ([How to configure _Cercis_](#4-how-to-configure-cercis))
 contains detailed instructions of how to configure these options.
 
 ### 3.1. Line length
 
 _Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's
@@ -180,15 +181,94 @@
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Black's default        | `False`                                                         |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
-### 3.4. "Simple" lines with long strings
+## 3.4. Closing bracket indentation
+
+This option lets people customize where the closing bracket should be. Note
+that both styles are OK according to
+[PEP8](https://peps.python.org/pep-0008/#indentation).
+
+<table>
+  <tr>
+    <td>
+
+```python
+# --closing-bracket-extra-indent=False
+
+def function(
+        arg1: int,
+        arg2: float,
+        arg3_with_long_name: list,
+) -> None:
+    print('Hello world')
+
+
+result = func2(
+    12345,
+    3.1415926,
+    [1, 2, 3],
+)
+
+
+something = {
+    'a': 1,
+    'b': 2,
+    'c': 3,
+}
+```
+
+  </td>
+
+  <td>
+
+```python
+# --closing-bracket-extra-indent=True
+
+def function(
+        arg1: int,
+        arg2: float,
+        arg3_with_long_name: list,
+        ) -> None:
+    print('Hello world')
+
+
+result = func2(
+    12345,
+    3.1415926,
+    [1, 2, 3],
+    )
+
+
+something = {
+    'a': 1,
+    'b': 2,
+    'c': 3,
+    }
+```
+
+  </td>
+
+  </tr>
+</table>
+
+| Option                 |                                                             |
+| ---------------------- | ----------------------------------------------------------- |
+| Name                   | `--closing-bracket-extra-indent`                            |
+| Abbreviation           | `-cbei`                                                     |
+| Default                | `False`                                                     |
+| Black's default        | `False`                                                     |
+| Command line usage     | `cercis -cbei=True myScript.py`                             |
+| `pyproject.toml` usage | `closing-bracket-extra-indent = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--closing-bracket-extra-indent=False]`              |
+
+### 3.5. "Simple" lines with long strings
 
 By default, Black wraps lines that exceed length limit. But for very simple
 lines (such as assigning a long string to a variable), line wrapping is not
 necessary.
 
 <table>
   <tr>
@@ -247,15 +327,15 @@
 | Abbreviation           | `-wl`                                                     |
 | Default                | `False`                                                   |
 | Black's default        | `True`                                                    |
 | Command line usage     | `cercis -wl=True myScript.py`                             |
 | `pyproject.toml` usage | `wrap-line-with-long-string = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--wrap-line-with-long-string=False]`              |
 
-### 3.5. Collapse nested brackets
+### 3.6. Collapse nested brackets
 
 _Cercis_ by default collapses nested brackets to make the code more compact.
 
 <table>
   <tr>
     <td>
 
@@ -323,15 +403,15 @@
 | Command line usage     | `cercis -cnb=True myScript.py`                          |
 | `pyproject.toml` usage | `collapse-nested-brackets = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--collapse-nested-brackets=False]`              |
 
 The code implementation of this option comes from
 [Pyink](https://github.com/google/pyink), another forked project from Black.
 
-### 3.6. Wrapping long lines ending with pragma comments [^](#3-cerciss-code-style)
+### 3.7. Wrapping long lines ending with pragma comments [^](#3-cerciss-code-style)
 
 "Pragma comments", in this context, mean the directives for Python linters
 usually to tell them to ignore certain errors. Pragma comments that _Cercis_
 currently recognizes include:
 
 - _noqa_: `# noqa: E501`
 - _type: ignore_: `# type: ignore[no-untyped-def]`
```

### Comparing `cercis-0.1.3/action.yml` & `cercis-0.1.4/action.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/mypy.ini` & `cercis-0.1.4/mypy.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tox.ini` & `cercis-0.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/PULL_REQUEST_TEMPLATE.md` & `cercis-0.1.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/dependabot.yml` & `cercis-0.1.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `cercis-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/ISSUE_TEMPLATE/config.yml` & `cercis-0.1.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/ISSUE_TEMPLATE/docs-issue.md` & `cercis-0.1.4/.github/ISSUE_TEMPLATE/docs-issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `cercis-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/ISSUE_TEMPLATE/style_issue.md` & `cercis-0.1.4/.github/ISSUE_TEMPLATE/style_issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/check-changelog.yml` & `cercis-0.1.4/.github/workflows/check-changelog.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/docker.yml` & `cercis-0.1.4/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/fuzz.yml` & `cercis-0.1.4/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/lint.yml` & `cercis-0.1.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/python-package.yml` & `cercis-0.1.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/python-publish.yml` & `cercis-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/test.yml` & `cercis-0.1.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/upload_binary.yml` & `cercis-0.1.4/.github/workflows/upload_binary.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/.github/workflows/version-check.yml` & `cercis-0.1.4/.github/workflows/version-check.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/action/main.py` & `cercis-0.1.4/action/main.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/autoload/black.vim` & `cercis-0.1.4/autoload/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/gallery/README.md` & `cercis-0.1.4/gallery/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/gallery/gallery.py` & `cercis-0.1.4/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/plugin/black.vim` & `cercis-0.1.4/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/scripts/check_version_and_changelog.py` & `cercis-0.1.4/scripts/check_version_and_changelog.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/scripts/diff_shades_gha_helper.py` & `cercis-0.1.4/scripts/diff_shades_gha_helper.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/scripts/fuzz.py` & `cercis-0.1.4/scripts/fuzz.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/scripts/make_width_table.py` & `cercis-0.1.4/scripts/make_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/scripts/migrate-black.py` & `cercis-0.1.4/scripts/migrate-black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blackd/__init__.py` & `cercis-0.1.4/src/blackd/__init__.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blackd/middlewares.py` & `cercis-0.1.4/src/blackd/middlewares.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/Grammar.txt` & `cercis-0.1.4/src/blib2to3/Grammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/LICENSE` & `cercis-0.1.4/src/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/PatternGrammar.txt` & `cercis-0.1.4/src/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/README` & `cercis-0.1.4/src/blib2to3/README`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pygram.py` & `cercis-0.1.4/src/blib2to3/pygram.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pytree.py` & `cercis-0.1.4/src/blib2to3/pytree.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/conv.py` & `cercis-0.1.4/src/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/driver.py` & `cercis-0.1.4/src/blib2to3/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/grammar.py` & `cercis-0.1.4/src/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/literals.py` & `cercis-0.1.4/src/blib2to3/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/parse.py` & `cercis-0.1.4/src/blib2to3/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/pgen.py` & `cercis-0.1.4/src/blib2to3/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/token.py` & `cercis-0.1.4/src/blib2to3/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/blib2to3/pgen2/tokenize.py` & `cercis-0.1.4/src/blib2to3/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/__init__.py` & `cercis-0.1.4/src/cercis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 from _cercis_version import version as __version__
 from blib2to3.pgen2 import token
 from blib2to3.pytree import Leaf, Node
 from cercis.cache import Cache, get_cache_info, read_cache, write_cache
 from cercis.comments import normalize_fmt_off
 from cercis.const import (
+    DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
     DEFAULT_COLLAPSE_NESTED_BRACKETS,
     DEFAULT_EXCLUDES,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_INCLUDES,
     DEFAULT_LINE_LENGTH,
     DEFAULT_SINGLE_QUOTE,
     DEFAULT_WRAP_LINE_WITH_LONG_STRING,
@@ -225,14 +226,25 @@
     default=DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     help=(
         "If True, use 8 spaces as indent in function definition;"
         " otherwise, use 8 (Black's default)."
     ),
 )
 @click.option(
+    "-cbei",
+    "--closing-bracket-extra-indent",
+    type=bool,
+    show_default=True,
+    default=DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
+    help=(
+        "If True, add an extra indentation level (4 or 8, depending on"
+        " --function-definition-extra-indent) to the closing bracket."
+    ),
+)
+@click.option(
     "-sq",
     "--single-quote",
     type=bool,
     show_default=True,
     default=DEFAULT_SINGLE_QUOTE,
     help="If True, format code using single quotes; otherwise use double quotes.",
 )
@@ -485,14 +497,15 @@
 )
 @click.pass_context
 def main(  # noqa: C901
         ctx: click.Context,
         code: Optional[str],
         line_length: int,
         function_definition_extra_indent: bool,
+        closing_bracket_extra_indent: bool,
         single_quote: bool,
         wrap_line_with_long_string: bool,
         collapse_nested_brackets: bool,
         wrap_pragma_comments: bool,
         target_version: List[TargetVersion],
         check: bool,
         diff: bool,
@@ -612,14 +625,15 @@
         skip_source_first_line=skip_source_first_line,
         string_normalization=not skip_string_normalization,
         magic_trailing_comma=not skip_magic_trailing_comma,
         experimental_string_processing=experimental_string_processing,
         preview=preview,
         python_cell_magics=set(python_cell_magics),
         function_definition_extra_indent=function_definition_extra_indent,
+        closing_bracket_extra_indent=closing_bracket_extra_indent,
         single_quote=single_quote,
         wrap_line_with_long_string=wrap_line_with_long_string,
         collapse_nested_brackets=collapse_nested_brackets,
         wrap_pragma_comments=wrap_pragma_comments,
     )
 
     if code is not None:
```

### Comparing `cercis-0.1.3/src/cercis/_width_table.py` & `cercis-0.1.4/src/cercis/_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/brackets.py` & `cercis-0.1.4/src/cercis/brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/cache.py` & `cercis-0.1.4/src/cercis/cache.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/comments.py` & `cercis-0.1.4/src/cercis/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/concurrency.py` & `cercis-0.1.4/src/cercis/concurrency.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/debug.py` & `cercis-0.1.4/src/cercis/debug.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/files.py` & `cercis-0.1.4/src/cercis/files.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/handle_ipynb_magics.py` & `cercis-0.1.4/src/cercis/handle_ipynb_magics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/linegen.py` & `cercis-0.1.4/src/cercis/linegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,22 +941,22 @@
     respected.
 
     If it's the body component, the result line is one-indented inside brackets and as
     such has its first leaf's prefix normalized and a trailing comma added when
     expected.
     """
     result = Line(mode=original.mode, depth=original.depth)
-    if component is _BracketSplitComponent.body:
-        result.inside_brackets = True
 
-        if mode.function_definition_extra_indent and original.is_def:
-            additional_depth = 2
-        else:
-            additional_depth = 1
+    if mode.function_definition_extra_indent and original.is_def:
+        additional_depth = 2
+    else:
+        additional_depth = 1
 
+    if component is _BracketSplitComponent.body:
+        result.inside_brackets = True
         result.depth += additional_depth
 
         if leaves:
             # Since body is a new indent level, remove spurious leading whitespace.
             normalize_prefix(leaves[0], inside_brackets=True)
             # Ensure a trailing comma for imports and standalone function arguments, but
             # be careful not to add one after any comments or within type annotations.
@@ -989,14 +989,18 @@
                         new_comma = Leaf(token.COMMA, ",")
                         leaves.insert(i + 1, new_comma)
                     break
 
     leaves_to_track: Set[LeafID] = set()
     if component is _BracketSplitComponent.head:
         leaves_to_track = get_leaves_inside_matching_brackets(leaves)
+
+    if mode.closing_bracket_extra_indent and component is _BracketSplitComponent.tail:
+        result.depth += additional_depth
+
     # Populate the line
     for leaf in leaves:
         result.append(
             leaf,
             preformatted=True,
             track_bracket=id(leaf) in leaves_to_track,
         )
```

### Comparing `cercis-0.1.3/src/cercis/lines.py` & `cercis-0.1.4/src/cercis/lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/mode.py` & `cercis-0.1.4/src/cercis/mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final
 else:
     from typing import Final
 
 from cercis.const import (
+    DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
     DEFAULT_COLLAPSE_NESTED_BRACKETS,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_LINE_LENGTH,
     DEFAULT_SINGLE_QUOTE,
     DEFAULT_WRAP_LINE_WITH_LONG_STRING,
     DEFAULT_WRAP_PRAGMA_COMMENTS,
 )
@@ -188,14 +189,15 @@
     is_ipynb: bool = False
     skip_source_first_line: bool = False
     magic_trailing_comma: bool = True
     experimental_string_processing: bool = False
     python_cell_magics: Set[str] = field(default_factory=set)
     preview: bool = False
     function_definition_extra_indent: bool = DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT
+    closing_bracket_extra_indent: bool = DEFAULT_CLOSING_BRACKET_EXTRA_INDENT
     single_quote: bool = DEFAULT_SINGLE_QUOTE
     wrap_line_with_long_string: bool = DEFAULT_WRAP_LINE_WITH_LONG_STRING
     collapse_nested_brackets: bool = DEFAULT_COLLAPSE_NESTED_BRACKETS
     wrap_pragma_comments: bool = DEFAULT_WRAP_PRAGMA_COMMENTS
 
     def __post_init__(self) -> None:
         if self.experimental_string_processing:
```

### Comparing `cercis-0.1.3/src/cercis/nodes.py` & `cercis-0.1.4/src/cercis/nodes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/numerics.py` & `cercis-0.1.4/src/cercis/numerics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/output.py` & `cercis-0.1.4/src/cercis/output.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/parsing.py` & `cercis-0.1.4/src/cercis/parsing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/report.py` & `cercis-0.1.4/src/cercis/report.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/rusty.py` & `cercis-0.1.4/src/cercis/rusty.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/strings.py` & `cercis-0.1.4/src/cercis/strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/trans.py` & `cercis-0.1.4/src/cercis/trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/utils_line_wrapping.py` & `cercis-0.1.4/src/cercis/utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/src/cercis/utils_linegen.py` & `cercis-0.1.4/src/cercis/utils_linegen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/optional.py` & `cercis-0.1.4/tests/optional.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/test_black.py` & `cercis-0.1.4/tests/test_black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/test_blackd.py` & `cercis-0.1.4/tests/test_blackd.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/test_format.py` & `cercis-0.1.4/tests/test_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import replace
 from typing import Any, Iterator
 from unittest.mock import patch
 
 import pytest
 
 import cercis
+from cercis import TargetVersion
 from tests.util import (
     DEFAULT_MODE,
     PY36_VERSIONS,
     all_data_cases,
     assert_format,
     dump_to_stderr,
     read_data,
@@ -248,19 +249,39 @@
     "filename, extra_indent",
     [
         ("func_def_extra_indent.py", True),  # Cercis's default
         ("func_def_no_extra_indent.py", False),  # Black's default
     ],
 )
 def test_function_definition_extra_indent(filename: str, extra_indent: bool) -> None:
-    mode = replace(DEFAULT_MODE, function_definition_extra_indent=extra_indent)
-    _override_single_quote_for_cleaner_future_rebase(mode)
+    mode = replace(
+        DEFAULT_MODE,
+        function_definition_extra_indent=extra_indent,
+        # Adding trailing commas after *args etc. are only supported in py36+
+        target_versions={TargetVersion.PY36},
+    )
     check_file("configurable_cases/func_def_indent", filename, mode)
 
 
+@pytest.mark.parametrize(
+    "filename, extra_indent",
+    [
+        ("no_extra_indent.py", False),
+        ("extra_indent.py", True),
+    ],
+)
+def test_closing_bracket_extra_indent(filename: str, extra_indent: bool) -> None:
+    mode = replace(
+        DEFAULT_MODE,
+        line_length=30,
+        closing_bracket_extra_indent=extra_indent,
+    )
+    check_file("configurable_cases/closing_bracket_indent", filename, mode)
+
+
 @pytest.mark.filterwarnings("ignore:invalid escape sequence.*:DeprecationWarning")
 @pytest.mark.parametrize(
     "filename",
     all_data_cases("configurable_cases/single_quote"),
 )
 def test_single_quote(filename: str) -> None:
     mode = replace(
```

### Comparing `cercis-0.1.3/tests/test_ipynb.py` & `cercis-0.1.4/tests/test_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/test_no_ipynb.py` & `cercis-0.1.4/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/test_trans.py` & `cercis-0.1.4/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/test_utils_line_wrapping.py` & `cercis-0.1.4/tests/test_utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/util.py` & `cercis-0.1.4/tests/util.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/conditional_expression.py` & `cercis-0.1.4/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/edge_cases.py` & `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/edge_cases.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py` & `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py` & `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py` & `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py` & `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py` & `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py` & `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py` & `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py` & `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/pragma_comments/Black_default.py` & `cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/pragma_comments/Cercis_default.py` & `cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/single_quote/docstring.py` & `cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/single_quote/docstring_preview.py` & `cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/single_quote/more_quotes.py` & `cercis-0.1.4/tests/data/configurable_cases/single_quote/more_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/single_quote/string_prefixes.py` & `cercis-0.1.4/tests/data/configurable_cases/single_quote/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/configurable_cases/single_quote/torture.py` & `cercis-0.1.4/tests/data/configurable_cases/single_quote/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `cercis-0.1.4/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/jupyter/notebook_trailing_newline.ipynb` & `cercis-0.1.4/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/jupyter/notebook_without_changes.ipynb` & `cercis-0.1.4/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/debug_visitor.out` & `cercis-0.1.4/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/debug_visitor.py` & `cercis-0.1.4/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/decorators.py` & `cercis-0.1.4/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/docstring_no_string_normalization.py` & `cercis-0.1.4/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `cercis-0.1.4/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/force_py36.py` & `cercis-0.1.4/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/force_pyi.py` & `cercis-0.1.4/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/long_strings_flag_disabled.py` & `cercis-0.1.4/tests/data/miscellaneous/long_strings_flag_disabled.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/python2_detection.py` & `cercis-0.1.4/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/string_quotes.py` & `cercis-0.1.4/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/miscellaneous/stub.pyi` & `cercis-0.1.4/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/cantfit.py` & `cercis-0.1.4/tests/data/preview/cantfit.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/comments7.py` & `cercis-0.1.4/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/format_unicode_escape_seq.py` & `cercis-0.1.4/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/long_dict_values.py` & `cercis-0.1.4/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/long_strings.py` & `cercis-0.1.4/tests/data/preview/long_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/long_strings__east_asian_width.py` & `cercis-0.1.4/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/long_strings__edge_case.py` & `cercis-0.1.4/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/long_strings__regression.py` & `cercis-0.1.4/tests/data/preview/long_strings__regression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/long_strings__type_annotations.py` & `cercis-0.1.4/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/multiline_strings.py` & `cercis-0.1.4/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/prefer_rhs_split.py` & `cercis-0.1.4/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview/trailing_comma.py` & `cercis-0.1.4/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview_context_managers/targeting_py38.py` & `cercis-0.1.4/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview_context_managers/targeting_py39.py` & `cercis-0.1.4/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_310/parenthesized_context_managers.py` & `cercis-0.1.4/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_310/pattern_matching_complex.py` & `cercis-0.1.4/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_310/pattern_matching_extras.py` & `cercis-0.1.4/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_310/pattern_matching_generic.py` & `cercis-0.1.4/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_310/pattern_matching_simple.py` & `cercis-0.1.4/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_310/pattern_matching_style.py` & `cercis-0.1.4/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_311/pep_646.py` & `cercis-0.1.4/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_311/pep_654.py` & `cercis-0.1.4/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_311/pep_654_style.py` & `cercis-0.1.4/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_36/numeric_literals.py` & `cercis-0.1.4/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_37/python37.py` & `cercis-0.1.4/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_38/pep_570.py` & `cercis-0.1.4/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_38/pep_572.py` & `cercis-0.1.4/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_38/pep_572_remove_parens.py` & `cercis-0.1.4/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_38/python38.py` & `cercis-0.1.4/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_39/python39.py` & `cercis-0.1.4/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/py_39/remove_with_brackets.py` & `cercis-0.1.4/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/attribute_access_on_number_literals.py` & `cercis-0.1.4/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/class_blank_parentheses.py` & `cercis-0.1.4/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/class_methods_new_line.py` & `cercis-0.1.4/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/collections.py` & `cercis-0.1.4/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments.py` & `cercis-0.1.4/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments2.py` & `cercis-0.1.4/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments3.py` & `cercis-0.1.4/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments4.py` & `cercis-0.1.4/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments5.py` & `cercis-0.1.4/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments6.py` & `cercis-0.1.4/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments9.py` & `cercis-0.1.4/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/comments_non_breaking_space.py` & `cercis-0.1.4/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/composition.py` & `cercis-0.1.4/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/composition_no_trailing_comma.py` & `cercis-0.1.4/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/docstring.py` & `cercis-0.1.4/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/docstring_preview.py` & `cercis-0.1.4/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/empty_lines.py` & `cercis-0.1.4/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/expression.diff` & `cercis-0.1.4/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/expression.py` & `cercis-0.1.4/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/fmtonoff.py` & `cercis-0.1.4/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/fmtonoff2.py` & `cercis-0.1.4/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/fmtonoff5.py` & `cercis-0.1.4/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/fmtskip2.py` & `cercis-0.1.4/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/fmtskip8.py` & `cercis-0.1.4/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/fstring.py` & `cercis-0.1.4/tests/data/simple_cases/fstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/function.py` & `cercis-0.1.4/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/function2.py` & `cercis-0.1.4/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/function_trailing_comma.py` & `cercis-0.1.4/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/import_spacing.py` & `cercis-0.1.4/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/one_element_subscript.py` & `cercis-0.1.4/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/power_op_spacing.py` & `cercis-0.1.4/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `cercis-0.1.4/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/remove_await_parens.py` & `cercis-0.1.4/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/remove_except_parens.py` & `cercis-0.1.4/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/remove_for_brackets.py` & `cercis-0.1.4/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `cercis-0.1.4/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/remove_parens.py` & `cercis-0.1.4/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/return_annotation_brackets.py` & `cercis-0.1.4/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/skip_magic_trailing_comma.py` & `cercis-0.1.4/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/slices.py` & `cercis-0.1.4/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/string_prefixes.py` & `cercis-0.1.4/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/torture.py` & `cercis-0.1.4/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `cercis-0.1.4/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/LICENSE` & `cercis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/LICENSE_ORIGINAL` & `cercis-0.1.4/LICENSE_ORIGINAL`

 * *Files identical despite different names*

### Comparing `cercis-0.1.3/pyproject.toml` & `cercis-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cercis"
-version = "0.1.3"
+version = "0.1.4"
 description = "A more configurable Python code formatter"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 authors = [
   { name = "Łukasz Langa", email = "lukasz@langa.pl" },
   { name = "jsh9", email = "" },
 ]
```

### Comparing `cercis-0.1.3/PKG-INFO` & `cercis-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cercis
-Version: 0.1.3
+Version: 0.1.4
 Summary: A more configurable Python code formatter
 Project-URL: Changelog, https://github.com/jsh9/cercis/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/jsh9/cercis
 Author: jsh9
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 License-File: LICENSE
@@ -131,17 +131,18 @@
 Black doesn't. Configurability is our main motivation behind creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 1. [Line length](#31-line-length)
 2. [Single quote vs double quote](#32-single-quote-vs-double-quote)
 3. [Extra indentation at function definition](#33-extra-indentation-at-function-definition)
-4. ["Simple" lines with long strings](#34-simple-lines-with-long-strings)
-5. [Collapse nested brackets](#35-collapse-nested-brackets)
-6. [Wrap pragma comments](#36-wrapping-long-lines-ending-with-pragma-comments)
+4. [Extra indentation at closing brackets](#34-closing-bracket-indentation)
+5. ["Simple" lines with long strings](#35-simple-lines-with-long-strings)
+6. [Collapse nested brackets](#36-collapse-nested-brackets)
+7. [Wrap pragma comments](#37-wrapping-long-lines-ending-with-pragma-comments)
 
 The next section ([How to configure _Cercis_](#4-how-to-configure-cercis))
 contains detailed instructions of how to configure these options.
 
 ### 3.1. Line length
 
 _Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's
@@ -226,15 +227,94 @@
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Black's default        | `False`                                                         |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
-### 3.4. "Simple" lines with long strings
+## 3.4. Closing bracket indentation
+
+This option lets people customize where the closing bracket should be. Note
+that both styles are OK according to
+[PEP8](https://peps.python.org/pep-0008/#indentation).
+
+<table>
+  <tr>
+    <td>
+
+```python
+# --closing-bracket-extra-indent=False
+
+def function(
+        arg1: int,
+        arg2: float,
+        arg3_with_long_name: list,
+) -> None:
+    print('Hello world')
+
+
+result = func2(
+    12345,
+    3.1415926,
+    [1, 2, 3],
+)
+
+
+something = {
+    'a': 1,
+    'b': 2,
+    'c': 3,
+}
+```
+
+  </td>
+
+  <td>
+
+```python
+# --closing-bracket-extra-indent=True
+
+def function(
+        arg1: int,
+        arg2: float,
+        arg3_with_long_name: list,
+        ) -> None:
+    print('Hello world')
+
+
+result = func2(
+    12345,
+    3.1415926,
+    [1, 2, 3],
+    )
+
+
+something = {
+    'a': 1,
+    'b': 2,
+    'c': 3,
+    }
+```
+
+  </td>
+
+  </tr>
+</table>
+
+| Option                 |                                                             |
+| ---------------------- | ----------------------------------------------------------- |
+| Name                   | `--closing-bracket-extra-indent`                            |
+| Abbreviation           | `-cbei`                                                     |
+| Default                | `False`                                                     |
+| Black's default        | `False`                                                     |
+| Command line usage     | `cercis -cbei=True myScript.py`                             |
+| `pyproject.toml` usage | `closing-bracket-extra-indent = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--closing-bracket-extra-indent=False]`              |
+
+### 3.5. "Simple" lines with long strings
 
 By default, Black wraps lines that exceed length limit. But for very simple
 lines (such as assigning a long string to a variable), line wrapping is not
 necessary.
 
 <table>
   <tr>
@@ -293,15 +373,15 @@
 | Abbreviation           | `-wl`                                                     |
 | Default                | `False`                                                   |
 | Black's default        | `True`                                                    |
 | Command line usage     | `cercis -wl=True myScript.py`                             |
 | `pyproject.toml` usage | `wrap-line-with-long-string = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--wrap-line-with-long-string=False]`              |
 
-### 3.5. Collapse nested brackets
+### 3.6. Collapse nested brackets
 
 _Cercis_ by default collapses nested brackets to make the code more compact.
 
 <table>
   <tr>
     <td>
 
@@ -369,15 +449,15 @@
 | Command line usage     | `cercis -cnb=True myScript.py`                          |
 | `pyproject.toml` usage | `collapse-nested-brackets = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--collapse-nested-brackets=False]`              |
 
 The code implementation of this option comes from
 [Pyink](https://github.com/google/pyink), another forked project from Black.
 
-### 3.6. Wrapping long lines ending with pragma comments [^](#3-cerciss-code-style)
+### 3.7. Wrapping long lines ending with pragma comments [^](#3-cerciss-code-style)
 
 "Pragma comments", in this context, mean the directives for Python linters
 usually to tell them to ignore certain errors. Pragma comments that _Cercis_
 currently recognizes include:
 
 - _noqa_: `# noqa: E501`
 - _type: ignore_: `# type: ignore[no-untyped-def]`
@@ -505,22 +585,29 @@
 
 ### 4.5. How to reproduce Black's behavior
 
 If you'd like to reproduce Black's behavior, simply set all the configurable
 options in [Section 3](#3-cerciss-code-style) to Black's default values.
 # Change Log
 
+## [0.1.4] - 2023-05-07
+
+- Added
+  - A new configurable option: `--closing-bracket-extra-indent`
+
 ## [0.1.3] - 2023-05-07
 
 - Added
+
   - A new configurable option: `--collapse-nested-brackets`
   - A new configurable option: `--wrap-pragma-comments`
   - Some Github workflow actions to make sure CHANGELOG.md is updated
 
 - Changed
+
   - Changed the default quote to single quote
   - Changed the default line length to 79 characters
 
 - Removed
   - Some unrelated documentation and config files
 
 ## [0.1.2] - 2023-05-04
```

