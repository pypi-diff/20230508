# Comparing `tmp/neo3-boa-0.8.3.tar.gz` & `tmp/neo3-boa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neo3-boa-0.8.3.tar", last modified: Mon Jul 19 19:36:14 2021, max compression
+gzip compressed data, was "dist/neo3-boa-0.9.0.tar", last modified: Mon Aug  2 17:17:41 2021, max compression
```

## Comparing `neo3-boa-0.8.3.tar` & `neo3-boa-0.9.0.tar`

### file list

```diff
@@ -1,682 +1,693 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.124867 neo3-boa-0.8.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4186 2021-07-19 19:36:14.124867 neo3-boa-0.8.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2577 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      116 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/analyser/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/analyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8668 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/astanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13946 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/astoptimizer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4571 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/builtinfunctioncallanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2853 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/constructanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4259 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/importanalyser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/analyser/model/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/model/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/model/functionarguments.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/analyser/model/optimizer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1163 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/model/optimizer/Operation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2981 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/model/optimizer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      856 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/model/symbolscope.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44188 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/moduleanalyser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/analyser/supportedstandard/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      182 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/supportedstandard/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3618 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/supportedstandard/standardanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    63712 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/analyser/typeanalyser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1460 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/boa3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/builtin/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2809 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/builtin/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      945 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/contract/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/builtin/interop/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      435 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/builtin/interop/blockchain/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1968 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/blockchain/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1375 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/blockchain/block.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1359 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/blockchain/transaction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.052866 neo3-boa-0.8.3/boa3/builtin/interop/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3505 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       67 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/contract/callflagstype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      904 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/contract/contract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6117 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/contract/contractmanifest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/crypto/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/crypto/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/iterator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      641 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/iterator/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/json/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      721 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/json/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/oracle/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1832 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/oracle/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/policy/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      885 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/policy/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/role/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/role/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/role/roletype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/runtime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2869 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/runtime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/runtime/notification.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/runtime/triggertype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/stdlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3758 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/stdlib/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/interop/storage/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2387 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/storage/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/storage/findoptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/storage/storagecontext.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1291 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/interop/storage/storagemap.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/builtin/type/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      577 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/builtin/type/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      865 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/cli.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/compiler/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/compiler/codegenerator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/codegenerator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    62848 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/codegenerator/codegenerator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29755 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/codegenerator/codegeneratorvisitor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4172 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/codegenerator/initstatementsvisitor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2509 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/codegenerator/stackmemento.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11609 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/codegenerator/vmcodemapping.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3484 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/compiler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17295 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/compiler/filegenerator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/env.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/exception/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10819 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/exception/CompilerError.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3505 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/exception/CompilerWarning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/exception/InvalidPathException.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/exception/NotLoadedException.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/exception/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.056866 neo3-boa-0.8.3/boa3/helpers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/helpers/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.060866 neo3-boa-0.8.3/boa3/model/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1651 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/attribute.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.060866 neo3-boa-0.8.3/boa3/model/builtin/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6788 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/builtin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1074 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/builtincallable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      374 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/builtinproperty.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.060866 neo3-boa-0.8.3/boa3/model/builtin/classmethod/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1381 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2654 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/appendmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2299 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/clearmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6294 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/countmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3568 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/extendmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4043 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/insertmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1794 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/mapkeysmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/mapvaluesmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3537 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/popmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3022 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/removemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1671 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/reversemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2459 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/toboolmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3289 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/tobytesmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/tointmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/classmethod/tostrmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.060866 neo3-boa-0.8.3/boa3/model/builtin/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      310 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/contract/abortmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      702 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/contract/nep17transferevent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/contract/nep5transferevent.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.064866 neo3-boa-0.8.3/boa3/model/builtin/decorator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/decorator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      884 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/decorator/builtindecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/decorator/metadatadecorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/decorator/publicdecorator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.064866 neo3-boa-0.8.3/boa3/model/builtin/internal/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/internal/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2308 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/internal/innerdeploymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/internal/internalmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.064866 neo3-boa-0.8.3/boa3/model/builtin/interop/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.064866 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1250 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3532 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/blocktype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      728 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/currenthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/currentindexmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/getblockmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/getcontractmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/getcurrentheightmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      910 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/gettransactionfromblockmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/gettransactionheightmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      633 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/gettransactionmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3450 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/transactiontype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.064866 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1400 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1612 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/callflagstype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1995 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/callmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.068866 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1809 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractabitype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1717 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1521 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractgrouptype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1844 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1671 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1884 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractparametertype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1766 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1516 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2971 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contracttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/createmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/createmultisigaccountmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      662 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/createstandardaccountmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/destroymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/getcallflagsmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/getgasscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      488 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/getminimumdeploymentfeemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/getneoscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      739 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/contract/updatemethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.068866 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      943 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      699 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/checkmultisigmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/checksigmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      857 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/hash160method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      853 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/hash256method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      472 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/ripemd160method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/sha256method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1116 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/verifywithecdsasecp256k1.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1116 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/verifywithecdsasecp256r1.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15175 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/interop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1011 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/interopevent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/interopinterfacetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/interopmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.068866 neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      213 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/getiteratorvalue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1466 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/iteratorinitmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/iteratornextmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3019 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/iteratortype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.068866 neo3-boa-0.8.3/boa3/model/builtin/interop/json/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      255 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/json/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/json/jsondeserializemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/json/jsonserializemethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/ContractManagement/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/ContractManagement/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1327 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/CryptoLib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/CryptoLib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1289 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Ledger/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Ledger/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1275 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      649 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Ledger/ledgermethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Oracle/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Oracle/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      629 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Oracle/oraclemethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/PolicyContract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/PolicyContract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1291 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      673 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/RoleManagement/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/RoleManagement/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1295 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/StdLib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/StdLib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1254 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      629 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1927 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/nativecontractmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      590 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/oraclegetpricemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1016 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/oraclerequestmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1711 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/oracletype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.072866 neo3-boa-0.8.3/boa3/model/builtin/interop/policy/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/policy/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/policy/getexecfeefactormethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      470 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/policy/getfeeperbytemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      475 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/policy/getstoragepricemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/policy/isblockedmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.076866 neo3-boa-0.8.3/boa3/model/builtin/interop/role/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/role/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      777 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/role/getdesignatedbyrolemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1418 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/role/roletype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.076866 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/burngasmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      860 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/checkwitnessmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getblocktimemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getcallingscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getentryscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      803 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getexecutingscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      681 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getgasleftmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getinvocationcountermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1673 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getnotificationsmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      685 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getplatformmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      495 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/gettriggermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/logmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2757 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/notificationtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1063 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/notifymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/scriptcontainermethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/triggertype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.076866 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1420 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/atoimethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/base58checkdecodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/base58checkencodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/base58decodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/base58encodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/base64decodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/base64encodemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/deserializemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      595 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/itoamethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      596 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/memorycomparemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1109 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/memorysearchmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      467 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/serializemethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.080866 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1103 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/findoptionstype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.080866 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1340 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/storagecontexttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3839 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagedeletemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4443 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagefindmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      574 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagegetcontextmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4002 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagegetmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagegetreadonlycontextmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.080866 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1444 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1436 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemapgetmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1777 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemapputmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3953 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemaptype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3891 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storageputmethod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.084866 neo3-boa-0.8.3/boa3/model/builtin/method/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1608 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      720 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/absmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      842 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/builtinevent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6146 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/builtinmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2699 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/bytearraymethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1520 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/createeventmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3117 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/ecpointmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2334 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/exceptionmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      687 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/exitmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5409 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/isinstancemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1693 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/lenmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4765 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/maxmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4719 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/minmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3683 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/printmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4258 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/rangemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4820 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/reversedmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      718 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/sqrtmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1479 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/strsplitmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1842 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/summethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3869 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/toscripthashmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3969 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/uint160method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3969 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/method/uint256method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/builtin/neometadatatype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4702 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/callable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1209 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/debuginstruction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/event.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      805 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/expression.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      824 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/identifiedsymbol.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.084866 neo3-boa-0.8.3/boa3/model/imports/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/imports/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4927 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/imports/builtin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2636 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/imports/importsymbol.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2902 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/imports/package.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5171 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3517 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/module.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.084866 neo3-boa-0.8.3/boa3/model/operation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.088866 neo3-boa-0.8.3/boa3/model/operation/binary/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.088866 neo3-boa-0.8.3/boa3/model/operation/binary/additional/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      258 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/additional/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5809 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/additional/membership.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2729 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/additional/notmembership.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.088866 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/addition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2017 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/concat.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1569 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/division.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1597 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/floordivision.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1584 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/modulo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/multiplication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1582 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/power.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2362 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/strmultiplication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1596 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/subtraction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3173 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/binaryoperation.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.088866 neo3-boa-0.8.3/boa3/model/operation/binary/logical/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      651 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1510 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/booleanand.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/booleanor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/leftshift.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1428 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/logicand.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/logicor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1428 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/logicxor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1451 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/logical/rightshift.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.092866 neo3-boa-0.8.3/boa3/model/operation/binary/relational/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1516 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/LessThan.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1533 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/Lessthanorequal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1092 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1522 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/greaterthan.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/greaterthanorequal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1263 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/identity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1341 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/notidentity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1529 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/numericequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/numericinequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1590 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/objectequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1567 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binary/relational/objectinequality.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4052 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/binaryop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2972 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/operation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2300 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/operator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.092866 neo3-boa-0.8.3/boa3/model/operation/unary/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/booleannot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1266 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/logicnot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1255 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/negative.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1570 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/noneidentity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1633 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/nonenotidentity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1321 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/positive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1467 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unary/unaryoperation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1937 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/operation/unaryop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      901 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/property.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.092866 neo3-boa-0.8.3/boa3/model/standards/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/standards/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1594 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/standards/neostandard.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1309 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/standards/nep17standard.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/standards/standardmethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      323 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/symbol.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.092866 neo3-boa-0.8.3/boa3/model/type/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.096866 neo3-boa-0.8.3/boa3/model/type/annotation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/annotation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1323 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/annotation/metatype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/annotation/optionaltype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3292 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/annotation/uniontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      807 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/anytype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/baseexceptiontype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.096866 neo3-boa-0.8.3/boa3/model/type/classes/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/classes/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/classes/classarraytype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      511 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/classes/classstructtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5211 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/classes/classtype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.096866 neo3-boa-0.8.3/boa3/model/type/collection/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1452 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/genericcollectiontype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5998 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/icollection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.096866 neo3-boa-0.8.3/boa3/model/type/collection/mapping/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/mapping/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      874 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/mapping/genericmappingtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4077 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/mapping/mappingtype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.096866 neo3-boa-0.8.3/boa3/model/type/collection/mapping/mutable/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/mapping/mutable/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/mapping/mutable/dicttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/mapping/mutable/mutablemappingtype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.096866 neo3-boa-0.8.3/boa3/model/type/collection/sequence/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      413 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/buffertype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1942 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/ecpointtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1101 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/genericsequencetype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.096866 neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1159 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/genericmutablesequencetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/listtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      737 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/mutablesequencetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1376 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/rangetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1462 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/reversedtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1032 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/sequencetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1326 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/tupletype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2091 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/uint160type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2091 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/collection/sequence/uint256type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5247 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/itype.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/model/type/primitive/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      917 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/booltype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      831 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/bytearraytype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1604 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/bytestype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      951 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/inttype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      885 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/nonetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/primitivetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1636 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/primitive/strtype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4459 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1477 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/typeutils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/model/type/typingmethod/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/typingmethod/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4383 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/type/typingmethod/casttypemethod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1571 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/model/variable.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1430 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/contracts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/contracts/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1822 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/contracts/neffile.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/core/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/core/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/core/types/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/core/types/InteropInterface.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/core/types/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/cryptography/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      603 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/cryptography/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/smart_contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/smart_contract/VoidType.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/smart_contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2045 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/smart_contract/notification.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3730 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/utils/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/vm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/CallCode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3440 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/TryCode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3228 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/VMCode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/vm/opcode/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    31512 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/opcode/Opcode.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26303 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/opcode/OpcodeInfo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1191 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/opcode/OpcodeInformation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/opcode/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo/vm/type/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      364 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/type/AbiType.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/type/ContractParameterType.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1205 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/type/Integer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1805 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/type/StackItem.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      483 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/type/String.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo/vm/type/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.100866 neo3-boa-0.8.3/boa3/neo3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.104866 neo3-boa-0.8.3/boa3/neo3/contracts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      202 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/contracts/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2526 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/contracts/contracttypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/contracts/findoptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/contracts/namedcurve.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.104866 neo3-boa-0.8.3/boa3/neo3/contracts/native/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/contracts/native/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/contracts/native/nativetypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7615 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/contracts/nef.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.104866 neo3-boa-0.8.3/boa3/neo3/core/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/core/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22856 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/core/serialization.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.104866 neo3-boa-0.8.3/boa3/neo3/core/types/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/core/types/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4432 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/core/types/biginteger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7914 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/core/types/uint.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/core/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.104866 neo3-boa-0.8.3/boa3/neo3/vm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       29 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/vm/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      398 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3/neo3/vm/vmstate.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.104866 neo3-boa-0.8.3/boa3_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.104866 neo3-boa-0.8.3/boa3_test/test_sc/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.108866 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      109 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/AssignSlice.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayAppend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      142 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayAppendWithBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayAppendWithMutableSequence.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      213 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayBoa2Test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      219 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayBoa2Test2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayBoa2Test3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayClear.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      145 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayExtend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      156 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayExtendWithBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayFromLiteralBytes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayFromString.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayFromVariableBytes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayGetValue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       90 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayGetValueNegativeIndex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayLiteral.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayReverse.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearraySetValue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      163 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearraySetValueNegativeIndex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayToInt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayToIntWithBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytearrayToIntWithBytesBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       95 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesClear.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesFromBytearray.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesGetValue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       86 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesGetValueNegativeIndex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesLiteral.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesReverse.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      119 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesSetValue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToBool.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      113 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltinHardCodedFalse.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltinHardCodedTrue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltinMismatchedTypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToInt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToIntWithBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToIntWithBuiltinMismatchedTypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToIntWithBytearrayBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       96 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToStr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToStrWithBuiltin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/BytesToStrWithBuiltinMismatchedTypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      154 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/SliceBoa2Test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      518 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/SliceBoa2Test2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      142 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/SliceWithCast.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      216 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/UInt160Bytes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      127 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/UInt160Int.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      216 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/UInt256Bytes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      127 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/UInt256Int.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.112866 neo3-boa-0.8.3/boa3_test/test_sc/import_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportTyping.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      122 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportTypingNotImplementedType.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportTypingWithAlias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      205 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportUserModule.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      203 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportUserModuleRecursiveImport.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      214 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportUserModuleWithAlias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportVariable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      196 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/FromImportWithGlobalVariables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportInteropWithAlias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportNonExistentPackage.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      129 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportPythonLib.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportTyping.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportTypingWithAlias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      221 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportUserModule.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      226 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportUserModuleRecursiveImport.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      199 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportUserModuleWithAlias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportUserModuleWithNotImportedSymbols.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/ImportUserModuleWithNotImportedVariables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      205 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/UserModuleWithRecursiveImport.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/import_test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.112866 neo3-boa-0.8.3/boa3_test/test_sc/interop_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/interop_test/UpdateContract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/test_sc/interop_test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.112866 neo3-boa-0.8.3/boa3_test/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10908 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/boa_test.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.116866 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12346 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_any.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22226 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_arithmetic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8432 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_assert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1293 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_boa_builtin_method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    41501 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_builtin_method.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21876 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_bytes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3634 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_class.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13576 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_constant.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17237 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8448 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_event.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16442 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_exception.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25010 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_file_generation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17489 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_for.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37776 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_function.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21977 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_if.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10497 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_import.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.116866 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16392 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_blockchain.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21675 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_contract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23476 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_crypto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_iterator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3825 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7352 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_oracle.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3123 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_policy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3460 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_role.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22322 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_runtime.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29473 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_stdlib.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30558 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_storage.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    38927 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16583 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_logical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7287 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_metadata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7531 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_multiple_expressions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21111 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_neo_types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4793 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_none.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3362 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_optional.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9219 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_python_operation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26697 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_range.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25996 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_relational.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3745 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_reversed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8052 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_string.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13717 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_test_engine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19115 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_tuple.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9317 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4990 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_typing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3264 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_union.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23569 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_variable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16987 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_while.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.120866 neo3-boa-0.8.3/boa3_test/tests/examples_tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25818 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_HTLC.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19094 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_NEP17.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    50994 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_amm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_hello_world.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21483 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_ico.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9844 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_nep5.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3024 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_update_contract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34385 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_wrapped_neo.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.120866 neo3-boa-0.8.3/boa3_test/tests/neo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/neo/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.120866 neo3-boa-0.8.3/boa3_test/tests/neo/smart_contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/neo/smart_contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2509 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/neo/smart_contract/test_neffile.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.120866 neo3-boa-0.8.3/boa3_test/tests/test_classes/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/TestExecutionException.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.120866 neo3-boa-0.8.3/boa3_test/tests/test_classes/binaryserializer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1947 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/binaryserializer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2191 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/block.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.120866 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1198 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neoabistruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      669 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neoeventstruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1869 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neomanifeststruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1166 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neomethodstruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1302 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neopermissionsstruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      966 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neostruct.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/nativeaccountstate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1111 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/nativecontractprefix.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/signer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5961 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/storage.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      670 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/testcontract.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14406 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/testengine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3164 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/transaction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.120866 neo3-boa-0.8.3/boa3_test/tests/test_classes/transactionattribute/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/transactionattribute/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2193 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      681 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/transactionattribute/transactionattributetype.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      968 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/boa3_test/tests/test_classes/witness.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-19 19:36:14.124867 neo3-boa-0.8.3/neo3_boa.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4186 2021-07-19 19:36:13.000000 neo3-boa-0.8.3/neo3_boa.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27551 2021-07-19 19:36:13.000000 neo3-boa-0.8.3/neo3_boa.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-07-19 19:36:13.000000 neo3-boa-0.8.3/neo3_boa.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2021-07-19 19:36:13.000000 neo3-boa-0.8.3/neo3_boa.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      139 2021-07-19 19:36:13.000000 neo3-boa-0.8.3/neo3_boa.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2021-07-19 19:36:13.000000 neo3-boa-0.8.3/neo3_boa.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2021-07-19 19:36:14.124867 neo3-boa-0.8.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4548 2021-07-19 19:36:01.000000 neo3-boa-0.8.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.200007 neo3-boa-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4186 2021-08-02 17:17:41.200007 neo3-boa-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2577 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.116007 neo3-boa-0.9.0/boa3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      116 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.116007 neo3-boa-0.9.0/boa3/analyser/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5887 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/analyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8668 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/astanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13946 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/astoptimizer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4571 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/builtinfunctioncallanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2853 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/constructanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4259 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/importanalyser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.116007 neo3-boa-0.9.0/boa3/analyser/model/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/model/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/model/functionarguments.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/analyser/model/optimizer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1163 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/model/optimizer/Operation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2981 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/model/optimizer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      856 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/model/symbolscope.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    44188 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/moduleanalyser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/analyser/supportedstandard/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      182 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/supportedstandard/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3618 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/supportedstandard/standardanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    63712 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/analyser/typeanalyser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1460 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/boa3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2809 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      945 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/contract/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      435 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/blockchain/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1968 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/blockchain/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/blockchain/block.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1359 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/blockchain/transaction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3505 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       67 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/contract/callflagstype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      904 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/contract/contract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6117 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/contract/contractmanifest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/crypto/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2922 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/crypto/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/iterator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      641 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/iterator/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/json/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      721 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/json/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/oracle/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1911 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/oracle/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/oracle/oracleresponsecode.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/policy/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      885 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/policy/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/role/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/role/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/role/roletype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/runtime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3180 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/runtime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/runtime/notification.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/runtime/triggertype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/stdlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3758 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/stdlib/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/interop/storage/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2387 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/storage/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/storage/findoptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/storage/storagecontext.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1291 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/interop/storage/storagemap.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/builtin/type/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      577 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/builtin/type/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      865 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/cli.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/compiler/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.120007 neo3-boa-0.9.0/boa3/compiler/codegenerator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/codegenerator/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    62848 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/codegenerator/codegenerator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29755 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/codegenerator/codegeneratorvisitor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4172 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/codegenerator/initstatementsvisitor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2509 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/codegenerator/stackmemento.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11609 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/codegenerator/vmcodemapping.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3484 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/compiler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17295 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/compiler/filegenerator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/env.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.124007 neo3-boa-0.9.0/boa3/exception/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10819 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/exception/CompilerError.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3505 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/exception/CompilerWarning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/exception/InvalidPathException.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/exception/NotLoadedException.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/exception/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.124007 neo3-boa-0.9.0/boa3/helpers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/helpers/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.124007 neo3-boa-0.9.0/boa3/model/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1651 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/attribute.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.124007 neo3-boa-0.9.0/boa3/model/builtin/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6886 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/builtin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1074 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/builtincallable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      374 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/builtinproperty.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.124007 neo3-boa-0.9.0/boa3/model/builtin/classmethod/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2654 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/appendmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2299 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/clearmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2131 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/countmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5279 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/countsequencemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8928 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/countstrmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3568 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/extendmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4043 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/insertmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1794 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/mapkeysmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/mapvaluesmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3537 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/popmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3022 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/removemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1671 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/reversemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2459 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/toboolmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3289 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/tobytesmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/tointmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/classmethod/tostrmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.128007 neo3-boa-0.9.0/boa3/model/builtin/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      310 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/contract/abortmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      702 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/contract/nep17transferevent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      540 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/contract/nep5transferevent.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.128007 neo3-boa-0.9.0/boa3/model/builtin/decorator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/decorator/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      884 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/decorator/builtindecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/decorator/metadatadecorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/decorator/publicdecorator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.128007 neo3-boa-0.9.0/boa3/model/builtin/internal/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/internal/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2308 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/internal/innerdeploymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/internal/internalmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.128007 neo3-boa-0.9.0/boa3/model/builtin/interop/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.128007 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1250 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3616 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/blocktype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      728 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/currenthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/currentindexmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/getblockmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/getcontractmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/getcurrentheightmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      910 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/gettransactionfromblockmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/gettransactionheightmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      633 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/gettransactionmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3450 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/transactiontype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.128007 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1400 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1612 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/callflagstype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1995 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/callmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1809 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractabitype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1717 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1521 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractgrouptype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1844 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1993 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1671 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1884 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractparametertype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1766 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1516 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2971 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contracttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/createmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/createmultisigaccountmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      662 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/createstandardaccountmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/destroymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/getcallflagsmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/getgasscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      488 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/getminimumdeploymentfeemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/getneoscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      739 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/contract/updatemethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      943 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      699 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/checkmultisigmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/checksigmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      857 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/hash160method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      853 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/hash256method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      472 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/ripemd160method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/sha256method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1116 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/verifywithecdsasecp256k1.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1116 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/verifywithecdsasecp256r1.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15716 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/interop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1011 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/interopevent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      544 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/interopinterfacetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/interopmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      213 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/getiteratorvalue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1466 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/iteratorinitmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/iteratornextmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3019 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/iteratortype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/json/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      255 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/json/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/json/jsondeserializemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/json/jsonserializemethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/ContractManagement/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/ContractManagement/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1327 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/CryptoLib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/CryptoLib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1289 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.132007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Ledger/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Ledger/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1275 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      649 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Ledger/ledgermethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.136007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Oracle/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Oracle/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      629 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Oracle/oraclemethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.136007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/PolicyContract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/PolicyContract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1291 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      673 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.136007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/RoleManagement/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/RoleManagement/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1295 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.136007 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/StdLib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/StdLib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1254 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      629 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1927 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/nativecontractmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.136007 neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      237 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      590 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/oraclegetpricemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1016 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/oraclerequestmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1591 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/oracleresponsecodetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1711 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/oracletype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.136007 neo3-boa-0.9.0/boa3/model/builtin/interop/policy/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/policy/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/policy/getexecfeefactormethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      470 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/policy/getfeeperbytemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      475 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/policy/getstoragepricemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/policy/isblockedmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.136007 neo3-boa-0.9.0/boa3/model/builtin/interop/role/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/role/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      777 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/role/getdesignatedbyrolemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1418 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/role/roletype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.140007 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2128 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/burngasmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      860 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/checkwitnessmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getblocktimemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getcallingscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getentryscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      803 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getexecutingscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      681 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getgasleftmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getinvocationcountermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      439 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getnetworkmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1673 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getnotificationsmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      685 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getplatformmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getrandommethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      495 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/gettriggermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/logmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2757 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/notificationtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1063 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/notifymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/scriptcontainermethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/triggertype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.144007 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1420 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/atoimethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/base58checkdecodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/base58checkencodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/base58decodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/base58encodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/base64decodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/base64encodemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      473 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/deserializemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      595 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/itoamethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      585 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/memorycomparemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1109 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/memorysearchmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      467 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/serializemethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.144007 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1103 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/findoptionstype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.144007 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       51 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1340 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/storagecontexttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3839 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagedeletemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4443 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagefindmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      574 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagegetcontextmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4002 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagegetmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagegetreadonlycontextmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.148007 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1444 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1436 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemapgetmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1777 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemapputmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3953 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemaptype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3891 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storageputmethod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.152007 neo3-boa-0.9.0/boa3/model/builtin/method/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1608 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      720 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/absmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      842 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/builtinevent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6146 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/builtinmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2699 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/bytearraymethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1520 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/createeventmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3117 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/ecpointmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2334 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/exceptionmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      687 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/exitmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5409 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/isinstancemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1693 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/lenmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4765 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/maxmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4719 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/minmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3683 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/printmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4258 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/rangemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4820 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/reversedmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      718 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/sqrtmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3615 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/strsplitmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1842 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/summethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3869 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/toscripthashmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3969 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/uint160method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3969 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/method/uint256method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/builtin/neometadatatype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4702 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/callable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1209 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/debuginstruction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/event.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      805 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/expression.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      824 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/identifiedsymbol.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.152007 neo3-boa-0.9.0/boa3/model/imports/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/imports/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4927 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/imports/builtin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2636 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/imports/importsymbol.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2902 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/imports/package.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5171 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3517 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/module.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.152007 neo3-boa-0.9.0/boa3/model/operation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.152007 neo3-boa-0.9.0/boa3/model/operation/binary/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.152007 neo3-boa-0.9.0/boa3/model/operation/binary/additional/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      258 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/additional/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5809 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/additional/membership.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2729 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/additional/notmembership.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.156007 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/addition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2017 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/concat.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1569 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/division.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1597 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/floordivision.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1584 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/modulo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/multiplication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1582 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/power.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2362 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/strmultiplication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1596 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/subtraction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3173 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/binaryoperation.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.156007 neo3-boa-0.9.0/boa3/model/operation/binary/logical/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      651 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1510 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/booleanand.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/booleanor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/leftshift.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1428 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/logicand.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/logicor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1428 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/logicxor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1451 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/logical/rightshift.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.160007 neo3-boa-0.9.0/boa3/model/operation/binary/relational/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1516 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/LessThan.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1533 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/Lessthanorequal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1092 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1522 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/greaterthan.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/greaterthanorequal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1263 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/identity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1341 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/notidentity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1529 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/numericequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/numericinequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1590 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/objectequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1567 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binary/relational/objectinequality.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4052 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/binaryop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2972 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/operation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2300 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/operator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.160007 neo3-boa-0.9.0/boa3/model/operation/unary/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/booleannot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1266 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/logicnot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1255 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/negative.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1570 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/noneidentity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1633 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/nonenotidentity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1321 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/positive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1467 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unary/unaryoperation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1937 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/operation/unaryop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      901 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/property.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.160007 neo3-boa-0.9.0/boa3/model/standards/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/standards/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1594 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/standards/neostandard.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1309 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/standards/nep17standard.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/standards/standardmethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      323 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/symbol.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.160007 neo3-boa-0.9.0/boa3/model/type/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.160007 neo3-boa-0.9.0/boa3/model/type/annotation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/annotation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1323 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/annotation/metatype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/annotation/optionaltype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3292 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/annotation/uniontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      807 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/anytype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/baseexceptiontype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.164007 neo3-boa-0.9.0/boa3/model/type/classes/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/classes/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/classes/classarraytype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      511 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/classes/classstructtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5211 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/classes/classtype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.164007 neo3-boa-0.9.0/boa3/model/type/collection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1452 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/genericcollectiontype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5998 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/icollection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.164007 neo3-boa-0.9.0/boa3/model/type/collection/mapping/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/mapping/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      874 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/mapping/genericmappingtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4077 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/mapping/mappingtype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.164007 neo3-boa-0.9.0/boa3/model/type/collection/mapping/mutable/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/mapping/mutable/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/mapping/mutable/dicttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/mapping/mutable/mutablemappingtype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.164007 neo3-boa-0.9.0/boa3/model/type/collection/sequence/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      413 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/buffertype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1942 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/ecpointtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1101 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/genericsequencetype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1159 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/genericmutablesequencetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1251 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/listtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      737 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/mutablesequencetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1376 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/rangetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1462 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/reversedtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1032 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/sequencetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1326 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/tupletype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2091 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/uint160type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2091 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/collection/sequence/uint256type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5247 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/itype.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/model/type/primitive/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      917 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/booltype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      831 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/bytearraytype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1604 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/bytestype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      951 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/inttype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      885 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/nonetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/primitivetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1636 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/primitive/strtype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4459 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1477 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/typeutils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/model/type/typingmethod/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/typingmethod/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4383 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/type/typingmethod/casttypemethod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1571 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/model/variable.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1430 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/contracts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/contracts/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1822 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/contracts/neffile.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/core/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/core/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/core/types/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/core/types/InteropInterface.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/core/types/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/cryptography/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      603 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/cryptography/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/smart_contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/smart_contract/VoidType.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/smart_contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2045 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/smart_contract/notification.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3730 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/utils/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.168007 neo3-boa-0.9.0/boa3/neo/vm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/CallCode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3440 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/TryCode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3228 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/VMCode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo/vm/opcode/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31512 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/opcode/Opcode.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26303 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/opcode/OpcodeInfo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1191 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/opcode/OpcodeInformation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/opcode/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo/vm/type/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      364 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/type/AbiType.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/type/ContractParameterType.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1205 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/type/Integer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1805 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/type/StackItem.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      483 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/type/String.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo/vm/type/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo3/contracts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      202 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/contracts/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2526 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/contracts/contracttypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      228 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/contracts/findoptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/contracts/namedcurve.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo3/contracts/native/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       77 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/contracts/native/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/contracts/native/nativetypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7615 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/contracts/nef.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo3/core/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/core/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22856 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/core/serialization.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo3/core/types/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/core/types/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4432 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/core/types/biginteger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7914 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/core/types/uint.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/core/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo3/network/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/network/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.172007 neo3-boa-0.9.0/boa3/neo3/network/payloads/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      111 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/network/payloads/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1468 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/network/payloads/oracleresponsecode.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.176007 neo3-boa-0.9.0/boa3/neo3/vm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       29 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/vm/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      398 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3/neo3/vm/vmstate.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.176007 neo3-boa-0.9.0/boa3_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.176007 neo3-boa-0.9.0/boa3_test/test_sc/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.180007 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      109 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/AssignSlice.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayAppend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      142 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayAppendWithBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayAppendWithMutableSequence.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      213 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayBoa2Test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      219 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayBoa2Test2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      165 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayBoa2Test3.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayClear.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      145 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayExtend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      156 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayExtendWithBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayFromLiteralBytes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayFromString.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayFromVariableBytes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayGetValue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       90 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayGetValueNegativeIndex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayLiteral.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayReverse.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearraySetValue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      163 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearraySetValueNegativeIndex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayToInt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayToIntWithBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytearrayToIntWithBytesBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       95 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesClear.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesFromBytearray.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesGetValue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       86 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesGetValueNegativeIndex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesLiteral.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesReverse.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      119 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesSetValue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToBool.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      113 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltinHardCodedFalse.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      105 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltinHardCodedTrue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToBoolWithBuiltinMismatchedTypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToInt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToIntWithBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToIntWithBuiltinMismatchedTypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToIntWithBytearrayBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       96 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToStr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      101 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToStrWithBuiltin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/BytesToStrWithBuiltinMismatchedTypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      154 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/SliceBoa2Test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      518 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/SliceBoa2Test2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      142 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/SliceWithCast.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      216 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/UInt160Bytes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      127 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/UInt160Int.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      216 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/UInt256Bytes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      127 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/UInt256Int.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.184007 neo3-boa-0.9.0/boa3_test/test_sc/import_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportTyping.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      122 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportTypingNotImplementedType.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportTypingWithAlias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      205 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportUserModule.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      203 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportUserModuleRecursiveImport.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      214 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportUserModuleWithAlias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportVariable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      196 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/FromImportWithGlobalVariables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportInteropWithAlias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportNonExistentPackage.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      129 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportPythonLib.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportTyping.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportTypingWithAlias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      221 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportUserModule.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      226 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportUserModuleRecursiveImport.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      199 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportUserModuleWithAlias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportUserModuleWithNotImportedSymbols.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/ImportUserModuleWithNotImportedVariables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      205 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/UserModuleWithRecursiveImport.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/import_test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.184007 neo3-boa-0.9.0/boa3_test/test_sc/interop_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/interop_test/UpdateContract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/test_sc/interop_test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.184007 neo3-boa-0.9.0/boa3_test/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10908 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/boa_test.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.192007 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12346 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_any.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22226 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_arithmetic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8432 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_assert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1293 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_boa_builtin_method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48062 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_builtin_method.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21876 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_bytes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3634 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_class.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13576 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_constant.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17237 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8448 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_event.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16442 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_exception.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25010 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_file_generation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17489 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_for.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37776 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_function.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21977 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_if.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10497 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_import.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.192007 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17407 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_blockchain.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21675 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_contract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23476 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_crypto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2338 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_iterator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3825 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7352 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_oracle.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3123 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_policy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3460 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_role.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23192 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_runtime.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29473 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_stdlib.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30558 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_storage.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    38927 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16583 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_logical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7287 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_metadata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7531 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_multiple_expressions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21111 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_neo_types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4793 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_none.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3362 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_optional.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9219 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_python_operation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26697 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_range.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25996 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_relational.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3745 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_reversed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8052 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_string.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13717 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_test_engine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19115 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_tuple.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9317 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4990 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_typing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3264 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_union.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23569 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_variable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16987 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_while.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.196007 neo3-boa-0.9.0/boa3_test/tests/examples_tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25818 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_HTLC.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19067 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_NEP17.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    50994 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_amm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_hello_world.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21483 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_ico.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9844 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_nep5.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3024 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_update_contract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34385 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_wrapped_neo.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.196007 neo3-boa-0.9.0/boa3_test/tests/neo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/neo/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.196007 neo3-boa-0.9.0/boa3_test/tests/neo/smart_contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/neo/smart_contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2509 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/neo/smart_contract/test_neffile.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.196007 neo3-boa-0.9.0/boa3_test/tests/test_classes/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       50 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/TestExecutionException.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.196007 neo3-boa-0.9.0/boa3_test/tests/test_classes/binaryserializer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1947 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/binaryserializer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2191 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/block.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.196007 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1198 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neoabistruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      669 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neoeventstruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1869 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neomanifeststruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1166 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neomethodstruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1302 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neopermissionsstruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      966 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neostruct.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/nativeaccountstate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1111 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/nativecontractprefix.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/signer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5961 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/storage.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      670 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/testcontract.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14406 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/testengine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3164 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/transaction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.200007 neo3-boa-0.9.0/boa3_test/tests/test_classes/transactionattribute/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/transactionattribute/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2193 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      681 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/transactionattribute/transactionattributetype.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      968 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/boa3_test/tests/test_classes/witness.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-02 17:17:41.200007 neo3-boa-0.9.0/neo3_boa.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4186 2021-08-02 17:17:40.000000 neo3-boa-0.9.0/neo3_boa.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27991 2021-08-02 17:17:41.000000 neo3-boa-0.9.0/neo3_boa.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-08-02 17:17:40.000000 neo3-boa-0.9.0/neo3_boa.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2021-08-02 17:17:40.000000 neo3-boa-0.9.0/neo3_boa.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      139 2021-08-02 17:17:40.000000 neo3-boa-0.9.0/neo3_boa.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2021-08-02 17:17:40.000000 neo3-boa-0.9.0/neo3_boa.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2021-08-02 17:17:41.200007 neo3-boa-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4548 2021-08-02 17:17:26.000000 neo3-boa-0.9.0/setup.py
```

### Comparing `neo3-boa-0.8.3/PKG-INFO` & `neo3-boa-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo3-boa
-Version: 0.8.3
+Version: 0.9.0
 Summary: A Python compiler for the Neo3 Virtual Machine
 Home-page: https://github.com/CityOfZion/neo3-boa
 License: Apache License 2.0
 Description: 
         ============================================
         Python compiler for the Neo3 Virtual Machine
         ============================================
