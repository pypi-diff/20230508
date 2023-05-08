# Comparing `tmp/cli_command_parser-2023.5.2.tar.gz` & `tmp/cli_command_parser-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2023.5.2.tar", last modified: Tue May  2 11:35:50 2023, max compression
+gzip compressed data, was "cli_command_parser-2023.5.8.tar", last modified: Mon May  8 11:55:54 2023, max compression
```

## Comparing `cli_command_parser-2023.5.2.tar` & `cli_command_parser-2023.5.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.513208 cli_command_parser-2023.5.2/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5610 2023-05-02 11:35:50.514207 cli_command_parser-2023.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.361159 cli_command_parser-2023.5.2/lib/
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.428205 cli_command_parser-2023.5.2/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1136 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2023-05-02 11:35:39.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0      463 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/actions.py
--rw-rw-rw-   0        0        0     2868 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    22573 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    12737 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    16435 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    16608 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.459208 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12765 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0    24495 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     7560 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0    10136 2023-04-23 16:53:29.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    13416 2023-03-29 11:48:12.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     8093 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.473206 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     6568 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    20558 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     8572 2022-09-18 21:50:31.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5440 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.495207 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2125 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6313 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     8563 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     7772 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0    21205 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6490 2023-01-14 20:20:57.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0    10756 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     7476 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.513208 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      300 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    27625 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    17312 2023-04-19 21:58:59.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    10686 2023-04-23 16:53:29.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     6913 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    25990 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0     2115 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     4201 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11384 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    15172 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0    10811 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1956 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     4968 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.438207 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     5610 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2314 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/pyproject.toml
--rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/readme.rst
--rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.5.2/requirements-dev.txt
--rw-rw-rw-   0        0        0     1293 2023-05-02 11:35:50.515208 cli_command_parser-2023.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.577103 cli_command_parser-2023.5.8/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5610 2023-05-08 11:55:54.577103 cli_command_parser-2023.5.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.453103 cli_command_parser-2023.5.8/lib/
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.510103 cli_command_parser-2023.5.8/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1136 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2023-05-08 11:55:42.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0      463 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/actions.py
+-rw-rw-rw-   0        0        0     2868 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    22365 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    12631 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    16428 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    16563 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.545104 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     7375 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0     9987 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    14808 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8078 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.554103 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     6914 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    20503 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     9198 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     5440 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.568104 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2105 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6363 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     8551 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     7734 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0    21187 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6490 2023-01-14 20:20:57.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    10659 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     7415 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.576103 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      300 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    27355 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    17032 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    10574 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     6884 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    25861 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0     2072 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4184 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11375 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    15172 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    10811 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     1956 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     4900 2023-05-08 11:55:32.000000 cli_command_parser-2023.5.8/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:55:54.520104 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     5610 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2314 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-08 11:55:54.000000 cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.8/readme.rst
+-rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.5.8/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1293 2023-05-08 11:55:54.580105 cli_command_parser-2023.5.8/setup.cfg
```

### Comparing `cli_command_parser-2023.5.2/LICENSE` & `cli_command_parser-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/PKG-INFO` & `cli_command_parser-2023.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2023.5.2
+Version: 2023.5.8
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/__init__.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/annotations.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/annotations.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/command_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.config = config
         self._process_parameters()
 
     def __repr__(self) -> str:
         positionals = len(self.positionals)
         options = len(self.options)
         cls_name = self.__class__.__name__
-        return f'<{cls_name}[command={self.command.__name__}, positionals={positionals!r}, options={options!r}]>'
+        return f'<{cls_name}[command={self.command.__name__}, {positionals=}, {options=}]>'
 
     @property
     def pass_thru(self) -> Optional[PassThru]:
         if self._pass_thru:
             return self._pass_thru
         elif self.parent:
             return self.parent.pass_thru
@@ -151,21 +151,19 @@
                 options.append(param)
             elif isinstance(param, ParamGroup):
                 # Groups will only be discovered here when defined with `as` - ex: `with ParamGroup(...) as foo:`
                 # Group members will always be discovered at the top level since context managers share the outer scope
                 groups.add(param)
             elif isinstance(param, PassThru):
                 if self.pass_thru:
-                    raise CommandDefinitionError(
-                        f'Invalid PassThru param={param!r} - it cannot follow another PassThru param'
-                    )
+                    raise CommandDefinitionError(f'Invalid PassThru {param=} - it cannot follow another PassThru param')
                 self._pass_thru = param
             else:
                 raise CommandDefinitionError(
-                    f'Unexpected type={param.__class__} for param={param!r} - custom parameters must extend'
+                    f'Unexpected type={param.__class__} for {param=} - custom parameters must extend'
                     ' BasePositional, BaseOption, or ParamGroup'
                 )
 
             if param.group:
                 _find_groups(groups, param)
 
         if self.config.add_help and self.command_parent is not None and (not self.parent or not self.parent._has_help):
@@ -180,26 +178,25 @@
             _groups, groups = groups, self.parent.groups.copy()
             groups.extend(_groups)
 
         self.groups = sorted(groups)
 
     def _process_positionals(self, params: List[BasePositional]):
         unfollowable = action_or_sub_cmd = split_index = None
-        parent = self.parent
-        if parent and parent._deferred_positionals:
+        if (parent := self.parent) and parent._deferred_positionals:
             params = parent._deferred_positionals + params
 
         for i, param in enumerate(params):
             if unfollowable:
                 if 0 in unfollowable.nargs:
                     why = 'because it is a positional that is not required'
                 else:
                     why = 'because it accepts a variable number of arguments with no specific choices defined'
                 raise CommandDefinitionError(
-                    f'Additional Positional parameters cannot follow {unfollowable} {why} - param={param!r} is invalid'
+                    f'Additional Positional parameters cannot follow {unfollowable} {why} - {param=} is invalid'
                 )
             elif isinstance(param, (SubCommand, Action)):
                 if action_or_sub_cmd:
                     raise CommandDefinitionError(
                         f'Only 1 Action xor SubCommand is allowed in a given Command - {self.command.__name__} cannot'
                         f' contain both {action_or_sub_cmd} and {param}'
                     )
@@ -220,29 +217,28 @@
                 self._deferred_positionals = params[split_index:]
             else:
                 params, self._deferred_positionals = params[:split_index], params[split_index:]
 
         self.positionals = params
 
     def _process_options(self, params: Collection[BaseOption]):
-        parent = self.parent
-        if parent:
+        if parent := self.parent:
             option_map = parent.option_map.copy()
             combo_option_map = parent.combo_option_map.copy()
             options = parent.options.copy()
         else:
             option_map = {}
             combo_option_map = {}
             options = []
 
         for param in params:
             options.append(param)
             opts = param.option_strs
             if not opts.has_min_opts():
-                raise ParameterDefinitionError(f'No option strings were registered for param={param!r}')
+                raise ParameterDefinitionError(f'No option strings were registered for {param=}')
             self._process_option_strs(param, 'long', opts.long, option_map, combo_option_map)
             self._process_option_strs(param, 'short', opts.short, option_map, combo_option_map)
 
         self.options = options
         self.option_map = option_map
         self._process_action_flags(options)
         self.combo_option_map = dict(sorted(combo_option_map.items(), key=lambda kv: (-len(kv[0]), kv[0])))  # noqa
@@ -266,15 +262,15 @@
                 )
 
     def _process_action_flags(self, options: List[BaseOption]):
         action_flags = sorted((p for p in options if isinstance(p, ActionFlag)))
         grouped_ordered_flags = {True: defaultdict(list), False: defaultdict(list)}
         for param in action_flags:
             if param.func is None:
-                raise ParameterDefinitionError(f'No function was registered for param={param!r}')
+                raise ParameterDefinitionError(f'No function was registered for {param=}')
             grouped_ordered_flags[param.before_main][param.order].append(param)  # noqa  # PyCharm infers the wrong type
 
         found_non_always = False
         invalid = {}
         for before_main, prio_params in grouped_ordered_flags.items():
             for prio, params in prio_params.items():
                 param: ActionFlag = params[0]  # Don't pop and check `if params` - all are needed for the group check
@@ -304,16 +300,15 @@
 
     # endregion
 
     # region Ambiguous Short Combo Handling
 
     def _strict_ambiguous_short_combo_check(self):
         # Called during initial Option processing when using AmbiguousComboMode.STRICT
-        potentially_ambiguous_combo_options = self._potentially_ambiguous_combo_options
-        if not potentially_ambiguous_combo_options:
+        if not (potentially_ambiguous_combo_options := self._potentially_ambiguous_combo_options):
             return
 
         param_conflicts_map = {
             param: singles.values() for param, singles in potentially_ambiguous_combo_options.values()
         }
         raise AmbiguousShortForm(param_conflicts_map)
 
@@ -447,15 +442,15 @@
             if param.accepts_values:
                 return param
         elif option.startswith('-'):
             for _, param, _ in self.short_option_to_param_value_pairs(option):
                 if param.accepts_values:
                     return param
         else:
-            raise ValueError(f'Invalid option={option!r}')
+            raise ValueError(f'Invalid {option=}')
         return None
 
     def find_nested_option_that_accepts_values(self, option: str) -> Optional[BaseOption]:
         for params in self._iter_nested_params():
             try:
                 param = params.find_option_that_accepts_values(option)
             except KeyError:
@@ -497,16 +492,15 @@
             if param.env_var and ctx.num_provided(param) == 0:
                 yield param
 
     def required_check_params(self) -> Iterator[Parameter]:
         ignore = SubCommand
         yield from (p for p in self.all_positionals if p.required and not p.group and not isinstance(p, ignore))
         yield from (p for p in self.options if p.required and not p.group)
-        pass_thru = self._pass_thru
-        if pass_thru and pass_thru.required and not pass_thru.group:
+        if (pass_thru := self._pass_thru) and pass_thru.required and not pass_thru.group:
             yield pass_thru
 
 
 def _find_groups(groups: Set[ParamGroup], param: ParamBase):
     group = param.group
     while group:
         groups.add(group)
@@ -514,12 +508,11 @@
 
 
 def _find_ambiguous_combos(
     single_char_combos: OptionMap, multi_char_combos: OptionMap
 ) -> Dict[str, Tuple[BaseOption, OptionMap]]:
     ambiguous_combo_options = {}
     for combo, param in multi_char_combos.items():
-        singles = {c: single_char_combos[c] for c in combo if c in single_char_combos}
-        if singles:
+        if singles := {c: single_char_combos[c] for c in combo if c in single_char_combos}:
             ambiguous_combo_options[combo] = (param, singles)
 
     return ambiguous_combo_options
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/commands.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,19 +108,17 @@
         :param argv: The arguments to parse (defaults to :data:`sys.argv`)
         :return: A Command instance with parsed arguments that is ready for :meth:`.__call__` or :meth:`.main`
         """
         ctx = get_or_create_context(cls, argv)
         cmd_cls = cls
         with ExitStack() as stack:
             stack.enter_context(ctx)
-            sub_cmd = CommandParser.parse_args_and_get_next_cmd(ctx)
-            while sub_cmd:
+            while sub_cmd := CommandParser.parse_args_and_get_next_cmd(ctx):
                 cmd_cls = sub_cmd
                 ctx = stack.enter_context(ctx._sub_context(cmd_cls))
-                sub_cmd = CommandParser.parse_args_and_get_next_cmd(ctx)
 
             return cmd_cls()
 
     # endregion
 
     def __call__(self, *args, **kwargs) -> int:
         """
