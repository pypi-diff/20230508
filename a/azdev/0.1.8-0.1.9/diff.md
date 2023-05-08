# Comparing `tmp/azdev-0.1.8.tar.gz` & `tmp/azdev-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vsts/work/1/a/azdev-0.1.8.tar", last modified: Sun Jan 19 05:40:08 2020, max compression
+gzip compressed data, was "/home/vsts/work/1/a/azdev-0.1.9.tar", last modified: Thu Mar 12 07:51:09 2020, max compression
```

## Comparing `azdev-0.1.8.tar` & `azdev-0.1.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/
--rw-r--r--   0 vsts      (1001) docker     (117)     3698 2020-01-19 05:39:57.000000 azdev-0.1.8/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (117)      181 2020-01-19 05:39:57.000000 azdev-0.1.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (117)     9682 2020-01-19 05:40:08.000000 azdev-0.1.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)     4427 2020-01-19 05:39:57.000000 azdev-0.1.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (117)     3481 2020-01-19 05:39:57.000000 azdev-0.1.8/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/
--rw-r--r--   0 vsts      (1001) docker     (117)      340 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1416 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2599 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/commands.py
--rw-r--r--   0 vsts      (1001) docker     (117)      910 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/completer.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/config/
--rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)      603 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/config/cli.flake8
--rw-r--r--   0 vsts      (1001) docker     (117)     2290 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/config/cli_pylintrc
--rw-r--r--   0 vsts      (1001) docker     (117)      550 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/config/ext.flake8
--rw-r--r--   0 vsts      (1001) docker     (117)     2516 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/config/ext_pylintrc
--rw-r--r--   0 vsts      (1001) docker     (117)     7743 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/help.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/mod_templates/
--rw-r--r--   0 vsts      (1001) docker     (117)       81 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (117)      228 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/README.rst
--rw-r--r--   0 vsts      (1001) docker     (117)      908 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1451 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/_help.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1178 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/_params.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1155 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (117)      142 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/azext_metadata.json
--rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/blank__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1765 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/commands.py
--rw-r--r--   0 vsts      (1001) docker     (117)      921 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/custom.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1322 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/module__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)      409 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/pkg_declare__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)      112 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (117)     2344 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/setup.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1581 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/mod_templates/test_service_scenario.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/operations/
--rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    11976 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/code_gen.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/operations/extensions/
--rw-r--r--   0 vsts      (1001) docker     (117)    12239 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3435 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/extensions/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/operations/help/
--rw-r--r--   0 vsts      (1001) docker     (117)    12805 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/help/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/operations/help/refdoc/
--rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/help/refdoc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1747 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/help/refdoc/conf.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2117 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/legal.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/operations/linter/
--rw-r--r--   0 vsts      (1001) docker     (117)     4954 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10530 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/linter.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2633 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rule_decorators.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/operations/linter/rules/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rules/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)      286 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rules/ci_exclusions.yml
--rw-r--r--   0 vsts      (1001) docker     (117)      894 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rules/command_group_rules.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1017 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rules/command_rules.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8543 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rules/help_rules.py
--rw-r--r--   0 vsts      (1001) docker     (117)      944 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rules/linter_exclusions.yml
--rw-r--r--   0 vsts      (1001) docker     (117)     1874 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/rules/parameter_rules.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4356 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/linter/util.py
--rw-r--r--   0 vsts      (1001) docker     (117)     4405 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/performance.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13949 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/pypi.py
--rw-r--r--   0 vsts      (1001) docker     (117)      915 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/python_sdk.py
--rw-r--r--   0 vsts      (1001) docker     (117)     2715 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/resource.py
--rw-r--r--   0 vsts      (1001) docker     (117)    13201 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/setup.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6332 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/style.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/operations/tests/
--rw-r--r--   0 vsts      (1001) docker     (117)    15027 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1029 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/operations/tests/pytest_runner.py
--rw-r--r--   0 vsts      (1001) docker     (117)    10227 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/params.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev/utilities/
--rw-r--r--   0 vsts      (1001) docker     (117)     1894 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3312 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/command.py
--rw-r--r--   0 vsts      (1001) docker     (117)     1172 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/config.py
--rw-r--r--   0 vsts      (1001) docker     (117)      815 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/const.py
--rw-r--r--   0 vsts      (1001) docker     (117)      893 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/display.py
--rw-r--r--   0 vsts      (1001) docker     (117)     3088 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/git_util.py
--rw-r--r--   0 vsts      (1001) docker     (117)     8876 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/path.py
--rw-r--r--   0 vsts      (1001) docker     (117)      642 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/pypi.py
--rw-r--r--   0 vsts      (1001) docker     (117)      456 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/testing.py
--rw-r--r--   0 vsts      (1001) docker     (117)      764 2020-01-19 05:39:57.000000 azdev-0.1.8/azdev/utilities/tools.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-19 05:40:08.000000 azdev-0.1.8/azdev.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (117)     9682 2020-01-19 05:40:07.000000 azdev-0.1.8/azdev.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)     2260 2020-01-19 05:40:07.000000 azdev-0.1.8/azdev.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2020-01-19 05:40:07.000000 azdev-0.1.8/azdev.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (117)       47 2020-01-19 05:40:07.000000 azdev-0.1.8/azdev.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (117)      213 2020-01-19 05:40:07.000000 azdev-0.1.8/azdev.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        6 2020-01-19 05:40:07.000000 azdev-0.1.8/azdev.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (117)      424 2020-01-19 05:39:57.000000 azdev-0.1.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (117)       67 2020-01-19 05:40:08.000000 azdev-0.1.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (117)     3003 2020-01-19 05:39:57.000000 azdev-0.1.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/
+-rw-r--r--   0 vsts      (1001) docker     (117)     3950 2020-03-12 07:50:59.000000 azdev-0.1.9/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (117)      181 2020-03-12 07:50:59.000000 azdev-0.1.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (117)     9982 2020-03-12 07:51:09.000000 azdev-0.1.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (117)     4427 2020-03-12 07:50:59.000000 azdev-0.1.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (117)     3481 2020-03-12 07:50:59.000000 azdev-0.1.9/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/
+-rw-r--r--   0 vsts      (1001) docker     (117)      340 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1416 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2599 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      910 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/completer.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/config/
+-rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      603 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/config/cli.flake8
+-rw-r--r--   0 vsts      (1001) docker     (117)     2290 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/config/cli_pylintrc
+-rw-r--r--   0 vsts      (1001) docker     (117)      550 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/config/ext.flake8
+-rw-r--r--   0 vsts      (1001) docker     (117)     2516 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/config/ext_pylintrc
+-rw-r--r--   0 vsts      (1001) docker     (117)     7723 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/help.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/mod_templates/
+-rw-r--r--   0 vsts      (1001) docker     (117)       81 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (117)      228 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (117)      908 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1451 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1178 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1155 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      142 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/azext_metadata.json
+-rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/blank__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1765 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      921 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1322 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/module__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      409 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/pkg_declare__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      112 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (117)     2344 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1581 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/mod_templates/test_service_scenario.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/operations/
+-rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    11976 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/code_gen.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/operations/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (117)    12086 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3435 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/extensions/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/operations/help/
+-rw-r--r--   0 vsts      (1001) docker     (117)    12805 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/help/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/operations/help/refdoc/
+-rw-r--r--   0 vsts      (1001) docker     (117)      317 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/help/refdoc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1747 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/help/refdoc/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2117 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/legal.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/operations/linter/
+-rw-r--r--   0 vsts      (1001) docker     (117)     4954 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10530 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/linter.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2633 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rule_decorators.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/operations/linter/rules/
+-rw-r--r--   0 vsts      (1001) docker     (117)        0 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rules/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      286 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rules/ci_exclusions.yml
+-rw-r--r--   0 vsts      (1001) docker     (117)      894 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rules/command_group_rules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1017 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rules/command_rules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8543 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rules/help_rules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      944 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rules/linter_exclusions.yml
+-rw-r--r--   0 vsts      (1001) docker     (117)     1874 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/rules/parameter_rules.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4356 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/linter/util.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     4405 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/performance.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13949 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/pypi.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      915 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/python_sdk.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     2715 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/resource.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    13201 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     6332 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/style.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/operations/tests/
+-rw-r--r--   0 vsts      (1001) docker     (117)    15027 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1029 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/operations/tests/pytest_runner.py
+-rw-r--r--   0 vsts      (1001) docker     (117)    10184 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/params.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev/utilities/
+-rw-r--r--   0 vsts      (1001) docker     (117)     1894 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3312 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/command.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     1172 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/config.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      815 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/const.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      893 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/display.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     3088 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/git_util.py
+-rw-r--r--   0 vsts      (1001) docker     (117)     8876 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/path.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      642 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/pypi.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      456 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/testing.py
+-rw-r--r--   0 vsts      (1001) docker     (117)      764 2020-03-12 07:50:59.000000 azdev-0.1.9/azdev/utilities/tools.py
+drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (117)     9982 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (117)     2260 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)        1 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)       47 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)      246 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)        6 2020-03-12 07:51:09.000000 azdev-0.1.9/azdev.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (117)      424 2020-03-12 07:50:59.000000 azdev-0.1.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (117)       67 2020-03-12 07:51:09.000000 azdev-0.1.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (117)     3048 2020-03-12 07:50:59.000000 azdev-0.1.9/setup.py
```

### Comparing `azdev-0.1.8/HISTORY.rst` & `azdev-0.1.9/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 Release History
 ===============
 
