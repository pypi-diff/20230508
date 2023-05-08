# Comparing `tmp/arch_lint-2.3.0.tar.gz` & `tmp/arch_lint-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_lint-2.3.0.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "arch_lint-2.4.0.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `arch_lint-2.3.0.tar` & `arch_lint-2.4.0.tar`

### file list

```diff
@@ -1,54 +1,60 @@
--rw-r--r--   0        0        0       85 1980-01-01 00:00:00.000000 arch_lint-2.3.0/.envrc
--rw-r--r--   0        0        0       40 1980-01-01 00:00:00.000000 arch_lint-2.3.0/.gitignore
--rw-r--r--   0        0        0     2184 1980-01-01 00:00:00.000000 arch_lint-2.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      235 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/__init__.py
--rw-r--r--   0        0        0     1732 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/_full_path.py
--rw-r--r--   0        0        0     1644 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/_utils.py
--rw-r--r--   0        0        0      109 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/dag/__init__.py
--rw-r--r--   0        0        0     1854 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/dag/_dag.py
--rw-r--r--   0        0        0     1766 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/dag/_dag_map.py
--rw-r--r--   0        0        0     4605 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/dag/check.py
--rw-r--r--   0        0        0      898 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/forbidden.py
--rw-r--r--   0        0        0     4257 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/graph.py
--rw-r--r--   0        0        0     1896 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/private.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/arch_lint/py.typed
--rw-r--r--   0        0        0      483 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/deps/default.nix
--rw-r--r--   0        0        0      217 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/deps/deprecated/stubs.nix
--rw-r--r--   0        0        0      363 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/deps/grimp/default.nix
--rw-r--r--   0        0        0      505 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/pkg/build.nix
--rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/pkg/check/tests.sh
--rwxr-xr-x   0        0        0      160 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/pkg/check/types.sh
--rw-r--r--   0        0        0      631 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/pkg/default.nix
--rw-r--r--   0        0        0      100 1980-01-01 00:00:00.000000 arch_lint-2.3.0/build/publish/default.nix
--rw-r--r--   0        0        0      220 1980-01-01 00:00:00.000000 arch_lint-2.3.0/ci/check.nix
--rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 arch_lint-2.3.0/ci/utils.sh
--rw-r--r--   0        0        0      983 1980-01-01 00:00:00.000000 arch_lint-2.3.0/default.nix
--rw-r--r--   0        0        0      987 1980-01-01 00:00:00.000000 arch_lint-2.3.0/flake.lock
--rw-r--r--   0        0        0      861 1980-01-01 00:00:00.000000 arch_lint-2.3.0/flake.nix
--rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 arch_lint-2.3.0/makes.lock.nix
--rw-r--r--   0        0        0      524 1980-01-01 00:00:00.000000 arch_lint-2.3.0/makes.nix
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/__init__.py
--rw-r--r--   0        0        0       71 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import/layer1/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import/layer1/_private_module/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import/layer1/_private_module/something.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_2/__init__.py
--rw-r--r--   0        0        0       73 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_2/foo.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_2/layer1/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_2/layer1/_private_module/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_2/layer1/_private_module/something.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_3/__init__.py
--rw-r--r--   0        0        0       83 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_3/foo.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_3/layer1/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_3/layer1/_private_module/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mock_module/illegal_import_3/layer1/_private_module/something.py
--rw-r--r--   0        0        0      787 1980-01-01 00:00:00.000000 arch_lint-2.3.0/mypy.ini
--rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 arch_lint-2.3.0/nix.conf
--rw-r--r--   0        0        0      484 1980-01-01 00:00:00.000000 arch_lint-2.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0      917 1980-01-01 00:00:00.000000 arch_lint-2.3.0/tests/arch.py
--rw-r--r--   0        0        0      908 1980-01-01 00:00:00.000000 arch_lint-2.3.0/tests/mock_arch.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.3.0/tests/py.typed
--rw-r--r--   0        0        0     2013 1980-01-01 00:00:00.000000 arch_lint-2.3.0/tests/test_mock_module.py
--rw-r--r--   0        0        0     1052 1980-01-01 00:00:00.000000 arch_lint-2.3.0/tests/test_self_arch.py
--rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 arch_lint-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 arch_lint-2.4.0/.envrc
+-rw-r--r--   0        0        0       40 1980-01-01 00:00:00.000000 arch_lint-2.4.0/.gitignore
+-rw-r--r--   0        0        0     2088 1980-01-01 00:00:00.000000 arch_lint-2.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      235 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/__init__.py
+-rw-r--r--   0        0        0     1732 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/_full_path.py
+-rw-r--r--   0        0        0     1644 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/_utils.py
+-rw-r--r--   0        0        0      109 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/dag/__init__.py
+-rw-r--r--   0        0        0     1854 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/dag/_dag.py
+-rw-r--r--   0        0        0     1766 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/dag/_dag_map.py
+-rw-r--r--   0        0        0     5426 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/dag/check.py
+-rw-r--r--   0        0        0      898 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/forbidden.py
+-rw-r--r--   0        0        0     4257 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/graph.py
+-rw-r--r--   0        0        0     1896 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/private.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/arch_lint/py.typed
+-rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/ci/utils.sh
+-rw-r--r--   0        0        0      724 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/default.nix
+-rw-r--r--   0        0        0      879 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/deps/default.nix
+-rw-r--r--   0        0        0      217 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/deps/deprecated/stubs.nix
+-rw-r--r--   0        0        0      363 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/deps/grimp/default.nix
+-rw-r--r--   0        0        0      251 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/deps/networkx.nix
+-rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/deps/override_utils.nix
+-rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/dev_env/default.nix
+-rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/dev_env/hook.sh
+-rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/dev_env/vs_settings.py
+-rw-r--r--   0        0        0      210 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/generic_builder/check.nix
+-rw-r--r--   0        0        0      341 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/generic_builder/default.nix
+-rw-r--r--   0        0        0      245 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/generic_builder/env.nix
+-rw-r--r--   0        0        0      310 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/generic_builder/metadata.nix
+-rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/generic_builder/pkg/check/tests.sh
+-rwxr-xr-x   0        0        0      160 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/generic_builder/pkg/check/types.sh
+-rw-r--r--   0        0        0      625 1980-01-01 00:00:00.000000 arch_lint-2.4.0/build/generic_builder/pkg/default.nix
+-rw-r--r--   0        0        0     1046 1980-01-01 00:00:00.000000 arch_lint-2.4.0/flake.lock
+-rw-r--r--   0        0        0     1154 1980-01-01 00:00:00.000000 arch_lint-2.4.0/flake.nix
+-rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 arch_lint-2.4.0/makes.lock.nix
+-rw-r--r--   0        0        0      524 1980-01-01 00:00:00.000000 arch_lint-2.4.0/makes.nix
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/__init__.py
+-rw-r--r--   0        0        0       71 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import/layer1/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import/layer1/_private_module/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import/layer1/_private_module/something.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_2/__init__.py
+-rw-r--r--   0        0        0       73 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_2/foo.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_2/layer1/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_2/layer1/_private_module/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_2/layer1/_private_module/something.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_3/__init__.py
+-rw-r--r--   0        0        0       83 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_3/foo.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_3/layer1/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_3/layer1/_private_module/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mock_module/illegal_import_3/layer1/_private_module/something.py
+-rw-r--r--   0        0        0      760 1980-01-01 00:00:00.000000 arch_lint-2.4.0/mypy.ini
+-rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 arch_lint-2.4.0/nix.conf
+-rw-r--r--   0        0        0      484 1980-01-01 00:00:00.000000 arch_lint-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      917 1980-01-01 00:00:00.000000 arch_lint-2.4.0/tests/arch.py
+-rw-r--r--   0        0        0      908 1980-01-01 00:00:00.000000 arch_lint-2.4.0/tests/mock_arch.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 arch_lint-2.4.0/tests/py.typed
+-rw-r--r--   0        0        0     2013 1980-01-01 00:00:00.000000 arch_lint-2.4.0/tests/test_mock_module.py
+-rw-r--r--   0        0        0     1052 1980-01-01 00:00:00.000000 arch_lint-2.4.0/tests/test_self_arch.py
+-rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 arch_lint-2.4.0/PKG-INFO
```