@@ -170,16 +168,15 @@
         :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
         """
         ctx = self.__ctx
         n_flags = ctx.action_flag_count
         if n_flags and not ctx.config.multiple_action_flags and n_flags > 1:
             raise ParamConflict(ctx.all_action_flags, 'combining multiple action flags is disabled')
 
-        before = ctx.categorized_action_flags[ActionPhase.BEFORE_MAIN]
-        if before:
+        if before := ctx.categorized_action_flags[ActionPhase.BEFORE_MAIN]:
             action = get_params(self).action
             if action is not None and not ctx.config.action_after_action_flags:
                 raise ParamConflict([action, *before], 'combining an action with action flags is disabled')
 
         for param in ctx.iter_action_flags(ActionPhase.PRE_INIT):
             param.func(self, *args, **kwargs)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/compat.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/compat.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/config.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     @classmethod
     def _missing_(cls, value: Union[str, int]) -> ShowDefaults:
         if isinstance(value, str):
             try:
                 return cls._member_map_[value.upper().replace('-', '_')]  # noqa
             except KeyError:
                 expected = ', '.join(cls._member_map_)
-                raise ValueError(f'Invalid {cls.__name__} value={value!r} - expected one of {expected}') from None
+                raise ValueError(f'Invalid {cls.__name__} {value=} - expected one of {expected}') from None
         return super()._missing_(value)
 
     def __or__(self, other: ShowDefaults) -> ShowDefaults:
         if ShowDefaults.NEVER in (self, other):
             return ShowDefaults.NEVER
         return super().__or__(other)  # noqa
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/context.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,16 +152,15 @@
         """
         with self:
             if recursive and self.parent:
                 parsed = self.parent.get_parsed(exclude, recursive)
             else:
                 parsed = {}
 
-            params = self.params
-            if params:
+            if params := self.params:
                 for group in (params.all_positionals, params.options, (params.pass_thru,)):
                     for param in group:
                         if param and param not in exclude:
                             try:
                                 parsed[param.name] = param.result_value()
                             except MissingArgument:
                                 parsed[param.name] = None
@@ -177,16 +176,15 @@
         try:
             return self.command.__class__.params(self.command)
         except AttributeError:  # self.command is None
             return None
 
     def get_error_handler(self) -> Union[ErrorHandler, NullErrorHandler]:
         """Returns the :class:`.ErrorHandler` configured to be used."""
-        error_handler = self.config.error_handler
-        if error_handler is _NotSet:
+        if (error_handler := self.config.error_handler) is _NotSet:
             return extended_error_handler
         elif error_handler is None:
             return NullErrorHandler()
         else:
             return error_handler
 
     # region Parsing
@@ -282,15 +280,15 @@
 
 
 def _normalize_config(
     config: AnyConfig, kwargs: Dict[str, Any], parent: Optional[Context], command: Optional[CommandType]
 ) -> CommandConfig:
     if config is not None:
         if kwargs:
-            raise TypeError(f'Cannot combine config={config!r} with keyword config arguments={kwargs}')
+            raise TypeError(f'Cannot combine {config=} with keyword config arguments={kwargs}')
         elif isinstance(config, CommandConfig):
             return config
         kwargs = config
 
     if parent:
         for key, val in parent.config._data.items():
             kwargs.setdefault(key, val)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.src_text = src_text
         parse_args = (self.src_text, self.path.as_posix()) if self.path else (self.src_text,)
         self.root_node = ast.parse(*parse_args)
 
     def __repr__(self) -> str:
         parsers = len(self.parsers)
         location = f' @ {self.path.as_posix()}' if self.path else ''
-        return f'<{self.__class__.__name__}[parsers={parsers!r}{location}]>'
+        return f'<{self.__class__.__name__}[{parsers=}{location}]>'
 
     @property
     def mod_cls_to_ast_cls_map(self) -> Dict[str, Dict[str, ParserCls]]:
         return self._parser_classes
 
     @classmethod
     def _register_parser(cls, module: str, name: str, ast_cls: ParserCls):
@@ -220,16 +220,15 @@
 
     @cached_property
     def init_func_kwargs(self) -> Dict[str, str]:
         return self._init_func_kwargs()
 
     def init_call_repr(self) -> str:
         arg_str = ', '.join(self.init_func_args)
-        kw_str = ', '.join(f'{k}={v}' for k, v in self.init_func_kwargs.items())
-        if kw_str:
+        if kw_str := ', '.join(f'{k}={v}' for k, v in self.init_func_kwargs.items()):
             arg_str = kw_str if not arg_str else (arg_str + ', ' + kw_str)
         return f'{self.init_func_name}({arg_str})'
 
     # endregion
 
     def pprint(self, indent: int = 0):
         print(f'{" " * indent} - {self!r}')
@@ -281,16 +280,15 @@
 
     # region Output Methods
 
     def pprint(self, indent: int = 0):
         print(f'{" " * indent} + {self!r}:')
         indent += 3
         for attr in self._children:
-            values = getattr(self, attr)
-            if values:
+            if values := getattr(self, attr):
                 for value in values:
                     value.pprint(indent)
 
     # endregion
 
 
 class ArgGroup(ArgCollection, represents=_ArgumentParser.add_argument_group):
@@ -320,15 +318,15 @@
         super().__init__(node, parent, tracked_refs, call)
         self._subparsers_actions = []
         # Note: sub_parsers aren't included in grouped_children since they need different handling during conversion
         self.sub_parsers = []
 
     def __repr__(self) -> str:
         sub_parsers = len(self.sub_parsers)
-        return f'<{self.__class__.__name__}[sub_parsers={sub_parsers!r}]: ``{self.init_call_repr()}``>'
+        return f'<{self.__class__.__name__}[{sub_parsers=}]: ``{self.init_call_repr()}``>'
 
     def _add_subparser(self, node: InitNode, call: Call, tracked_refs: TrackedRefMap, sub_parser_cls: ParserCls = None):
         # Using default of None since the class hasn't been defined at the time it would need to be set as default
         return self._add_child(sub_parser_cls or SubParser, self.sub_parsers, node, call, tracked_refs)
 
 
 class SubParser(AstArgumentParser, represents=_SubParsersAction.add_parser):
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/command_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,26 +299,25 @@
         yield f'{prefix}with ParamGroup({self._get_args()}):'
         yield from self.format_members(prefix, indent + 4)
 
     def _get_args(self) -> str:
         # log.debug(f'Processing args for {self.ast_obj._init_func_bound}')
         description = self.ast_obj.init_func_kwargs.get('description')
         # TODO: Missing required=True
-        title = self.ast_obj.init_func_kwargs.get('title')
-        if title:
+        if title := self.ast_obj.init_func_kwargs.get('title'):
             title_str = literal_eval(title)
             if title_str.lower().endswith(' options'):
                 if description:
                     title = repr(title_str[:-7].rstrip())
                 else:
                     description, title = title, None
 
         args = [title] if title else []
         if description:
-            args.append(f'description={description}')
+            args.append(f'{description=!s}')
         if isinstance(self.ast_obj, MutuallyExclusiveGroup):
             args.append('mutually_exclusive=True')
         return ', '.join(args)
 
 
 class ParamConverter(Converter[ParserArg], converts=ParserArg):
     ast_obj: ParserArg
@@ -369,25 +368,24 @@
 
     @cached_property
     def _attr_name(self) -> str:
         return next(name for name in self._attr_name_candidates() if name not in RESERVED)
 
     def _attr_name_candidates(self) -> Iterator[str]:
         dest = self.ast_obj.init_func_raw_kwargs.get('dest')
-        if dest is not None and isinstance(dest, (Constant, Str)):  # Str is for 3.7 compatibility
+        if dest is not None and isinstance(dest, Constant):
             yield getattr(dest, dest._fields[0])  # .value for Constant, .s for Str
 
         long, short, plain = self._grouped_opt_strs
         if self.is_positional or self.is_pass_thru:
             yield from plain
         if self.is_option or self.is_pass_thru:
             for group in (long, short):
                 for opt in group:
-                    opt = opt.lstrip('-')
-                    if opt:
+                    if opt := opt.lstrip('-'):
                         yield opt
         while True:
             yield f'param_{next(self._counter)}'
 
     # endregion
 
     # region Arg Processing
@@ -407,53 +405,50 @@
         return len(long) == 1 and long[0][2:] == self._attr_name
 
     def get_pos_args(self) -> Iterable[str]:
         return (repr(arg) for arg in self.cmd_option_strs)
 
     def get_cls_and_kwargs(self) -> Tuple[str, BaseArgs]:
         kwargs = self.ast_obj.init_func_kwargs.copy()
-        help_arg = kwargs.get('help')
-        if help_arg and help_arg in self.ast_obj.get_tracked_refs('argparse', 'SUPPRESS', ()):
+        if (help_arg := kwargs.get('help')) and help_arg in self.ast_obj.get_tracked_refs('argparse', 'SUPPRESS', ()):
             kwargs.update({'hide': 'True', 'help': None})
 
         if self.is_pass_thru:
             return 'PassThru', PassThruArgs.from_kwargs(**kwargs)
 
-        action = kwargs.pop('action', None)
-        if action:
+        if action := kwargs.pop('action', None):
             action = literal_eval(action)
 
         if self.is_positional:
             if action and action not in ('store', 'append'):
-                raise ConversionError(f'{self.ast_obj}: action={action!r} is not supported for Positional parameters')
+                raise ConversionError(f'{self.ast_obj}: {action=} is not supported for Positional parameters')
             return 'Positional', ParamArgs.init_positional(action, **kwargs)
         elif self.is_option:
             kwargs['name_mode'] = self.name_mode
             if not action and 'const' in kwargs:
                 action = 'append_const' if 'nargs' in kwargs else 'store_const'
             if action:
                 if action in ('store_true', 'store_false', 'store_const', 'append_const'):
                     return 'Flag', FlagArgs.init_flag(action, **kwargs)
                 elif action == 'count':
                     return 'Counter', FlagArgs.init_counter(**kwargs)
                 elif action not in ('store', 'append'):
-                    raise ConversionError(f'{self.ast_obj}: action={action!r} is not supported for Option parameters')
+                    raise ConversionError(f'{self.ast_obj}: {action=} is not supported for Option parameters')
 
             return 'Option', OptionArgs.init_option(self.ast_obj, action, **kwargs)
 
         raise ConversionError(f'Unable to determine a suitable Parameter type for {self.ast_obj!r}')
 
     # endregion
 
     # region High Level Param Type
 
     @cached_property
     def is_pass_thru(self) -> bool:
-        nargs = self.ast_obj.init_func_kwargs.get('nargs')
-        if not nargs:
+        if not (nargs := self.ast_obj.init_func_kwargs.get('nargs')):
             return False
         # TODO: Refactor to take advantage of new nargs=REMAINDER support
         return nargs in self.ast_obj.get_tracked_refs('argparse', 'REMAINDER', ())
 
     @cached_property
     def is_positional(self) -> bool:
         long, short, plain = self._grouped_opt_strs
@@ -495,17 +490,16 @@
             else:
                 others.append(converter)
                 others.extend(i_converters)
 
         for positional in positionals:
             yield from positional.format_lines(indent)
 
-        sub_parsers = getattr(self.parent.ast_obj, 'sub_parsers', None)
-        if sub_parsers:
-            log.debug(f'Found sub_parsers={sub_parsers}')
+        if sub_parsers := getattr(self.parent.ast_obj, 'sub_parsers', None):
+            log.debug(f'Found {sub_parsers=}')
             try:
                 name = literal_eval(sub_parsers[0].init_func_kwargs['dest']).replace('-', '_')
             except (KeyError, ValueError):
                 name = 'sub_cmd'
             else:
                 if name in RESERVED:
                     name = 'sub_cmd'
@@ -531,16 +525,15 @@
     def to_str(self, *args: str) -> str:
         return self._to_str(args, ['help'])
 
     @classmethod
     def from_kwargs(cls, **kwargs):
         keys = set(f.name for f in fields(cls)).intersection(kwargs)
         filtered = {key: kwargs[key] for key in keys}
-        help_str = filtered.get('help')
-        if help_str:
+        if help_str := filtered.get('help'):
             # log.debug(f'Processing {help_str=}')
             try:
                 help_str = literal_eval(help_str)
             except ValueError:  # likely an f-string
                 pass
             else:
                 if help_str.endswith('(default: %(default)s)'):