+0.1.9
+++++++
+* azdev extension publish: add --storage-account-key and remove --storage-subscription
+* azdev extension update-index: remove unnecessary warning that will fail this command
+* CI: use `pip install -e` instead in ADO to fix fix import bug
+
 0.1.8
 ++++++
 * fix: azdev test cannot be used in python 3.8.1 or later
 
 0.1.7
 ++++++
 * fix: azdev test cannot find core tests
```

### Comparing `azdev-0.1.8/PKG-INFO` & `azdev-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: azdev
-Version: 0.1.8
+Version: 0.1.9
 Summary: Microsoft Azure CLI Developer Tools
 Home-page: https://github.com/Azure/azure-cli-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Description: Microsoft Azure CLI Dev Tools (azdev)
         =====================================
@@ -113,14 +113,20 @@
         
         
         .. :changelog:
         
         Release History
         ===============
         
+        0.1.9
+        ++++++
+        * azdev extension publish: add --storage-account-key and remove --storage-subscription
+        * azdev extension update-index: remove unnecessary warning that will fail this command
+        * CI: use `pip install -e` instead in ADO to fix fix import bug
+        
         0.1.8
         ++++++
         * fix: azdev test cannot be used in python 3.8.1 or later
         
         0.1.7
         ++++++
         * fix: azdev test cannot find core tests