### Comparing `arch_lint-2.3.0/.gitlab-ci.yml` & `arch_lint-2.4.0/.gitlab-ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .with_nix: &with_nix
   image: nixos/nix:2.6.0
   before_script:
     - cp ./nix.conf /etc/nix/nix.conf
     - nix-env -iA nixpkgs.jq
     - nix-env -iA cachix -f https://cachix.org/api/v1/install
-    - source ./ci/utils.sh
+    - source ./build/ci/utils.sh
 
 
 .in_dev_branch: &in_dev_branch
   rules:
     - if: '$CI_COMMIT_TAG != null'
       when: never
     - if: '$CI_COMMIT_BRANCH =~ /^v\d+$/'
@@ -57,53 +57,46 @@
 
 lint-bash:
   image: ghcr.io/fluidattacks/makes:21.11
   stage: lint
   <<: *in_dev_branch
   script: m . /formatBash && m . /lintBash
 
-build-runtime-env:
+build-for-python38:
   <<: *with_nix
   <<: *in_dev_branch
   stage: build
   script:
-    - build ".#python38.env.runtime"
+    - build ".#python38.pkg"
 
-build-dev-env:
+build-for-python39:
   <<: *with_nix
   <<: *in_dev_branch
   stage: build
   script:
-    - build ".#python38.env.dev"
+    - build ".#python39.pkg"
 