```

### Comparing `neo3-boa-0.8.3/README.rst` & `neo3-boa-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/analyser.py` & `neo3-boa-0.9.0/boa3/analyser/analyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/astanalyser.py` & `neo3-boa-0.9.0/boa3/analyser/astanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/astoptimizer.py` & `neo3-boa-0.9.0/boa3/analyser/astoptimizer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/builtinfunctioncallanalyser.py` & `neo3-boa-0.9.0/boa3/analyser/builtinfunctioncallanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/constructanalyser.py` & `neo3-boa-0.9.0/boa3/analyser/constructanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/importanalyser.py` & `neo3-boa-0.9.0/boa3/analyser/importanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/model/functionarguments.py` & `neo3-boa-0.9.0/boa3/analyser/model/functionarguments.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/model/optimizer/Operation.py` & `neo3-boa-0.9.0/boa3/analyser/model/optimizer/Operation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/model/optimizer/__init__.py` & `neo3-boa-0.9.0/boa3/analyser/model/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/model/symbolscope.py` & `neo3-boa-0.9.0/boa3/analyser/model/symbolscope.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/moduleanalyser.py` & `neo3-boa-0.9.0/boa3/analyser/moduleanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/supportedstandard/standardanalyser.py` & `neo3-boa-0.9.0/boa3/analyser/supportedstandard/standardanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/analyser/typeanalyser.py` & `neo3-boa-0.9.0/boa3/analyser/typeanalyser.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/boa3.py` & `neo3-boa-0.9.0/boa3/boa3.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/contract/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/blockchain/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/blockchain/block.py` & `neo3-boa-0.9.0/boa3/builtin/interop/blockchain/block.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     :vartype version: int
     :ivar previous_hash: the hash of the previous block
     :vartype previous_hash: UInt256
     :ivar merkle_root: the merkle root of the transactions
     :vartype merkle_root: UInt256
     :ivar timestamp: UTC timestamp of the block in milliseconds
     :vartype timestamp: int
