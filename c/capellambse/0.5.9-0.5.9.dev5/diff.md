# Comparing `tmp/capellambse-0.5.9.tar.gz` & `tmp/capellambse-0.5.9.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capellambse-0.5.9.tar", last modified: Tue Jan 17 15:54:58 2023, max compression
+gzip compressed data, was "capellambse-0.5.9.dev5.tar", last modified: Wed Jan 11 13:58:03 2023, max compression
```

## Comparing `capellambse-0.5.9.tar` & `capellambse-0.5.9.dev5.tar`

### file list

```diff
@@ -1,360 +1,358 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.895506 capellambse-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-17 15:54:44.000000 capellambse-0.5.9/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-17 15:54:44.000000 capellambse-0.5.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.831506 capellambse-0.5.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-01-17 15:54:44.000000 capellambse-0.5.9/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.831506 capellambse-0.5.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-17 15:54:44.000000 capellambse-0.5.9/.github/workflows/build-test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-01-17 15:54:44.000000 capellambse-0.5.9/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-17 15:54:44.000000 capellambse-0.5.9/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-01-17 15:54:44.000000 capellambse-0.5.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-01-17 15:54:44.000000 capellambse-0.5.9/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.835506 capellambse-0.5.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-17 15:54:44.000000 capellambse-0.5.9/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-17 15:54:44.000000 capellambse-0.5.9/.vscode/launch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-01-17 15:54:44.000000 capellambse-0.5.9/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.835506 capellambse-0.5.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/LICENSES/.license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-17 15:54:44.000000 capellambse-0.5.9/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-01-17 15:54:44.000000 capellambse-0.5.9/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-01-17 15:54:44.000000 capellambse-0.5.9/LICENSES/OFL-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-17 15:54:44.000000 capellambse-0.5.9/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-01-17 15:54:58.895506 capellambse-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-01-17 15:54:44.000000 capellambse-0.5.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.839506 capellambse-0.5.9/capellambse/
--rw-r--r--   0 runner    (1001) docker     (123)   147528 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/OpenSans-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/OpenSans-Regular.ttf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/_namespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.843506 capellambse-0.5.9/capellambse/aird/
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19773 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_box_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_edge_factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.843506 capellambse-0.5.9/capellambse/aird/_filters/
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_filters/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_filters/global.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_semantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/aird/diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/auditing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/decl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.843506 capellambse-0.5.9/capellambse/diagram/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/diagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35751 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/diagram/_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/diagram/_json_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/diagram/_styleclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/diagram/_vector2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    31322 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/diagram/capstyle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.843506 capellambse-0.5.9/capellambse/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/extensions/pvmt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.843506 capellambse-0.5.9/capellambse/extensions/reqif/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/extensions/reqif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24600 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/extensions/reqif/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    21683 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/extensions/reqif/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.843506 capellambse-0.5.9/capellambse/filehandler/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/filehandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28877 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/filehandler/git.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/filehandler/git_askpass.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/filehandler/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/filehandler/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.847506 capellambse-0.5.9/capellambse/known_models/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/docs.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/docs.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/test-5.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/test-5.0.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/test-5.2.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/test-5.2.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/test-lib.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/known_models/test-lib.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.847506 capellambse-0.5.9/capellambse/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/loader/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/loader/exs.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/loader/filehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/loader/modelinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/loader/xmltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.847506 capellambse-0.5.9/capellambse/model/
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.847506 capellambse-0.5.9/capellambse/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46620 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/common/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/common/element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.847506 capellambse-0.5.9/capellambse/model/crosslayer/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/capellacommon.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/capellacore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/cs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/fa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.847506 capellambse-0.5.9/capellambse/model/crosslayer/information/
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/information/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/information/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/information/datavalue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/crosslayer/modellingcore.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.847506 capellambse-0.5.9/capellambse/model/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/layers/ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/layers/la.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/layers/oa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/layers/pa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/model/modeltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.851506 capellambse-0.5.9/capellambse/pvmt/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/pvmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/pvmt/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/pvmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/pvmt/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/pvmt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/pvmt/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (123)     9246 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.851506 capellambse-0.5.9/capellambse/svg/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/svg/decorations.py
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/svg/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/svg/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/svg/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/svg/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    39012 2023-01-17 15:54:44.000000 capellambse-0.5.9/capellambse/svg/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.843506 capellambse-0.5.9/capellambse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-01-17 15:54:58.000000 capellambse-0.5.9/capellambse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-01-17 15:54:58.000000 capellambse-0.5.9/capellambse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:54:58.000000 capellambse-0.5.9/capellambse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-17 15:54:58.000000 capellambse-0.5.9/capellambse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:54:58.000000 capellambse-0.5.9/capellambse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-17 15:54:58.000000 capellambse-0.5.9/capellambse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-17 15:54:58.000000 capellambse-0.5.9/capellambse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.851506 capellambse-0.5.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.855506 capellambse-0.5.9/docs/capella-python-api/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/.user.af
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/.user.af.license
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/capella-python-api.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/capella-python-api.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)  2401904 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/capella-python-api.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/capella-python-api.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)   423416 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/capella-python-api.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/capella-python-api/capella-python-api.capella.license
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.855506 capellambse-0.5.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.855506 capellambse-0.5.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.867506 capellambse-0.5.9/docs/source/_static/img/
--rw-r--r--   0 runner    (1001) docker     (123)   123866 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-32.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-32.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   252319 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-36.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   195330 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-50.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-50.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   269678 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-36.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   296885 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-38.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-38.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   107980 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-44.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-44.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   342922 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-57.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-57.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   145863 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_19-50.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_19-50.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   157252 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-16.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-16.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   162695 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-21.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-21.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   216963 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-46.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-46.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   160237 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_22-09.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_22-09.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    85598 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_22-39.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-09_22-39.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   119471 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-10_22-35.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-10_22-35.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   250047 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-10_22-59.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-10_22-59.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    97595 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_18-18.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_18-18.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   103437 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_18-51.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_18-51.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   201117 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_19-12.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_19-12.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)    62130 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_20-06.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_20-06.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   121761 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_20-10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_20-10.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   209735 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_21-03.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-12_21-03.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   315538 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-13_20-46.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-13_20-46.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   107832 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-17_11-50.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/2021-05-17_11-50.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   110983 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/core-pkg-deps-raw.svg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/core-pkg-deps-raw.svg.license
--rw-r--r--   0 runner    (1001) docker     (123)    68428 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/crosslayer_intro.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/crosslayer_intro.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)   106498 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/dep-graph-oa.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/dep-graph-oa.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/github-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/harrys_wand.png
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/harrys_wand.png.license
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/waypoints.png
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/_static/img/waypoints.png.license
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.867506 capellambse-0.5.9/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/development/developing-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/development/how-to-explore-capella-mm.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/development/low-level-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/development/repl.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.871506 capellambse-0.5.9/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   141050 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/01 Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/01 Introduction.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)   105076 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/02 Intro to Physical Architecture API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/02 Intro to Physical Architecture API.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)    40158 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/03 Data Values.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/03 Data Values.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)   120797 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/04 Intro to Jinja templating.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/04 Intro to Jinja templating.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)    34853 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/05 Introduction to Libraries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/05 Introduction to Libraries.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)    38679 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/06 Introduction to Requirement access and management.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/06 Introduction to Requirement access and management.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)    29862 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/07 Code Generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/07 Code Generation.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)   205632 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/09 Context Diagrams.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/09 Context Diagrams.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/10 Declarative Modeling.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/examples/10 Declarative Modeling.ipynb.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.871506 capellambse-0.5.9/docs/source/howtos/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/howtos/howtos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.871506 capellambse-0.5.9/docs/source/start/
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/start/declarative.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/start/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/start/intro-to-api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.871506 capellambse-0.5.9/docs/source/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-17 15:54:44.000000 capellambse-0.5.9/docs/source/tools/sphinx-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-17 15:54:44.000000 capellambse-0.5.9/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 15:54:44.000000 capellambse-0.5.9/git-conventional-commits.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-17 15:54:44.000000 capellambse-0.5.9/git-conventional-commits.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-01-17 15:54:44.000000 capellambse-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 15:54:58.895506 capellambse-0.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.875506 capellambse-0.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.827506 capellambse-0.5.9/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.875506 capellambse-0.5.9/tests/data/Library Project/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/Library Project.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/Library Project.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)    72057 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/Library Project.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/Library Project.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)    31460 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/Library Project.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Project/Library Project.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.879506 capellambse-0.5.9/tests/data/Library Test/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/Library Test.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/Library Test.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/Library Test.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/Library Test.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/Library Test.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/Library Test/Library Test.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.879506 capellambse-0.5.9/tests/data/decl/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/coffee-machine.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.879506 capellambse-0.5.9/tests/data/decl/empty_project_52/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.827506 capellambse-0.5.9/tests/data/melodymodel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.883506 capellambse-0.5.9/tests/data/melodymodel/5_0/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)  2013536 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)   323425 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.887506 capellambse-0.5.9/tests/data/melodymodel/5_2/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)  1647555 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)   272917 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.887506 capellambse-0.5.9/tests/data/melodymodel/6_0/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)  1611675 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)   270229 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.891507 capellambse-0.5.9/tests/data/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)    58360 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)    28391 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.capella.license
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.repr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.repr.txt.license
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/parser/TestItems.txt.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.891507 capellambse-0.5.9/tests/data/pvmt/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/PVMTTest.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/PVMTTest.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)    32863 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/PVMTTest.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/PVMTTest.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)    47372 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/PVMTTest.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/PVMTTest.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.891507 capellambse-0.5.9/tests/data/pvmt/expected-output/
--rw-r--r--   0 runner    (1001) docker     (123)    48022 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/expected-output/apply.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/pvmt/expected-output/apply.capella.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:54:58.895506 capellambse-0.5.9/tests/data/writemodel/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/.project
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/.project.license
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/WriteTestModel.afm
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/WriteTestModel.afm.license
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/WriteTestModel.aird
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/WriteTestModel.aird.license
--rw-r--r--   0 runner    (1001) docker     (123)    22525 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/WriteTestModel.capella
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/data/writemodel/WriteTestModel.capella.license
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_aird_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_aird_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_auditing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_decl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_model_creation_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)    39051 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_model_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_pvmt.py
--rw-r--r--   0 runner    (1001) docker     (123)    33491 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_reqif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_svg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_vector2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_xlayer_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_xlayer_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_xlayer_fa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-01-17 15:54:44.000000 capellambse-0.5.9/tests/test_xlayer_information.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.067781 capellambse-0.5.9.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.987780 capellambse-0.5.9.dev5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.987780 capellambse-0.5.9.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.github/workflows/build-test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.987780 capellambse-0.5.9.dev5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/.vscode/launch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.991780 capellambse-0.5.9.dev5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/LICENSES/.license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/LICENSES/OFL-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-01-11 13:58:03.067781 capellambse-0.5.9.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.991780 capellambse-0.5.9.dev5/capellambse/
+-rw-r--r--   0 runner    (1001) docker     (123)   147528 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/OpenSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/OpenSans-Regular.ttf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/_namespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.995780 capellambse-0.5.9.dev5/capellambse/aird/
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19773 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_box_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_edge_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.995780 capellambse-0.5.9.dev5/capellambse/aird/_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_filters/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_filters/global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/aird/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/auditing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/decl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.995780 capellambse-0.5.9.dev5/capellambse/diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/diagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35751 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/diagram/_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/diagram/_json_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/diagram/_vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31322 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/diagram/capstyle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.995780 capellambse-0.5.9.dev5/capellambse/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/extensions/pvmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.999780 capellambse-0.5.9.dev5/capellambse/extensions/reqif/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/extensions/reqif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24600 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/extensions/reqif/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21683 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/extensions/reqif/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.999780 capellambse-0.5.9.dev5/capellambse/filehandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/filehandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28877 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/filehandler/git.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/filehandler/git_askpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/filehandler/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/filehandler/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.999780 capellambse-0.5.9.dev5/capellambse/known_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/docs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/docs.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/test-5.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/test-5.0.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/test-5.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/test-5.2.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/test-lib.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/known_models/test-lib.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.999780 capellambse-0.5.9.dev5/capellambse/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/loader/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/loader/exs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/loader/filehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/loader/modelinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/loader/xmltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.003780 capellambse-0.5.9.dev5/capellambse/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.003780 capellambse-0.5.9.dev5/capellambse/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46620 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/common/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/common/element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.003780 capellambse-0.5.9.dev5/capellambse/model/crosslayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/capellacommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/capellacore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/fa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.003780 capellambse-0.5.9.dev5/capellambse/model/crosslayer/information/
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/information/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/information/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/information/datavalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/crosslayer/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.003780 capellambse-0.5.9.dev5/capellambse/model/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/layers/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/layers/la.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/layers/oa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/layers/pa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/model/modeltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.007780 capellambse-0.5.9.dev5/capellambse/pvmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/pvmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/pvmt/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/pvmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/pvmt/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/pvmt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/pvmt/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9246 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.007780 capellambse-0.5.9.dev5/capellambse/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/svg/decorations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/svg/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/svg/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/svg/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/svg/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39012 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/capellambse/svg/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.991780 capellambse-0.5.9.dev5/capellambse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-01-11 13:58:02.000000 capellambse-0.5.9.dev5/capellambse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-01-11 13:58:02.000000 capellambse-0.5.9.dev5/capellambse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 13:58:02.000000 capellambse-0.5.9.dev5/capellambse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-11 13:58:02.000000 capellambse-0.5.9.dev5/capellambse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 13:58:02.000000 capellambse-0.5.9.dev5/capellambse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-11 13:58:02.000000 capellambse-0.5.9.dev5/capellambse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-11 13:58:02.000000 capellambse-0.5.9.dev5/capellambse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.007780 capellambse-0.5.9.dev5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.011780 capellambse-0.5.9.dev5/docs/capella-python-api/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/.user.af
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/.user.af.license
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)  2401904 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)   423416 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.capella.license
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.015780 capellambse-0.5.9.dev5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.015780 capellambse-0.5.9.dev5/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.031781 capellambse-0.5.9.dev5/docs/source/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   123866 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-32.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-32.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   252319 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-36.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   195330 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-50.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-50.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   269678 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-36.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   296885 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-38.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-38.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   107980 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-44.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-44.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   342922 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-57.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-57.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   145863 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_19-50.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_19-50.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   157252 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-16.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-16.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   162695 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-21.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-21.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   216963 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-46.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-46.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   160237 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_22-09.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_22-09.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    85598 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_22-39.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_22-39.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   119471 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-10_22-35.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-10_22-35.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   250047 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-10_22-59.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-10_22-59.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    97595 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_18-18.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_18-18.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   103437 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_18-51.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_18-51.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   201117 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_19-12.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_19-12.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    62130 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_20-06.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_20-06.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   121761 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_20-10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_20-10.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   209735 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_21-03.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_21-03.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   315538 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-13_20-46.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-13_20-46.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   107832 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-17_11-50.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-17_11-50.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   110983 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/core-pkg-deps-raw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/core-pkg-deps-raw.svg.license
+-rw-r--r--   0 runner    (1001) docker     (123)    68428 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/crosslayer_intro.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/crosslayer_intro.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)   106498 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/dep-graph-oa.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/dep-graph-oa.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/github-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/harrys_wand.png
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/harrys_wand.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/waypoints.png
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/_static/img/waypoints.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.031781 capellambse-0.5.9.dev5/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/development/developing-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/development/how-to-explore-capella-mm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/development/low-level-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/development/repl.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.035781 capellambse-0.5.9.dev5/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   141050 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/01 Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/01 Introduction.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)   105076 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/02 Intro to Physical Architecture API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/02 Intro to Physical Architecture API.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)    40158 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/03 Data Values.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/03 Data Values.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)   120797 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/04 Intro to Jinja templating.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/04 Intro to Jinja templating.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)    34853 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/05 Introduction to Libraries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/05 Introduction to Libraries.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)    38679 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/06 Introduction to Requirement access and management.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/06 Introduction to Requirement access and management.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)    29862 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/07 Code Generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/07 Code Generation.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)   205632 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/09 Context Diagrams.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/09 Context Diagrams.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/10 Declarative Modeling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/examples/10 Declarative Modeling.ipynb.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.035781 capellambse-0.5.9.dev5/docs/source/howtos/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/howtos/howtos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.035781 capellambse-0.5.9.dev5/docs/source/start/
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/start/declarative.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/start/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/start/intro-to-api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.035781 capellambse-0.5.9.dev5/docs/source/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/docs/source/tools/sphinx-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/git-conventional-commits.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/git-conventional-commits.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 13:58:03.067781 capellambse-0.5.9.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.039780 capellambse-0.5.9.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.987780 capellambse-0.5.9.dev5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.039780 capellambse-0.5.9.dev5/tests/data/Library Project/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)    72057 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)    31460 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.043781 capellambse-0.5.9.dev5/tests/data/Library Test/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.043781 capellambse-0.5.9.dev5/tests/data/decl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/coffee-machine.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.043781 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:02.987780 capellambse-0.5.9.dev5/tests/data/melodymodel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.047781 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)  2013536 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)   323425 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.051781 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)  1647555 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)   272917 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.059781 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)  1611675 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)   270229 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.063781 capellambse-0.5.9.dev5/tests/data/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58360 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)    28391 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.capella.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.repr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.repr.txt.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/parser/TestItems.txt.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.063781 capellambse-0.5.9.dev5/tests/data/pvmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)    32863 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)    47372 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.063781 capellambse-0.5.9.dev5/tests/data/pvmt/expected-output/
+-rw-r--r--   0 runner    (1001) docker     (123)    48022 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/expected-output/apply.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/pvmt/expected-output/apply.capella.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 13:58:03.067781 capellambse-0.5.9.dev5/tests/data/writemodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)    22525 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.capella.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_aird_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_aird_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_auditing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_decl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_model_creation_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38512 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_model_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_pvmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33491 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_reqif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_xlayer_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_xlayer_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_xlayer_fa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-01-11 13:57:38.000000 capellambse-0.5.9.dev5/tests/test_xlayer_information.py
```

### Comparing `capellambse-0.5.9/.github/workflows/build-test-publish.yml` & `capellambse-0.5.9.dev5/.github/workflows/build-test-publish.yml`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/.github/workflows/docs.yml` & `capellambse-0.5.9.dev5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/.github/workflows/lint.yml` & `capellambse-0.5.9.dev5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/.gitignore` & `capellambse-0.5.9.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/.pre-commit-config.yaml` & `capellambse-0.5.9.dev5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/.vscode/launch.json` & `capellambse-0.5.9.dev5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/CONTRIBUTING.rst` & `capellambse-0.5.9.dev5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/LICENSES/Apache-2.0.txt` & `capellambse-0.5.9.dev5/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/LICENSES/CC0-1.0.txt` & `capellambse-0.5.9.dev5/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/LICENSES/OFL-1.1.txt` & `capellambse-0.5.9.dev5/LICENSES/OFL-1.1.txt`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/MAINTAINERS.md` & `capellambse-0.5.9.dev5/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/PKG-INFO` & `capellambse-0.5.9.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capellambse
-Version: 0.5.9
+Version: 0.5.9.dev5
 Summary: Provides access to Capella MBSE projects in Python
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/py-capellambse
 Project-URL: Documentation, https://dsd-dbs.github.io/py-capellambse
 Keywords: arcadia,capella,mbse,model-based systems engineering
 Platform: any