@@ -593,16 +586,15 @@
     type: OptStr = None
     nargs: OptStr = None
     choices: OptStr = None
 
     @classmethod
     def init_positional(cls, action: OptStr = None, nargs: OptStr = None, **kwargs):
         if nargs is not None:
-            parsed = literal_eval_or_none(nargs)
-            if parsed is not None:
+            if (parsed := literal_eval_or_none(nargs)) is not None:
                 nargs_obj = Nargs(parsed)
                 if action in ('store', None) and nargs_obj == 1:
                     action = nargs = None
             else:
                 nargs_obj = None
         else:
             nargs_obj = Nargs(1)
@@ -615,21 +607,21 @@
 @dataclass
 class OptionArgs(ParamArgs):
     name_mode: OptStr = None
 
     @classmethod
     def init_option(cls, arg: ParserArg, action: OptStr = None, nargs: OptStr = None, const: OptStr = None, **kwargs):
         if const:
-            log.warning(f'{arg}: ignoring const={const!r} - it is only supported for Flag and Counter parameters')
+            log.warning(f'{arg}: ignoring {const=} - it is only supported for Flag and Counter parameters')
 
         if nargs == "'*'":
             nargs = "'+'"
         if action == 'append':
             if not nargs:
-                log.debug(f"{arg}: using default nargs='+' because action={action!r} and no nargs value was provided")
+                log.debug(f"{arg}: using default nargs='+' because {action=} and no nargs value was provided")
                 nargs = "'+'"
             action = None
         elif action == 'store':
             if nargs == '1':
                 nargs = None
             action = None
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/conversion/visitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,26 +64,23 @@
         tracked_refs.default_factory = None
         return tracked_refs
 
     # region Imports
 
     def visit_Import(self, node: Import):
         for module_name, as_name in imp_names(node):
-            name_tracked_map = self._mod_name_tracked_map.get(module_name)
-            if name_tracked_map:
+            if name_tracked_map := self._mod_name_tracked_map.get(module_name):
                 log.debug(f'Found module import: {module_name} as {as_name}')
                 for name, tracked in name_tracked_map.items():
                     self.scopes[f'{as_name}.{name}'] = tracked
 
     def visit_ImportFrom(self, node: ImportFrom):
-        name_tracked_map = self._mod_name_tracked_map.get(node.module)
-        if name_tracked_map:
+        if name_tracked_map := self._mod_name_tracked_map.get(node.module):
             for name, as_name in imp_names(node):
-                tracked = name_tracked_map.get(name)
-                if tracked:
+                if tracked := name_tracked_map.get(name):
                     log.debug(f'Found tracked import: {node.module}.{name} as {as_name}')
                     self.scopes[as_name] = tracked
 
     # endregion
 
     # region Scope Changes
 
@@ -101,15 +98,15 @@
                 self._visit_for_elements(node, node.target.id, ele_names)
         else:
             self.generic_visit(node)
 
     visit_AsyncFor = visit_For
 
     def _visit_for_smart(self, node: For, loop_var: str, ele_names: List[str]):
-        log.debug(f'Attempting smart for loop visit for loop_var={loop_var!r} in ele_names={ele_names!r}')
+        log.debug(f'Attempting smart for loop visit for {loop_var=} in {ele_names=}')
         refs = [ref for ref in (self.scopes.get(name) for name in ele_names) if ref]
         # log.debug(f'  > Found {len(refs)=}, {len(ele_names)=}')
 
         if len(refs) == len(ele_names) and all(isinstance(ref, AstArgumentParser) for ref in refs):
             parents = set(ref.parent for ref in refs)
             log.debug(f'  > Found parents={len(parents)}')
             if len(parents) == 1:
@@ -121,16 +118,15 @@
 
         log.debug('Falling back to generic loop handling')
         self._visit_for_elements(node, loop_var, ele_names)
 
     def _visit_for_elements(self, node: For, loop_var: str, ele_names: List[str]):
         visited_any = False
         for name in ele_names:
-            ref = self.scopes.get(name)
-            if ref:
+            if ref := self.scopes.get(name):
                 visited_any = True
                 self.scopes[loop_var] = ref
                 self.generic_visit(node)
 
         if not visited_any:
             self.generic_visit(node)
 
@@ -157,38 +153,33 @@
             can_call = attr in obj.visit_funcs
         except (AttributeError, TypeError):
             return None
         return getattr(obj, attr) if can_call else None
 
     def visit_withitem(self, item):
         context_expr = item.context_expr
-        func = self.resolve_ref(context_expr)
-        if func:
+        if func := self.resolve_ref(context_expr):
             call = context_expr if isinstance(context_expr, Call) else None
             result = func(item, call, self.get_tracked_refs())
-            as_name = item.optional_vars
-            if as_name:
+            if as_name := item.optional_vars:
                 self.scopes[get_name_repr(as_name)] = result
 
     def visit_Assign(self, node: Assign):
         value = node.value
         if isinstance(value, (Attribute, Name)):  # Assigning an alias to a variable
-            ref = self.resolve_ref(value)
-            if ref:
+            if ref := self.resolve_ref(value):
                 for target in node.targets:
                     self.scopes[get_name_repr(target)] = ref
         elif isinstance(value, Call):
-            result = self.visit_Call(value)
-            if result is not _NoCall:
+            if (result := self.visit_Call(value)) is not _NoCall:
                 for target in node.targets:
                     self.scopes[get_name_repr(target)] = result  # noq
 
     def visit_Call(self, node: Call):
-        func = self.resolve_ref(node.func)
-        if func:
+        if func := self.resolve_ref(node.func):
             return func(node, node, self.get_tracked_refs())
         return _NoCall
 
 
 class TrackedRef:
     __slots__ = ('module', 'name')
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/core.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,15 @@
         **kwargs,
     ) -> CommandCls:
         metadata = {k: v for k, v in ((k, kwargs.pop(k)) for k in META_KEYS.intersection(kwargs)) if v}
         namespace['_CommandMeta__params'] = None  # Prevent commands from inheriting parent params
         namespace['_CommandMeta__metadata'] = None  # Prevent commands from inheriting parent metadata directly
         namespace['_CommandMeta__parents'] = None  # Prevent commands from inheriting parents directly
 
-        config = mcs._prepare_config(bases, config, kwargs)
-        if config:
+        if config := mcs._prepare_config(bases, config, kwargs):
             namespace['_CommandMeta__config'] = config
 
         cls = super().__new__(mcs, name, bases, namespace, **kwargs)
         mcs._commands.add(cls)
         mcs._maybe_register_sub_cmd(cls, bases, choice, choices, help)
         if metadata:  # If no overrides were provided, then initialize lazily later
             cls.__metadata = ProgramMetadata.for_command(cls, parent=mcs._from_parent(mcs.meta, bases), **metadata)
@@ -94,42 +93,37 @@
     @classmethod
     def _maybe_register_sub_cmd(
         mcs, cls, bases: Bases, choice: str = None, choices: Choices = None, help: str = None  # noqa
     ):
         if ABC in bases:
             return
         has_both = choices or choice is not None
-        parent = mcs.parent(cls, False)
-        if parent:
-            sub_cmd = mcs.params(parent).sub_command
-            if sub_cmd:
+        if parent := mcs.parent(cls, False):
+            if sub_cmd := mcs.params(parent).sub_command:
                 for choice, choice_help in _choice_items(choice, choices):
                     sub_cmd.register_command(choice, cls, choice_help or help)
             elif has_both:
-                warn(
-                    f'choices={choices} were not registered for {cls} because'
-                    f' its parent={parent!r} has no SubCommand parameter'
-                )
+                warn(f'{choices=} were not registered for {cls} because its {parent=} has no SubCommand parameter')
         elif has_both:
-            warn(f'choices={choices} were not registered for {cls} because it has no parent Command')
+            warn(f'{choices=} were not registered for {cls} because it has no parent Command')
 
     @classmethod
     def _from_parent(mcs, meth: Callable[[CommandCls], T], bases: Bases) -> Optional[T]:
         for base in bases:
             if isinstance(base, mcs):
                 return meth(base)
         return None
 
     # region Config Methods
 
     @classmethod
     def _prepare_config(mcs, bases: Bases, config: AnyConfig, kwargs: Dict[str, Any]) -> Config:
         if config is not None:
             if kwargs:
-                raise CommandDefinitionError(f'Cannot combine config={config!r} with keyword config arguments={kwargs}')
+                raise CommandDefinitionError(f'Cannot combine {config=} with keyword config arguments={kwargs}')
             elif isinstance(config, CommandConfig):
                 return config
             kwargs = config  # It was a dict
 
         parent_config = mcs._from_parent(mcs.config, bases)
         if kwargs or (not parent_config and ABC not in bases):
             cfg_kwargs = {k: kwargs.pop(k) for k in CommandConfig.FIELDS.intersection(kwargs)}
@@ -187,16 +181,15 @@
             parent = mcs.parent(cls, True)
             parent_params = mcs.params(parent) if parent is not None else None
             cls.__params = params = CommandParameters(cls, parent, parent_params, mcs.config(cls, DEFAULT_CONFIG))
         return params
 
     @classmethod
     def meta(mcs, cls: CommandCls, no_sys_argv: Bool = False) -> ProgramMetadata:
-        meta = cls.__metadata
-        if not meta:
+        if not (meta := cls.__metadata):
             parent_meta = mcs._from_parent(mcs.meta, type.mro(cls)[1:])
             cls.__metadata = meta = ProgramMetadata.for_command(cls, parent=parent_meta, no_sys_argv=no_sys_argv)
         return meta
 
 
 def _mro(cmd_cls):
     try:
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/documentation.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/documentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,31 +86,29 @@
     """
     with Context(allow_argv_prog=False):
         module = import_module(path)
     commands = {key: val for key, val in module.__dict__.items() if not key.startswith('__') and _is_command(val)}
     if top_only:
         commands = top_level_commands(commands)
 
-    doc_str = module.__doc__
-    if doc_str:
+    if doc_str := module.__doc__:
         for command in commands.values():
             get_metadata(command).pkg_doc_str = doc_str
 
     return commands
 
 
 def top_level_commands(commands: Commands) -> Commands:
     """Filter the given commands to only the ones that do not have a parent present in the provided dict of commands"""
     if len(commands) <= 1:
         return commands
 
     indirect_parents = defaultdict(set)
     for name, command in commands.items():
-        sub_command = get_params(command).sub_command
-        if sub_command:
+        if sub_command := get_params(command).sub_command:
             for choice in sub_command.choices.values():
                 indirect_parents[choice.target].add(command)
 
     all_commands = set(commands.values())
 
     filtered = {}
     for name, command in commands.items():
@@ -234,15 +232,17 @@
         index_subdir: str = None,
         caption: str = None,
         **kwargs,
     ):
         names = [self.document_script(path, subdir, top_only=top_only, **kwargs) for path in paths]
         if index_name or index_header or index_subdir:
             name = index_name or subdir
-            self.write_index(name, index_header or name.title(), names, subdir, caption, index_subdir)
+            self.write_index(
+                name, index_header or name.title(), names, content_subdir=subdir, caption=caption, subdir=index_subdir
+            )
 
     def document_module(self, module: str, subdir: str = None):
         """
         Generate an RST file to document a Python module.
 
         :param module: The name of the module that should be documented, using ``package.module`` notation.
         :param subdir: If specified, write RST output for the specified module in this subdirectory, relative to the
@@ -259,49 +259,58 @@
         subdir: str = None,
         *,
         name: str = None,
         header: str = None,
         index: Bool = True,
         empty: Bool = False,
         caption: str = None,
+        max_depth: int = 4,
     ) -> List[str]:
         """
         :param pkg_name: The name of the package to document
         :param pkg_path: The path to the package
         :param subdir: The output subdirectory for package contents
         :param name: The name to use for the index file
         :param header: Header text to use in the index (default is based on the package name)
         :param index: Whether the index file should be created
         :param empty: Whether an index file should be created if the package had no modules to document
         :param caption: A caption to use for the index
+        :param max_depth: The maximum depth of the table of contents tree.  Use ``-1`` to allow unlimited depth.
         :return: List of the names from the contents of the package
         """
         if name:
             index_subdir = content_subdir = f'{subdir}/{name}' if subdir else name
         else:
             index_subdir = None
             content_subdir = subdir
 