+    :ivar nonce: a random number used once in the cryptography
+    :vartype nonce: int
     :ivar index: the index of the block
     :vartype index: int
     :ivar primary_index: the primary index of the consensus node that generated this block
     :vartype primary_index: int
     :ivar next_consensus: the script hash of the consensus nodes that generates the next block
     :vartype next_consensus: UInt160
     :ivar transaction_count: the number of transactions on this block
@@ -27,11 +29,12 @@
 
     def __init__(self):
         self.hash: UInt256 = UInt256()
         self.version: int = 0
         self.previous_hash: UInt256 = UInt256()
         self.merkle_root: UInt256 = UInt256()
         self.timestamp: int = 0
+        self.nonce: int = 0
         self.index: int = 0
         self.primary_index: int = 0
         self.next_consensus: UInt160 = UInt160()
         self.transaction_count: int = 0
```

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/blockchain/transaction.py` & `neo3-boa-0.9.0/boa3/builtin/interop/blockchain/transaction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/contract/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/contract/contract.py` & `neo3-boa-0.9.0/boa3/builtin/interop/contract/contract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/contract/contractmanifest.py` & `neo3-boa-0.9.0/boa3/builtin/interop/contract/contractmanifest.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/crypto/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/iterator/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/json/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/json/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/oracle/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/oracle/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Union
 
+from boa3.builtin.interop.oracle.oracleresponsecode import OracleResponseCode
+
 
 class Oracle:
     """
     Neo Oracle Service is an out-of-chain data access service built into Neo N3. It allows users to request the external
     data sources in smart contracts, and Oracle nodes designated by the committee will access the specified data source
     then pass the result in the callback function to continue executing the smart contract logic.
     """
```

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/policy/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/runtime/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/runtime/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,26 +58,46 @@
     :type script_hash: UInt160
     :return: It will return an array of all matched notifications
     :rtype: List[Notification]
     """
     pass
 
 
+def get_network() -> int:
+    """
+    Gets the magic number of the current network.
+
+    :return: the magic number of the current network
+    :rtype: int
+    """
+    pass
+
+
 def burn_gas(gas: int):
     """
     Burns GAS to benefit the NEO ecosystem.
 
     :param gas: the amount of GAS that will be burned
     :type gas: int
 
     :raise Exception: raised if gas value is negative.
     """
     pass
 
 
+def get_random() -> int:
+    """
+    Gets the next random number.
+
+    :return: the next random number
+    :rtype: int
+    """
+    pass
+
+
 executing_script_hash: UInt160 = UInt160()
 """
 Gets the script hash of the current context.
 
 :meta hide-value:
 """
```

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/runtime/notification.py` & `neo3-boa-0.9.0/boa3/builtin/interop/runtime/notification.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/stdlib/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/stdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/storage/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/interop/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/storage/storagecontext.py` & `neo3-boa-0.9.0/boa3/builtin/interop/storage/storagecontext.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/interop/storage/storagemap.py` & `neo3-boa-0.9.0/boa3/builtin/interop/storage/storagemap.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/builtin/type/__init__.py` & `neo3-boa-0.9.0/boa3/builtin/type/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/cli.py` & `neo3-boa-0.9.0/boa3/cli.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/codegenerator/__init__.py` & `neo3-boa-0.9.0/boa3/compiler/codegenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/codegenerator/codegenerator.py` & `neo3-boa-0.9.0/boa3/compiler/codegenerator/codegenerator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/codegenerator/codegeneratorvisitor.py` & `neo3-boa-0.9.0/boa3/compiler/codegenerator/codegeneratorvisitor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/codegenerator/initstatementsvisitor.py` & `neo3-boa-0.9.0/boa3/compiler/codegenerator/initstatementsvisitor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/codegenerator/stackmemento.py` & `neo3-boa-0.9.0/boa3/compiler/codegenerator/stackmemento.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/codegenerator/vmcodemapping.py` & `neo3-boa-0.9.0/boa3/compiler/codegenerator/vmcodemapping.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/compiler.py` & `neo3-boa-0.9.0/boa3/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/compiler/filegenerator.py` & `neo3-boa-0.9.0/boa3/compiler/filegenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             "permissions": [
                 {
                     "contract": "*",
                     "methods": "*"
                 }
             ],
             "trusts": [],
-            "features": [],
+            "features": {},
             "supportedstandards": self._metadata.supported_standards,
             "extra": self._metadata.extra if len(self._metadata.extra) > 0 else None
         }
 
     def _get_abi_info(self) -> Dict[str, Any]:
         """
         Gets the abi information in a dictionary format