```

### Comparing `capellambse-0.5.9/README.rst` & `capellambse-0.5.9.dev5/README.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/OpenSans-Regular.ttf` & `capellambse-0.5.9.dev5/capellambse/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/__init__.py` & `capellambse-0.5.9.dev5/capellambse/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/_namespaces.py` & `capellambse-0.5.9.dev5/capellambse/_namespaces.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/__init__.py` & `capellambse-0.5.9.dev5/capellambse/aird/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_box_factories.py` & `capellambse-0.5.9.dev5/capellambse/aird/_box_factories.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_common.py` & `capellambse-0.5.9.dev5/capellambse/aird/_common.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_edge_factories.py` & `capellambse-0.5.9.dev5/capellambse/aird/_edge_factories.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_filters/__init__.py` & `capellambse-0.5.9.dev5/capellambse/aird/_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_filters/composite.py` & `capellambse-0.5.9.dev5/capellambse/aird/_filters/composite.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_filters/global.py` & `capellambse-0.5.9.dev5/capellambse/aird/_filters/global.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_semantic.py` & `capellambse-0.5.9.dev5/capellambse/aird/_semantic.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_styling.py` & `capellambse-0.5.9.dev5/capellambse/aird/_styling.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/aird/_visual.py` & `capellambse-0.5.9.dev5/capellambse/aird/_visual.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/auditing.py` & `capellambse-0.5.9.dev5/capellambse/auditing.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/cli_helpers.py` & `capellambse-0.5.9.dev5/capellambse/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/decl.py` & `capellambse-0.5.9.dev5/capellambse/decl.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/diagram/_diagram.py` & `capellambse-0.5.9.dev5/capellambse/diagram/_diagram.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/diagram/_json_enc.py` & `capellambse-0.5.9.dev5/capellambse/diagram/_json_enc.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/diagram/_vector2d.py` & `capellambse-0.5.9.dev5/capellambse/diagram/_vector2d.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/diagram/capstyle.py` & `capellambse-0.5.9.dev5/capellambse/diagram/capstyle.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/extensions/pvmt.py` & `capellambse-0.5.9.dev5/capellambse/extensions/pvmt.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/extensions/reqif/elements.py` & `capellambse-0.5.9.dev5/capellambse/extensions/reqif/elements.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/extensions/reqif/exporter.py` & `capellambse-0.5.9.dev5/capellambse/extensions/reqif/exporter.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/filehandler/__init__.py` & `capellambse-0.5.9.dev5/capellambse/filehandler/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/filehandler/git.py` & `capellambse-0.5.9.dev5/capellambse/filehandler/git.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/filehandler/http.py` & `capellambse-0.5.9.dev5/capellambse/filehandler/http.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/filehandler/local.py` & `capellambse-0.5.9.dev5/capellambse/filehandler/local.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/helpers.py` & `capellambse-0.5.9.dev5/capellambse/helpers.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/loader/core.py` & `capellambse-0.5.9.dev5/capellambse/loader/core.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/loader/exs.py` & `capellambse-0.5.9.dev5/capellambse/loader/exs.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/loader/xmltools.py` & `capellambse-0.5.9.dev5/capellambse/loader/xmltools.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/__init__.py` & `capellambse-0.5.9.dev5/capellambse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/common/__init__.py` & `capellambse-0.5.9.dev5/capellambse/model/common/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/common/accessors.py` & `capellambse-0.5.9.dev5/capellambse/model/common/accessors.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/common/element.py` & `capellambse-0.5.9.dev5/capellambse/model/common/element.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/__init__.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/capellacommon.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/capellacommon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: Copyright DB Netz AG and the capellambse contributors
 # SPDX-License-Identifier: Apache-2.0
 
 """Classes handling Mode/State-Machines and related content."""
 from .. import common as c