-        contents = self._generate_code_rsts(pkg_name, pkg_path, content_subdir)
+        contents = self._generate_code_rsts(pkg_name, pkg_path, content_subdir, max_depth=max_depth)
         if (not contents and not empty) or not index:
             return contents
 
         if not header:
-            header = '{} Package'.format(pkg_name.split('.')[-1].title())
+            header = f'{pkg_name.split(".")[-1].title()} Package'
 
-        self.write_index(name or pkg_name, header, contents, index_subdir, caption=caption, subdir=subdir)
+        self.write_index(
+            name=name or pkg_name,
+            header=header,
+            contents=contents,
+            content_subdir=index_subdir,
+            caption=caption,
+            subdir=subdir,
+            max_depth=max_depth,
+        )
         return contents
 
-    def _generate_code_rsts(self, pkg_name: str, pkg_path: Path, subdir: str = None) -> List[str]:
+    def _generate_code_rsts(self, pkg_name: str, pkg_path: Path, subdir: str = None, max_depth: int = 4) -> List[str]:
         contents = []
         for path in pkg_path.iterdir():
             if path.is_dir():
                 sub_pkg_name = f'{pkg_name}.{path.name}'
-                pkg_modules = self.document_package(sub_pkg_name, path, subdir)
-                if pkg_modules:
+                if self.document_package(sub_pkg_name, path, subdir, max_depth=max_depth):
                     contents.append(sub_pkg_name)
             elif path.is_file() and path.suffix == '.py' and not path.name.startswith('__'):
                 name = f'{pkg_name}.{path.stem}'
                 if name in self.skip_modules:
                     continue
                 contents.append(name)
                 self.document_module(name, subdir)
@@ -309,27 +318,44 @@
         return contents
 
     def write_index(
         self,
         name: str,
         header: str,
         contents: Strings,
+        *,
         content_subdir: str = None,
-        caption: str = None,
         subdir: str = None,
+        caption: str = None,
+        max_depth: int = 4,
+        **kwargs,
     ):
+        """
+        Write an RST index file with a table of contents that references one or more other documents.
+
+        :param name: The file name to use when saving this index.
+        :param header: The name of the index document.  Written as a header above the ``toctree`` directive.
+        :param contents: The names of the documents to include in the table of contents for this index.
+        :param content_subdir: The subdirectory that contains the RST files referenced by ``contents``, if any / not
+          included in the ``contents`` values already.
+        :param subdir: The output subdirectory to use when writing this index, if any.
+        :param caption: A caption to use for the index
+        :param max_depth: The maximum depth of the table of contents tree.  Use ``-1`` to allow unlimited depth.
+        :param kwargs: Additional keyword arguments to be included as ``:key: <value>`` options to the ``toctree``
+          directive.
+        """
         content_fmt = '    {}' if content_subdir is None else f'    {content_subdir}/{{}}'
-        rendered = rst_toc_tree(header, content_fmt, contents, caption=caption)
+        rendered = rst_toc_tree(header, content_fmt, contents, caption=caption, max_depth=max_depth, **kwargs)
         self.write_rst(name, rendered, subdir)
 
     def write_rst(self, name: str, content: str, subdir: str = None):
         target_dir = self.output_dir.joinpath(subdir) if subdir else self.output_dir
         if not self.dry_run and not target_dir.exists():
             target_dir.mkdir(parents=True)
 
         prefix = '[DRY RUN] Would write' if self.dry_run else 'Writing'
         path = target_dir.joinpath(name + self.ext)
         log.debug(f'{prefix} {path.as_posix()}')
         if not self.dry_run:
-            # Path.write_text on 3.7 does not support `newline`
+            # Path.write_text on 3.8 does not support `newline`
             with path.open('w', encoding=self.encoding, newline=self.newline) as f:
                 f.write(content)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/error_handling.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
 class CommandParserException(Exception):
     """Base class for all other Command Parser exceptions"""
 
     code: int = 3
 
     def show(self) -> bool:
-        message = str(self)
-        if message:
+        if message := str(self):
             print(message, file=sys.stderr)
         return True
 
     def exit(self):
         self.show()
         sys.exit(self.code)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,16 +54,15 @@
 
     def format_usage(self, delim: str = ' ', sub_cmd_choice: str = None) -> str:
         meta = get_metadata(self.command)
         if meta.usage:
             return meta.usage
 
         params = self.params.all_positionals + self.params.options  # noqa
-        pass_thru = self.params.pass_thru
-        if pass_thru is not None:
+        if (pass_thru := self.params.pass_thru) is not None:
             params.append(pass_thru)
 
         parts = ['usage:', meta.prog]
         if sub_cmd_choice:
             parts.append(sub_cmd_choice)
         else:
             parts.extend(get_usage_sub_cmds(self.command))
@@ -77,63 +76,64 @@
         if meta.description:
             parts += [meta.description, '']
 
         for group in self.groups:
             if group.show_in_help:
                 parts.append(group.formatter.format_help())
 
-        epilog = meta.format_epilog(ctx.config.extended_epilog)
-        if epilog:
+        if epilog := meta.format_epilog(ctx.config.extended_epilog):
             parts.append(epilog)
 
         return '\n'.join(parts)
 
     def _format_rst(
         self, include_epilog: Bool = False, sub_cmd_choice: str = None, no_sys_argv: Bool = False
     ) -> Iterator[str]:
         """Generate the RST content for the specific Command associated with this formatter"""
         meta = get_metadata(self.command, no_sys_argv=no_sys_argv)
+        # TODO: Line wrap usage text?
         yield from ('::', '', '    ' + self.format_usage(sub_cmd_choice=sub_cmd_choice), '', '')
         if meta.description:
             yield meta.description
             yield ''
 
+        # TODO: The subcommand names in the group containing subcommand targets should link to their respective
+        #  subcommand sections
         for group in self.groups:
             if group.show_in_help:
                 table: RstTable = group.formatter.rst_table()  # noqa
                 yield from table.iter_build()  # noqa
 
-        if include_epilog:
-            epilog = meta.format_epilog(ctx.config.extended_epilog)
-            if epilog:
-                yield epilog
+        if include_epilog and (epilog := meta.format_epilog(ctx.config.extended_epilog)):
+            yield epilog
 
     def format_rst(
         self, fix_name: Bool = True, fix_name_func: NameFunc = None, init_level: int = 1, no_sys_argv: Bool = False
     ) -> str:
         """Generate the RST content for the Command associated with this formatter and all of its subcommands"""
         # TODO: Nested subcommands do not have full sections, but they should
         meta = get_metadata(self.command, no_sys_argv=no_sys_argv)
         name = meta.doc_name
+        # TODO: Usage name for subcommands seems to always be ``build_docs.py``
         if fix_name:
             name = fix_name_func(name) if fix_name_func else _fix_name(name)
 
+        # TODO: Use class docstring as description if no description is provided?
+
         parts = [rst_header(name, init_level), '']
-        if ctx.config.show_docstring:
-            doc_str = meta.get_doc_str()
-            if doc_str:
-                parts += [doc_str, '']
+        if ctx.config.show_docstring and (doc_str := meta.get_doc_str()):
+            parts += [doc_str, '']
 
         parts.append('')
         parts.extend(self._format_rst(True, no_sys_argv=no_sys_argv))
 
-        sub_command = get_params(self.command).sub_command
-        if sub_command and sub_command.show_in_help:
+        if (sub_command := get_params(self.command).sub_command) and sub_command.show_in_help:
             parts += ['', rst_header('Subcommands', init_level + 1), '']
             for cmd_name, choice in sub_command.choices.items():
+                # TODO: Config to disable inherited docstring/description from being printed for each subcommand
                 parts += ['', rst_header(f'Subcommand: {cmd_name}', init_level + 2), '']
                 if choice.help:
                     parts += [choice.help, '']
 
                 try:
                     formatter = get_formatter(choice.target)
                 except TypeError:  # choice.target is None (it is the default choice, pointing back to the same Command)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,15 @@
         except KeyError:
             return text
 
     def format_metavar(self) -> str:
         param = self.param
         if param.metavar:
             return param.metavar
-        t = param.type
-        if t is not None:
+        if (t := param.type) is not None:
             try:
                 config = ctx.config
                 metavar = t.format_metavar(config.choice_delim, config.sort_choices)
             except Exception:  # noqa  # pylint: disable=W0703
                 pass
             else:
                 if metavar is not NotImplemented:
@@ -180,16 +179,15 @@
             return f'{primary} | {alts}'
         else:
             return f'{opts.get_usage_opt(False)} | {opts.get_usage_opt(True)}'
 
     def format_description(self, rst: Bool = False, alt: bool = False) -> str:
         if not alt:
             return super().format_description(rst=rst)
-        alt_help = self.param.alt_help
-        if alt_help:
+        if alt_help := self.param.alt_help:
             return super().format_description(rst=rst, description=alt_help)
         return ''
 
     def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
         opts = self.param.option_strs
         primary = format_help_entry(opts.primary_option_strs(), self.format_description(), prefix, tw_offset)
         alt_desc = self.format_description(alt=True)
@@ -293,16 +291,15 @@
             except KeyError:
                 target_choice_map[key] = cls(choice)
 
         return target_choice_map.values()
 
     def add(self, choice: Choice):
         self.choices.append(choice)
-        choice_str = choice.choice
-        if choice_str:
+        if choice_str := choice.choice:
             self.choice_strs.append(choice_str)
 
     def format(self, default_mode: SubcommandAliasHelpMode, tw_offset: int = 0, prefix: str = '') -> Iterator[str]:
         """
         :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured.
         :param tw_offset: Terminal width offset for text width calculations.
         :param prefix: Prefix to add to every line (primarily intended for use with nested groups).
@@ -317,19 +314,18 @@
         mode.
 
         :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured.
         :return: Generator that yields 3-tuples containing the :class:`.Choice` object, the choice string value, and
           the help text / description for that choice / alias.
         """
         first = self.choices[0]
-        config = get_config(first.target)
         # If it's not a Command, get_config will return None.  If it is a Command, then it will use its config.  If the
         # alias mode is not set on that target Command, but it is set on its parent, then this will use that parent's
         # setting.
-        if config:
+        if config := get_config(first.target):
             mode = config.cmd_alias_mode or default_mode
         else:
             mode = default_mode
 
         if mode == SubcommandAliasHelpMode.ALIAS:
             yield from self.prepare_aliases()
         elif mode == SubcommandAliasHelpMode.REPEAT:
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,23 @@
     yield ''
     yield from _rst_directive('toctree', options=options, check=True)
     yield ''
     yield from map(content_fmt.format, sorted(contents))
 
 
 def rst_toc_tree(name: str, content_fmt: str, contents: Strings, max_depth: int = 4, **kwargs) -> str:
+    """
+    :param name: The name of the section.  Written as a header above the ``toctree`` directive.
+    :param content_fmt: The format string used to indent/prefix each entry in the contents to include in this table
+      of contents.
+    :param contents: The names of the documents to include in this table of contents.
+    :param max_depth: The maximum depth of the table of contents tree.  Use ``-1`` to allow unlimited depth.
+    :param kwargs: Keyword arguments to be included as ``:key: <value>`` options to the ``toctree`` directive.
+    :return: The RST header and table of contents directive as a string.
+    """
     return '\n'.join(_rst_toc_tree(name, content_fmt, contents, max_depth, **kwargs))
 
 
 def rst_list_table(data: Dict[str, str], value_pad: int = 20) -> str:
     max_key = max(map(len, data))
     max_val = max(map(len, data.values()))
     widths = f'{max_key} {max_val + value_pad}'
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,15 @@
     'Day', 'Month', 'TimeDelta', 'DateTime', 'Date', 'Time', 'DTFormatMode',
     'normalize_input_type',
 ]
 # fmt: on
 
 
 def normalize_input_type(type_func: InputTypeFunc, param_choices: ChoicesType) -> _t.Optional[TypeFunc]:
-    choices_provided = param_choices is not None
-    if choices_provided:
+    if choices_provided := param_choices is not None:
         if not param_choices:
             raise _ParameterDefinitionError(
                 f'Invalid choices={param_choices!r} - when specified, choices cannot be empty'
             )
         elif isinstance(param_choices, range):
             return Range(param_choices, type_func)
         elif isinstance(type_func, (Range, range)):
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/choices.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 if TYPE_CHECKING:
     from ..typing import Bool
 
 __all__ = ['Choices', 'ChoiceMap', 'EnumChoices']
 
 EnumT = TypeVar('EnumT', bound=Enum)
 
+# TODO: Add support for input validation based on regex or fnmatch pattern
+
 
 class _ChoicesBase(InputType[T], ABC):
     choices: Collection[T]
     type: Optional[TypeFunc] = None
     case_sensitive: bool = True
 
     def __contains__(self, value: str) -> bool:
@@ -68,15 +70,15 @@
 
         raise InvalidChoiceError(value, self.choices)
 
     def format_metavar(self, choice_delim: str = ',', sort_choices: bool = False) -> str:
         choices = map(str, self.choices)
         if sort_choices:
             choices = sorted(choices)
-        return '{{{}}}'.format(choice_delim.join(choices))
+        return f'{{{choice_delim.join(choices)}}}'
 
 
 class Choices(_ChoicesBase[T]):
     """
     Validates that values are members of the collection of allowed values.
 
     :param choices: A collection of choices allowed for a given Parameter.
@@ -84,17 +86,17 @@
       a single string argument.
     :param case_sensitive: Whether choices should be case-sensitive.  Defaults to True.  If the choices values are not
       all strings, then this cannot be set to False.
     """
 
     def __init__(self, choices: Collection[T], type: TypeFunc = None, case_sensitive: Bool = True):  # noqa
         if not case_sensitive and not all(isinstance(c, str) for c in choices):
-            raise TypeError(f'Cannot combine case_sensitive=False with non-str choices={choices}')
+            raise TypeError(f'Cannot combine case_sensitive=False with non-str {choices=}')
         elif isinstance(type, EnumChoices) and not any(isinstance(c, type.enum) for c in choices):
-            raise TypeError(f'Invalid choices={choices} for type={type}')
+            raise TypeError(f'Invalid {choices=} for {type=}')
 
         self.choices = choices
         self.type = type
         self.case_sensitive = case_sensitive
 
     def _choices_repr(self, delim: str = ',') -> str:
         return delim.join(map(repr, sorted(self.choices)))
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         encoding: str = None,
         errors: str = None,
         lazy: Bool = True,
         parents: Bool = False,
         **kwargs,
     ):
         if not lazy and allows_write(mode):
-            raise ValueError(f'Cannot combine mode={mode!r} with lazy=False for {self.__class__.__name__}')
+            raise ValueError(f'Cannot combine {mode=} with lazy=False for {self.__class__.__name__}')
         if not allows_write(mode):
             kwargs.setdefault('exists', True)
         kwargs.setdefault('type', StatMode.FILE)
         super().__init__(**kwargs)
         self.mode = mode
         self.encoding = encoding
         self.errors = errors