-test-check:
+build-for-python310:
   <<: *with_nix
   <<: *in_dev_branch
-  stage: test
+  stage: build
   script:
-    - build ".#python38.check.tests"
+    - build ".#python310.pkg"
 
-type-check:
+build-for-python311:
   <<: *with_nix
   <<: *in_dev_branch
-  stage: test
-  script:
-    - build ".#python38.check.types"
-
-build-for-min-python:
-  <<: *with_nix
-  <<: *new_version
   stage: build
   script:
-    - build ".#python38.pkg"
+    - build ".#python311.pkg"
 
 deploy-to-pypi:
   <<: *with_nix
   <<: *new_version
   stage: deploy
   script:
     - src=$(pwd)
     - nix develop -i
       -k FLIT_USERNAME
       -k FLIT_PASSWORD
-      ".#publish" -c
+      ".#python311.publish" -c
         flit -f "${src}/pyproject.toml" publish
```

### Comparing `arch_lint-2.3.0/arch_lint/_full_path.py` & `arch_lint-2.4.0/arch_lint/_full_path.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/arch_lint/_utils.py` & `arch_lint-2.4.0/arch_lint/_utils.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/arch_lint/dag/_dag.py` & `arch_lint-2.4.0/arch_lint/dag/_dag.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/arch_lint/dag/_dag_map.py` & `arch_lint-2.4.0/arch_lint/dag/_dag_map.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/arch_lint/dag/check.py` & `arch_lint-2.4.0/arch_lint/dag/check.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     FullPathModule,
     ImportGraph,
 )
 from pathlib import (
     Path,
 )
 from typing import (
+    Callable,
     FrozenSet,
     NoReturn,
     Optional,
     Tuple,
     Union,
 )
 
@@ -101,35 +102,52 @@
 
 
 def dag_completeness_from_dir(
     dag: DAG,
     dir_path: Path,
     raise_if_excess: bool,
     parent: Optional[FullPathModule],
+    path_filter: Callable[[Path], bool] = lambda _: True,
 ) -> Union[None, NoReturn]:
+    """
+    Check a DAG object completeness taking the elements of
+    `dir_path` as the complete expected list of modules.
+
+    - `dir_path` children are transformed into FullPathModule
+    using children name as the module name.
+    - if `parent` is provided then the FullPathModule object from
+    `dir_path` children will be expected to be children of `parent`
+    - `path_filter` used to filter the children of `dir_path` that
+    will be transformed
+    """
+
     def _to_module(raw: str) -> Union[FullPathModule, Exception]:
         if parent:
             _parent = parent.assert_child(raw)
             return _parent
         return FullPathModule.from_raw(raw)
 
     if dir_path.is_dir():
         expected = _utils.transform_sets(
-            frozenset(p.name for p in dir_path.iterdir()),
+            frozenset(p.name for p in filter(path_filter, dir_path.iterdir())),
             _to_module,
         )
         if isinstance(expected, Exception):
             raise expected
         return dag_completeness_from_set(dag, expected, raise_if_excess)
     raise Exception("Expected a dir path")
 
 
 def dag_map_completeness(
     dag_map: DagMap, graph: ImportGraph, parent: FullPathModule
 ) -> Union[None, NoReturn]:
+    """
+    Check a DagMap object completeness taking the children of
+    `parent` as the complete expected list of modules.
+    """
     parent_dag = dag_map.get(parent)
     children = graph.find_children(parent)
     if not parent_dag and len(children) > 1:
         raise Exception(f"Missing module at DagMap i.e. {parent}")
     if parent_dag:
         dag_completeness(parent_dag, graph, parent)
     for c in children:
@@ -142,14 +160,18 @@
     return None
 
 
 def check_dag(
     dag: DAG,
     graph: ImportGraph,
 ) -> Union[None, NoReturn]:
+    """
+    Check a DAG object completeness taking the children of
+    `parent` as the complete expected list of modules.
+    """
     for n, c in enumerate(dag.layers):
         _check_independence(graph, c)
         for lower_modules in dag.layers[n + 1 :]:
             _check_dag_over_modules(
                 graph,
                 lower_modules,
                 c,
```

### Comparing `arch_lint-2.3.0/arch_lint/forbidden.py` & `arch_lint-2.4.0/arch_lint/forbidden.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/arch_lint/graph.py` & `arch_lint-2.4.0/arch_lint/graph.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/arch_lint/private.py` & `arch_lint-2.4.0/arch_lint/private.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/flake.lock` & `arch_lint-2.4.0/flake.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777777%*

 * *Differences: {"'nodes'": "{'nixpkgs': {'locked': {'lastModified': 1679793451, 'narHash': "*

 * *            "'sha256-JafTtgMDATE8dZOImBhWMA9RCn9AP8FVOpN+9K/tTlg=', 'rev': "*

 * *            "'0cd51a933d91078775b300cf0f29aa3495231aa2'}, 'original': {'rev': "*

 * *            "'0cd51a933d91078775b300cf0f29aa3495231aa2'}}}"}*

```diff
@@ -13,24 +13,25 @@
                 "owner": "numtide",
                 "repo": "nix-filter",
                 "type": "github"
             }
         },
         "nixpkgs": {
             "locked": {
-                "lastModified": 1658172557,
-                "narHash": "sha256-oMwKOcpt9IsuW3g7ZcSZEnTJOMgw9jzVxJOF+15xjNs=",
+                "lastModified": 1679793451,
+                "narHash": "sha256-JafTtgMDATE8dZOImBhWMA9RCn9AP8FVOpN+9K/tTlg=",
                 "owner": "nixos",
                 "repo": "nixpkgs",
-                "rev": "02da3a122947e0ae1c024d276b03cb487f2266bd",
+                "rev": "0cd51a933d91078775b300cf0f29aa3495231aa2",
                 "type": "github"
             },
             "original": {
                 "owner": "nixos",
                 "repo": "nixpkgs",
+                "rev": "0cd51a933d91078775b300cf0f29aa3495231aa2",
                 "type": "github"
             }
         },
         "root": {
             "inputs": {
                 "nix_filter": "nix_filter",
                 "nixpkgs": "nixpkgs"
```

### Comparing `arch_lint-2.3.0/makes.nix` & `arch_lint-2.4.0/makes.nix`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/mypy.ini` & `arch_lint-2.4.0/mypy.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 [mypy]
-ignore_missing_imports = False
-
-disallow_any_unimported = True
-disallow_any_expr = True
 disallow_any_decorated = True
+disallow_any_expr = True
 disallow_any_explicit = True
 disallow_any_generics = True
+disallow_any_unimported = True
+disallow_incomplete_defs = True
 disallow_subclassing_any = True
-
 disallow_untyped_calls = True
-disallow_untyped_defs = True
-disallow_incomplete_defs = True
-check_untyped_defs = True
 disallow_untyped_decorators = True
+disallow_untyped_defs = True
 
+check_untyped_defs = True
 no_implicit_optional = True
+strict = True
+strict_equality = True
 strict_optional = True
 
 warn_redundant_casts = True
 warn_unused_ignores = True
 warn_no_return = True
 warn_return_any = True
 warn_unreachable = True
 
-show_none_errors = True
 ignore_errors = False
-
+ignore_missing_imports = False
 allow_untyped_globals = False
 allow_redefinition = False
 local_partial_types = False
 implicit_reexport = False
-strict_equality = True
-strict = True
 
 [mypy-grimp.*]
 ignore_missing_imports = True
```

### Comparing `arch_lint-2.3.0/tests/arch.py` & `arch_lint-2.4.0/tests/arch.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/tests/mock_arch.py` & `arch_lint-2.4.0/tests/mock_arch.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/tests/test_mock_module.py` & `arch_lint-2.4.0/tests/test_mock_module.py`

 * *Files identical despite different names*

### Comparing `arch_lint-2.3.0/tests/test_self_arch.py` & `arch_lint-2.4.0/tests/test_self_arch.py`

 * *Files identical despite different names*