```

### Comparing `azdev-0.1.8/README.md` & `azdev-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/README.rst` & `azdev-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/__main__.py` & `azdev-0.1.9/azdev/__main__.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/commands.py` & `azdev-0.1.9/azdev/commands.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/completer.py` & `azdev-0.1.9/azdev/completer.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/config/cli.flake8` & `azdev-0.1.9/azdev/config/cli.flake8`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/config/cli_pylintrc` & `azdev-0.1.9/azdev/config/cli_pylintrc`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/config/ext.flake8` & `azdev-0.1.9/azdev/config/ext.flake8`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/config/ext_pylintrc` & `azdev-0.1.9/azdev/config/ext_pylintrc`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/help.py` & `azdev-0.1.9/azdev/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,15 @@
 
 helps['extension publish'] = """
     short-summary: Build and publish an extension to a storage account.
     long-summary: Storage parameters may be persisted in the [defaults] section of your config file for convenience.
     examples:
         - name: Publish the contoso extension to a storage account and update the index. This will then be ready for a PR.
           text: >
-            azdev extension publish contoso --update-index --storage-account mystorage --storage-container extensions
-            --storage-subscription {subscriptionId}
+            azdev extension publish contoso --update-index --storage-account mystorage --storage-account-key 0000-0000 --storage-container extensions
 """
 
 
 helps['extension update-index'] = """
     short-summary: Update the extensions index.json from a built WHL file.
 """