@@ -206,14 +206,14 @@
     :param kwargs: Additional keyword arguments to pass to :class:`.File`
     """
 
     def __init__(self, *, mode: str = 'rb', **kwargs):
         import pickle
 
         if 't' in mode:
-            raise ValueError(f'Invalid mode={mode!r} - pickle does not read/write text')
+            raise ValueError(f'Invalid {mode=} - pickle does not read/write text')
         if 'b' not in mode:
             mode += 'b'
 
         write = allows_write(mode, True)
         kwargs['pass_file'] = True
         super().__init__(pickle.dump if write else pickle.load, mode=mode, **kwargs)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/numeric.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}({self.range!r}, snap={self.snap!r}, type={self.type!r})>'
 
     def _range_str(self, var: str = 'N') -> str:
         rng_min, rng_max = min(self.range), max(self.range)
         step = abs(self.range.step)
         base = f'{rng_min} <= {var} <= {rng_max}'
-        return base if step == 1 else f'{base}, step={step}'
+        return base if step == 1 else f'{base}, {step=}'
 
     def __call__(self, value: str) -> NT:
         value = self.type(value)
         if value in self.range:
             return value
         elif self.snap:
             rng_min = min(self.range)
@@ -131,30 +131,30 @@
         max: Number = None,  # noqa
         include_min: Bool = True,
         include_max: Bool = False,
     ):
         if min is None and max is None:
             raise ValueError('NumRange inputs must be initialized with at least one of min and/or max values')
         elif min is not None and max is not None and min >= max:
-            raise ValueError(f'Invalid min={min} >= max={max} - min must be less than max')
+            raise ValueError(f'Invalid {min=} >= {max=} - min must be less than max')
 
         if type is None:
             self.type = float if isinstance(min, float) or isinstance(max, float) else int
         else:
             self.type = type
 
         if snap:
             if self.type is float:
                 raise TypeError('Unable to snap to extrema with type=float')
             real_min = min if include_min else min + 1
             real_max = max if include_max else max - 1
             if real_min >= real_max:
                 raise ValueError(
-                    f'Invalid min={min} >= max={max} with snap=True, include_min={include_min},'
-                    f' include_max={include_max} - snap would produce invalid values'
+                    f'Invalid {min=} >= {max=} with snap=True, {include_min=},'
+                    f' {include_max=} - snap would produce invalid values'
                 )
 
         self.snap = snap
         self.min = self.type(min) if min is not None else min   # for floats especially, such as a range like 0~1, this
         self.max = self.type(max) if max is not None else max   # helps to highlight the type in reprs
         self.include_min = include_min
         self.include_max = include_max
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,28 +323,28 @@
             raise ValueError(f'Invalid numeric weekday={value!r}') from e
 
         if 1 <= month <= 12:
             return month
 
         with different_locale(self.locale):
             raise InputValidationError(
-                f'Invalid month={month} - expected a value between 1 ({month_name[1]}) and 12 ({month_name[12]})'
+                f'Invalid {month=} - expected a value between 1 ({month_name[1]}) and 12 ({month_name[12]})'
             )
 
 
 # endregion
 
 
 class TimeDelta(InputType[timedelta]):
     __slots__ = ('unit',)
 
     def __init__(self, unit: TimeUnit):
         unit = unit.lower()
         if unit not in _TIMEDELTA_UNITS:
-            raise TypeError(f'Invalid unit={unit!r} - expected one of: {", ".join(sorted(_TIMEDELTA_UNITS))}')
+            raise TypeError(f'Invalid {unit=} - expected one of: {", ".join(sorted(_TIMEDELTA_UNITS))}')
         self.unit = unit
         # TODO: min/max params like NumRange?
 
     def __call__(self, value: Union[str, int, float]) -> timedelta:
         if isinstance(value, str):
             try:
                 value = float(value.replace(',', '').replace('_', ''))  # allow comma or _ between thousands
@@ -529,10 +529,10 @@
         return now + value
     elif isinstance(value, date):
         return datetime.combine(value, time())
     elif isinstance(value, time):
         today = date.today() if now is None else now.date()
         return datetime.combine(today, value)
     raise TypeError(
-        f'Unexpected datetime specifier type={value.__class__.__name__} for value={value!r}'
+        f'Unexpected datetime specifier type={value.__class__.__name__} for {value=}'
         ' (expected datetime, date, time, timedelta, or None)'
     )
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/metadata.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,31 +142,27 @@
         return _repr(self)
 
     def format_epilog(self, extended: Bool = True) -> str:
         parts = [self.epilog] if self.epilog else []
         if parts and not extended:
             return parts[0]
 
-        version = self.version
-        if version:
+        if version := self.version:
             version = f' [ver. {version}]'
         if self.email:
             parts.append(f'Report {self.prog}{version} bugs to {self.email}')
-        url = self.docs_url or self.url
-        if url:
+        if url := self.docs_url or self.url:
             parts.append(f'Online documentation: {url}')
         return '\n\n'.join(parts)
 
     def get_doc_str(self, strip: bool = True) -> OptStr:
-        doc_str = self.pkg_doc_str
-        if doc_str and strip:
+        if (doc_str := self.pkg_doc_str) and strip:
             doc_str = doc_str.strip()
         if not doc_str:
-            doc_str = self.doc_str
-            if doc_str and strip:
+            if (doc_str := self.doc_str) and strip:
                 doc_str = doc_str.strip()
         return doc_str
 
 
 def _repr(obj, indent=0) -> str:
     if not isinstance(obj, ProgramMetadata):
         return repr(obj)
@@ -205,30 +201,28 @@
         parent: Optional[ProgramMetadata],
         no_sys_argv: Bool,
         command: CommandType,
     ) -> Tuple[OptStr, str]:
         if prog:
             return prog, 'class kwargs'
 
-        ep_name = self._from_entry_point(command)
         # TODO: This isn't working for documentation generation...
-        if ep_name:
+        if ep_name := self._from_entry_point(command):
             return ep_name, 'entry_points'
 
         if no_sys_argv is None:
             try:
                 no_sys_argv = not ctx.allow_argv_prog
             except NoActiveContext:
                 no_sys_argv = False
 
         if parent and parent.prog != parent.path.name and (not no_sys_argv or parent.prog_src != 'sys.argv'):
             return parent.prog, parent.prog_src
         elif not no_sys_argv:
-            argv_name = self._from_sys_argv()
-            if argv_name:
+            if argv_name := self._from_sys_argv():
                 return argv_name, 'sys.argv'
 
         return cmd_path.name, 'path'
 
     def _from_entry_point(self, command: CommandType) -> OptStr:
         main_mod = 'cli_command_parser.commands'
         for prog, obj, obj_mod, obj_name in self._iter_entry_point_candidates(command):
@@ -239,15 +233,15 @@
 
     def _iter_entry_point_candidates(self, command: CommandType):
         try:
             # TODO: This likely won't work for a base command in one module, sub commands defined in separate modules,
             #  and main imported from cli_command_parser in the package's __init__/__main__ module...
             obj_prog_map = self.mod_obj_prog_map[command.__module__]
             module = modules[command.__module__]
-        except KeyError as e:
+        except KeyError:
             pass
         else:
             for obj_name, prog in obj_prog_map.items():
                 base_name = obj_name.split('.', 1)[0]
                 try:
                     obj = getattr(module, base_name)
                 except AttributeError:
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/nargs.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/nargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,25 +37,25 @@
     variable: bool
 
     def __init__(self, nargs: NargsValue):  # pylint: disable=R0912
         self._orig = nargs
         self.range = None
         if isinstance(nargs, int):
             if nargs < 0:
-                raise ValueError(f'Invalid nargs={nargs!r} integer - must be >= 0')
+                raise ValueError(f'Invalid {nargs=} integer - must be >= 0')
             self.min = self.max = nargs
             self.allowed = (nargs,)
         elif isinstance(nargs, str):
             try:
                 self.min, self.max = self.allowed = NARGS_STR_RANGES[nargs]
             except KeyError as e:
-                raise ValueError(f'Invalid nargs={nargs!r} string - expected one of ?, *, or +') from e
+                raise ValueError(f'Invalid {nargs=} string - expected one of ?, *, or +') from e
         elif isinstance(nargs, range):
             if not 0 <= nargs.start < nargs.stop or nargs.step < 0:
-                raise ValueError(f'Invalid nargs={nargs!r} range - expected positive step and 0 <= start < stop')
+                raise ValueError(f'Invalid {nargs=} range - expected positive step and 0 <= start < stop')
             self.range = nargs
             self.allowed = nargs
             self.min = nargs.start
             # As long as range.start < range.stop and range.step > 0, it will yield at least 1 value
             self.max = next(reversed(nargs))  # simpler than calculating, especially for step!=1
         elif isinstance(nargs, set):
             if not nargs:
@@ -77,15 +77,15 @@
             if not (isinstance(a, int) and (b in _UNBOUND or isinstance(b, int))):
                 raise TypeError(SEQ_ERROR_FMT.format(nargs))
             elif 0 > a or (b not in _UNBOUND and a > b):
                 raise ValueError(SEQ_ERROR_FMT.format(nargs))
         elif nargs is REMAINDER:
             self.min, self.max = self.allowed = (0, REMAINDER)
         else:
-            raise TypeError(f'Unexpected type={nargs.__class__.__name__} for nargs={nargs!r}')
+            raise TypeError(f'Unexpected type={nargs.__class__.__name__} for {nargs=}')
 
         self.variable = self.min != self.max
         self._has_upper_bound = self.max not in _UNBOUND
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self._orig!r})'
 
@@ -94,15 +94,15 @@
         if rng is not None:
             return f'{rng.start} ~ {rng.stop}' if rng.step == 1 else f'{rng.start} ~ {rng.stop} (step={rng.step})'
         elif not self._has_upper_bound:
             return f'{self.min} or more' if self.max is None else self.max.__class__.__name__
         elif self.min == self.max:
             return str(self.min)
         elif isinstance(self.allowed, frozenset):
-            return '{{{}}}'.format(','.join(map(str, sorted(self.allowed))))  # pylint: disable=C0209
+            return f'{{{",".join(map(str, sorted(self.allowed)))}}}'
         else:
             return f'{self.min} ~ {self.max}'
 
     def __contains__(self, num: int) -> bool:
         """See :meth:`.satisfied`"""
         return self.satisfied(num)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,22 +102,20 @@
 
     def __init__(self, name: str = None, required: Bool = False, help: str = None, hide: Bool = False):  # noqa
         self.__doc__ = help  # Prevent this class's docstring from showing up for params in generated documentation
         self.required = required
         self.name = name
         self.help = help
         self.hide = hide
-        group = get_active_param_group()
-        if group:
+        if group := get_active_param_group():
             group.register(self)  # noqa  # This sets self.group = group
 
     @property
     def name(self) -> str:
-        name = self._name
-        if name is not None:
+        if (name := self._name) is not None:
             return name
         return self._default_name()
 
     @name.setter
     def name(self, value: Optional[str]):
         if value is not None:
             self._name = value
@@ -255,19 +253,19 @@
         metavar: str = None,
         help: str = None,  # noqa
         hide: Bool = False,
         show_default: Bool = None,
     ):
         if action not in self._actions:
             raise ParameterDefinitionError(
-                f'Invalid action={action!r} for {self.__class__.__name__} - valid actions: {sorted(self._actions)}'
+                f'Invalid {action=} for {self.__class__.__name__} - valid actions: {sorted(self._actions)}'
             )
         if required and default is not _NotSet:
             raise ParameterDefinitionError(
-                f'Invalid combination of required=True with default={default!r} for {self.__class__.__name__} -'
+                f'Invalid combination of required=True with {default=} for {self.__class__.__name__} -'
                 ' required Parameters cannot have a default value'
             )
         super().__init__(name=name, required=required, help=help, hide=hide)
         self.action = action
         self.default = None if default is _NotSet and not required and self.nargs.max == 1 else default
         self.metavar = metavar
         if show_default is not None:
@@ -283,16 +281,15 @@
         if (
             not (choices or type_attr is None)
             or not self._config(command).allow_annotation_type
             or self.nargs.max is REMAINDER
         ):
             return
 
-        annotated_type = get_descriptor_value_type(command, name)
-        if annotated_type is None:
+        if (annotated_type := get_descriptor_value_type(command, name)) is None:
             return
         elif choices:
             type_attr.type = annotated_type
         else:  # self.type must be None
             # Choices present earlier would have already been converted
             self.type = normalize_input_type(annotated_type, None)
 
@@ -301,16 +298,15 @@
         type_attr = self.type
         return isinstance(type_attr, _ChoicesBase) and type_attr.choices
 
     # endregion
 
     def __repr__(self) -> str:
         attr_names = ('action', 'const', 'default', 'type', 'choices', 'required', 'hide', 'help')
-        extra_attrs = self._repr_attrs
-        if extra_attrs:
+        if extra_attrs := self._repr_attrs:
             attr_names = chain(attr_names, extra_attrs)
 
         attrs = ((a, getattr(self, a, None)) for a in attr_names)
         kwargs = ', '.join(f'{a}={v!r}' for a, v in attrs if v not in (None, _NotSet) and not (a == 'hide' and not v))
         return f'{self.__class__.__name__}({self.name!r}, {kwargs})'
 
     # region Argument Handling
@@ -326,16 +322,15 @@
     def __get__(self, command, owner):
         if command is None:
             return self
 
         with self._ctx(command):
             value = self.result()
 
-        name = self._name
-        if name is not None:
+        if (name := self._name) is not None:
             command.__dict__[name] = value  # Skip __get__ on subsequent accesses
         return value
 
     def _get_parsed_and_max_reached(self) -> Tuple[List[T_co], bool]:
         parsed = ctx.get_parsed_value(self)
         try:
             nargs_max_reached = len(parsed) >= self.nargs.max
@@ -377,30 +372,30 @@
         try:
             return type_func(value)
         except InvalidChoiceError as e:
             raise InvalidChoice(self, e.invalid, e.choices) from e
         except InputValidationError as e:
             raise BadArgument(self, str(e)) from e
         except (TypeError, ValueError) as e:
-            raise BadArgument(self, f'bad value={value!r} for type={type_func!r}: {e}') from e
+            raise BadArgument(self, f'bad {value=} for type={type_func!r}: {e}') from e
         except Exception as e:
-            raise BadArgument(self, f'unable to cast value={value!r} to type={type_func!r}') from e
+            raise BadArgument(self, f'unable to cast {value=} to type={type_func!r}') from e
 
     def validate(self, value: Optional[T_co]):
         if isinstance(value, str) and value.startswith('-'):
             if self.allow_leading_dash == AllowLeadingDash.NUMERIC:
                 if len(value) > 1 and not _is_numeric(value):
-                    raise BadArgument(self, f'invalid value={value!r}')
+                    raise BadArgument(self, f'invalid {value=}')
             elif self.allow_leading_dash == AllowLeadingDash.NEVER:
-                raise BadArgument(self, f'invalid value={value!r}')
+                raise BadArgument(self, f'invalid {value=}')
         elif value is None:
             if not self.accepts_none:
                 raise MissingArgument(self)
         elif not self.accepts_values:
-            raise BadArgument(self, f'does not accept values, but value={value!r} was provided')
+            raise BadArgument(self, f'does not accept values, but {value=} was provided')
 
     def is_valid_arg(self, value: Any) -> bool:
         try:
             self.validate(value)
         except (InvalidChoice, BadArgument, MissingArgument):
             return False
         else:
@@ -415,40 +410,37 @@
     def _fix_default_collection(self, values) -> Optional[T_co]:
         type_func = self.type
         if type_func is None or not isinstance(type_func, InputType) or not isinstance(values, (list, tuple, set)):
             return values
         return values.__class__(map(type_func.fix_default, values))
 
     def result_value(self) -> Optional[T_co]:
-        value = ctx.get_parsed_value(self)
-        if value is _NotSet:
+        if (value := ctx.get_parsed_value(self)) is _NotSet:
             if self.required:
                 raise MissingArgument(self)
             else:
                 return self._fix_default(self.default)
 
         if self.action == 'store':
             return value
 
         # action == 'append' or 'store_all'
         if not value:
-            default = self.default
-            if default is not _NotSet:
+            if (default := self.default) is not _NotSet:
                 if isinstance(default, Collection) and not isinstance(default, str):
                     value = self._fix_default_collection(default)
                 else:
                     value.append(self._fix_default(default))
 
         nargs = self.nargs
-        val_count = len(value)
-        if val_count == 0 and 0 not in nargs:
+        if (val_count := len(value)) == 0 and 0 not in nargs:
             if self.required:
                 raise MissingArgument(self)
         elif val_count not in nargs:
-            raise BadArgument(self, f'expected nargs={nargs!r} values but found {val_count}')
+            raise BadArgument(self, f'expected {nargs=} values but found {val_count}')
 
         return value
 
     result = result_value
 
     def can_pop_counts(self) -> List[int]:  # noqa
         return []
@@ -479,16 +471,15 @@
     def _init_value_factory(self):
         if self.action == 'append':
             return []
         return super()._init_value_factory()  # noqa
 
     @parameter_action
     def store(self: Parameter, value: T_co):
-        prev = ctx.get_parsed_value(self)
-        if prev is not _NotSet:
+        if (prev := ctx.get_parsed_value(self)) is not _NotSet:
             raise ParamUsageError(self, f'can only be specified once - found multiple values: {prev!r}, {value!r}')
         ctx.set_parsed_value(self, value)
 
     @parameter_action
     def append(self: Parameter, value: T_co):
         parsed, nargs_max_reached = self._get_parsed_and_max_reached()
         if nargs_max_reached:
@@ -500,27 +491,25 @@
     def _pre_pop_values(self: Parameter):
         if self.action != 'append' or not self.nargs.variable or self.type not in (None, str):
             return []
 
         return ctx.get_parsed_value(self)
 
     def can_pop_counts(self) -> List[int]:
-        values = self._pre_pop_values()
-        if not values:
+        if not (values := self._pre_pop_values()):
             return []
 
         n_values = len(values)
         return [i for i in range(1, n_values) if self.nargs.satisfied(n_values - i)]
 
     def _reset(self: Union[Parameter, BasicActionMixin]) -> List[str]:
         if self.action != 'append' or self.type not in (None, str):
             raise UnsupportedAction
 
-        values = ctx.get_parsed_value(self)
-        if not values:
+        if not (values := ctx.get_parsed_value(self)):
             return values
 
         ctx.set_parsed_value(self, self._init_value_factory())
         ctx._provided[self] = 0
         return values
 
     def pop_last(self: Union[Parameter, BasicActionMixin], count: int = 1) -> List[str]:
@@ -576,17 +565,15 @@
         if default_ok is not None:
             cls._default_ok = default_ok
 
     def __init__(self, action: str, *, required: Bool = True, default: Any = _NotSet, **kwargs):
         default_bad = not self._default_ok or 0 not in self.nargs
         if not required and default_bad:
             cls_name = self.__class__.__name__
-            raise ParameterDefinitionError(
-                f'All {cls_name} parameters must be required - invalid required={required!r}'
-            )
+            raise ParameterDefinitionError(f'All {cls_name} parameters must be required - invalid {required=}')
         elif default_bad and default is not _NotSet:
             cls_name = self.__class__.__name__
             raise ParameterDefinitionError(f"The 'default' arg is not supported for {cls_name} parameters")
         super().__init__(action, default=default, required=required, **kwargs)
 
 
 class BaseOption(Parameter[T_co], ABC):
@@ -634,27 +621,25 @@
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
         if not self.option_strs.name_mode:
             self.option_strs.name_mode = command.__class__.config(command).option_name_mode
         self.option_strs.update(name)
 
     def env_vars(self) -> Iterator[str]:
-        env_var = self.env_var
-        if env_var:
+        if env_var := self.env_var:
             if isinstance(env_var, str):
                 yield env_var
             else:
                 yield from env_var
 
 
 def get_active_param_group() -> Optional[ParamGroup]:
     try:
         return _group_stack.get()[-1]
     except (AttributeError, IndexError):
         return None
 
 
 def _validate_opt_strs(opt_strs: Collection[str]):
-    bad = ', '.join(opt for opt in opt_strs if not 0 < opt.count('-', 0, 3) < 3 or opt.endswith('-') or '=' in opt)
-    if bad:
+    if bad := ', '.join(opt for opt in opt_strs if not 0 < opt.count('-', 0, 3) < 3 or opt.endswith('-') or '=' in opt):
         msg = f"Bad option(s) - they must start with '--' or '-', may not end with '-', and may not contain '=': {bad}"
         raise ParameterDefinitionError(msg)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/choice_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,15 @@
     @classmethod
     def _validate_positional(cls, value: str, prefix: str = 'choice'):
         if not value or value.startswith('-'):
             raise cls._choice_validation_exc(
                 f"Invalid {cls.__name__} {prefix}={value!r} - may not be empty or start with '-'"
             )
 
-        bad = {c for c in value if (c in whitespace and c != ' ') or c not in printable}
-        if bad:
+        if bad := {c for c in value if (c in whitespace and c != ' ') or c not in printable}:
             raise cls._choice_validation_exc(f'Invalid {cls.__name__} {prefix}={value!r} - invalid characters: {bad}')
 
     def register_choice(self, choice: str, target: T = _NotSet, help: str = None):  # noqa
         self._validate_positional(choice)
         self._register_choice(choice, target, help)
 
     def _register_choice(
@@ -138,16 +137,16 @@
     ):
         try:
             existing = self.choices[choice]
         except KeyError:
             self.choices[choice] = Choice(choice, target, help, local)
             self._update_nargs()
         else:
-            prefix = 'Invalid default' if choice is None else f'Invalid choice={choice!r} for'
-            raise CommandDefinitionError(f'{prefix} target={target!r} - already assigned to {existing}')
+            prefix = 'Invalid default' if choice is None else f'Invalid {choice=} for'
+            raise CommandDefinitionError(f'{prefix} {target=} - already assigned to {existing}')
 
     def _no_choices_error(self) -> NoReturn:
         raise CommandDefinitionError(f'No choices were registered for {self}')
 
     # endregion
 
     # region Argument Handling
@@ -160,45 +159,36 @@
 
         ctx.get_parsed_value(self).extend(values)
         n_values = len(values)
         ctx.record_action(self, n_values - 1)  # - 1 because it was already called before dispatching to this method
         return n_values
 
     def validate(self, value: str):
-        choices = self.choices
-        if not choices:
+        if not (choices := self.choices):
             self._no_choices_error()
 
         values = (*ctx.get_parsed_value(self), value)
-        choice = ' '.join(values)
-        if choice in choices:
+        if (choice := ' '.join(values)) in choices:
             return
         elif len(values) > self.nargs.max:
             raise BadArgument(self, 'too many values')
         prefix = choice + ' '
         if not any(c.startswith(prefix) for c in choices if c):
             raise InvalidChoice(self, prefix[:-1], choices)
 
     def result_value(self) -> OptStr:
-        choices = self.choices
-        if not choices:
+        if not (choices := self.choices):
             self._no_choices_error()
-
-        values = ctx.get_parsed_value(self)
-        if not values:
+        if not (values := ctx.get_parsed_value(self)):
             if None in choices:
                 return None
             raise MissingArgument(self)
-
-        val_count = len(values)
-        if val_count not in self.nargs:
+        if (val_count := len(values)) not in self.nargs:
             raise BadArgument(self, f'expected nargs={self.nargs} values but found {val_count}')
-
-        choice = ' '.join(values)
-        if choice not in choices:
+        if (choice := ' '.join(values)) not in choices:
             raise InvalidChoice(self, choice, choices)
         return choice
 
     result = result_value
 
     def target(self) -> T:
         choice = self.result_value()
@@ -273,16 +263,15 @@
 
         try:
             self.register_choice(choice, command, help)
         except CommandDefinitionError:
             from ..core import get_parent
 
             parent = get_parent(command)
-            target = self.choices[choice].target
-            msg = f'Invalid choice={choice!r} for {command} with parent={parent!r} - already assigned to {target}'
+            msg = f'Invalid {choice=} for {command} with {parent=} - already assigned to {self.choices[choice].target}'
             raise CommandDefinitionError(msg) from None
 
         return command
 
     def register(
         self, command_or_choice: Union[str, CommandCls] = None, *, choice: str = None, help: str = None  # noqa
     ) -> Callable[[CommandCls], CommandCls]:
@@ -301,17 +290,15 @@
           ``choice`` string value.
         :param help: (Keyword-only) The help text / description to be displayed for this choice
         """
         if command_or_choice is None:
             return partial(self.register_command, choice, help=help)
         elif isinstance(command_or_choice, str):
             if choice is not None:
-                raise CommandDefinitionError(
-                    f'Cannot combine a positional command_or_choice={command_or_choice!r} choice with choice={choice!r}'
-                )
+                raise CommandDefinitionError(f'Cannot combine a positional {command_or_choice=} choice with {choice=}')
             return partial(self.register_command, command_or_choice, help=help)
         else:
             return self.register_command(choice, command_or_choice, help=help)  # noqa
 
     def _no_choices_error(self) -> NoReturn:
         raise CommandDefinitionError(f'{ctx.command}.{self.name} = {self} has no sub Commands')
 
@@ -374,17 +361,15 @@
         :return: The original method, unchanged.  When called explicitly, a
           `partial <https://docs.python.org/3/library/functools.html#functools.partial>`__ method will be returned
           first, which will automatically be called by the interpreter with the method to be decorated, and that call
           will return the original method.
         """
         if isinstance(method_or_choice, str):
             if choice is not None:
-                raise CommandDefinitionError(
-                    f'Cannot combine a positional method_or_choice={method_or_choice!r} choice with choice={choice!r}'
-                )
+                raise CommandDefinitionError(f'Cannot combine a positional {method_or_choice=} choice with {choice=}')
             method_or_choice, choice = None, method_or_choice
 
         if method_or_choice is None:
             return partial(self.register_action, choice, help=help, default=default)
         else:
             return self.register_action(choice, method_or_choice, help=help, default=default)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,18 +74,15 @@
         return f'{self.__class__.__name__}#{self._num:06d}'
 
     # region Boilerplate Methods
 
     def __repr__(self) -> str:
         exclusive, dependent = str(self.mutually_exclusive)[0], str(self.mutually_dependent)[0]
         members = len(self.members)
-        return (
-            f'<{self.__class__.__name__}[{self.name!r},'
-            f' members={members!r}, m.exclusive={exclusive}, m.dependent={dependent}]>'
-        )
+        return f'<{self.__class__.__name__}[{self.name!r}, {members=}, m.{exclusive=!s}, m.{dependent=!s}]>'
 
     def __hash__(self) -> int:
         return super().__hash__()
 
     def __eq__(self, other: ParamGroup) -> bool:
         if isinstance(other, ParamGroup) and self.group == other.group:
             attrs = ('mutually_exclusive', 'mutually_dependent', 'name', 'description', 'members')
@@ -149,19 +146,19 @@
         self.members.extend(params)
 
     def register(self, param: ParamOrGroup):
         if self.mutually_exclusive:
             if (isinstance(param, BasePositional) and 0 not in param.nargs) or isinstance(param, PassThru):
                 cls_name = param.__class__.__name__
                 raise CommandDefinitionError(
-                    f'Cannot add param={param!r} to {self} - {cls_name} parameters cannot be mutually exclusive'
+                    f'Cannot add {param=} to {self} - {cls_name} parameters cannot be mutually exclusive'
                 )
             elif isinstance(param, BaseOption) and param.required:
                 raise CommandDefinitionError(
-                    f'Cannot add param={param!r} to {self} - required parameters cannot be mutually exclusive'
+                    f'Cannot add {param=} to {self} - required parameters cannot be mutually exclusive'
                     ' (but the group can be required)'
                 )
 
         self.members.append(param)
         param.group = self
 
     def register_all(self, params: Iterable[ParamOrGroup]):
@@ -204,16 +201,15 @@
             be = 'was' if len(provided) == 1 else 'were'
             raise ParamsMissing(missing, f'because {p_str} {be} provided')
         elif self.mutually_exclusive and not 0 <= len(provided) < 2:
             raise ParamConflict(provided, 'they are mutually exclusive - only one is allowed')
 
     @property
     def in_mutually_exclusive_group(self) -> bool:
-        parent = self.group
-        if not parent:
+        if not (parent := self.group):
             return False
         return parent.mutually_exclusive
 
     def validate(self):
         """
         Validate mutual dependency / exclusivity of members and that required members have been provided when they are
         expected to be (based on mutual dependence/exclusivity and nesting).
@@ -227,16 +223,15 @@
         self._check_conflicts(provided, missing)
         if not missing:
             return
         req_any, req_all = self._classify_required()
         if not provided and req_any:
             raise ParamsMissing(missing, partial=not req_all)
         elif provided or not self.in_mutually_exclusive_group:
-            req_missing = [p for p in missing if p.required]
-            if req_missing:
+            if req_missing := [p for p in missing if p.required]:
                 raise ParamsMissing(req_missing)
 
     def _classify_required(self) -> Tuple[bool, bool]:
         """Returns a tuple of (req_any, req_all)"""
         if self.mutually_dependent and (self.required or any(p.required for p in self.members)):
             return True, True
         elif self.required:
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/option_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     _short: Set[str]
 
     def __init__(self, option_strs: Collection[str], name_mode: Union[OptionNameMode, str, None] = _NotSet):
         self.name_mode = OptionNameMode(name_mode) if name_mode is not _NotSet else None
         self._display_long = self._long = {opt for opt in option_strs if opt.startswith('--')}
         self._short = short_opts = {opt for opt in option_strs if 1 == opt.count('-', 0, 2)}
         self.combinable = {opt[1:] for opt in short_opts if len(opt) == 2}
-        bad_opts = ', '.join(opt for opt in short_opts if '-' in opt[1:])
-        if bad_opts:
+        if bad_opts := ', '.join(opt for opt in short_opts if '-' in opt[1:]):
             raise ParameterDefinitionError(f"Bad short option(s) - may not contain '-': {bad_opts}")
 
     def __repr__(self) -> str:
         options = ', '.join(self.all_option_strs())
         return f'<{self.__class__.__name__}[name_mode={self.name_mode}][{options}]>'
 
     def has_long(self) -> Bool:
@@ -130,16 +129,15 @@
             self._long.add(option)
             if mode_val & 8:  # OptionNameMode.BOTH_UNDERSCORE = OptionNameMode.DASH | 4 | 8
                 self._display_long.add(option)
 
     @property
     def alt_allowed(self) -> Set[str]:
         allowed = set(self._alt_long)
-        short = self._alt_short
-        if short:
+        if short := self._alt_short:
             allowed.add(short)
             allowed.add(short[1:])
         return allowed
 
     # @property
     # def long_primary(self) -> List[str]:
     #     return [opt for opt in self.long if opt not in self._alt_long]
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,19 @@
         if nargs is not None:
             self.nargs = Nargs(nargs)
         if 0 in self.nargs:
             details = 'use Flag or Counter for Options with 0 args'
             if isinstance(nargs, range) and nargs.start == 0 and nargs.step != nargs.stop:
                 suffix = f', {nargs.step}' if nargs.step != 1 else ''
                 details = f'try using range({nargs.step}, {nargs.stop}{suffix}) instead, or {details}'
-            raise ParameterDefinitionError(f'Invalid nargs={nargs!r} - {details}')
+            raise ParameterDefinitionError(f'Invalid {nargs=} - {details}')
         if action is _NotSet:
             action = 'store' if self.nargs == 1 else 'append'
         elif action == 'store' and self.nargs != 1:
-            raise ParameterDefinitionError(f'Invalid nargs={self.nargs} for action={action!r}')
+            raise ParameterDefinitionError(f'Invalid nargs={self.nargs} for {action=}')
         super().__init__(*option_strs, action=action, default=default, required=required, **kwargs)
         self.type = normalize_input_type(type, choices)
         self._validate_nargs_and_allow_leading_dash(allow_leading_dash)
 
 
 class _Flag(BaseOption[T_co], ABC):
     nargs = Nargs(0)
