# Comparing `tmp/aiddl_core-0.3.0.tar.gz` & `tmp/aiddl_core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiddl_core-0.3.0.tar", last modified: Thu Mar  2 09:19:05 2023, max compression
+gzip compressed data, was "aiddl_core-0.3.1.tar", last modified: Mon May  8 08:51:22 2023, max compression
```

## Comparing `aiddl_core-0.3.0.tar` & `aiddl_core-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1053 2023-03-01 15:53:35.000000 aiddl_core-0.3.0/LICENSE
--rw-rw-r--   0 uekn      (1000) uekn      (1000)      912 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/PKG-INFO
--rw-rw-r--   0 uekn      (1000) uekn      (1000)      276 2023-03-02 09:06:00.000000 aiddl_core-0.3.0/README.md
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)        0 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/__init__.py
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core/container/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)       58 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/container/__init__.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)    15824 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/container/container.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     2750 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/container/entry.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1414 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/container/module.py
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core/function/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     5034 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/__init__.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     8087 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/default.py
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core/function/eval/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)        0 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/__init__.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     2312 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/collection.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     2042 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/higher_order.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     4599 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/logic.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     3633 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/misc.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1149 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/numerical.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1722 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/python.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)      204 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/string.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)    10454 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/eval/type.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     3908 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/evaluator.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     3069 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/function.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     7835 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/function/function_registry.py
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core/parser/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)       86 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/parser/__init__.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)    14405 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/parser/parser.py
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core/representation/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)      463 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/__init__.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     3708 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/collection.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     2599 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/entref.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     2203 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/funref.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     5384 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/inf.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     6926 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/int.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1682 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/keyval.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     5767 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/list.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1131 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/nan.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     3707 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/num.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     7203 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/rat.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     6179 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/real.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     4328 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/set.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)      847 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/str.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     2655 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/substitution.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     3132 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/sym.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     4779 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/term.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     4775 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/tuple.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1276 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/representation/var.py
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core/util/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)        0 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/util/__init__.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1617 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/util/combo_iterator.py
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1893 2023-01-12 12:16:54.000000 aiddl_core-0.3.0/aiddl_core/util/logger.py
-drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core.egg-info/
--rw-rw-r--   0 uekn      (1000) uekn      (1000)      912 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core.egg-info/PKG-INFO
--rw-rw-r--   0 uekn      (1000) uekn      (1000)     1711 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core.egg-info/SOURCES.txt
--rw-rw-r--   0 uekn      (1000) uekn      (1000)        1 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core.egg-info/dependency_links.txt
--rw-rw-r--   0 uekn      (1000) uekn      (1000)       11 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/aiddl_core.egg-info/top_level.txt
--rw-rw-r--   0 uekn      (1000) uekn      (1000)      636 2023-03-02 09:19:05.000000 aiddl_core-0.3.0/setup.cfg
--rw-rw-r--   0 uekn      (1000) uekn      (1000)       69 2023-03-01 15:53:19.000000 aiddl_core-0.3.0/setup.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1053 2023-03-01 15:53:35.000000 aiddl_core-0.3.1/LICENSE
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)      859 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/PKG-INFO
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)      276 2023-03-02 09:06:00.000000 aiddl_core-0.3.1/README.md
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)        0 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/__init__.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core/container/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)       58 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/container/__init__.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)    15824 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/container/container.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     2750 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/container/entry.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1414 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/container/module.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core/function/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     5034 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/__init__.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     8087 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/default.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core/function/eval/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)        0 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/__init__.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     2312 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/collection.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     2042 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/higher_order.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     4599 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/logic.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     3633 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/misc.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1149 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/numerical.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1722 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/python.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)      204 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/string.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)    10454 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/eval/type.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     3908 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/evaluator.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     3069 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/function.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     7835 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/function/function_registry.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core/parser/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)       86 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/parser/__init__.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)    14405 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/parser/parser.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core/representation/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)      463 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/__init__.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     3708 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/collection.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     2599 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/entref.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     2203 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/funref.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     5384 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/inf.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     6926 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/int.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1682 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/keyval.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     5767 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/list.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1131 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/nan.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     3707 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/num.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     7203 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/rat.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     6179 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/real.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     4328 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/set.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)      847 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/str.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     2655 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/substitution.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     3132 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/sym.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     4779 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/term.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     4769 2023-05-08 07:59:55.000000 aiddl_core-0.3.1/aiddl_core/representation/tuple.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1276 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/representation/var.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core/util/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)        0 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/util/__init__.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1617 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/util/combo_iterator.py
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1893 2023-01-12 12:16:54.000000 aiddl_core-0.3.1/aiddl_core/util/logger.py
+drwxrwxr-x   0 uekn      (1000) uekn      (1000)        0 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/aiddl_core.egg-info/
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)      859 2023-05-08 08:51:22.000000 aiddl_core-0.3.1/aiddl_core.egg-info/PKG-INFO
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)     1711 2023-05-08 08:51:22.000000 aiddl_core-0.3.1/aiddl_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)        1 2023-05-08 08:51:22.000000 aiddl_core-0.3.1/aiddl_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)       11 2023-05-08 08:51:22.000000 aiddl_core-0.3.1/aiddl_core.egg-info/top_level.txt
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)      668 2023-05-08 08:51:22.294400 aiddl_core-0.3.1/setup.cfg
+-rw-rw-r--   0 uekn      (1000) uekn      (1000)       69 2023-03-01 15:53:19.000000 aiddl_core-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiddl_core-0.3.0/LICENSE` & `aiddl_core-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/container/container.py` & `aiddl_core-0.3.1/aiddl_core/container/container.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/container/entry.py` & `aiddl_core-0.3.1/aiddl_core/container/entry.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/container/module.py` & `aiddl_core-0.3.1/aiddl_core/container/module.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/__init__.py` & `aiddl_core-0.3.1/aiddl_core/function/__init__.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/default.py` & `aiddl_core-0.3.1/aiddl_core/function/default.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/eval/collection.py` & `aiddl_core-0.3.1/aiddl_core/function/eval/collection.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/eval/higher_order.py` & `aiddl_core-0.3.1/aiddl_core/function/eval/higher_order.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/eval/logic.py` & `aiddl_core-0.3.1/aiddl_core/function/eval/logic.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/eval/misc.py` & `aiddl_core-0.3.1/aiddl_core/function/eval/misc.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/eval/numerical.py` & `aiddl_core-0.3.1/aiddl_core/function/eval/numerical.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/eval/python.py` & `aiddl_core-0.3.1/aiddl_core/function/eval/python.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/eval/type.py` & `aiddl_core-0.3.1/aiddl_core/function/eval/type.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/evaluator.py` & `aiddl_core-0.3.1/aiddl_core/function/evaluator.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/function.py` & `aiddl_core-0.3.1/aiddl_core/function/function.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/function/function_registry.py` & `aiddl_core-0.3.1/aiddl_core/function/function_registry.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/parser/parser.py` & `aiddl_core-0.3.1/aiddl_core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/collection.py` & `aiddl_core-0.3.1/aiddl_core/representation/collection.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/entref.py` & `aiddl_core-0.3.1/aiddl_core/representation/entref.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/funref.py` & `aiddl_core-0.3.1/aiddl_core/representation/funref.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/inf.py` & `aiddl_core-0.3.1/aiddl_core/representation/inf.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/int.py` & `aiddl_core-0.3.1/aiddl_core/representation/int.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/keyval.py` & `aiddl_core-0.3.1/aiddl_core/representation/keyval.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/list.py` & `aiddl_core-0.3.1/aiddl_core/representation/list.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/nan.py` & `aiddl_core-0.3.1/aiddl_core/representation/nan.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/num.py` & `aiddl_core-0.3.1/aiddl_core/representation/num.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/rat.py` & `aiddl_core-0.3.1/aiddl_core/representation/rat.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/real.py` & `aiddl_core-0.3.1/aiddl_core/representation/real.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/set.py` & `aiddl_core-0.3.1/aiddl_core/representation/set.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/str.py` & `aiddl_core-0.3.1/aiddl_core/representation/str.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/substitution.py` & `aiddl_core-0.3.1/aiddl_core/representation/substitution.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/sym.py` & `aiddl_core-0.3.1/aiddl_core/representation/sym.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/term.py` & `aiddl_core-0.3.1/aiddl_core/representation/term.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/tuple.py` & `aiddl_core-0.3.1/aiddl_core/representation/tuple.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                     return None
             return sCombined
         return None
 
     def put(self, key, value):
         l_new = []
         for t in self._internal_list:
-            if not isinstance(t, KeyVal) or t.get_key() != key:
+            if not isinstance(t, KeyVal) or t.key != key:
                 l_new.append(t)
         l_new.append(KeyVal(key, value))
         return Tuple(l_new)
 
     def __iter__(self):
         super(term.Term, self).__setattr__("_next_id", -1)
         return self
```

### Comparing `aiddl_core-0.3.0/aiddl_core/representation/var.py` & `aiddl_core-0.3.1/aiddl_core/representation/var.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/util/combo_iterator.py` & `aiddl_core-0.3.1/aiddl_core/util/combo_iterator.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core/util/logger.py` & `aiddl_core-0.3.1/aiddl_core/util/logger.py`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/aiddl_core.egg-info/SOURCES.txt` & `aiddl_core-0.3.1/aiddl_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiddl_core-0.3.0/setup.cfg` & `aiddl_core-0.3.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = aiddl_core
-version = 0.3.0
+version = 0.3.1
 author = Uwe Köckemann
 author_email = uwe.kockemann@oru.se
-description = Core Library for the AIDDL Framework for Integrative AI
+description = Core Library for the AI Domain Definition Language (AIDDL) Framework for Integrative AI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://www.aiddl.org
 project_urls = 
 	Bug Tracker =  https://github.com/uwe-koeckemann/AIDDL/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