```

### Comparing `azdev-0.1.8/azdev/mod_templates/_client_factory.py` & `azdev-0.1.9/azdev/mod_templates/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/_help.py` & `azdev-0.1.9/azdev/mod_templates/_help.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/_params.py` & `azdev-0.1.9/azdev/mod_templates/_params.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/_validators.py` & `azdev-0.1.9/azdev/mod_templates/_validators.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/commands.py` & `azdev-0.1.9/azdev/mod_templates/commands.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/custom.py` & `azdev-0.1.9/azdev/mod_templates/custom.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/module__init__.py` & `azdev-0.1.9/azdev/mod_templates/module__init__.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/setup.py` & `azdev-0.1.9/azdev/mod_templates/setup.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/mod_templates/test_service_scenario.py` & `azdev-0.1.9/azdev/mod_templates/test_service_scenario.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/code_gen.py` & `azdev-0.1.9/azdev/operations/code_gen.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/extensions/__init__.py` & `azdev-0.1.9/azdev/operations/extensions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,14 +195,16 @@
         raise CLIError("Unable to find 'index.json' in your extension repos. Have "
                        "you cloned 'azure-cli-extensions' and added it to you repo "
                        "sources with `azdev extension repo add`?")
 
     NAME_REGEX = r'.*/([^/]*)-\d+.\d+.\d+'
 
     for extension in extensions:
+        # Get the URL
+        extension = extension[extension.index('https'):]
         # Get extension WHL from URL
         if not extension.endswith('.whl') or not extension.startswith('https:'):
             raise CLIError('usage error: only URL to a WHL file currently supported.')
 
         # TODO: extend to consider other options
         ext_path = extension
 
@@ -264,15 +266,15 @@
         command = 'setup.py bdist_wheel -b bdist -d {} --universal'.format(dist_dir)
         result = py_cmd(command, "Building extension '{}'...".format(path), is_module=False)
         if result.error:
             raise result.error  # pylint: disable=raising-bad-type
     os.chdir(original_cwd)
 
 