-from . import capellacore, modellingcore
+from . import capellacore
 
 XT_TRAFO = "org.polarsys.capella.core.data.capellacommon:TransfoLink"
 XT_ABSTRACT_STATE_REAL = (
     "org.polarsys.capella.core.data.capellacommon:AbstractStateRealization"
 )
 
 
@@ -110,17 +110,20 @@
     effects = c.AttrProxyAccessor(
         c.GenericElement, "effect", aslist=c.MixedElementList
     )
     guard = c.AttrProxyAccessor(capellacore.Constraint, "guard")
 
 
 @c.xtype_handler(None)
-class GenericTrace(modellingcore.TraceableElement):
+class GenericTrace(c.GenericElement):
     """A trace between two elements."""
 
+    source = c.AttrProxyAccessor(c.GenericElement, attr="sourceElement")
+    target = c.AttrProxyAccessor(c.GenericElement, attr="targetElement")
+
     @property
     def name(self) -> str:  # type: ignore[override]
         """Return the name."""
         direction = ""
         if self.target is not None:
             direction = f" to {self.target.name} ({self.target.uuid})"
```

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/capellacore.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/capellacore.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/cs.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/cs.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/fa.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/fa.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,25 +33,14 @@
 XT_COMP_EX_ALLOC = (
     "org.polarsys.capella.core.data.fa:ComponentExchangeAllocation"
 )
 XT_FCALLOC = "org.polarsys.capella.core.data.fa:ComponentFunctionalAllocation"
 
 
 @c.xtype_handler(None)
-class ControlNode(c.GenericElement):
-    """A node with a specific control-kind."""
-
-    _xmltag = "ownedSequenceNodes"
-
-    kind = xmltools.EnumAttributeProperty(
-        "_element", "kind", modeltypes.ControlNodeKind, writable=False
-    )
-
-
-@c.xtype_handler(None)
 class FunctionRealization(c.GenericElement):
     """A realization that links to a function."""
 
     _xmltag = "ownedFunctionRealizations"
 
 
 class AbstractExchange(c.GenericElement):
@@ -183,15 +172,14 @@
     )
     involved_links = c.LinkAccessor[AbstractExchange](
         None,  # FIXME fill in tag
         FunctionalChainInvolvementLink,
         aslist=c.MixedElementList,
         attr="involved",
     )
-    control_nodes = c.DirectProxyAccessor(ControlNode, aslist=c.ElementList)
 
     @property
     def involved(self) -> c.MixedElementList:
         return self.involved_functions + self.involved_links
 
 
 @c.xtype_handler(None)
```

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/information/__init__.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/information/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 Information object-relations map (ontology):
 
 .. diagram:: [CDB] Information [Ontology]
 """
 
 from __future__ import annotations
 
+from lxml import etree
+
 from capellambse.loader import xmltools
 
 from ... import common as c
 from ... import modeltypes
-from .. import capellacommon, capellacore, modellingcore
+from .. import capellacommon, capellacore
 from . import datatype, datavalue
 
 
 def _allocated_exchange_items(
     obj: c.GenericElement,
 ) -> c.ElementList[c.GenericElement]:
     try:
@@ -57,15 +59,14 @@
 
 @c.xtype_handler(None)
 class Association(c.GenericElement):
     """An Association."""
 
     _xmltag = "ownedAssociations"
 
-    members: c.Accessor[Property]
     navigable_members: c.Accessor[Property]
     source_role: c.Accessor[Property]
 
     @property
     def roles(self) -> c.ElementList[Property]:
         roles = []
         if self.source_role:
@@ -74,21 +75,14 @@
 
         assert isinstance(self.navigable_members, c.ElementList)
         roles.extend(prop._element for prop in self.navigable_members)
         return c.ElementList(self._model, roles, Property)
 
 
 @c.xtype_handler(None)
-class PortAllocation(modellingcore.TraceableElement):
-    """An exchange between a ComponentPort and FunctionalPort."""
-
-    _xmltag = "ownedPortAllocations"
-
-
-@c.xtype_handler(None)
 class Property(c.GenericElement):
     """A Property of a Class."""
 
     _xmltag = "ownedFeatures"
 
     is_ordered = xmltools.BooleanAttributeProperty(
         "_element",
@@ -182,19 +176,22 @@
             self.owned_properties + self.super.properties
             if self.super is not None
             else self.owned_properties
         )
 
 
 @c.xtype_handler(None)
-class InformationRealization(modellingcore.TraceableElement):
+class InformationRealization(c.GenericElement):
     """A realization for a Class."""
 
     _xmltag = "ownedInformationRealizations"
 
+    source = c.AttrProxyAccessor(Class, "sourceElement")
+    target = c.AttrProxyAccessor(Class, "targetElement")
+
 
 @c.xtype_handler(None)
 class Union(Class):
     """A Union."""
 
     _xmltag = "ownedClasses"
 
@@ -285,19 +282,14 @@
 )
 c.set_accessor(
     DataPkg, "packages", c.DirectProxyAccessor(DataPkg, aslist=c.ElementList)
 )
 c.set_accessor(ExchangeItemElement, "owner", c.ParentAccessor(ExchangeItem))
 c.set_accessor(
     Association,
-    "members",
-    c.DirectProxyAccessor(Property, aslist=c.ElementList),
-)
-c.set_accessor(
-    Association,
     "navigable_members",
     c.AttrProxyAccessor(Property, "navigableMembers", aslist=c.ElementList),
 )
 c.set_accessor(Association, "source_role", c.DirectProxyAccessor(Property))
 c.set_accessor(
     Class,
     "realized_classes",
```

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/information/datatype.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/information/datatype.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/information/datavalue.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/information/datavalue.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/crosslayer/interaction.py` & `capellambse-0.5.9.dev5/capellambse/model/crosslayer/interaction.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/diagram.py` & `capellambse-0.5.9.dev5/capellambse/model/diagram.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/layers/ctx.py` & `capellambse-0.5.9.dev5/capellambse/model/layers/ctx.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/layers/la.py` & `capellambse-0.5.9.dev5/capellambse/model/layers/la.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/layers/oa.py` & `capellambse-0.5.9.dev5/capellambse/model/layers/oa.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     fa,
     information,
     interaction,
 )
 
 XT_ARCH = "org.polarsys.capella.core.data.oa:OperationalAnalysis"
 
+XT_EOCI = (
+    "org.polarsys.capella.core.data.oa:EntityOperationalCapabilityInvolvement"
+)
+
 
 @c.xtype_handler(XT_ARCH)
 class OperationalActivity(fa.AbstractFunction):
     """An operational activity."""
 
     _xmltag = "ownedOperationalActivities"
```

### Comparing `capellambse-0.5.9/capellambse/model/layers/pa.py` & `capellambse-0.5.9.dev5/capellambse/model/layers/pa.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/model/modeltypes.py` & `capellambse-0.5.9.dev5/capellambse/model/modeltypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,15 +204,7 @@
 
 class ScenarioKind(_StringyEnumMixin, _enum.Enum):
     UNSET = _enum.auto()
     DATA_FLOW = _enum.auto()
     FUNCTIONAL = _enum.auto()
     INTERACTION = _enum.auto()
     INTERFACE = _enum.auto()
-
-
-class ControlNodeKind(_StringyEnumMixin, _enum.Enum):
-    """ControlNode kind."""
-
-    OR = _enum.auto()
-    AND = _enum.auto()
-    ITERATE = _enum.auto()
```

### Comparing `capellambse-0.5.9/capellambse/pvmt/core.py` & `capellambse-0.5.9.dev5/capellambse/pvmt/core.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/pvmt/exceptions.py` & `capellambse-0.5.9.dev5/capellambse/pvmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/pvmt/model.py` & `capellambse-0.5.9.dev5/capellambse/pvmt/model.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/pvmt/types.py` & `capellambse-0.5.9.dev5/capellambse/pvmt/types.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/pvmt/validation.py` & `capellambse-0.5.9.dev5/capellambse/pvmt/validation.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/repl.py` & `capellambse-0.5.9.dev5/capellambse/repl.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/sphinx.py` & `capellambse-0.5.9.dev5/capellambse/sphinx.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/svg/decorations.py` & `capellambse-0.5.9.dev5/capellambse/svg/decorations.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/svg/drawing.py` & `capellambse-0.5.9.dev5/capellambse/svg/drawing.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/svg/generate.py` & `capellambse-0.5.9.dev5/capellambse/svg/generate.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/svg/helpers.py` & `capellambse-0.5.9.dev5/capellambse/svg/helpers.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/svg/style.py` & `capellambse-0.5.9.dev5/capellambse/svg/style.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse/svg/symbols.py` & `capellambse-0.5.9.dev5/capellambse/svg/symbols.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/capellambse.egg-info/PKG-INFO` & `capellambse-0.5.9.dev5/capellambse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capellambse
-Version: 0.5.9
+Version: 0.5.9.dev5
 Summary: Provides access to Capella MBSE projects in Python
 Author: DB Netz AG
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/DSD-DBS/py-capellambse
 Project-URL: Documentation, https://dsd-dbs.github.io/py-capellambse
 Keywords: arcadia,capella,mbse,model-based systems engineering
 Platform: any
```

### Comparing `capellambse-0.5.9/capellambse.egg-info/SOURCES.txt` & `capellambse-0.5.9.dev5/capellambse.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 capellambse/aird/diagram.py
 capellambse/aird/_filters/__init__.py
 capellambse/aird/_filters/composite.py
 capellambse/aird/_filters/global.py
 capellambse/diagram/__init__.py
 capellambse/diagram/_diagram.py
 capellambse/diagram/_json_enc.py
-capellambse/diagram/_styleclass.py
 capellambse/diagram/_vector2d.py
 capellambse/diagram/capstyle.py
 capellambse/extensions/__init__.py
 capellambse/extensions/pvmt.py
 capellambse/extensions/reqif/__init__.py
 capellambse/extensions/reqif/elements.py
 capellambse/extensions/reqif/exporter.py
@@ -86,15 +85,14 @@
 capellambse/model/common/element.py
 capellambse/model/crosslayer/__init__.py
 capellambse/model/crosslayer/capellacommon.py
 capellambse/model/crosslayer/capellacore.py
 capellambse/model/crosslayer/cs.py
 capellambse/model/crosslayer/fa.py
 capellambse/model/crosslayer/interaction.py
-capellambse/model/crosslayer/modellingcore.py
 capellambse/model/crosslayer/information/__init__.py
 capellambse/model/crosslayer/information/datatype.py
 capellambse/model/crosslayer/information/datavalue.py
 capellambse/model/layers/__init__.py
 capellambse/model/layers/ctx.py
 capellambse/model/layers/la.py
 capellambse/model/layers/oa.py
```

### Comparing `capellambse-0.5.9/capellambse.egg-info/entry_points.txt` & `capellambse-0.5.9.dev5/capellambse.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/Makefile` & `capellambse-0.5.9.dev5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/capella-python-api/capella-python-api.aird` & `capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/capella-python-api/capella-python-api.capella` & `capellambse-0.5.9.dev5/docs/capella-python-api/capella-python-api.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/make.bat` & `capellambse-0.5.9.dev5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-32.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-32.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-36.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-36.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_10-50.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_10-50.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-36.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-36.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-38.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-38.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-44.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-44.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_17-57.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_17-57.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_19-50.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_19-50.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-16.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-16.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-21.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-21.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_21-46.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_21-46.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_22-09.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_22-09.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-09_22-39.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-09_22-39.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-10_22-35.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-10_22-35.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-10_22-59.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-10_22-59.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-12_18-18.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_18-18.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-12_18-51.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_18-51.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-12_19-12.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_19-12.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-12_20-06.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_20-06.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-12_20-10.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_20-10.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-12_21-03.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-12_21-03.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-13_20-46.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-13_20-46.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/2021-05-17_11-50.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/2021-05-17_11-50.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/core-pkg-deps-raw.svg` & `capellambse-0.5.9.dev5/docs/source/_static/img/core-pkg-deps-raw.svg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/crosslayer_intro.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/crosslayer_intro.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/dep-graph-oa.jpg` & `capellambse-0.5.9.dev5/docs/source/_static/img/dep-graph-oa.jpg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/github-logo.svg` & `capellambse-0.5.9.dev5/docs/source/_static/img/github-logo.svg`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/harrys_wand.png` & `capellambse-0.5.9.dev5/docs/source/_static/img/harrys_wand.png`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/_static/img/waypoints.png` & `capellambse-0.5.9.dev5/docs/source/_static/img/waypoints.png`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/conf.py` & `capellambse-0.5.9.dev5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/development/developing-docs.rst` & `capellambse-0.5.9.dev5/docs/source/development/developing-docs.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/development/how-to-explore-capella-mm.rst` & `capellambse-0.5.9.dev5/docs/source/development/how-to-explore-capella-mm.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/development/low-level-api.rst` & `capellambse-0.5.9.dev5/docs/source/development/low-level-api.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/01 Introduction.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/01 Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/02 Intro to Physical Architecture API.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/02 Intro to Physical Architecture API.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/03 Data Values.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/03 Data Values.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/04 Intro to Jinja templating.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/04 Intro to Jinja templating.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/05 Introduction to Libraries.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/05 Introduction to Libraries.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/06 Introduction to Requirement access and management.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/06 Introduction to Requirement access and management.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/07 Code Generation.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/07 Code Generation.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/09 Context Diagrams.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/09 Context Diagrams.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/examples/10 Declarative Modeling.ipynb` & `capellambse-0.5.9.dev5/docs/source/examples/10 Declarative Modeling.ipynb`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/index.rst` & `capellambse-0.5.9.dev5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/start/declarative.rst` & `capellambse-0.5.9.dev5/docs/source/start/declarative.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/start/installation.rst` & `capellambse-0.5.9.dev5/docs/source/start/installation.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/docs/source/start/intro-to-api.rst` & `capellambse-0.5.9.dev5/docs/source/start/intro-to-api.rst`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/pyproject.toml` & `capellambse-0.5.9.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/conftest.py` & `capellambse-0.5.9.dev5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/Library Project/Library Project.aird` & `capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/Library Project/Library Project.capella` & `capellambse-0.5.9.dev5/tests/data/Library Project/Library Project.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/Library Test/Library Test.aird` & `capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/Library Test/Library Test.capella` & `capellambse-0.5.9.dev5/tests/data/Library Test/Library Test.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/decl/coffee-machine.yml` & `capellambse-0.5.9.dev5/tests/data/decl/coffee-machine.yml`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.aird` & `capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/decl/empty_project_52/empty_project_52.capella` & `capellambse-0.5.9.dev5/tests/data/decl/empty_project_52/empty_project_52.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.afm` & `capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.afm`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.aird` & `capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/5_0/Melody Model Test.capella` & `capellambse-0.5.9.dev5/tests/data/melodymodel/5_0/Melody Model Test.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.afm` & `capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.afm`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.aird` & `capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/5_2/Melody Model Test.capella` & `capellambse-0.5.9.dev5/tests/data/melodymodel/5_2/Melody Model Test.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.afm` & `capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.afm`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.aird` & `capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/melodymodel/6_0/Melody Model Test.capella` & `capellambse-0.5.9.dev5/tests/data/melodymodel/6_0/Melody Model Test.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/parser/TestItems.afm` & `capellambse-0.5.9.dev5/tests/data/parser/TestItems.afm`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/parser/TestItems.aird` & `capellambse-0.5.9.dev5/tests/data/parser/TestItems.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/parser/TestItems.capella` & `capellambse-0.5.9.dev5/tests/data/parser/TestItems.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/parser/TestItems.json` & `capellambse-0.5.9.dev5/tests/data/parser/TestItems.json`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/parser/TestItems.repr.txt` & `capellambse-0.5.9.dev5/tests/data/parser/TestItems.repr.txt`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/parser/TestItems.txt` & `capellambse-0.5.9.dev5/tests/data/parser/TestItems.txt`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/pvmt/PVMTTest.aird` & `capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/pvmt/PVMTTest.capella` & `capellambse-0.5.9.dev5/tests/data/pvmt/PVMTTest.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/pvmt/expected-output/apply.capella` & `capellambse-0.5.9.dev5/tests/data/pvmt/expected-output/apply.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/writemodel/WriteTestModel.aird` & `capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.aird`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/data/writemodel/WriteTestModel.capella` & `capellambse-0.5.9.dev5/tests/data/writemodel/WriteTestModel.capella`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_aird_filters.py` & `capellambse-0.5.9.dev5/tests/test_aird_filters.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_aird_parser.py` & `capellambse-0.5.9.dev5/tests/test_aird_parser.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_auditing.py` & `capellambse-0.5.9.dev5/tests/test_auditing.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_cli_helpers.py` & `capellambse-0.5.9.dev5/tests/test_cli_helpers.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_decl.py` & `capellambse-0.5.9.dev5/tests/test_decl.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_helpers.py` & `capellambse-0.5.9.dev5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_model_creation_deletion.py` & `capellambse-0.5.9.dev5/tests/test_model_creation_deletion.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_model_layers.py` & `capellambse-0.5.9.dev5/tests/test_model_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -688,33 +688,14 @@
     assert fnc in chain.involvements
     assert fnc.involved == target
     assert (
         fnc.name == f"[FunctionalChainInvolvementFunction] to {expected_end}"
     )
 
 
-@pytest.mark.parametrize(
-    ["chain_uuid", "control_nodes"],
-    [
-        pytest.param(
-            "d588e41f-ec4d-4fa9-ad6d-056868c66274", 3, id="OperationalProcess"
-        ),
-        pytest.param(
-            "dfc4341d-253a-4ae9-8a30-63a9d9faca39", 9, id="FunctionalChain"
-        ),
-    ],
-)
-def test_FunctionalChainInvolvement_has_control_nodes(
-    model_5_2: capellambse.MelodyModel, chain_uuid: str, control_nodes: int
-) -> None:
-    chain = model_5_2.by_uuid(chain_uuid)
-
-    assert len(chain.control_nodes) == control_nodes
-
-
 class TestArchitectureLayers:
     @pytest.mark.parametrize(
         "layer,definitions",
         [
             pytest.param(
                 "oa",
                 [
```

### Comparing `capellambse-0.5.9/tests/test_model_loading.py` & `capellambse-0.5.9.dev5/tests/test_model_loading.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_pvmt.py` & `capellambse-0.5.9.dev5/tests/test_pvmt.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_reqif.py` & `capellambse-0.5.9.dev5/tests/test_reqif.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_svg.py` & `capellambse-0.5.9.dev5/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_vector2d.py` & `capellambse-0.5.9.dev5/tests/test_vector2d.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_xlayer_common.py` & `capellambse-0.5.9.dev5/tests/test_xlayer_common.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_xlayer_cs.py` & `capellambse-0.5.9.dev5/tests/test_xlayer_cs.py`

 * *Files identical despite different names*

### Comparing `capellambse-0.5.9/tests/test_xlayer_information.py` & `capellambse-0.5.9.dev5/tests/test_xlayer_information.py`

 * *Files identical despite different names*