@@ -138,21 +138,21 @@
                 return self.take_env_var_action(value, env_var)
             except ParamUsageError as e:
                 if not self.strict_env:
                     log.warning(e)
                     return
                 raise
 
-        raise ParamUsageError(self, f'received value={value!r} but no values are accepted for action={self.action!r}')
+        raise ParamUsageError(self, f'received {value=} but no values are accepted for action={self.action!r}')
 
     def prepare_env_var_value(self, value: str, env_var: str) -> T_co:
         try:
             return self.type(value)
         except Exception as e:
-            raise ParamUsageError(self, f'unable to parse value={value!r} from env_var={env_var!r}: {e}') from e
+            raise ParamUsageError(self, f'unable to parse {value=} from {env_var=}: {e}') from e
 
     @abstractmethod
     def take_env_var_action(self, value: str, env_var: str):
         raise NotImplementedError
 
     def would_accept(self, value: Optional[str], short_combo: bool = False) -> bool:  # noqa
         return value is None
@@ -201,29 +201,29 @@
         self, *option_strs: str, action: str = 'store_const', default: TD = _NotSet, const: TC = _NotSet, **kwargs
     ):
         if const is _NotSet:
             try:
                 const = self.__default_const_map[default]
             except KeyError as e:
                 cls = self.__class__.__name__
-                raise ParameterDefinitionError(f"Missing parameter='const' for {cls} with default={default!r}") from e
+                raise ParameterDefinitionError(f"Missing parameter='const' for {cls} with {default=}") from e
         if default is _NotSet:
             default = self.__default_const_map.get(const)  # will be True, False, or None
         if default is False:  # Avoid surprises for custom non-truthy values
             kwargs.setdefault('show_default', False)
         super().__init__(*option_strs, action=action, default=default, **kwargs)
         self.const = const
 
     def take_env_var_action(self, value: str, env_var: str):
         parsed = self.prepare_env_var_value(value, env_var)
         if self.use_env_value:
             if parsed == self.const:
                 getattr(self, self.action)()
             elif parsed != self.default:
-                raise BadArgument(self, f'invalid value={parsed!r} from env_var={env_var!r}')
+                raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
         elif parsed:
             getattr(self, self.action)()
 
     @parameter_action
     def store_const(self):
         ctx.set_parsed_value(self, self.const)
 
@@ -291,22 +291,22 @@
             raise ParameterDefinitionError(f"Bad alt_prefix - may not contain '=' or start with '-': {alt_prefix}")
         elif not alt_prefix and not alt_long:
             alt_prefix = 'no'
 
         try:
             _pos, _neg = consts
         except (ValueError, TypeError) as e:
-            msg = f'Invalid consts={consts!r} - expected a 2-tuple of (positive, negative) constants to store'
+            msg = f'Invalid {consts=} - expected a 2-tuple of (positive, negative) constants to store'
             raise ParameterDefinitionError(msg) from e
 
         if default is _NotSet and not kwargs.get('required', False):
             default = None
         if default in consts:
             raise ParameterDefinitionError(
-                f'Invalid default={default!r} with consts={consts!r} - the default must not match either value'
+                f'Invalid {default=} with {consts=} - the default must not match either value'
             )
 
         alt_opt_strs = filter(None, (alt_short, alt_long))
         super().__init__(*option_strs, *alt_opt_strs, action=action, default=default, **kwargs)
         self.consts = consts
         self.option_strs.add_alts(alt_prefix, alt_long, alt_short)
         if alt_help:
@@ -341,15 +341,15 @@
 
     def take_env_var_action(self, value: str, env_var: str):
         parsed = self.prepare_env_var_value(value, env_var)
         if self.use_env_value:
             if parsed in self.consts:
                 self._store_const(parsed)
             elif parsed != self.default:
-                raise BadArgument(self, f'invalid value={parsed!r} from env_var={env_var!r}')
+                raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
         else:
             self._store_const(self.consts[0] if parsed else self.consts[1])
 
 
 # region Action Flag
 
 
@@ -378,16 +378,15 @@
         func: Callable = None,
         before_main: Bool = True,  # noqa  # pylint: disable=W0621
         always_available: Bool = False,
         **kwargs,
     ):
         expected = {'action': 'store_const', 'default': False, 'const': _NotSet}
         found = {k: kwargs.setdefault(k, v) for k, v in expected.items()}
-        bad = {k: v for k, v in found.items() if expected[k] != v}
-        if bad:
+        if bad := {k: v for k, v in found.items() if expected[k] != v}:
             raise ParameterDefinitionError(f'Unsupported kwargs for {self.__class__.__name__}: {bad}')
         elif always_available and not before_main:
             raise ParameterDefinitionError('always_available=True cannot be combined with before_main=False')
         super().__init__(*option_strs, **kwargs)
         self.func = func
         self.order = order
         self.before_main = before_main
@@ -441,16 +440,16 @@
         # Allow the method to be called, regardless of whether it was specified
         if command is None:
             return self
         return partial(self.func, command)  # imitates a bound method
 
     def result(self) -> Optional[Callable]:
         if self.result_value():
-            if self.func:
-                return self.func
+            if func := self.func:
+                return func
             raise ParameterDefinitionError(f'No function was registered for {self}')
         return None
 
 
 #: Alias for :class:`ActionFlag`
 action_flag = ActionFlag  # pylint: disable=C0103
 
@@ -486,16 +485,15 @@
     """
 
     type = int
     nargs = Nargs('?')
 
     def __init__(self, *option_strs: str, action: str = 'append', default: int = 0, const: int = 1, **kwargs):
         vals = {'const': const, 'default': default}
-        bad_types = ', '.join(f'{k}={v!r}' for k, v in vals.items() if not isinstance(v, self.type))
-        if bad_types:
+        if bad_types := ', '.join(f'{k}={v!r}' for k, v in vals.items() if not isinstance(v, self.type)):
             raise ParameterDefinitionError(f'Invalid type for parameters (expected int): {bad_types}')
         super().__init__(*option_strs, action=action, default=default, **kwargs)
         self.const = const
 
     def _init_value_factory(self):
         return self.default
 
@@ -504,30 +502,30 @@
             return self.const
         try:
             return self.type(value)
         except (ValueError, TypeError) as e:
             combinable = self.option_strs.combinable
             if short_combo and combinable and all(c in combinable for c in value):
                 return len(value) + 1  # +1 for the -short that preceded this value
-            raise BadArgument(self, f'bad counter value={value!r}') from e
+            raise BadArgument(self, f'bad counter {value=}') from e
 
     @parameter_action
     def append(self, value: Optional[int]):
         if value is None:
             value = self.const
         current = ctx.get_parsed_value(self)
         ctx.set_parsed_value(self, current + value)
 
     def validate(self, value: Any):
         if value is None or isinstance(value, self.type):
             return
         try:
             value = self.type(value)
         except (ValueError, TypeError) as e:
-            raise BadArgument(self, f'invalid value={value!r} (expected an integer)') from e
+            raise BadArgument(self, f'invalid {value=} (expected an integer)') from e
         else:
             return
 
     def result_value(self) -> int:
         return ctx.get_parsed_value(self)
 
     result = result_value
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,24 +43,22 @@
 
     def take_action(  # pylint: disable=W0237
         self, values: Strings, short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
     ):
         value = ctx.get_parsed_value(self)
         if value is not _NotSet:
             raise ParamUsageError(
-                self,
-                f'can only be specified once - found values={values!r} but a stored value={value!r} already exists',
+                self, f'can only be specified once - found {values=} but a stored {value=} already exists'
             )
 
         ctx.record_action(self)
         normalized = list(map(self.prepare_value, values))
         return getattr(self, self.action)(normalized)
 
     def result_value(self) -> Any:
-        value = ctx.get_parsed_value(self)
-        if value is _NotSet:
+        if (value := ctx.get_parsed_value(self)) is _NotSet:
             if self.required:
                 raise MissingArgument(self)
             return self.default
         return value
 
     result = result_value
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parameters/positionals.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
             self.nargs = Nargs(nargs)
             if self.nargs == 0:
                 cls_name = self.__class__.__name__
                 raise ParameterDefinitionError(f'Invalid nargs={self.nargs} - {cls_name} must allow at least 1 value')
         if action is _NotSet:
             action = 'store' if self.nargs == 1 or self.nargs == Nargs('?') else 'append'
         elif action == 'store' and self.nargs.max != 1:
-            raise ParameterDefinitionError(f'Invalid action={action!r} for nargs={self.nargs}')
+            raise ParameterDefinitionError(f'Invalid {action=} for nargs={self.nargs}')
         required = 0 not in self.nargs
         if default is not _NotSet and required:
             raise ParameterDefinitionError(
-                f'Invalid default={default!r} - only allowed for Positional parameters when nargs=? or nargs=*'
+                f'Invalid {default=} - only allowed for Positional parameters when nargs=? or nargs=*'
             )
         kwargs.setdefault('required', required)
         super().__init__(action=action, default=default, **kwargs)
         self.type = normalize_input_type(type, choices)
         self._validate_nargs_and_allow_leading_dash(allow_leading_dash)
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parse_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def __repr__(self) -> str:
         return f'AnyWord({self.nargs!r}, remaining={self.remaining}, n={self.n})'
 
     def __add__(self, other: int) -> AnyWord:
         remaining = self.remaining - other
         if remaining < 0:
-            raise ValueError(f'Unable to add {other} to {self!r} - remaining={remaining} is invalid')
+            raise ValueError(f'Unable to add {other} to {self!r} - {remaining=} is invalid')
         return AnyWord(self.nargs, remaining, self.n + other)
 
     def __eq__(self, other: AnyWord) -> bool:
         try:
             return self.nargs == other.nargs and self.remaining == other.remaining and self.n == other.n
         except AttributeError:
             return False
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/parser.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/testing.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/testing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/typing.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/typing.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser/utils.py` & `cli_command_parser-2023.5.8/lib/cli_command_parser/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             else:
                 invert = False
 
             try:
                 member = cls._missing_str(value)
             except KeyError:
                 expected = ', '.join(cls._member_map_)
-                raise ValueError(f'Invalid {cls.__name__} value={value!r} - expected one of {expected}') from None
+                raise ValueError(f'Invalid {cls.__name__} {value=} - expected one of {expected}') from None
             else:
                 return ~member if invert else member  # pylint: disable=E1130
         elif not isinstance(value, int):
             raise TypeError(f'Unexpected type={value.__class__.__name__} for a {cls.__name__}')
 
         return super()._missing_(value)
 
@@ -117,16 +117,15 @@
                     return tmp
 
         raise KeyError
 
     def _decompose(self) -> List[FlagEnum]:
         if self._name_ is None or '|' in self._name_:  # | check is for 3.11 where pseudo-members are assigned names
             val = self._value_
-            members = ((mem, mem._value_) for mem in self.__class__)
-            return sorted(mem for mem, mem_val in members if mem_val & val == mem_val)  # noqa
+            return sorted(mem for mem in self.__class__ if (mem_val := mem._value_) & val == mem_val)  # noqa
         return [self]
 
     def __lt__(self, other: FlagEnum) -> bool:
         return self._value_ < other._value_
 
 
 class Terminal:  # pylint: disable=R0903
@@ -156,8 +155,8 @@
     except (TypeError, ValueError):
         pass
     lower = value.lower()
     if lower in {'t', 'true', 'y', 'yes'}:
         return True
     elif lower in {'f', 'false', 'n', 'no'}:
         return False
-    raise ValueError(f'Unable to parse boolean value from value={value!r}')
+    raise ValueError(f'Unable to parse boolean value from {value=}')
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-command-parser
-Version: 2023.5.2
+Version: 2023.5.8
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2023.5.8/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/readme.rst` & `cli_command_parser-2023.5.8/readme.rst`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.5.2/setup.cfg` & `cli_command_parser-2023.5.8/setup.cfg`

 * *Files identical despite different names*