```

### Comparing `neo3-boa-0.8.3/boa3/constants.py` & `neo3-boa-0.9.0/boa3/constants.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/exception/CompilerError.py` & `neo3-boa-0.9.0/boa3/exception/CompilerError.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/exception/CompilerWarning.py` & `neo3-boa-0.9.0/boa3/exception/CompilerWarning.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/attribute.py` & `neo3-boa-0.9.0/boa3/model/attribute.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/builtin.py` & `neo3-boa-0.9.0/boa3/model/builtin/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,18 @@
     # python builtin class constructor
     ByteArray = ByteArrayMethod()
     Range = RangeMethod()
     Reversed = ReversedMethod()
     Exception = ExceptionMethod()
 
     # python class method
+    CountSequence = CountSequenceMethod()
+    CountStr = CountStrMethod()
     SequenceAppend = AppendMethod()
     SequenceClear = ClearMethod()
-    SequenceCount = CountMethod()
     SequenceExtend = ExtendMethod()
     SequenceInsert = InsertMethod()
     SequencePop = PopMethod()
     SequenceRemove = RemoveMethod()
     SequenceReverse = ReverseMethod()
     DictKeys = MapKeysMethod()
     DictValues = MapValuesMethod()
@@ -79,29 +80,30 @@
 
     _python_builtins: List[IdentifiedSymbol] = [Abs,
                                                 ByteArray,
                                                 ConvertToBool,
                                                 ConvertToBytes,
                                                 ConvertToInt,
                                                 ConvertToStr,
+                                                CountSequence,
+                                                CountStr,
                                                 DictKeys,
                                                 DictValues,
                                                 Exception,
                                                 Exit,
                                                 IsInstance,
                                                 Len,
                                                 Max,
                                                 Min,
                                                 Print,
                                                 Range,
                                                 Reversed,
                                                 ScriptHash,
                                                 SequenceAppend,
                                                 SequenceClear,
-                                                SequenceCount,
                                                 SequenceExtend,
                                                 SequenceInsert,
                                                 SequencePop,
                                                 SequenceRemove,
                                                 SequenceReverse,
                                                 Sqrt,
                                                 StrSplit,
```

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/builtincallable.py` & `neo3-boa-0.9.0/boa3/model/builtin/builtincallable.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 __all__ = ['AppendMethod',
            'ClearMethod',
-           'CountMethod',
+           'CountSequenceMethod',
+           'CountStrMethod',
            'ExtendMethod',
            'InsertMethod',
            'MapKeysMethod',
            'MapValuesMethod',
            'PopMethod',
            'RemoveMethod',
            'ReverseMethod',
            'ToBoolMethod',
            'ToBytesMethod',
            'ToIntMethod',
            'ToStrMethod']
 
 from boa3.model.builtin.classmethod.appendmethod import AppendMethod
 from boa3.model.builtin.classmethod.clearmethod import ClearMethod
-from boa3.model.builtin.classmethod.countmethod import CountMethod
+from boa3.model.builtin.classmethod.countsequencemethod import CountSequenceMethod
+from boa3.model.builtin.classmethod.countstrmethod import CountStrMethod
 from boa3.model.builtin.classmethod.extendmethod import ExtendMethod
 from boa3.model.builtin.classmethod.insertmethod import InsertMethod
 from boa3.model.builtin.classmethod.mapkeysmethod import MapKeysMethod
 from boa3.model.builtin.classmethod.mapvaluesmethod import MapValuesMethod
 from boa3.model.builtin.classmethod.popmethod import PopMethod
 from boa3.model.builtin.classmethod.removemethod import RemoveMethod
 from boa3.model.builtin.classmethod.reversemethod import ReverseMethod
```

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/appendmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/appendmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/clearmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/clearmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/countmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/countsequencemethod.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,37 @@
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
-from boa3.model.builtin.method.builtinmethod import IBuiltinMethod
+from boa3.model.builtin.classmethod.countmethod import CountMethod
 from boa3.model.expression import IExpression
 from boa3.model.type.collection.sequence.sequencetype import SequenceType
 from boa3.model.type.itype import IType
 from boa3.model.variable import Variable
 from boa3.neo.vm.opcode.Opcode import Opcode
 
 
-class CountMethod(IBuiltinMethod):
+class CountSequenceMethod(CountMethod):
 
     def __init__(self, sequence_type: Optional[SequenceType] = None, arg_value: Optional[IType] = None):
         from boa3.model.type.type import Type
-        identifier = 'count'
         if not isinstance(sequence_type, SequenceType):
             sequence_type = Type.sequence
         if not isinstance(arg_value, IType):
             arg_value = Type.any
 
         args: Dict[str, Variable] = {
             'self': Variable(sequence_type),
             'value': Variable(arg_value)
         }
-        super().__init__(identifier, args, return_type=Type.int)
 
-    @property
-    def _arg_self(self) -> Variable:
-        return self.args['self']
-
-    @property
-    def _arg_value(self) -> Variable:
-        return self.args['value']
+        super().__init__(args)
 
     @property
     def is_supported(self) -> bool:
-        sequence_type: IType = self._arg_self.type
         value_type: IType = self._arg_value.type
 
-        # TODO: change when 'str.count()' is supported
-        from boa3.model.type.primitive.strtype import StrType
-        if isinstance(sequence_type, StrType):
-            return False
-
         # TODO: change when 'sequence.count(list or tuple)' is supported
         from boa3.model.type.collection.sequence.mutable.listtype import ListType
         from boa3.model.type.collection.sequence.tupletype import TupleType
         if isinstance(value_type, (ListType, TupleType)):
             return False
         return True
 
@@ -69,99 +55,86 @@
 
     @property
     def opcode(self) -> List[Tuple[Opcode, bytes]]:
         from boa3.compiler.codegenerator import get_bytes_count
 
         jmp_place_holder = (Opcode.JMP, b'\x01')
 
-        repack_array = [            # recreates an array to not change the original one
+        # region Sequence logic
+
+        repack_array = [  # recreates an array to not change the original one
             (Opcode.UNPACK, b''),
             (Opcode.PACK, b''),
         ]
 
-        sequence_initialize = [     # initializes variables
-            (Opcode.PUSH0, b''),    # count = 0
+        sequence_initialize = [  # initializes variables
+            (Opcode.PUSH0, b''),  # count = 0
             (Opcode.OVER, b''),
             (Opcode.SIZE, b''),
-            (Opcode.DEC, b''),      # index = len(sequence) - -1
+            (Opcode.DEC, b''),  # index = len(sequence) - -1
         ]
 
-        sequence_verify_while = [   # verifies if all the elements from the sequence were visited
-            (Opcode.DUP, b''),      # would be equivalent to: while (index >= 0)
+        sequence_verify_while = [  # verifies if all the elements from the sequence were visited
+            (Opcode.DUP, b''),  # would be equivalent to: while (index >= 0)
             (Opcode.SIGN, b''),
-            (Opcode.PUSH0, b''),    # if index < 0:
-            jmp_place_holder,           # jump to clean the stack
+            (Opcode.PUSH0, b''),  # if index < 0:
+            jmp_place_holder,  # jump to clean the stack
         ]
 
-        sequence_get_element = [    # gets a element from the sequence
+        sequence_get_element = [  # gets a element from the sequence
             (Opcode.PUSH2, b''),
             (Opcode.PICK, b''),
             (Opcode.OVER, b''),
             (Opcode.PICKITEM, b'')  # element = sequence[index]
         ]
 
-        sequence_equals = [         # verifies if the element and the given value are the same
+        sequence_equals = [  # verifies if the element and the given value are the same
             (Opcode.PUSH4, b''),
             (Opcode.PICK, b''),
-            (Opcode.EQUAL, b''),    # if element != value:
-            jmp_place_holder            # jump to list_tuple_count_index_dec
+            (Opcode.EQUAL, b''),  # if element != value:
+            jmp_place_holder  # jump to list_tuple_count_index_dec
         ]
 
-        sequence_count_inc = [      # increment count if element == value
+        sequence_count_inc = [  # increment count if element == value
             (Opcode.SWAP, b''),
-            (Opcode.INC, b''),      # count++
+            (Opcode.INC, b''),  # count++
             (Opcode.SWAP, b''),
         ]
 
         num_jmp_code = get_bytes_count(sequence_count_inc)
         jmp_to_dec_statement = Opcode.get_jump_and_data(Opcode.JMPIFNOT, num_jmp_code, True)
         sequence_equals[-1] = jmp_to_dec_statement
 
         list_tuple_count_index_dec = [  # decreases the index
-            (Opcode.DEC, b''),          # index--
+            (Opcode.DEC, b''),  # index--
             # return to the while verification
         ]
 
         num_jmp_code = -get_bytes_count(list_tuple_count_index_dec + sequence_count_inc + sequence_equals +
                                         sequence_get_element + sequence_verify_while)
         jmp_back_to_while_verify_statement = Opcode.get_jump_and_data(Opcode.JMP, num_jmp_code)
         list_tuple_count_index_dec.append(jmp_back_to_while_verify_statement)
 
         num_jmp_code = get_bytes_count(sequence_get_element + sequence_equals +
                                        sequence_count_inc + list_tuple_count_index_dec)
         jmp_to_clean_statement = Opcode.get_jump_and_data(Opcode.JMPLT, num_jmp_code, True)
         sequence_verify_while[-1] = jmp_to_clean_statement
 
-        clean_stack = [
+        sequence_clean_stack = [
             (Opcode.DROP, b''),
             (Opcode.REVERSE3, b''),
             (Opcode.DROP, b''),
             (Opcode.DROP, b''),
         ]
 
+        # endregion
+
         return (
             repack_array +
             sequence_initialize +
             sequence_verify_while +
             sequence_get_element +
             sequence_equals +
             sequence_count_inc +
             list_tuple_count_index_dec +
-            clean_stack
+            sequence_clean_stack
         )
-
-    @property
-    def _args_on_stack(self) -> int:
-        return len(self.args)
-
-    @property
-    def _body(self) -> Optional[str]:
-        return
-
-    def build(self, value: Any) -> IBuiltinMethod:
-        if isinstance(value, List) or isinstance(value, list):
-            if len(value) == 2:
-                if type(value[0]) == type(self.args['self'].type) and type(value[1]) == type(self.args['value'].type):
-                    return self
-
-                return CountMethod(value[0], value[1])
-        return super().build(value)
```

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/extendmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/extendmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/insertmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/insertmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/mapkeysmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/mapkeysmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/mapvaluesmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/mapvaluesmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/popmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/popmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/removemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/removemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/reversemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/reversemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/toboolmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/toboolmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/tobytesmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/tobytesmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/tointmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/tointmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/classmethod/tostrmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/classmethod/tostrmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/contract/abortmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/contract/abortmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/contract/nep17transferevent.py` & `neo3-boa-0.9.0/boa3/model/builtin/contract/nep17transferevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/contract/nep5transferevent.py` & `neo3-boa-0.9.0/boa3/model/builtin/contract/nep5transferevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/decorator/builtindecorator.py` & `neo3-boa-0.9.0/boa3/model/builtin/decorator/builtindecorator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/internal/innerdeploymethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/internal/innerdeploymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/internal/internalmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/internal/internalmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/blocktype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/blocktype.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
         self._variables: Dict[str, Variable] = {
             'hash': Variable(uint256),
             'version': Variable(Type.int),
             'previous_hash': Variable(uint256),
             'merkle_root': Variable(uint256),
             'timestamp': Variable(Type.int),
+            'nonce': Variable(Type.int),
             'index': Variable(Type.int),
             'primary_index': Variable(Type.int),
             'next_consensus': Variable(UInt160Type.build()),
             'transaction_count': Variable(Type.int)
         }
         self._constructor: Method = None
 
@@ -90,20 +91,21 @@
         uint256_default = Integer(32).to_byte_array() + bytes(32)
 
         return [
             (Opcode.PUSH0, b''),  # transaction_count
             (Opcode.PUSHDATA1, uint160_default),  # next_consensus
             (Opcode.PUSH0, b''),  # primary_index
             (Opcode.PUSH0, b''),  # index
+            (Opcode.PUSH0, b''),  # nonce
             (Opcode.PUSH0, b''),  # timestamp
             (Opcode.PUSHDATA1, uint256_default),  # merkle_root
             (Opcode.PUSHDATA1, uint256_default),  # previous_hash
             (Opcode.PUSH0, b''),  # version
             (Opcode.PUSHDATA1, uint256_default),  # hash
-            (Opcode.PUSH9, b''),
+            (Opcode.PUSH10, b''),
             (Opcode.PACK, b'')
         ]
 
     @property
     def _args_on_stack(self) -> int:
         return len(self.args)
```

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/currenthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/currenthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/currentindexmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/currentindexmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/getblockmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/getblockmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/getcontractmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/getcontractmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/getcurrentheightmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/getcurrentheightmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/gettransactionfromblockmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/gettransactionfromblockmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/gettransactionheightmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/gettransactionheightmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/gettransactionmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/gettransactionmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/blockchain/transactiontype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/blockchain/transactiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/callflagstype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/callflagstype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/callmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/callmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractabitype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractabitype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contracteventdescriptortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractgrouptype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractgrouptype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractmanifesttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractmethoddescriptortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractparameterdefinitiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractparametertype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractparametertype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiondescriptortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contractmanifest/contractpermissiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/contracttype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/contracttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/createmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/createmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/createmultisigaccountmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/createmultisigaccountmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/createstandardaccountmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/createstandardaccountmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/getcallflagsmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/getcallflagsmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/getgasscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/getgasscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/getneoscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/getneoscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/contract/updatemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/contract/updatemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/checkmultisigmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/checkmultisigmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/checksigmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/checksigmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/hash160method.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/hash160method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/hash256method.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/hash256method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/verifywithecdsasecp256k1.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/verifywithecdsasecp256k1.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/crypto/verifywithecdsasecp256r1.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/crypto/verifywithecdsasecp256r1.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/interop.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/interop.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     BlockType = BlockType.build()
     CallFlagsType = CallFlagsType()
     ContractManifestType = ContractManifestType.build()
     ContractType = ContractType.build()
     FindOptionsType = FindOptionsType()
     Iterator = IteratorType.build()
     NotificationType = NotificationType.build()
+    OracleResponseCode = OracleResponseCodeType.build()
     OracleType = OracleType.build()
     RoleType = RoleType.build()
     StorageContextType = StorageContextType.build()
     StorageMapType = StorageMapType.build()
     TransactionType = TransactionType.build()
     TriggerType = TriggerType()
 
@@ -120,15 +121,17 @@
     BlockTime = BlockTimeProperty()
     BurnGas = BurnGasMethod()
     CallingScriptHash = CallingScriptHashProperty()
     CheckWitness = CheckWitnessMethod()
     EntryScriptHash = EntryScriptHashProperty()
     ExecutingScriptHash = ExecutingScriptHashProperty()
     GasLeft = GasLeftProperty()
+    GetNetwork = GetNetworkMethod()
     GetNotifications = GetNotificationsMethod(NotificationType)
+    GetRandom = GetRandomMethod()
     GetTrigger = GetTriggerMethod(TriggerType)
     InvocationCounter = InvocationCounterProperty()
     Log = LogMethod()
     Notify = NotifyMethod()
     Platform = PlatformProperty()
     ScriptContainer = ScriptContainerProperty()
 
@@ -250,22 +253,28 @@
                                    ]
                           )
 
     NotificationModule = Package(identifier=NotificationType.identifier.lower(),
                                  types=[NotificationType]
                                  )
 
+    OracleResponseCodeModule = Package(identifier=OracleResponseCode.identifier.lower(),
+                                       types=[OracleResponseCode]
+                                       )
+
     OracleModule = Package(identifier=OracleType.identifier.lower(),
                            types=[OracleType]
                            )
 
     OraclePackage = Package(identifier=InteropPackage.Oracle,
-                            types=[OracleType
+                            types=[OracleResponseCode,
+                                   OracleType
                                    ],
-                            packages=[OracleModule
+                            packages=[OracleModule,
+                                      OracleResponseCodeModule
                                       ]
                             )
 
     TriggerTypeModule = Package(identifier=TriggerType.identifier.lower(),
                                 types=[TriggerType]
                                 )
 
@@ -293,15 +302,17 @@
                                          Platform,
                                          InvocationCounter,
                                          EntryScriptHash,
                                          ScriptContainer
                                          ],
                              methods=[BurnGas,
                                       CheckWitness,
+                                      GetNetwork,
                                       GetNotifications,
+                                      GetRandom,
                                       GetTrigger,
                                       Log,
                                       Notify
                                       ],
                              packages=[NotificationModule,
                                        TriggerTypeModule
                                        ]
```

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/interopevent.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/interopevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/interopinterfacetype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/interopinterfacetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/interopmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/interopmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/getiteratorvalue.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/getiteratorvalue.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/iteratorinitmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/iteratorinitmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/iteratornextmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/iteratornextmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/iterator/iteratortype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/iterator/iteratortype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/ContractManagement/contractmanagementmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/ContractManagement/getcontractmanagementscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/CryptoLib/cryptolibmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/CryptoLib/getcryptolibscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Ledger/getledgerscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Ledger/ledgermethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Ledger/ledgermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Oracle/getoraclescripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/Oracle/oraclemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/Oracle/oraclemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/PolicyContract/getpolicycontractscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/PolicyContract/policycontractmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/RoleManagement/getrolemanagementscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/nativecontract/nativecontractmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/nativecontract/nativecontractmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/oraclegetpricemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/oraclegetpricemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/oraclerequestmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/oraclerequestmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/oracle/oracletype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/oracle/oracletype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/policy/isblockedmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/policy/isblockedmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/role/getdesignatedbyrolemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/role/getdesignatedbyrolemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/role/roletype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/role/roletype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 __all__ = ['BlockTimeProperty',
            'BurnGasMethod',
            'CallingScriptHashProperty',
            'CheckWitnessMethod',
            'EntryScriptHashProperty',
            'ExecutingScriptHashProperty',
            'GasLeftProperty',
+           'GetNetworkMethod',
            'GetNotificationsMethod',
+           'GetRandomMethod',
            'InvocationCounterProperty',
            'LogMethod',
            'NotificationType',
            'NotifyMethod',
            'PlatformProperty',
            'ScriptContainerProperty',
            'GetTriggerMethod',
@@ -20,15 +22,17 @@
 from boa3.model.builtin.interop.runtime.checkwitnessmethod import CheckWitnessMethod
 from boa3.model.builtin.interop.runtime.getblocktimemethod import BlockTimeProperty
 from boa3.model.builtin.interop.runtime.getcallingscripthashmethod import CallingScriptHashProperty
 from boa3.model.builtin.interop.runtime.getentryscripthashmethod import EntryScriptHashProperty
 from boa3.model.builtin.interop.runtime.getexecutingscripthashmethod import ExecutingScriptHashProperty
 from boa3.model.builtin.interop.runtime.getgasleftmethod import GasLeftProperty
 from boa3.model.builtin.interop.runtime.getinvocationcountermethod import InvocationCounterProperty
+from boa3.model.builtin.interop.runtime.getnetworkmethod import GetNetworkMethod
 from boa3.model.builtin.interop.runtime.getnotificationsmethod import GetNotificationsMethod
 from boa3.model.builtin.interop.runtime.getplatformmethod import PlatformProperty
+from boa3.model.builtin.interop.runtime.getrandommethod import GetRandomMethod
 from boa3.model.builtin.interop.runtime.gettriggermethod import GetTriggerMethod
 from boa3.model.builtin.interop.runtime.logmethod import LogMethod
 from boa3.model.builtin.interop.runtime.notificationtype import NotificationType
 from boa3.model.builtin.interop.runtime.notifymethod import NotifyMethod
 from boa3.model.builtin.interop.runtime.scriptcontainermethod import ScriptContainerProperty
 from boa3.model.builtin.interop.runtime.triggertype import TriggerType
```

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/checkwitnessmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/checkwitnessmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getblocktimemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getblocktimemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getcallingscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getcallingscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getentryscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getentryscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getexecutingscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getexecutingscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getgasleftmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getgasleftmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getinvocationcountermethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getinvocationcountermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getnotificationsmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getnotificationsmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/getplatformmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/getplatformmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/notificationtype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/notificationtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/notifymethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/notifymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/scriptcontainermethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/scriptcontainermethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/runtime/triggertype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/runtime/triggertype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/atoimethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/atoimethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/itoamethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/itoamethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/memorycomparemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/memorycomparemethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import ast
 from typing import Dict
 
 from boa3.model.builtin.interop.nativecontract import StdLibMethod
 from boa3.model.variable import Variable
 
 
 class MemoryCompareMethod(StdLibMethod):
```

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/stdlib/memorysearchmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/stdlib/memorysearchmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/findoptionstype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/findoptionstype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/storagecontextasreadonlymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/storagecontextcreatemapmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagecontext/storagecontexttype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagecontext/storagecontexttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagedeletemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagedeletemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagefindmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagefindmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagegetcontextmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagegetcontextmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagegetmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagegetmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagegetreadonlycontextmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagegetreadonlycontextmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemapdeletemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemapgetmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemapgetmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemapputmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemapputmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storagemap/storagemaptype.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storagemap/storagemaptype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/interop/storage/storageputmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/interop/storage/storageputmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/__init__.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/absmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/absmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/builtinevent.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/builtinevent.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/builtinmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/builtinmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/bytearraymethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/bytearraymethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/createeventmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/createeventmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/ecpointmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/ecpointmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/exceptionmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/exceptionmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/exitmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/exitmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/isinstancemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/isinstancemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/lenmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/lenmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/maxmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/maxmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/minmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/minmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/printmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/printmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/rangemethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/rangemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/reversedmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/reversedmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/sqrtmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/sqrtmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/summethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/summethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/toscripthashmethod.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/toscripthashmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/uint160method.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/uint160method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/builtin/method/uint256method.py` & `neo3-boa-0.9.0/boa3/model/builtin/method/uint256method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/callable.py` & `neo3-boa-0.9.0/boa3/model/callable.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/debuginstruction.py` & `neo3-boa-0.9.0/boa3/model/debuginstruction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/event.py` & `neo3-boa-0.9.0/boa3/model/event.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/expression.py` & `neo3-boa-0.9.0/boa3/model/expression.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/identifiedsymbol.py` & `neo3-boa-0.9.0/boa3/model/identifiedsymbol.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/imports/builtin.py` & `neo3-boa-0.9.0/boa3/model/imports/builtin.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/imports/importsymbol.py` & `neo3-boa-0.9.0/boa3/model/imports/importsymbol.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/imports/package.py` & `neo3-boa-0.9.0/boa3/model/imports/package.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/method.py` & `neo3-boa-0.9.0/boa3/model/method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/module.py` & `neo3-boa-0.9.0/boa3/model/module.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/additional/membership.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/additional/membership.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/additional/notmembership.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/additional/notmembership.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/__init__.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/addition.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/addition.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/concat.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/concat.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/division.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/division.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/floordivision.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/floordivision.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/modulo.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/modulo.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/multiplication.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/multiplication.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/power.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/power.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/strmultiplication.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/strmultiplication.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/arithmetic/subtraction.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/arithmetic/subtraction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/binaryoperation.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/binaryoperation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/__init__.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/booleanand.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/booleanand.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/booleanor.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/booleanor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/leftshift.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/leftshift.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/logicand.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/logicand.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/logicor.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/logicor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/logicxor.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/logicxor.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/logical/rightshift.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/logical/rightshift.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/LessThan.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/LessThan.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/Lessthanorequal.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/Lessthanorequal.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/__init__.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/greaterthan.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/greaterthan.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/greaterthanorequal.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/greaterthanorequal.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/identity.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/identity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/notidentity.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/notidentity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/numericequality.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/numericequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/numericinequality.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/numericinequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/objectequality.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/objectequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binary/relational/objectinequality.py` & `neo3-boa-0.9.0/boa3/model/operation/binary/relational/objectinequality.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/binaryop.py` & `neo3-boa-0.9.0/boa3/model/operation/binaryop.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/operation.py` & `neo3-boa-0.9.0/boa3/model/operation/operation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/operator.py` & `neo3-boa-0.9.0/boa3/model/operation/operator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unary/booleannot.py` & `neo3-boa-0.9.0/boa3/model/operation/unary/booleannot.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unary/logicnot.py` & `neo3-boa-0.9.0/boa3/model/operation/unary/logicnot.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unary/negative.py` & `neo3-boa-0.9.0/boa3/model/operation/unary/negative.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unary/noneidentity.py` & `neo3-boa-0.9.0/boa3/model/operation/unary/noneidentity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unary/nonenotidentity.py` & `neo3-boa-0.9.0/boa3/model/operation/unary/nonenotidentity.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unary/positive.py` & `neo3-boa-0.9.0/boa3/model/operation/unary/positive.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unary/unaryoperation.py` & `neo3-boa-0.9.0/boa3/model/operation/unary/unaryoperation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/operation/unaryop.py` & `neo3-boa-0.9.0/boa3/model/operation/unaryop.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/property.py` & `neo3-boa-0.9.0/boa3/model/property.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/standards/neostandard.py` & `neo3-boa-0.9.0/boa3/model/standards/neostandard.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/standards/nep17standard.py` & `neo3-boa-0.9.0/boa3/model/standards/nep17standard.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/standards/standardmethod.py` & `neo3-boa-0.9.0/boa3/model/standards/standardmethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/annotation/metatype.py` & `neo3-boa-0.9.0/boa3/model/type/annotation/metatype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/annotation/optionaltype.py` & `neo3-boa-0.9.0/boa3/model/type/annotation/optionaltype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/annotation/uniontype.py` & `neo3-boa-0.9.0/boa3/model/type/annotation/uniontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/anytype.py` & `neo3-boa-0.9.0/boa3/model/type/anytype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/baseexceptiontype.py` & `neo3-boa-0.9.0/boa3/model/type/baseexceptiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/classes/classtype.py` & `neo3-boa-0.9.0/boa3/model/type/classes/classtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/genericcollectiontype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/genericcollectiontype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/icollection.py` & `neo3-boa-0.9.0/boa3/model/type/collection/icollection.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/mapping/genericmappingtype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/mapping/genericmappingtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/mapping/mappingtype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/mapping/mappingtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/mapping/mutable/dicttype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/mapping/mutable/dicttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/mapping/mutable/mutablemappingtype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/mapping/mutable/mutablemappingtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/ecpointtype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/ecpointtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/genericsequencetype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/genericsequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/genericmutablesequencetype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/genericmutablesequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/listtype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/listtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/mutable/mutablesequencetype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/mutable/mutablesequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/rangetype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/rangetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/reversedtype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/reversedtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/sequencetype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/sequencetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/tupletype.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/tupletype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/uint160type.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/uint160type.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/collection/sequence/uint256type.py` & `neo3-boa-0.9.0/boa3/model/type/collection/sequence/uint256type.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/itype.py` & `neo3-boa-0.9.0/boa3/model/type/itype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/primitive/booltype.py` & `neo3-boa-0.9.0/boa3/model/type/primitive/booltype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/primitive/bytearraytype.py` & `neo3-boa-0.9.0/boa3/model/type/primitive/bytearraytype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/primitive/bytestype.py` & `neo3-boa-0.9.0/boa3/model/type/primitive/bytestype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/primitive/inttype.py` & `neo3-boa-0.9.0/boa3/model/type/primitive/inttype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/primitive/nonetype.py` & `neo3-boa-0.9.0/boa3/model/type/primitive/nonetype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/primitive/strtype.py` & `neo3-boa-0.9.0/boa3/model/type/primitive/strtype.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/type.py` & `neo3-boa-0.9.0/boa3/model/type/type.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/typeutils.py` & `neo3-boa-0.9.0/boa3/model/type/typeutils.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/type/typingmethod/casttypemethod.py` & `neo3-boa-0.9.0/boa3/model/type/typingmethod/casttypemethod.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/model/variable.py` & `neo3-boa-0.9.0/boa3/model/variable.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/__init__.py` & `neo3-boa-0.9.0/boa3/neo/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/contracts/neffile.py` & `neo3-boa-0.9.0/boa3/neo/contracts/neffile.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/cryptography/__init__.py` & `neo3-boa-0.9.0/boa3/neo/cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/smart_contract/notification.py` & `neo3-boa-0.9.0/boa3/neo/smart_contract/notification.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/utils/__init__.py` & `neo3-boa-0.9.0/boa3/neo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/CallCode.py` & `neo3-boa-0.9.0/boa3/neo/vm/CallCode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/TryCode.py` & `neo3-boa-0.9.0/boa3/neo/vm/TryCode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/VMCode.py` & `neo3-boa-0.9.0/boa3/neo/vm/VMCode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/opcode/Opcode.py` & `neo3-boa-0.9.0/boa3/neo/vm/opcode/Opcode.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/opcode/OpcodeInfo.py` & `neo3-boa-0.9.0/boa3/neo/vm/opcode/OpcodeInfo.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/opcode/OpcodeInformation.py` & `neo3-boa-0.9.0/boa3/neo/vm/opcode/OpcodeInformation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/type/ContractParameterType.py` & `neo3-boa-0.9.0/boa3/neo/vm/type/ContractParameterType.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/type/Integer.py` & `neo3-boa-0.9.0/boa3/neo/vm/type/Integer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo/vm/type/StackItem.py` & `neo3-boa-0.9.0/boa3/neo/vm/type/StackItem.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo3/contracts/contracttypes.py` & `neo3-boa-0.9.0/boa3/neo3/contracts/contracttypes.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo3/contracts/native/nativetypes.py` & `neo3-boa-0.9.0/boa3/neo3/contracts/native/nativetypes.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo3/contracts/nef.py` & `neo3-boa-0.9.0/boa3/neo3/contracts/nef.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo3/core/serialization.py` & `neo3-boa-0.9.0/boa3/neo3/core/serialization.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo3/core/types/biginteger.py` & `neo3-boa-0.9.0/boa3/neo3/core/types/biginteger.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo3/core/types/uint.py` & `neo3-boa-0.9.0/boa3/neo3/core/types/uint.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3/neo3/core/utils.py` & `neo3-boa-0.9.0/boa3/neo3/core/utils.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/test_sc/bytes_test/SliceBoa2Test2.py` & `neo3-boa-0.9.0/boa3_test/test_sc/bytes_test/SliceBoa2Test2.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/boa_test.py` & `neo3-boa-0.9.0/boa3_test/tests/boa_test.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_any.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_any.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_arithmetic.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_assert.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_assert.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_boa_builtin_method.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_boa_builtin_method.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_builtin_method.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_builtin_method.py`

 * *Files 10% similar despite different names*

```diff
@@ -936,30 +936,28 @@
 
     # endregion
 
     # region sum test
 
     def test_sum(self):
         path = self.get_contract_path('Sum.py')
-        self.compile_and_save(path)
         engine = TestEngine()
 
         val = [1, 2, 3, 4]
         expected_result = sum(val)
         result = self.run_smart_contract(engine, path, 'main', val)
         self.assertEqual(expected_result, result)
 
         val = list(range(10, 20, 2))
         expected_result = sum(val)
         result = self.run_smart_contract(engine, path, 'main', val)
         self.assertEqual(expected_result, result)
 
     def test_sum_with_start(self):
         path = self.get_contract_path('SumWithStart.py')
-        self.compile_and_save(path)
         engine = TestEngine()
 
         val = [1, 2, 3, 4]
         expected_result = sum(val, 10)
         result = self.run_smart_contract(engine, path, 'main', val, 10)
         self.assertEqual(expected_result, result)
 
@@ -986,14 +984,47 @@
 
     def test_str_split(self):
         path = self.get_contract_path('StrSplit.py')
         engine = TestEngine()
 
         string = '1#2#3#4'
         separator = '#'
+        maxsplit = 2
+        expected_result = string.split(separator, maxsplit)
+        result = self.run_smart_contract(engine, path, 'main', string, separator, maxsplit)
+        self.assertEqual(expected_result, result)
+
+        string = '1#2#3#4'
+        separator = '#'
+        maxsplit = 1
+        expected_result = string.split(separator, maxsplit)
+        result = self.run_smart_contract(engine, path, 'main', string, separator, maxsplit)
+        self.assertEqual(expected_result, result)
+
+        string = '1#2#3#4'
+        separator = '#'
+        maxsplit = 0
+        expected_result = string.split(separator, maxsplit)
+        result = self.run_smart_contract(engine, path, 'main', string, separator, maxsplit)
+        self.assertEqual(expected_result, result)
+
+        string = 'unit123test123str123split'
+        separator = '123'
+        maxsplit = 1
+        expected_result = string.split(separator, maxsplit)
+        result = self.run_smart_contract(engine, path, 'main', string, separator, maxsplit)
+        self.assertEqual(expected_result, result)
+
+    def test_str_split_maxsplit_default(self):
+        path = self.get_contract_path('StrSplitMaxsplitDefault.py')
+        engine = TestEngine()
+        self.compile_and_save(path)
+
+        string = '1#2#3#4'
+        separator = '#'
         expected_result = string.split(separator)
         result = self.run_smart_contract(engine, path, 'main', string, separator)
         self.assertEqual(expected_result, result)
 
         string = 'unit123test123str123split'
         separator = '123'
         expected_result = string.split(separator)
@@ -1117,13 +1148,148 @@
         path = self.get_contract_path('CountRange.py')
         engine = TestEngine()
 
         expected_result = range(10).count(1)
         result = self.run_smart_contract(engine, path, 'main')
         self.assertEqual(expected_result, result)
 
+    def test_count_sequence_too_many_parameters(self):
+        path = self.get_contract_path('CountSequenceTooManyArguments.py')
+        self.assertCompilerLogs(CompilerError.UnexpectedArgument, path)
+
+    def test_count_sequence_too_few_parameters(self):
+        path = self.get_contract_path('CountSequenceTooFewArguments.py')
+        self.assertCompilerLogs(CompilerError.UnfilledArgument, path)
+
     def test_count_str(self):
         path = self.get_contract_path('CountStr.py')
-        # TODO: change test when str.count(substring, start, end) is implemented in the Opcode
+        engine = TestEngine()
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = 0
+        end = 43
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = 0
+        end = 1000
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = 0
+        end = -1000
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = 0
+        end = -4
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = 23
+        end = 43
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = -11
+        end = 43
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = -1000
+        end = 43
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeee'
+        substr = 'e'
+        start = 1000
+        end = 43
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'a string that will be used in the unit test'
+        substr = 'string'
+        start = 0
+        end = 43
+        expected_result = str_.count(substr, start, end)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start, end)
+        self.assertEqual(expected_result, result)
+
+    def test_count_str_end_default(self):
+        path = self.get_contract_path('CountStrEndDefault.py')
+        engine = TestEngine()
+
+        str_ = 'a string that will be used in the unit test'
+        substr = 'string'
+        start = 0
+        expected_result = str_.count(substr, start)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'a string that will be used in the unit test'
+        substr = 'string'
+        start = 4
+        expected_result = str_.count(substr, start)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeee'
+        substr = 'e'
+        start = 0
+        expected_result = str_.count(substr, start)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeee'
+        substr = 'e'
+        start = 5
+        expected_result = str_.count(substr, start)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr, start)
+        self.assertEqual(expected_result, result)
+
+    def test_count_str_default(self):
+        path = self.get_contract_path('CountStrDefault.py')
+        engine = TestEngine()
+
+        str_ = 'a string that will be used in the unit test'
+        substr = 'string'
+        expected_result = str_.count(substr)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr)
+        self.assertEqual(expected_result, result)
+
+        str_ = 'eeeeeeeeeee'
+        substr = 'e'
+        expected_result = str_.count(substr)
+        result = self.run_smart_contract(engine, path, 'main', str_, substr)
+        self.assertEqual(expected_result, result)
+
+    def test_count_str_too_many_parameters(self):
+        path = self.get_contract_path('CountStrTooManyArguments.py')
         self.assertCompilerLogs(CompilerError.UnexpectedArgument, path)
 
+    def test_count_str_too_few_parameters(self):
+        path = self.get_contract_path('CountStrTooFewArguments.py')
+        self.assertCompilerLogs(CompilerError.UnfilledArgument, path)
+
     # endregion
```

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_bytes.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_bytes.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_class.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_class.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_constant.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_dict.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_event.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_event.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_exception.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_file_generation.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_file_generation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_for.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_for.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_function.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_function.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_if.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_if.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_import.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_import.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_blockchain.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_blockchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,35 @@
 from boa3_test.tests.test_classes.testengine import TestEngine
 
 
 class TestBlockchainInterop(BoaTest):
 
     default_folder: str = 'test_sc/interop_test/blockchain'
 
+    def test_block_constructor(self):
+        path = self.get_contract_path('Block.py')
+        engine = TestEngine()
+
+        result = self.run_smart_contract(engine, path, 'main')
+        self.assertIsInstance(result, list)
+        self.assertEqual(10, len(result))
+        for k in range(len(result)):
+            if isinstance(result[k], str):
+                result[k] = String(result[k]).to_bytes()
+        self.assertEqual(UInt256(), UInt256(result[0]))   # hash
+        self.assertEqual(0, result[1])   # version
+        self.assertEqual(UInt256(), UInt256(result[2]))   # previous_hash
+        self.assertEqual(UInt256(), UInt256(result[3]))   # merkle_root
+        self.assertEqual(0, result[4])   # timestamp
+        self.assertEqual(0, result[5])   # nonce
+        self.assertEqual(0, result[6])   # index
+        self.assertEqual(0, result[7])   # primary_index
+        self.assertEqual(UInt160(), UInt160(result[8]))   # next_consensus
+        self.assertEqual(0, result[9])   # transaction_count
+
     def test_get_current_height(self):
         expected_output = (
             Opcode.SYSCALL
             + Interop.CurrentHeight.getter.interop_method_hash
             + Opcode.RET
         )
 
@@ -68,45 +89,45 @@
     def test_get_block_by_index(self):
         path = self.get_contract_path('GetBlockByIndex.py')
 
         engine = TestEngine()
         index = 0
         result = self.run_smart_contract(engine, path, 'Main', index)
         self.assertIsInstance(result, list)
-        self.assertEqual(9, len(result))
-        self.assertEqual(index, result[5])
+        self.assertEqual(10, len(result))
+        self.assertEqual(index, result[6])
 
         index = 10
         result = self.run_smart_contract(engine, path, 'Main', index)
         self.assertIsNone(result)
 
         engine.increase_block(10)
         result = self.run_smart_contract(engine, path, 'Main', index)
         self.assertIsInstance(result, list)
-        self.assertEqual(9, len(result))
-        self.assertEqual(index, result[5])
+        self.assertEqual(10, len(result))
+        self.assertEqual(index, result[6])
 
     def test_get_block_by_hash(self):
         path = self.get_contract_path('GetBlockByHash.py')
 
         engine = TestEngine()
         engine.increase_block(1)
         block_hash = bytes(32)
         result = self.run_smart_contract(engine, path, 'Main', block_hash)
         self.assertIsNone(result)
 
         from boa3.neo import from_hex_str
         # TODO: using genesis block hash for testing, change when TestEngine returns blocks hashes
-        block_hash = from_hex_str('0xc3db4ba50ede4f9e749bd97e1499953ae17e65a415c6bf9e38c01cf92b03d156')
+        block_hash = from_hex_str('0x1f4d1defa46faa5e7b9b8d3f79a06bec777d7c26c4aa5f6f5899a291daa87c15')
 
         result = self.run_smart_contract(engine, path, 'Main', block_hash)
         self.assertIsInstance(result, list)
-        self.assertEqual(9, len(result))
+        self.assertEqual(10, len(result))
         self.assertEqual(block_hash, result[0])
-        self.assertEqual(0, result[5])  # genesis block's index is zero
+        self.assertEqual(0, result[6])  # genesis block's index is zero
 
     def test_get_block_mismatched_types(self):
         path = self.get_contract_path('GetBlockMismatchedTypes.py')
         self.assertCompilerLogs(CompilerError.MismatchedTypes, path)
 
     def test_transaction_init(self):
         path = self.get_contract_path('Transaction.py')
```

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_contract.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_contract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_crypto.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_crypto.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_iterator.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_iterator.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_json.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_json.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_oracle.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_oracle.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_policy.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_policy.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_role.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_role.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_runtime.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -614,20 +614,42 @@
         self.assertIsInstance(result[4], int)
         self.assertIsInstance(result[5], int)
         self.assertIsInstance(result[6], int)
         if isinstance(result[6], str):
             result[6] = String(result[6]).to_bytes()
         self.assertIsInstance(result[7], bytes)
 
+    def test_get_network(self):
+        path = self.get_contract_path('GetNetwork.py')
+        engine = TestEngine()
+
+        result = self.run_smart_contract(engine, path, 'main')
+        self.assertEqual(5195086, result)   # Neo3 main net's magic number
+
+    def test_get_network_too_many_parameters(self):
+        path = self.get_contract_path('GetNetworkTooManyArguments.py')
+        self.assertCompilerLogs(CompilerError.UnexpectedArgument, path)
+
     def test_import_runtime(self):
         path = self.get_contract_path('ImportRuntime.py')
         engine = TestEngine()
 
         result = self.run_smart_contract(engine, path, 'main')
         self.assertIsInstance(result, int)
 
     def test_import_interop_runtime(self):
         path = self.get_contract_path('ImportInteropRuntime.py')
         engine = TestEngine()
 
         result = self.run_smart_contract(engine, path, 'main')
         self.assertIsInstance(result, int)
+
+    def test_get_random(self):
+        path = self.get_contract_path('GetRandom.py')
+        engine = TestEngine()
+
+        result = self.run_smart_contract(engine, path, 'main')
+        self.assertIsInstance(result, int)
+
+    def test_get_random_too_many_parameters(self):
+        path = self.get_contract_path('GetRandomTooManyArguments.py')
+        self.assertCompilerLogs(CompilerError.UnexpectedArgument, path)
```

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_stdlib.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_interop/test_storage.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_interop/test_storage.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_list.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_list.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_logical.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_logical.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_metadata.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_multiple_expressions.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_multiple_expressions.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_neo_types.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_neo_types.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_none.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_none.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_optional.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_optional.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_python_operation.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_python_operation.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_range.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_range.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_relational.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_relational.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_reversed.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_reversed.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_string.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_string.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_test_engine.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_test_engine.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_tuple.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_types.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_types.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_typing.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_union.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_union.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_variable.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/compiler_tests/test_while.py` & `neo3-boa-0.9.0/boa3_test/tests/compiler_tests/test_while.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_HTLC.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_HTLC.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_NEP17.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_NEP17.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from boa3 import constants
-from boa3.boa3 import Boa3
 from boa3.neo import to_script_hash
 from boa3.neo.cryptography import hash160
 from boa3.neo.vm.type.String import String
 from boa3_test.tests.boa_test import BoaTest
 from boa3_test.tests.test_classes.TestExecutionException import TestExecutionException
 from boa3_test.tests.test_classes.testengine import TestEngine
```

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_amm.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_amm.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_hello_world.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_ico.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_ico.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_nep5.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_nep5.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_update_contract.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_update_contract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/examples_tests/test_wrapped_neo.py` & `neo3-boa-0.9.0/boa3_test/tests/examples_tests/test_wrapped_neo.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/neo/smart_contract/test_neffile.py` & `neo3-boa-0.9.0/boa3_test/tests/neo/smart_contract/test_neffile.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/binaryserializer/__init__.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/binaryserializer/__init__.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/block.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/block.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neoabistruct.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neoabistruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neoeventstruct.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neoeventstruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neomanifeststruct.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neomanifeststruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neomethodstruct.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neomethodstruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neopermissionsstruct.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neopermissionsstruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/contract/neostruct.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/contract/neostruct.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/nativeaccountstate.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/nativeaccountstate.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/nativecontractprefix.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/nativecontractprefix.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/signer.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/signer.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/storage.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/storage.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/testcontract.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/testcontract.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/testengine.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/testengine.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/transaction.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/transaction.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/transactionattribute/oracleresponse.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/transactionattribute/transactionattribute.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/boa3_test/tests/test_classes/witness.py` & `neo3-boa-0.9.0/boa3_test/tests/test_classes/witness.py`

 * *Files identical despite different names*

### Comparing `neo3-boa-0.8.3/neo3_boa.egg-info/PKG-INFO` & `neo3-boa-0.9.0/neo3_boa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo3-boa
-Version: 0.8.3
+Version: 0.9.0
 Summary: A Python compiler for the Neo3 Virtual Machine
 Home-page: https://github.com/CityOfZion/neo3-boa
 License: Apache License 2.0
 Description: 
         ============================================
         Python compiler for the Neo3 Virtual Machine
         ============================================
```

### Comparing `neo3-boa-0.8.3/neo3_boa.egg-info/SOURCES.txt` & `neo3-boa-0.9.0/neo3_boa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 boa3/builtin/interop/contract/callflagstype.py
 boa3/builtin/interop/contract/contract.py
 boa3/builtin/interop/contract/contractmanifest.py
 boa3/builtin/interop/crypto/__init__.py
 boa3/builtin/interop/iterator/__init__.py
 boa3/builtin/interop/json/__init__.py
 boa3/builtin/interop/oracle/__init__.py
+boa3/builtin/interop/oracle/oracleresponsecode.py
 boa3/builtin/interop/policy/__init__.py
 boa3/builtin/interop/role/__init__.py
 boa3/builtin/interop/role/roletype.py
 boa3/builtin/interop/runtime/__init__.py
 boa3/builtin/interop/runtime/notification.py
 boa3/builtin/interop/runtime/triggertype.py
 boa3/builtin/interop/stdlib/__init__.py
@@ -80,14 +81,16 @@
 boa3/model/builtin/builtincallable.py
 boa3/model/builtin/builtinproperty.py
 boa3/model/builtin/neometadatatype.py
 boa3/model/builtin/classmethod/__init__.py
 boa3/model/builtin/classmethod/appendmethod.py
 boa3/model/builtin/classmethod/clearmethod.py
 boa3/model/builtin/classmethod/countmethod.py
+boa3/model/builtin/classmethod/countsequencemethod.py
+boa3/model/builtin/classmethod/countstrmethod.py
 boa3/model/builtin/classmethod/extendmethod.py
 boa3/model/builtin/classmethod/insertmethod.py
 boa3/model/builtin/classmethod/mapkeysmethod.py
 boa3/model/builtin/classmethod/mapvaluesmethod.py
 boa3/model/builtin/classmethod/popmethod.py
 boa3/model/builtin/classmethod/removemethod.py
 boa3/model/builtin/classmethod/reversemethod.py
@@ -184,14 +187,15 @@
 boa3/model/builtin/interop/nativecontract/RoleManagement/rolemanagementmethod.py
 boa3/model/builtin/interop/nativecontract/StdLib/__init__.py
 boa3/model/builtin/interop/nativecontract/StdLib/getstdlibscripthashmethod.py
 boa3/model/builtin/interop/nativecontract/StdLib/stdlibmethod.py
 boa3/model/builtin/interop/oracle/__init__.py
 boa3/model/builtin/interop/oracle/oraclegetpricemethod.py
 boa3/model/builtin/interop/oracle/oraclerequestmethod.py
+boa3/model/builtin/interop/oracle/oracleresponsecodetype.py
 boa3/model/builtin/interop/oracle/oracletype.py
 boa3/model/builtin/interop/policy/__init__.py
 boa3/model/builtin/interop/policy/getexecfeefactormethod.py
 boa3/model/builtin/interop/policy/getfeeperbytemethod.py
 boa3/model/builtin/interop/policy/getstoragepricemethod.py
 boa3/model/builtin/interop/policy/isblockedmethod.py
 boa3/model/builtin/interop/role/__init__.py
@@ -202,16 +206,18 @@
 boa3/model/builtin/interop/runtime/checkwitnessmethod.py
 boa3/model/builtin/interop/runtime/getblocktimemethod.py
 boa3/model/builtin/interop/runtime/getcallingscripthashmethod.py
 boa3/model/builtin/interop/runtime/getentryscripthashmethod.py
 boa3/model/builtin/interop/runtime/getexecutingscripthashmethod.py
 boa3/model/builtin/interop/runtime/getgasleftmethod.py
 boa3/model/builtin/interop/runtime/getinvocationcountermethod.py
+boa3/model/builtin/interop/runtime/getnetworkmethod.py
 boa3/model/builtin/interop/runtime/getnotificationsmethod.py
 boa3/model/builtin/interop/runtime/getplatformmethod.py
+boa3/model/builtin/interop/runtime/getrandommethod.py
 boa3/model/builtin/interop/runtime/gettriggermethod.py
 boa3/model/builtin/interop/runtime/logmethod.py
 boa3/model/builtin/interop/runtime/notificationtype.py
 boa3/model/builtin/interop/runtime/notifymethod.py
 boa3/model/builtin/interop/runtime/scriptcontainermethod.py
 boa3/model/builtin/interop/runtime/triggertype.py
 boa3/model/builtin/interop/stdlib/__init__.py
@@ -403,14 +409,17 @@
 boa3/neo3/contracts/native/nativetypes.py
 boa3/neo3/core/__init__.py
 boa3/neo3/core/serialization.py
 boa3/neo3/core/utils.py
 boa3/neo3/core/types/__init__.py
 boa3/neo3/core/types/biginteger.py
 boa3/neo3/core/types/uint.py
+boa3/neo3/network/__init__.py
+boa3/neo3/network/payloads/__init__.py
+boa3/neo3/network/payloads/oracleresponsecode.py
 boa3/neo3/vm/__init__.py
 boa3/neo3/vm/vmstate.py
 boa3_test/__init__.py
 boa3_test/test_sc/__init__.py
 boa3_test/test_sc/bytes_test/AssignSlice.py
 boa3_test/test_sc/bytes_test/BytearrayAppend.py
 boa3_test/test_sc/bytes_test/BytearrayAppendWithBuiltin.py
```

### Comparing `neo3-boa-0.8.3/setup.py` & `neo3-boa-0.9.0/setup.py`

 * *Files identical despite different names*