-def publish_extensions(extensions, storage_subscription, storage_account, storage_container,
+def publish_extensions(extensions, storage_account, storage_account_key, storage_container,
                        dist_dir='dist', update_index=False, yes=False):
 
     heading('Publish Extensions')
 
     require_azure_cli()
 
     # rebuild the extensions
@@ -287,30 +289,29 @@
     uploaded_urls = []
 
     subheading('Uploading WHLs')
     for whl_path in whl_files:
         whl_file = os.path.split(whl_path)[-1]
         # check if extension already exists unless user opted not to
         if not yes:
-            command = 'az storage blob exists --subscription {} --account-name {} -c {} -n {}'.format(
-                storage_subscription, storage_account, storage_container, whl_file)
-            exists = json.loads(cmd(command).result)['exists']
+            from azure.storage.blob import BlockBlobService
+            client = BlockBlobService(account_name=storage_account, account_key=storage_account_key)
+            exists = client.exists(container_name=storage_container, blob_name=whl_file)
+
             if exists:
                 if not prompt_y_n(
                         "{} already exists. You may need to bump the extension version. Replace?".format(whl_file),
                         default='n'):
                     logger.warning("Skipping '%s'...", whl_file)
                     continue
         # upload the WHL file
-        command = 'az storage blob upload --subscription {} --account-name {} -c {} -n {} -f {}'.format(
-            storage_subscription, storage_account, storage_container, whl_file, os.path.abspath(whl_path))
-        cmd(command, "Uploading '{}'...".format(whl_file))
-        command = 'az storage blob url --subscription {} --account-name {} -c {} -n {} -otsv'.format(
-            storage_subscription, storage_account, storage_container, whl_file)
-        url = cmd(command).result
+        client.create_blob_from_path(container_name=storage_container, blob_name=whl_file,
+                                     file_path=os.path.abspath(whl_path))
+        url = client.make_blob_url(container_name=storage_container, blob_name=whl_file)
+
         logger.info(url)
         uploaded_urls.append(url)
 
     if update_index:
         subheading('Updating Index')
         update_extension_index(uploaded_urls)
```

### Comparing `azdev-0.1.8/azdev/operations/extensions/util.py` & `azdev-0.1.9/azdev/operations/extensions/util.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/help/__init__.py` & `azdev-0.1.9/azdev/operations/help/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 import tempfile
 
 from subprocess import check_call, check_output, CalledProcessError
 
 from knack.util import CLIError
 from knack.log import get_logger
 
+from azure.cli.core.extension.operations import list_available_extensions, list_extensions as list_cli_extensions  # pylint: disable=import-error
 from azdev.utilities import (
     display, heading, subheading,
     get_cli_repo_path, get_path_table
 )
 
 from azdev.utilities.tools import require_azure_cli
 from azdev.operations.extensions import list_extensions as list_dev_cli_extensions
-from azure.cli.core.extension.operations import list_available_extensions, list_extensions as list_cli_extensions  # pylint: disable=import-error
 
 DOC_MAP_NAME = 'doc_source_map.json'
 HELP_FILE_NAME = '_help.py'
 DOC_SOURCE_MAP_PATH = os.path.join('doc', 'sphinx', 'azhelpgen', DOC_MAP_NAME)
 
 _logger = get_logger(__name__)
```

### Comparing `azdev-0.1.8/azdev/operations/help/refdoc/conf.py` & `azdev-0.1.9/azdev/operations/help/refdoc/conf.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/legal.py` & `azdev-0.1.9/azdev/operations/legal.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/__init__.py` & `azdev-0.1.9/azdev/operations/linter/__init__.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/linter.py` & `azdev-0.1.9/azdev/operations/linter/linter.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/rule_decorators.py` & `azdev-0.1.9/azdev/operations/linter/rule_decorators.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/rules/command_group_rules.py` & `azdev-0.1.9/azdev/operations/linter/rules/command_group_rules.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/rules/command_rules.py` & `azdev-0.1.9/azdev/operations/linter/rules/command_rules.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/rules/help_rules.py` & `azdev-0.1.9/azdev/operations/linter/rules/help_rules.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/rules/linter_exclusions.yml` & `azdev-0.1.9/azdev/operations/linter/rules/linter_exclusions.yml`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/rules/parameter_rules.py` & `azdev-0.1.9/azdev/operations/linter/rules/parameter_rules.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/linter/util.py` & `azdev-0.1.9/azdev/operations/linter/util.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/performance.py` & `azdev-0.1.9/azdev/operations/performance.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/pypi.py` & `azdev-0.1.9/azdev/operations/pypi.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/python_sdk.py` & `azdev-0.1.9/azdev/operations/python_sdk.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/resource.py` & `azdev-0.1.9/azdev/operations/resource.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/setup.py` & `azdev-0.1.9/azdev/operations/setup.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/style.py` & `azdev-0.1.9/azdev/operations/style.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/tests/__init__.py` & `azdev-0.1.9/azdev/operations/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/operations/tests/pytest_runner.py` & `azdev-0.1.9/azdev/operations/tests/pytest_runner.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/params.py` & `azdev-0.1.9/azdev/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 
     with ArgumentsContext(self, 'extension publish') as c:
         c.argument('update_index', action='store_true', help='Update the index.json file after publishing is complete.')
 
     with ArgumentsContext(self, 'extension publish') as c:
         c.argument('storage_account', help='Name of the storage account to publish to. Environment variable: AZDEV_DEFAULTS_STORAGE_ACCOUNT.', arg_group='Storage', configured_default='storage_account')
         c.argument('storage_container', help='Name of the storage container to publish to. Environment variable: AZDEV_DEFAULTS_STORAGE_CONTAINER.', arg_group='Storage', configured_default='storage_container')
-        c.argument('storage_subscription', help='Subscription ID of the storage account. Environment variable: AZDEV_DEFAULTS_STORAGE_SUBSCRIPTION.', arg_group='Storage', configured_default='storage_subscription')
+        c.argument('storage_account_key', help='Key of the storage account to publish to. ', arg_group='Storage',
+                   configured_default='storage_account')
 
     for scope in ['extension add', 'extension remove', 'extension build', 'extension publish']:
         with ArgumentsContext(self, scope) as c:
             c.positional('extensions', metavar='NAME', nargs='+', help='Space-separated list of extension names.')
 
     for scope in ['extension repo add', 'extension repo remove']:
         with ArgumentsContext(self, scope) as c:
```

### Comparing `azdev-0.1.8/azdev/utilities/__init__.py` & `azdev-0.1.9/azdev/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/command.py` & `azdev-0.1.9/azdev/utilities/command.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/config.py` & `azdev-0.1.9/azdev/utilities/config.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/const.py` & `azdev-0.1.9/azdev/utilities/const.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/display.py` & `azdev-0.1.9/azdev/utilities/display.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/git_util.py` & `azdev-0.1.9/azdev/utilities/git_util.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/path.py` & `azdev-0.1.9/azdev/utilities/path.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/pypi.py` & `azdev-0.1.9/azdev/utilities/pypi.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev/utilities/tools.py` & `azdev-0.1.9/azdev/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/azdev.egg-info/PKG-INFO` & `azdev-0.1.9/azdev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: azdev
-Version: 0.1.8
+Version: 0.1.9
 Summary: Microsoft Azure CLI Developer Tools
 Home-page: https://github.com/Azure/azure-cli-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Description: Microsoft Azure CLI Dev Tools (azdev)
         =====================================
@@ -113,14 +113,20 @@
         
         
         .. :changelog:
         
         Release History
         ===============
         
+        0.1.9
+        ++++++
+        * azdev extension publish: add --storage-account-key and remove --storage-subscription
+        * azdev extension update-index: remove unnecessary warning that will fail this command
+        * CI: use `pip install -e` instead in ADO to fix fix import bug
+        
         0.1.8
         ++++++
         * fix: azdev test cannot be used in python 3.8.1 or later
         
         0.1.7
         ++++++
         * fix: azdev test cannot find core tests
```

### Comparing `azdev-0.1.8/azdev.egg-info/SOURCES.txt` & `azdev-0.1.9/azdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azdev-0.1.8/setup.py` & `azdev-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         'mock',
         'pytest~=4.4.0',
         'pytest-xdist',
         'pyyaml',
         'requests',
         'sphinx==1.6.7',
         'tox',
-        'wheel==0.30.0'
+        'wheel==0.30.0',
+        'azure-storage-blob>=1.3.1,<2.0.0',
     ],
     extras_require={
         ":python_version<'3.0'": ['pylint==1.9.2', 'futures'],
         ":python_version>='3.0'": ['pylint==2.3.0']
     },
     package_data={
         'azdev.config': ['*.*', 'cli_pylintrc', 'ext_pylintrc'],
```

